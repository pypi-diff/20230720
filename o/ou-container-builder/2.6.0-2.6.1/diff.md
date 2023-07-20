# Comparing `tmp/ou_container_builder-2.6.0.tar.gz` & `tmp/ou_container_builder-2.6.1.tar.gz`

## Comparing `ou_container_builder-2.6.0.tar` & `ou_container_builder-2.6.1.tar`

### file list

```diff
@@ -1,912 +1,912 @@
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/Dockerfile
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/prepare_release.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tox.ini
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/pyvenv.cfg
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.csh
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.fish
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.nu
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/activate_this.py
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip-3.11
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip3
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/python -> /usr/bin/python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/python3.11 -> python
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel-3.11
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel3
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/bin/wheel3.11
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.virtualenv
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18328 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28722 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    18817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18442 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    27696 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    32782 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18864 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    84101 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109388 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    71556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53572 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99195 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/METADATA
--rw-r--r--   0        0        0    72198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/top_level.txt
--rw-r--r--   0        0        0   109451 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    80078 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   133344 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    22975 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_normalization.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    19778 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-32.exe
--rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-64.exe
--rw-r--r--   0        0        0   137216 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    21087 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    47046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/glob.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-32.exe
--rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-64.exe
--rw-r--r--   0        0        0   137728 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    47115 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    39968 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/py312compat.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/warnings.py
--rw-r--r--   0        0        0     8608 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_log.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0    19616 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    48643 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17861 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50174 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17899 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30188 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18099 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31503 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    87692 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    31965 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    28906 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    13755 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    26184 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   274907 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/METADATA
--rw-r--r--   0        0        0    34553 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/top_level.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/__main__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py
--rw-r--r--   0        0        0    19868 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/bdist_wheel.py
--rw-r--r--   0        0        0    16143 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/macosx_libfile.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/metadata.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/util.py
--rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/wheelfile.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/convert.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/pack.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/tags.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/unpack.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/vendor.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py
--rw-r--r--   0        0        0    39047 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py
--rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/METADATA
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/WHEEL
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/Makefile
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/building.rst
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/conf.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/index.rst
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/installation.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/index.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/main.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs.rst
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/utils.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/validator.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/content.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/env.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/scripts.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/services.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/core/web_apps.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/jupyterlab.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/mariadb.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/nbclassic.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/api/packs/tutorial_server.rst
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/content.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/environment.rst
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/flags.rst
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/hacks.rst
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/image.rst
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/index.rst
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/jupyter_server_config.rst
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/module.rst
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/packages.rst
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/packs.rst
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/scripts.rst
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/server.rst
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/services.rst
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/sources.rst
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/configuration/web_apps.rst
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/code-server.rst
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/index.rst
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/jupyterlab.rst
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/mariadb.rst
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/nbclassic.rst
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/docs/packs/tutorial_server.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/__about__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/__init__.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/__main__.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/builder.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/settings.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/utils.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/base.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/content.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/env.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/hacks.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/jupyter_server.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/packages.py
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/scripts.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/services.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/startup.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/core/web_apps.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/__init__.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/code_server.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/jupyterlab.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/mariadb.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/nbclassic.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/packs/tutorial_server.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/Dockerfile.jinja2
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/content/content_config.yaml
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/services/sudoers
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/startup/home-dir.sudoers
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/core/startup/start.sh
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/packs/code_server/vscode.svg
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/packs/mariadb/setup.sh
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/ou_container_builder/templates/packs/tutorial-server/production.ini
--rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/demo-tests.sh
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/run-all.sh
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/code_server/ContainerConfig.yaml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/code_server_pinned/ContainerConfig.yaml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/jupyterlab/v3/ContainerConfig.yaml
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/jupyterlab/v4/ContainerConfig.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/mariadb/ContainerConfig.yaml
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/nbclassic/ContainerConfig.yaml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/nbclassic/content/Welcome.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/openrefine/ContainerConfig.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/tutorial_server/ContainerConfig.yaml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/demos/tutorial_server/content/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_content_settings.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_hacks_settings.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_image_settings.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_module_settings.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_packages_settings.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_scripts_settings.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_server_settings.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_sources_settings.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/test_webapps_settings.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/tests/unittests/validator_tests/util.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/.gitignore
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/README.md
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 ou_container_builder-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/Dockerfile
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/prepare_release.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tox.ini
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/activate
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/activate_this.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/pip
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/pip-3.11
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/pip3
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/python -> /usr/bin/python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/wheel
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/wheel-3.11
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/wheel3
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/bin/wheel3.11
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.virtualenv
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18328 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    28722 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    18817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    20435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18442 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    27696 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    32782 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18864 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22216 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    84101 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   275233 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0        0        0   108032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   109388 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    71556 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53572 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    99195 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0    72198 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0   109451 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    80078 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   133344 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    22975 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_normalization.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    19778 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0        0        0   137216 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    21087 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    47046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/glob.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0        0        0   137728 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    47115 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    39968 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/py312compat.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/warnings.py
+-rw-r--r--   0        0        0     8608 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/_log.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0    19616 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    48643 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    17861 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8072 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50174 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17899 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13715 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30188 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    18928 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18099 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22013 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31503 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    30153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19232 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16596 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    87692 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    31965 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    28906 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    13755 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16353 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    26184 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   274907 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/METADATA
+-rw-r--r--   0        0        0    34553 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/__main__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py
+-rw-r--r--   0        0        0    19868 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/bdist_wheel.py
+-rw-r--r--   0        0        0    16143 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/macosx_libfile.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/metadata.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/util.py
+-rw-r--r--   0        0        0     7674 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/wheelfile.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/convert.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/pack.py
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/tags.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/unpack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/vendor.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py
+-rw-r--r--   0        0        0    39047 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/METADATA
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/WHEEL
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/Makefile
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/building.rst
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/conf.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/index.rst
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/installation.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/core.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/index.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/main.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/packs.rst
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/utils.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/validator.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/core/content.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/core/env.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/core/scripts.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/core/services.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/core/web_apps.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/packs/jupyterlab.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/packs/mariadb.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/packs/nbclassic.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/api/packs/tutorial_server.rst
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/content.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/environment.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/flags.rst
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/hacks.rst
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/image.rst
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/index.rst
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/jupyter_server_config.rst
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/module.rst
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/packages.rst
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/packs.rst
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/scripts.rst
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/server.rst
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/services.rst
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/sources.rst
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/configuration/web_apps.rst
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/packs/code-server.rst
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/packs/index.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/packs/jupyterlab.rst
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/packs/mariadb.rst
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/packs/nbclassic.rst
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/docs/packs/tutorial_server.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/__about__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/__main__.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/builder.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/settings.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/utils.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/base.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/content.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/env.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/hacks.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/jupyter_server.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/packages.py
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/scripts.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/services.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/startup.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/core/web_apps.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/packs/__init__.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/packs/code_server.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/packs/jupyterlab.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/packs/mariadb.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/packs/nbclassic.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/packs/tutorial_server.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/Dockerfile.jinja2
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/core/content/content_config.yaml
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/core/services/sudoers
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/core/startup/home-dir.sudoers
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/core/startup/start.sh
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/packs/code_server/vscode.svg
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/packs/mariadb/setup.sh
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/ou_container_builder/templates/packs/tutorial-server/production.ini
+-rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/demo-tests.sh
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/run-all.sh
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/code_server/ContainerConfig.yaml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/code_server_pinned/ContainerConfig.yaml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/jupyterlab/v3/ContainerConfig.yaml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/jupyterlab/v4/ContainerConfig.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/mariadb/ContainerConfig.yaml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/nbclassic/ContainerConfig.yaml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/nbclassic/content/Welcome.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/openrefine/ContainerConfig.yaml
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/tutorial_server/ContainerConfig.yaml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/demos/tutorial_server/content/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_content_settings.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_hacks_settings.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_image_settings.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_module_settings.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_packages_settings.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_scripts_settings.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_server_settings.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_sources_settings.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/test_webapps_settings.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/tests/unittests/validator_tests/util.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/.gitignore
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/README.md
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 ou_container_builder-2.6.1/PKG-INFO
```

### Comparing `ou_container_builder-2.6.0/.gitlab-ci.yml` & `ou_container_builder-2.6.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/CHANGELOG.md` & `ou_container_builder-2.6.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 2.6.1
+
+* **Update**: Update ou_container_launcher to >= 1.2.0
+
 ## 2.6.0
 
 * **New**: Add rustc as a core install
 
 ## 2.5.0
 
 * **Update**: Allow the user to restart any services
```

### Comparing `ou_container_builder-2.6.0/prepare_release.py` & `ou_container_builder-2.6.1/prepare_release.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Script to prepare the version information for a release."""
 import re
 from typing import List
 
-VERSION = "2.5.0"
+VERSION = "2.6.1"
 
 
 def readlines(filename: str) -> list[str]:
     """Read a file as a list of lines."""
     with open(filename) as in_f:
         return in_f.readlines()
 
@@ -25,10 +25,12 @@
             return re.sub(pattern, fr"\g<1>{version}\g<2>", line)
         else:
             return line
 
     writelines(filename, map(replace_version, readlines(filename)))
 
 
-update_version("docs/conf.py", r"(^release = ')[0-9]+\.[0-9]+\.[0-9]+(?:b[0-9]+)?('$)", VERSION)
-update_version("pyproject.toml", r'(^version = ")[0-9]+\.[0-9]+\.[0-9]+(?:b[0-9]+)?("$)', VERSION)
+update_version("docs/conf.py", r'(^release = ")[0-9]+\.[0-9]+\.[0-9]+(?:b[0-9]+)?("$)', VERSION)
+update_version(
+    "ou_container_builder/__about__.py", r'(^__version__ = ")[0-9]+\.[0-9]+\.[0-9]+(?:b[0-9]+)?("$)', VERSION
+)
 update_version("CHANGELOG.md", r"(## )Dev($)", VERSION)
```

### Comparing `ou_container_builder-2.6.0/.venv/bin/activate` & `ou_container_builder-2.6.1/.venv/bin/activate`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/bin/activate.csh` & `ou_container_builder-2.6.1/.venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/bin/activate.fish` & `ou_container_builder-2.6.1/.venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/bin/activate.nu` & `ou_container_builder-2.6.1/.venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/bin/activate.ps1` & `ou_container_builder-2.6.1/.venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/bin/activate_this.py` & `ou_container_builder-2.6.1/.venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_virtualenv.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__main__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cache.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/six.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/METADATA` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/RECORD` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pip-23.1.2.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_imp.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_importlib.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_itertools.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_normalization.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_normalization.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_path.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_reqs.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_reqs.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/archive_util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/build_meta.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-32.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-64.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli-arm64.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/cli.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/dep_util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/depends.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/discovery.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/dist.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/errors.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/extension.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/glob.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-32.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-64.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui-arm64.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/gui.exe` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/installer.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/launch.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/logging.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/monkey.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/msvc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/namespaces.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/package_index.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/sandbox.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/warnings.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/warnings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/windows_support.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/alias.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/develop.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/test.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/expand.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/LICENSE` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/METADATA` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/RECORD` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/entry_points.txt` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/setuptools-67.8.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/bdist_wheel.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/macosx_libfile.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/metadata.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/util.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/wheelfile.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/__init__.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/convert.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/pack.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/tags.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/tags.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/cli/unpack.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/LICENSE.txt` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/METADATA` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/RECORD` & `ou_container_builder-2.6.1/.venv/lib/python3.11/site-packages/wheel-0.40.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/Makefile` & `ou_container_builder-2.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/building.rst` & `ou_container_builder-2.6.1/docs/building.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/conf.py` & `ou_container_builder-2.6.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OU Container Builder"
 copyright = "2021, Mark Hall"  # noqa: A001
 author = "Mark Hall"
 
 # The full version, including alpha/beta/rc tags
-release = "2.5.0"
+release = "2.6.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `ou_container_builder-2.6.0/docs/index.rst` & `ou_container_builder-2.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/make.bat` & `ou_container_builder-2.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/content.rst` & `ou_container_builder-2.6.1/docs/configuration/content.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/environment.rst` & `ou_container_builder-2.6.1/docs/configuration/environment.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/flags.rst` & `ou_container_builder-2.6.1/docs/configuration/flags.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/hacks.rst` & `ou_container_builder-2.6.1/docs/configuration/hacks.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/image.rst` & `ou_container_builder-2.6.1/docs/configuration/image.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/index.rst` & `ou_container_builder-2.6.1/docs/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/jupyter_server_config.rst` & `ou_container_builder-2.6.1/docs/configuration/jupyter_server_config.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/module.rst` & `ou_container_builder-2.6.1/docs/configuration/module.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/packages.rst` & `ou_container_builder-2.6.1/docs/configuration/packages.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/scripts.rst` & `ou_container_builder-2.6.1/docs/configuration/scripts.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/server.rst` & `ou_container_builder-2.6.1/docs/configuration/server.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/services.rst` & `ou_container_builder-2.6.1/docs/configuration/services.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/sources.rst` & `ou_container_builder-2.6.1/docs/configuration/sources.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/configuration/web_apps.rst` & `ou_container_builder-2.6.1/docs/configuration/web_apps.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/packs/code-server.rst` & `ou_container_builder-2.6.1/docs/packs/code-server.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/packs/mariadb.rst` & `ou_container_builder-2.6.1/docs/packs/mariadb.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/docs/packs/tutorial_server.rst` & `ou_container_builder-2.6.1/docs/packs/tutorial_server.rst`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/__main__.py` & `ou_container_builder-2.6.1/ou_container_builder/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/builder.py` & `ou_container_builder-2.6.1/ou_container_builder/builder.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/settings.py` & `ou_container_builder-2.6.1/ou_container_builder/settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/utils.py` & `ou_container_builder-2.6.1/ou_container_builder/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/base.py` & `ou_container_builder-2.6.1/ou_container_builder/core/base.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/content.py` & `ou_container_builder-2.6.1/ou_container_builder/core/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     if "content" in settings and settings["content"]:
         settings = merge_settings(settings, {"flags": {"ou_container_content": True}})
     if "flags" in settings and settings["flags"]:
         if "ou_container_content" in settings["flags"] and settings["flags"]["ou_container_content"]:
             settings = merge_settings(
                 settings,
                 {
-                    "packages": {"pip": ["ou-container-content>=1.1.3"]},
+                    "packages": {"pip": ["ou-container-content>=1.2.0"]},
                     "scripts": {"build": [{"commands": ["ou-container-content prepare"]}]},
                 },
             )
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> None:
```

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/env.py` & `ou_container_builder-2.6.1/ou_container_builder/core/env.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/hacks.py` & `ou_container_builder-2.6.1/ou_container_builder/core/hacks.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/jupyter_server.py` & `ou_container_builder-2.6.1/ou_container_builder/core/jupyter_server.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/packages.py` & `ou_container_builder-2.6.1/ou_container_builder/core/packages.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/scripts.py` & `ou_container_builder-2.6.1/ou_container_builder/core/scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/services.py` & `ou_container_builder-2.6.1/ou_container_builder/core/services.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/startup.py` & `ou_container_builder-2.6.1/ou_container_builder/core/startup.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/core/web_apps.py` & `ou_container_builder-2.6.1/ou_container_builder/core/web_apps.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/packs/code_server.py` & `ou_container_builder-2.6.1/ou_container_builder/packs/code_server.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/packs/jupyterlab.py` & `ou_container_builder-2.6.1/ou_container_builder/packs/jupyterlab.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/packs/mariadb.py` & `ou_container_builder-2.6.1/ou_container_builder/packs/mariadb.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/packs/nbclassic.py` & `ou_container_builder-2.6.1/ou_container_builder/packs/nbclassic.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/packs/tutorial_server.py` & `ou_container_builder-2.6.1/ou_container_builder/packs/tutorial_server.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/templates/Dockerfile.jinja2` & `ou_container_builder-2.6.1/ou_container_builder/templates/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/templates/core/content/content_config.yaml` & `ou_container_builder-2.6.1/ou_container_builder/templates/core/content/content_config.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/templates/packs/code_server/vscode.svg` & `ou_container_builder-2.6.1/ou_container_builder/templates/packs/code_server/vscode.svg`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/templates/packs/mariadb/setup.sh` & `ou_container_builder-2.6.1/ou_container_builder/templates/packs/mariadb/setup.sh`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/ou_container_builder/templates/packs/tutorial-server/production.ini` & `ou_container_builder-2.6.1/ou_container_builder/templates/packs/tutorial-server/production.ini`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/demos/demo-tests.sh` & `ou_container_builder-2.6.1/tests/demos/demo-tests.sh`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml` & `ou_container_builder-2.6.1/tests/demos/custom_apt_key_dearmor/ContainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod` & `ou_container_builder-2.6.1/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf` & `ou_container_builder-2.6.1/tests/demos/custom_apt_key_dearmor/mongodb-org/mongod.conf`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/demos/nbclassic/content/Welcome.ipynb` & `ou_container_builder-2.6.1/tests/demos/nbclassic/content/Welcome.ipynb`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/demos/openrefine/ContainerConfig.yaml` & `ou_container_builder-2.6.1/tests/demos/openrefine/ContainerConfig.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/unittests/validator_tests/test_content_settings.py` & `ou_container_builder-2.6.1/tests/unittests/validator_tests/test_content_settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/unittests/validator_tests/test_image_settings.py` & `ou_container_builder-2.6.1/tests/unittests/validator_tests/test_image_settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/unittests/validator_tests/test_module_settings.py` & `ou_container_builder-2.6.1/tests/unittests/validator_tests/test_module_settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/unittests/validator_tests/test_scripts_settings.py` & `ou_container_builder-2.6.1/tests/unittests/validator_tests/test_scripts_settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/unittests/validator_tests/test_server_settings.py` & `ou_container_builder-2.6.1/tests/unittests/validator_tests/test_server_settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/unittests/validator_tests/test_sources_settings.py` & `ou_container_builder-2.6.1/tests/unittests/validator_tests/test_sources_settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/tests/unittests/validator_tests/test_webapps_settings.py` & `ou_container_builder-2.6.1/tests/unittests/validator_tests/test_webapps_settings.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/README.md` & `ou_container_builder-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/pyproject.toml` & `ou_container_builder-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.6.0/PKG-INFO` & `ou_container_builder-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-container-builder
-Version: 2.6.0
+Version: 2.6.1
 Project-URL: Documentation, https://github.com/unknown/ou-container-builder#readme
 Project-URL: Issues, https://github.com/unknown/ou-container-builder/issues
 Project-URL: Source, https://github.com/unknown/ou-container-builder
 Author-email: Mark Hall <mark.hall@work.room3b.eu>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

