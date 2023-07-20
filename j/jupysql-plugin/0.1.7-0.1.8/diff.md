# Comparing `tmp/jupysql_plugin-0.1.7.tar.gz` & `tmp/jupysql_plugin-0.1.8.tar.gz`

## Comparing `jupysql_plugin-0.1.7.tar` & `jupysql_plugin-0.1.8.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/babel.config.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/environment.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jest.config.js
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/noxfile.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/package.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/setup.cfg
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/setup.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/tsconfig.json
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/doc/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/_version.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/_widgets.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/package.json
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/122.83febd31f97f409ed32e.js
--rw-r--r--   0        0        0   448079 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js.LICENSE.txt
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js
--rw-r--r--   0        0        0    32377 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/238.248c93b1dc2fa4a4015a.js
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js.LICENSE.txt
--rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js
--rw-r--r--   0        0        0    39339 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/40.4f257c905f8cbcacb158.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/40.4f257c905f8cbcacb158.js.LICENSE.txt
--rw-r--r--   0        0        0    60929 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/520.482c287db47780739825.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/520.482c287db47780739825.js.LICENSE.txt
--rw-r--r--   0        0        0   237389 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js
--rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js
--rw-r--r--   0        0        0    23542 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js
--rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js
--rw-r--r--   0        0        0   228074 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js
--rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/remoteEntry.e80d3b8b00f5114eb1bb.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/style.js
--rw-r--r--   0        0        0    42216 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/server_handlers/dashboard.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/widgets/__init__.py
--rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/widgets/connector_widget.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupyter-config/jupyter_notebook_config.d/jupysql_plugin.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupyter-config/jupyter_server_config.d/jupysql_plugin.json
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/comm.ts
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/connector.ts
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/customconnector.ts
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/dialog.tsx
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/extension.ts
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/formatter.ts
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/index-widgets.ts
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/index.ts
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/keywords.json
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/version.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/__tests__/jupysql_plugin.spec.ts
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/const/env.ts
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/utils/util.ts
--rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/widgets/connector.ts
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/widgets/form.ts
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/widgets/table.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/base.css
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/connector.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/index.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/widget.css
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/icons/add_primary.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/icons/delete_outline_black.svg
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/README.md
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/babel.config.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/environment.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jest.config.js
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/noxfile.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/package.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/setup.cfg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/setup.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/tsconfig.json
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/doc/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/_version.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/_widgets.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/package.json
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/122.83febd31f97f409ed32e.js
+-rw-r--r--   0        0        0   448079 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js.LICENSE.txt
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js
+-rw-r--r--   0        0        0    33851 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/238.47dc92159927183c530c.js
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js.LICENSE.txt
+-rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js
+-rw-r--r--   0        0        0    40330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js.LICENSE.txt
+-rw-r--r--   0        0        0    60929 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/520.482c287db47780739825.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/520.482c287db47780739825.js.LICENSE.txt
+-rw-r--r--   0        0        0   237389 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js
+-rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js
+-rw-r--r--   0        0        0    23542 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js
+-rw-r--r--   0        0        0   228074 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js
+-rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/remoteEntry.1515ab0c4408d370a1f1.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/style.js
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/server_handlers/dashboard.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/widgets/__init__.py
+-rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/widgets/connector_widget.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupyter-config/jupyter_notebook_config.d/jupysql_plugin.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupyter-config/jupyter_server_config.d/jupysql_plugin.json
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/comm.ts
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/connector.ts
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/customconnector.ts
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/dialog.tsx
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/extension.ts
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/formatter.ts
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/index-widgets.ts
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/index.ts
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/keywords.json
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/version.ts
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/__tests__/dialog.spec.tsx
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/__tests__/jupysql_plugin.spec.ts
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/const/env.ts
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/utils/util.ts
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/widgets/connector.ts
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/widgets/form.ts
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/widgets/table.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/base.css
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/connector.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/index.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/widget.css
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/icons/add_primary.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/icons/delete_outline_black.svg
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/README.md
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/PKG-INFO
```

### Comparing `jupysql_plugin-0.1.7/RELEASE.md` & `jupysql_plugin-0.1.8/RELEASE.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,17 +17,22 @@
 ```bash
 git tag -a VERSION -m MESSAGE
 git push --tag
 ```
 
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
-*Note:* The following command needs NodeJS
+*Note:* The following command needs NodeJS:
+
 
 ```bash
+# clean files before building
+jlpm clean:all
+
+# build the package
 python -m build
 ```
 
 Then to upload the package to PyPI, do:
 
 ```bash
 twine upload dist/*
```

### Comparing `jupysql_plugin-0.1.7/jest.config.js` & `jupysql_plugin-0.1.8/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/noxfile.py` & `jupysql_plugin-0.1.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/package.json` & `jupysql_plugin-0.1.8/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725188575302992%*

 * *Differences: {"'dependencies'": "{'react': '^17.0.2', 'clean': '^4.0.2'}",*

 * * "'devDependencies'": "{'@testing-library/jest-dom': '^5.16.5', '@testing-library/react': "*

 * *                      "'^12.1.2', '@types/jest-when': '^3.5.2', 'jest-when': '^3.5.2', "*

 * *                      "'react-dom': '^17.0.2'}",*

 * * "'version'": "'0.1.8'"}*

```diff
@@ -23,34 +23,40 @@
         "@jupyterlab/statedb": "^3.6.2",
         "@lumino/widgets": "<2.0.0",
         "@mui/icons-material": "^5.11.16",
         "@mui/material": "^5.13.4",
         "@types/codemirror": "^5.60.7",
         "@types/underscore": "^1.11.4",
         "bootstrap": "^5.2.3",
-        "react": "^18.2.0",
+        "clean": "^4.0.2",
+        "react": "^17.0.2",
         "sql-formatter": "^12.2.0",
         "underscore": "^1.13.6"
     },
     "description": "Jupyterlab extension for JupySQL",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^3.1.0",
         "@jupyterlab/testutils": "^3.0.0",
+        "@testing-library/jest-dom": "^5.16.5",
+        "@testing-library/react": "^12.1.2",
         "@types/bootstrap": "^5.2.6",
         "@types/jest": "^26.0.0",
+        "@types/jest-when": "^3.5.2",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "jest": "^26.0.0",
+        "jest-when": "^3.5.2",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
+        "react-dom": "^17.0.2",
         "rimraf": "^3.0.2",
         "stylelint": "^14.3.0",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^6.0.0",
         "stylelint-config-standard": "~24.0.0",
         "stylelint-prettier": "^2.0.0",
         "ts-jest": "^26.0.0",
@@ -117,15 +123,15 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.7",
+    "version": "0.1.8",
     "workspaces": {
         "packages": [
             "jupysql_plugin",
             "ui-tests"
         ]
     }
 }
```

### Comparing `jupysql_plugin-0.1.7/tsconfig.json` & `jupysql_plugin-0.1.8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/doc/README.md` & `jupysql_plugin-0.1.8/doc/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/__init__.py` & `jupysql_plugin-0.1.8/jupysql_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/_widgets.py` & `jupysql_plugin-0.1.8/jupysql_plugin/_widgets.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/package.json` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9720659589795745%*

 * *Differences: {"'dependencies'": "{'react': '^17.0.2', 'clean': '^4.0.2'}",*

 * * "'devDependencies'": "{'@testing-library/jest-dom': '^5.16.5', '@testing-library/react': "*

 * *                      "'^12.1.2', '@types/jest-when': '^3.5.2', 'jest-when': '^3.5.2', "*

 * *                      "'react-dom': '^17.0.2'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1515ab0c4408d370a1f1.js'}}",*

 * * "'version'": "'0.1.8'"}*

```diff
@@ -23,34 +23,40 @@
         "@jupyterlab/statedb": "^3.6.2",
         "@lumino/widgets": "<2.0.0",
         "@mui/icons-material": "^5.11.16",
         "@mui/material": "^5.13.4",
         "@types/codemirror": "^5.60.7",
         "@types/underscore": "^1.11.4",
         "bootstrap": "^5.2.3",
-        "react": "^18.2.0",
+        "clean": "^4.0.2",
+        "react": "^17.0.2",
         "sql-formatter": "^12.2.0",
         "underscore": "^1.13.6"
     },
     "description": "Jupyterlab extension for JupySQL",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^3.1.0",
         "@jupyterlab/testutils": "^3.0.0",
+        "@testing-library/jest-dom": "^5.16.5",
+        "@testing-library/react": "^12.1.2",
         "@types/bootstrap": "^5.2.6",
         "@types/jest": "^26.0.0",
+        "@types/jest-when": "^3.5.2",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-prettier": "^3.1.4",
         "jest": "^26.0.0",
+        "jest-when": "^3.5.2",
         "npm-run-all": "^4.1.5",
         "prettier": "^2.1.1",
+        "react-dom": "^17.0.2",
         "rimraf": "^3.0.2",
         "stylelint": "^14.3.0",
         "stylelint-config-prettier": "^9.0.4",
         "stylelint-config-recommended": "^6.0.0",
         "stylelint-config-standard": "~24.0.0",
         "stylelint-prettier": "^2.0.0",
         "ts-jest": "^26.0.0",
@@ -60,15 +66,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ploomber/jupysql-plugin.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e80d3b8b00f5114eb1bb.js",
+            "load": "static/remoteEntry.1515ab0c4408d370a1f1.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupysql_plugin/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -122,15 +128,15 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.7",
+    "version": "0.1.8",
     "workspaces": {
         "packages": [
             "jupysql_plugin",
             "ui-tests"
         ]
     }
 }
```

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/238.248c93b1dc2fa4a4015a.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/238.47dc92159927183c530c.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,33 +1,33 @@
 (self.webpackChunkjupysql_plugin = self.webpackChunkjupysql_plugin || []).push([
     [238], {
         3238: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
-                DeployingExtension: () => Z,
-                FormattingExtension: () => K,
-                MODULE_NAME: () => D,
+                DeployingExtension: () => Y,
+                FormattingExtension: () => Z,
+                MODULE_NAME: () => A,
                 MODULE_VERSION: () => L,
-                RegisterNotebookCommListener: () => Y,
-                default: () => Q
+                RegisterNotebookCommListener: () => Q,
+                default: () => X
             });
             var o = {};
             n.r(o), n.d(o, {
-                FormModel: () => R,
-                FormView: () => P
+                FormModel: () => P,
+                FormView: () => q
             });
             var i = {};
             n.r(i), n.d(i, {
-                TableModel: () => F,
-                TableView: () => B
+                TableModel: () => B,
+                TableView: () => U
             });
             var l = {};
             n.r(l), n.d(l, {
-                ConnectorModel: () => H,
-                ConnectorView: () => W
+                ConnectorModel: () => W,
+                ConnectorView: () => V
             });
             var a, s = n(3792),
                 r = n(127),
                 c = n(6548);
             class d extends c.DataConnector {
                 constructor(e) {
                     super(), this._connectors = e
@@ -74,20 +74,20 @@
                         start: o.offset,
                         end: o.offset + o.value.length,
                         matches: l,
                         metadata: {}
                     }
                 }
             }(p || (p = {}));
-            var h = n(9235),
-                v = n(2297),
+            var v = n(9235),
+                h = n(2297),
                 g = n(5923),
                 b = n(6303),
                 y = n(6560);
-            class C {
+            class f {
                 constructor(e) {
                     this.notebookTracker = e
                 }
                 async formatAllCodeCells(e, t, n) {
                     return this.formatCells(!1, e, t, n)
                 }
                 getCodeCells(e = !0, t) {
@@ -125,16 +125,16 @@
                     }
                 }
                 applicable(e, t) {
                     const n = this.notebookTracker.currentWidget;
                     return n && t === n
                 }
             }
-            var f = n(6271),
-                w = n.n(f),
+            var C = n(6271),
+                w = n.n(C),
                 E = n(6319),
                 _ = n(9418);
             var k = n(344),
                 x = n(5139);
             async function T(e = "", t = {}) {
                 const n = x.ServerConnection.makeSettings(),
                     o = k.URLExt.join(n.baseUrl, "dashboard", e);
@@ -150,236 +150,254 @@
                 } catch (e) {
                     console.log("Not a JSON response body.", i)
                 }
                 if (!i.ok) throw new x.ServerConnection.ResponseError(i, l.message || l);
                 return l
             }
             const N = e => {
-                var t, n;
-                const o = e.notebook_path,
-                    [i] = (0, f.useState)((null === (n = null === (t = null == e ? void 0 : e.metadata) || void 0 === t ? void 0 : t.get("ploomber")) || void 0 === n ? void 0 : n.project_id) || ""),
-                    [l, a] = (0, f.useState)(!0),
-                    [s, r] = (0, f.useState)(!1),
-                    [c, d] = (0, f.useState)(!1),
-                    [u, m] = (0, f.useState)(!1),
-                    [p, h] = (0, f.useState)(""),
-                    [v, g] = (0, f.useState)(null),
-                    [b, y] = (0, f.useState)("init"),
-                    [C, k] = (0, f.useState)("");
-                (0, f.useEffect)((() => {
-                    x()
-                }), []), (0, f.useEffect)((() => {
-                    "success" === b && (i ? (m(!1), N()) : m(!0))
-                }), [b]);
-                const x = async () => {
-                    await T("apikey").then((e => {
-                        null != (null == e ? void 0 : e.data) && (h(e.data), y("success"))
-                    })).catch((e => {
-                        console.error(`The jupyterlab_examples_server server extension appears to be missing.\n${e}`)
-                    })), a(!1)
-                }, N = async () => {
-                    r(!0);
-                    const t = {
-                        notebook_path: o,
-                        api_key: p,
-                        project_id: i
+                    var t, n, o, i, l, a;
+                    return "missing file" == (null === (t = null == e ? void 0 : e.message) || void 0 === t ? void 0 : t.type) ? w().createElement("div", {
+                        "data-testid": "error-message-area"
+                    }, w().createElement(E.Typography, {
+                        variant: "subtitle1",
+                        gutterBottom: !0
+                    }, " A ", w().createElement("code", null, null === (o = null === (n = null == e ? void 0 : e.message) || void 0 === n ? void 0 : n.detail) || void 0 === o ? void 0 : o.fileName), " file with dependencies is required to deploy your notebook. Please add it at ", w().createElement("code", null, null === (l = null === (i = null == e ? void 0 : e.message) || void 0 === i ? void 0 : i.detail) || void 0 === l ? void 0 : l.filePath), ". To learn more, see the ", w().createElement("a", {
+                        target: "_blank",
+                        rel: "noopener noreferrer",
+                        href: "https://docs.cloud.ploomber.io/en/latest/dashboards/jupyterlab-plugin.html#create-sample-notebook-and-requirements-txt"
+                    }, "docs"))) : w().createElement(E.Typography, {
+                        variant: "subtitle1",
+                        gutterBottom: !0
+                    }, null === (a = null == e ? void 0 : e.message) || void 0 === a ? void 0 : a.detail)
+                },
+                S = e => {
+                    var t, n;
+                    const o = e.notebook_path,
+                        [i] = (0, C.useState)((null === (n = null === (t = null == e ? void 0 : e.metadata) || void 0 === t ? void 0 : t.get("ploomber")) || void 0 === n ? void 0 : n.project_id) || ""),
+                        [l, a] = (0, C.useState)(!0),
+                        [s, r] = (0, C.useState)(!1),
+                        [c, d] = (0, C.useState)(!1),
+                        [u, m] = (0, C.useState)(!1),
+                        [p, v] = (0, C.useState)(""),
+                        [h, g] = (0, C.useState)(""),
+                        [b, y] = (0, C.useState)("init"),
+                        [f, k] = (0, C.useState)(null),
+                        [x, S] = (0, C.useState)("");
+                    (0, C.useEffect)((() => {
+                        j()
+                    }), []), (0, C.useEffect)((() => {
+                        "success" === b && (i ? (m(!1), O()) : m(!0))
+                    }), [b]);
+                    const j = async () => {
+                        await T("apikey").then((e => {
+                            null != (null == e ? void 0 : e.data) && (v(e.data), y("success"))
+                        })).catch((e => {
+                            console.error(`The jupyterlab_examples_server server extension appears to be missing.\n${e}`)
+                        })), a(!1)
+                    }, O = async () => {
+                        r(!0);
+                        const t = {
+                            notebook_path: o,
+                            api_key: p,
+                            project_id: i
+                        };
+                        await T("job", {
+                            body: JSON.stringify(t),
+                            method: "POST"
+                        }).then((t => {
+                            var n, o, i = t.deployment_result,
+                                l = {
+                                    type: "generic",
+                                    detail: ""
+                                };
+                            "missing file" === (null == i ? void 0 : i.type) && (null == i ? void 0 : i.detail) ? (l.type = i.type, l.detail = {
+                                fileName: "requirements.txt",
+                                filePath: i.detail
+                            }, k(l)) : (null == i ? void 0 : i.detail) || (null == i ? void 0 : i.message) ? (l.detail = i.detail || i.message, k(l)) : (g("https://platform.ploomber.io/dashboards/" + (null == i ? void 0 : i.project_id) + "/" + (null == i ? void 0 : i.id)), null === (n = null == e ? void 0 : e.metadata) || void 0 === n || n.set("ploomber", {
+                                project_id: null == i ? void 0 : i.project_id
+                            }), null === (o = null == e ? void 0 : e.context) || void 0 === o || o.save())
+                        })), r(!1)
+                    }, D = {
+                        init: {
+                            label: "API Key",
+                            variant: "outlined",
+                            color: "primary"
+                        },
+                        success: {
+                            label: "Valid API Key",
+                            variant: "filled",
+                            color: "success"
+                        },
+                        error: {
+                            label: "Please enter valid API Key",
+                            variant: "filled",
+                            color: "warning"
+                        }
                     };
-                    await T("job", {
-                        body: JSON.stringify(t),
-                        method: "POST"
-                    }).then((t => {
-                        var n = t.deployment_result;
-                        if (n.detail || n.message) {
-                            var o = n.detail || n.message;
-                            k(o)
-                        } else g("https://platform.ploomber.io/dashboards/" + n.project_id + "/" + n.id), null == e || e.metadata.set("ploomber", {
-                            project_id: n.project_id
-                        }), e.context.save()
-                    })).catch((e => {
-                        k(e)
-                    })), r(!1)
-                }, S = {
-                    init: {
-                        label: "API Key",
+                    return w().createElement(E.Box, {
+                        p: 6,
+                        style: {
+                            width: 600
+                        }
+                    }, l || s ? w().createElement(E.Box, {
+                        sx: {
+                            display: "flex",
+                            justifyContent: "center",
+                            alignItems: "center"
+                        }
+                    }, w().createElement(E.CircularProgress, null)) : w().createElement(w().Fragment, null, w().createElement(E.Grid, {
+                        container: !0,
+                        spacing: 4,
+                        alignItems: "center",
+                        direction: "column"
+                    }, "success" !== b && w().createElement("div", null, w().createElement(E.Grid, {
+                        item: !0,
+                        container: !0,
+                        direction: "row",
+                        alignItems: "center",
+                        width: "100%"
+                    }, w().createElement(E.Grid, {
+                        container: !0,
+                        direction: "row",
+                        alignItems: "center",
+                        spacing: 1
+                    }, w().createElement(E.Grid, {
+                        item: !0,
+                        xs: 10
+                    }, w().createElement(E.TextField, {
+                        id: "api-key-input",
+                        size: "small",
+                        onChange: e => {
+                            v(e.target.value)
+                        },
+                        value: p,
+                        label: D[b].label,
+                        variant: D[b].variant,
+                        color: D[b].color,
+                        error: "error" == b,
+                        fullWidth: !0,
+                        focused: !0
+                    })), w().createElement(E.Grid, {
+                        item: !0,
+                        xs: 2,
+                        alignItems: "center",
+                        justifyContent: "center"
+                    }, w().createElement(E.Button, {
+                        onClick: async () => {
+                            a(!0);
+                            const e = {
+                                api_key: p
+                            };
+                            await T("apikey", {
+                                body: JSON.stringify(e),
+                                method: "POST"
+                            }).then((e => {
+                                "success" == (null == e ? void 0 : e.result) ? y("success"): y("error")
+                            })).catch((t => {
+                                console.error(`Error on POST ${e}.\n${t}`)
+                            })), a(!1)
+                        },
+                        variant: "contained",
+                        size: "small"
+                    }, "CONFIRM")))), w().createElement(E.Grid, {
+                        item: !0,
+                        container: !0,
+                        direction: "row",
+                        alignItems: "center",
+                        width: "100%"
+                    }, w().createElement(E.Link, {
+                        href: "https://www.platform.ploomber.io/register/",
+                        target: "_blank",
+                        rel: "noopener noreferrer"
+                    }, "Click here to get an API Key"))), "success" == b && w().createElement(E.Grid, {
+                        item: !0,
+                        container: !0,
+                        alignItems: "center",
+                        spacing: 4,
+                        direction: "column"
+                    }, u ? w().createElement(w().Fragment, null, w().createElement(w().Fragment, null, w().createElement(E.Typography, {
+                        variant: "subtitle1",
+                        gutterBottom: !0
+                    }, "Clicking on deploy will upload your notebook to Ploomber Cloud servers"), w().createElement(E.Button, {
+                        onClick: async () => {
+                            m(!1), await O()
+                        },
+                        variant: "contained",
+                        size: "small",
+                        color: "primary",
+                        disabled: "" !== h,
+                        endIcon: w().createElement(_.Z, null)
+                    }, "CONFIRM "))) : w().createElement(w().Fragment, null, f ? w().createElement(N, {
+                        message: f
+                    }) : w().createElement(w().Fragment, null, w().createElement(E.Grid, {
+                        item: !0,
+                        justifyContent: "center",
+                        xs: 12
+                    }, "Check your deployment status here:"), w().createElement(E.Grid, {
+                        item: !0,
+                        justifyContent: "center",
+                        xs: 12
+                    }, w().createElement(E.Chip, {
+                        label: h,
                         variant: "outlined",
-                        color: "primary"
-                    },
-                    success: {
-                        label: "Valid API Key",
-                        variant: "filled",
-                        color: "success"
-                    },
-                    error: {
-                        label: "Please enter valid API Key",
-                        variant: "filled",
-                        color: "warning"
-                    }
+                        onClick: () => {
+                            window.open(h), d(!0), S("Deployment Success")
+                        }
+                    }), w().createElement(E.Snackbar, {
+                        open: c,
+                        onClose: () => d(!1),
+                        autoHideDuration: 2e3,
+                        message: x
+                    }))))))))
                 };
-                return w().createElement(E.Box, {
-                    p: 6,
-                    style: {
-                        width: 600
-                    }
-                }, l || s ? w().createElement(E.Box, {
-                    sx: {
-                        display: "flex",
-                        justifyContent: "center",
-                        alignItems: "center"
-                    }
-                }, w().createElement(E.CircularProgress, null)) : w().createElement(w().Fragment, null, w().createElement(E.Grid, {
-                    container: !0,
-                    spacing: 4,
-                    alignItems: "center",
-                    direction: "column"
-                }, "success" !== b && w().createElement("div", null, w().createElement(E.Grid, {
-                    item: !0,
-                    container: !0,
-                    direction: "row",
-                    alignItems: "center",
-                    width: "100%"
-                }, w().createElement(E.Grid, {
-                    container: !0,
-                    direction: "row",
-                    alignItems: "center",
-                    spacing: 1
-                }, w().createElement(E.Grid, {
-                    item: !0,
-                    xs: 10
-                }, w().createElement(E.TextField, {
-                    id: "api-key",
-                    size: "small",
-                    onChange: e => {
-                        h(e.target.value)
-                    },
-                    value: p,
-                    label: S[b].label,
-                    variant: S[b].variant,
-                    color: S[b].color,
-                    error: "error" == b,
-                    fullWidth: !0,
-                    focused: !0
-                })), w().createElement(E.Grid, {
-                    item: !0,
-                    xs: 2,
-                    alignItems: "center",
-                    justifyContent: "center"
-                }, w().createElement(E.Button, {
-                    onClick: async () => {
-                        a(!0);
-                        const e = {
-                            api_key: p
-                        };
-                        await T("apikey", {
-                            body: JSON.stringify(e),
-                            method: "POST"
-                        }).then((e => {
-                            y("success")
-                        })).catch((t => {
-                            console.error(`Error on POST ${e}.\n${t}`)
-                        })), a(!1)
-                    },
-                    variant: "contained",
-                    size: "small"
-                }, "CONFIRM")))), w().createElement(E.Grid, {
-                    item: !0,
-                    container: !0,
-                    direction: "row",
-                    alignItems: "center",
-                    width: "100%"
-                }, w().createElement(E.Link, {
-                    href: "https://www.platform.ploomber.io/register/",
-                    target: "_blank",
-                    rel: "noopener noreferrer"
-                }, "Click here to get an API Key"))), "success" == b && w().createElement(E.Grid, {
-                    item: !0,
-                    container: !0,
-                    alignItems: "center",
-                    spacing: 4,
-                    direction: "column"
-                }, u ? w().createElement(w().Fragment, null, w().createElement(w().Fragment, null, w().createElement(E.Typography, {
-                    variant: "subtitle1",
-                    gutterBottom: !0
-                }, "Clicking on deploy will upload your notebook to Ploomber Cloud servers"), w().createElement(E.Button, {
-                    onClick: async () => {
-                        m(!1), await N()
-                    },
-                    variant: "contained",
-                    size: "small",
-                    color: "primary",
-                    disabled: v,
-                    endIcon: w().createElement(_.Z, null)
-                }, "CONFIRM "))) : w().createElement(w().Fragment, null, C ? w().createElement(E.Typography, {
-                    variant: "subtitle1",
-                    gutterBottom: !0
-                }, C) : w().createElement(w().Fragment, null, w().createElement(E.Grid, {
-                    item: !0,
-                    justifyContent: "center",
-                    xs: 12
-                }, "Check your deployment status here:"), w().createElement(E.Grid, {
-                    item: !0,
-                    justifyContent: "center",
-                    xs: 12
-                }, w().createElement(E.Chip, {
-                    label: v,
-                    variant: "outlined",
-                    onClick: () => {
-                        navigator.clipboard.writeText(v), d(!0)
-                    }
-                }), w().createElement(E.Snackbar, {
-                    open: c,
-                    onClose: () => d(!1),
-                    autoHideDuration: 2e3,
-                    message: "Copied to clipboard"
-                }))))))))
-            };
-            class S extends b.ReactWidget {
+            class j extends b.ReactWidget {
                 constructor(e) {
                     super(), this.state = {
                         notebookPath: e.notebookPath,
                         metadata: e.metadata,
                         context: e.context
                     }
                 }
                 render() {
-                    return w().createElement(N, {
+                    return w().createElement(S, {
                         notebook_path: this.state.notebookPath,
                         metadata: this.state.metadata,
                         context: this.state.context
                     })
                 }
             }
-            var j = n(2673);
-            const O = n(4147),
-                L = O.version,
-                D = O.name;
+            var O = n(2673);
+            const D = n(4147),
+                L = D.version,
+                A = D.name;
             var M = n(3379),
-                A = n.n(M),
-                I = n(7517);
-            A()(I.Z, {
+                I = n.n(M),
+                R = n(7517);
+            I()(R.Z, {
                 insert: "head",
                 singleton: !1
-            }), I.Z.locals;
-            class R extends j.DOMWidgetModel {
+            }), R.Z.locals;
+            class P extends O.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: R.model_name,
-                        _model_module: R.model_module,
-                        _model_module_version: R.model_module_version,
-                        _view_name: R.view_name,
-                        _view_module: R.view_module,
-                        _view_module_version: R.view_module_version,
+                        _model_name: P.model_name,
+                        _model_module: P.model_module,
+                        _model_module_version: P.model_module_version,
+                        _view_name: P.view_name,
+                        _view_module: P.view_module,
+                        _view_module_version: P.view_module_version,
                         value: "Hello World"
                     }
                 }
             }
-            R.serializers = {
-                ...j.DOMWidgetModel.serializers
-            }, R.model_name = "FormModel", R.model_module = D, R.model_module_version = L, R.view_name = "FormView", R.view_module = D, R.view_module_version = L;
-            class P extends j.DOMWidgetView {
+            P.serializers = {
+                ...O.DOMWidgetModel.serializers
+            }, P.model_name = "FormModel", P.model_module = A, P.model_module_version = L, P.view_name = "FormView", P.view_module = A, P.view_module_version = L;
+            class q extends O.DOMWidgetView {
                 render() {
                     this.el.classList.add("custom-widget"), this.el.innerHTML = '\n        <form id="myForm">\n        <label for="protocol">Select a protocol:</label>\n        <select id="protocol" name="protocol">\n          <option value="HTTP">HTTP</option>\n          <option value="HTTPS">HTTPS</option>\n        </select>\n      \n        <label for="port">Enter a port:</label>\n        <input type="number" id="port" name="port">\n\n        <div id="confirmationMessage"></div>\n      \n        <button type="submit">Submit</button>\n      </form>\n      \n', this.el.querySelector("#myForm").addEventListener("submit", this.handleFormSubmit.bind(this)), this.model.on("msg:custom", this.handleMessage.bind(this))
                 }
                 handleFormSubmit(e) {
                     e.preventDefault();
                     const t = e.target,
                         n = new FormData(t),
@@ -398,33 +416,33 @@
                     if ("display_confirmation_message" === e.method) {
                         const t = this.el.querySelector("#confirmationMessage");
                         t && (t.textContent = e.message)
                     }
                 }
             }
             n(4039);
-            var q = n(9982);
-            class F extends j.DOMWidgetModel {
+            var F = n(9982);
+            class B extends O.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: F.model_name,
-                        _model_module: F.model_module,
-                        _model_module_version: F.model_module_version,
-                        _view_name: F.view_name,
-                        _view_module: F.view_module,
-                        _view_module_version: F.view_module_version,
+                        _model_name: B.model_name,
+                        _model_module: B.model_module,
+                        _model_module_version: B.model_module_version,
+                        _view_name: B.view_name,
+                        _view_module: B.view_module,
+                        _view_module_version: B.view_module_version,
                         value: "Hello World"
                     }
                 }
             }
-            F.serializers = {
-                ...j.DOMWidgetModel.serializers
-            }, F.model_name = "TableModel", F.model_module = D, F.model_module_version = L, F.view_name = "TableView", F.view_module = D, F.view_module_version = L;
-            class B extends j.DOMWidgetView {
+            B.serializers = {
+                ...O.DOMWidgetModel.serializers
+            }, B.model_name = "TableModel", B.model_module = A, B.model_module_version = L, B.view_name = "TableView", B.view_module = A, B.view_module_version = L;
+            class U extends O.DOMWidgetView {
                 render() {
                     const e = [{
                         symbol: "AAPL",
                         price: 142.34,
                         change: 1.25
                     }, {
                         symbol: "GOOGL",
@@ -438,44 +456,44 @@
                         symbol: "AMZN",
                         price: 3310.98,
                         change: -7.92
                     }];
                     this.el.innerHTML = `\n      <table class="table">\n        <thead>\n          <tr>\n            <th data-bs-toggle="tooltip" data-bs-placement="top" title="symbol">Symbol</th>\n            <th data-bs-toggle="tooltip" data-bs-placement="top" title="price">Price</th>\n            <th data-bs-toggle="tooltip" data-bs-placement="top" title="change">Change</th>\n          </tr>\n        </thead>\n        <tbody>\n          ${e.map((e=>`\n            <tr>\n              <td>${e.symbol}</td>\n              <td>${e.price}</td>\n              <td>${e.change}</td>\n            </tr>\n          `)).join("")}\n        </tbody>\n      </table>\n    `, Array.from(this.el.querySelectorAll('[data-bs-toggle="tooltip"]')).forEach((t => {
                         const n = t.getAttribute("title"),
                             o = e.map((e => e[n])).join(", ");
-                        new q.Tooltip(t, {
+                        new F.Tooltip(t, {
                             title: o
                         })
                     }))
                 }
             }
-            var U = n(9889);
-            A()(U.Z, {
+            var H = n(9889);
+            I()(H.Z, {
                 insert: "head",
                 singleton: !1
-            }), U.Z.locals;
-            class H extends j.DOMWidgetModel {
+            }), H.Z.locals;
+            class W extends O.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: H.model_name,
-                        _model_module: H.model_module,
-                        _model_module_version: H.model_module_version,
-                        _view_name: H.view_name,
-                        _view_module: H.view_module,
-                        _view_module_version: H.view_module_version,
-                        connections: H.connections,
-                        connections_templates: H.connections_templates
+                        _model_name: W.model_name,
+                        _model_module: W.model_module,
+                        _model_module_version: W.model_module_version,
+                        _view_name: W.view_name,
+                        _view_module: W.view_module,
+                        _view_module_version: W.view_module_version,
+                        connections: W.connections,
+                        connections_templates: W.connections_templates
                     }
                 }
             }
-            H.serializers = {
-                ...j.DOMWidgetModel.serializers
-            }, H.model_name = "ConnectorModel", H.model_module = D, H.model_module_version = L, H.view_name = "ConnectorModel", H.view_module = D, H.view_module_version = L, H.connections = [], H.connections_templates = [];
-            class W extends j.DOMWidgetView {
+            W.serializers = {
+                ...O.DOMWidgetModel.serializers
+            }, W.model_name = "ConnectorModel", W.model_module = A, W.model_module_version = L, W.view_name = "ConnectorModel", W.view_module = A, W.view_module_version = L, W.connections = [], W.connections_templates = [];
+            class V extends O.DOMWidgetView {
                 constructor() {
                     super(...arguments), this.connections = JSON.parse(this.model.get("connections")), this.connectionsTemplates = JSON.parse(this.model.get("connections_templates")), this.activeConnection = ""
                 }
                 render() {
                     this.el.classList.add("connector-widget"), this.drawConnectorUI(this.connections), this.model.on("msg:custom", this.handleMessage.bind(this))
                 }
                 drawConnectorUI(e) {
@@ -616,24 +634,24 @@
                     t.innerText = "Connected", t.classList.add("primary")
                 }
                 showErrorMessage(e) {
                     const t = this.el.querySelector(".user-error-message");
                     t.querySelector("pre").innerHTML = `${e}`, t.style.display = "block"
                 }
             }
-            const V = {
+            const J = {
                 ...o,
                 ...i,
                 ...l
             };
-            var J;
+            var z;
             ! function(e) {
                 e.invoke = "completer:invoke", e.invokeNotebook = "completer:invoke-notebook", e.select = "completer:select", e.selectNotebook = "completer:select-notebook"
-            }(J || (J = {}));
-            const z = {
+            }(z || (z = {}));
+            const $ = {
                 id: "completer",
                 autoStart: !0,
                 requires: [s.ICompletionManager, r.INotebookTracker],
                 activate: async (e, t, n) => {
                     console.log("JupyterLab extension jupysql-plugin is activated!"), n.widgetAdded.connect(((e, n) => {
                         var o, i;
                         let l = null !== (i = null === (o = n.content.activeCell) || void 0 === o ? void 0 : o.editor) && void 0 !== i ? i : null;
@@ -646,77 +664,77 @@
                             },
                             u = new d([]),
                             p = t.register({
                                 connector: u,
                                 editor: l,
                                 parent: n
                             }),
-                            h = () => {
+                            v = () => {
                                 var e, t;
                                 l = null !== (t = null === (e = n.content.activeCell) || void 0 === e ? void 0 : e.editor) && void 0 !== t ? t : null, c.session = n.sessionContext.session, c.sessionContext = n.sessionContext, c.editor = l, p.editor = l;
                                 const o = new s.KernelConnector(c),
                                     i = new s.ContextConnector(c),
                                     a = new m(c);
                                 p.connector = new d([o, i, a])
                             };
-                        n.content.activeCellChanged.connect(h), n.sessionContext.sessionChanged.connect(h)
-                    })), e.commands.addCommand(J.invokeNotebook, {
+                        n.content.activeCellChanged.connect(v), n.sessionContext.sessionChanged.connect(v)
+                    })), e.commands.addCommand(z.invokeNotebook, {
                         execute: () => {
                             var t;
                             const o = n.currentWidget;
-                            if (o && "code" === (null === (t = o.content.activeCell) || void 0 === t ? void 0 : t.model.type)) return e.commands.execute(J.invoke, {
+                            if (o && "code" === (null === (t = o.content.activeCell) || void 0 === t ? void 0 : t.model.type)) return e.commands.execute(z.invoke, {
                                 id: o.id
                             })
                         }
-                    }), e.commands.addCommand(J.selectNotebook, {
+                    }), e.commands.addCommand(z.selectNotebook, {
                         execute: () => {
                             const t = n.currentWidget && n.currentWidget.id;
-                            if (t) return e.commands.execute(J.select, {
+                            if (t) return e.commands.execute(z.select, {
                                 id: t
                             })
                         }
                     }), e.commands.addKeyBinding({
-                        command: J.selectNotebook,
+                        command: z.selectNotebook,
                         keys: ["Enter"],
                         selector: ".jp-Notebook .jp-mod-completer-active"
                     })
                 }
             };
-            class $ {
+            class G {
                 constructor(e, t, n) {
                     var o, i;
                     this.app = e, this.tracker = t, this.code_mirror = n, null === (i = null === (o = this.tracker) || void 0 === o ? void 0 : o.activeCellChanged) || void 0 === i || i.connect((() => {
                         var e;
                         if (null !== (null === (e = this.tracker) || void 0 === e ? void 0 : e.activeCell)) {
                             const e = this.tracker.activeCell;
                             if (null !== e && "code" === (null == e ? void 0 : e.model.type)) {
                                 const t = null == e ? void 0 : e.editor,
-                                    n = v.debounce((() => {
+                                    n = h.debounce((() => {
                                         var e;
                                         const n = null === (e = t.getLine(t.firstLine())) || void 0 === e ? void 0 : e.trim();
                                         (null == n ? void 0 : n.startsWith("%%sql")) ? t.editor.setOption("mode", "text/x-sql"): t.editor.setOption("mode", "text/x-ipython")
                                     }), 300);
                                 t.editor.on("change", n), n()
                             }
                         }
                     }))
                 }
             }
-            const G = {
+            const K = {
                 id: "@ploomber/sql-syntax-highlighting",
                 autoStart: !0,
-                requires: [r.INotebookTracker, h.ICodeMirror],
+                requires: [r.INotebookTracker, v.ICodeMirror],
                 optional: [],
                 activate: function(e, t, n) {
-                    new $(e, t, n), console.log("SQLCodeMirror loaded.")
+                    new G(e, t, n), console.log("SQLCodeMirror loaded.")
                 }
             };
-            class K {
+            class Z {
                 constructor(e) {
-                    this.notebookCodeFormatter = new C(e)
+                    this.notebookCodeFormatter = new f(e)
                 }
                 createNew(e, t) {
                     const n = new b.ToolbarButton({
                         className: "format-sql-button",
                         label: "Format SQL",
                         onClick: () => {
                             this.notebookCodeFormatter.formatAllCodeCells(void 0, void 0, e.content)
@@ -724,34 +742,34 @@
                         tooltip: "Format all %%sql cells"
                     });
                     return n.node.setAttribute("data-testid", "format-btn"), e.toolbar.insertItem(10, "formatSQL", n), new g.DisposableDelegate((() => {
                         n.dispose()
                     }))
                 }
             }
-            class Z {
+            class Y {
                 constructor() {}
                 createNew(e, t) {
                     const n = new b.ToolbarButton({
                         className: "deploy-nb-button",
                         label: "Deploy Notebook",
                         onClick: () => {
                             ! function(e, t) {
-                                const n = new S({
+                                const n = new j({
                                     notebookPath: e.context.contentsModel.path,
                                     metadata: e.model.metadata,
                                     context: t
                                 });
                                 new b.Dialog({
                                     title: "Deploy Notebook",
                                     body: n,
                                     buttons: [{
-                                        label: "Cancel",
+                                        label: "Close",
                                         caption: "",
-                                        className: "",
+                                        className: "bg-info",
                                         accept: !1,
                                         actions: [],
                                         displayType: "default",
                                         iconClass: "",
                                         iconLabel: ""
                                     }]
                                 }).launch()
@@ -760,15 +778,15 @@
                         tooltip: "Deploy Notebook as dashboards"
                     });
                     return n.node.setAttribute("data-testid", "deploy-btn"), e.toolbar.insertItem(10, "deployNB", n), new g.DisposableDelegate((() => {
                         n.dispose()
                     }))
                 }
             }
-            class Y {
+            class Q {
                 createNew(e, t) {
                     return setTimeout((() => {
                         (e => {
                             var t;
                             const n = null === (t = e.sessionContext.session) || void 0 === t ? void 0 : t.kernel;
                             n && document.addEventListener("onUpdateTableWidget", (async e => {
                                 const t = e.detail.data,
@@ -786,38 +804,38 @@
                                     document.body.dispatchEvent(n)
                                 }
                             }))
                         })(t)
                     }), 5e3), new g.DisposableDelegate((() => {}))
                 }
             }
-            const Q = [z, G, {
+            const X = [$, K, {
                 activate: (e, t) => {
-                    e.docRegistry.addWidgetExtension("Notebook", new K(t)), e.docRegistry.addWidgetExtension("Notebook", new Z), e.docRegistry.addWidgetExtension("Notebook", new Y)
+                    e.docRegistry.addWidgetExtension("Notebook", new Z(t)), e.docRegistry.addWidgetExtension("Notebook", new Y), e.docRegistry.addWidgetExtension("Notebook", new Q)
                 },
                 autoStart: !0,
                 id: "formatting",
                 requires: [r.INotebookTracker]
             }, {
                 id: "jupysql-plugin:plugin",
-                requires: [j.IJupyterWidgetRegistry],
+                requires: [O.IJupyterWidgetRegistry],
                 activate: function(e, t) {
                     t.registerWidget({
-                        name: D,
+                        name: A,
                         version: L,
-                        exports: V
+                        exports: J
                     })
                 },
                 autoStart: !0
             }]
         },
         9889: (e, t, n) => {
             "use strict";
             n.d(t, {
-                Z: () => h
+                Z: () => v
             });
             var o = n(3645),
                 i = n.n(o),
                 l = n(1667),
                 a = n.n(l),
                 s = n(9941),
                 r = n.n(s),
@@ -825,15 +843,15 @@
                 d = n.n(c),
                 u = i()((function(e) {
                     return e[1]
                 })),
                 m = a()(r()),
                 p = a()(d());
             u.push([e.id, ":root {\n    --danger: #f53649;\n    --white: #ffffff;\n    --margin: 10px;\n    --primary: #206eef;\n  }\n\n.connector-widget .connection-button-container .connection-button-actions {\n    display: inline-flex;\n    width: 100%;\n}\n\n.connector-widget #connectionsButtonsContainer {\n    display: grid;\n}\n\n.connector-widget .connection-button-container .delete-connection-button {\n    margin-left: 10px;\n    background-repeat: no-repeat;\n    background-size: 24px;\n    background-position: center;\n    background-image: url(" + m + ");\n    background-color: transparent;\n    border: none;\n    width: 24px;\n}\n\n.create-new-connection {\n    display: inline-flex;\n    color: var(--primary)\n}\n\n.create-new-connection:hover {\n    cursor: pointer;\n}\n\n.create-new-connection .icon{\n    background-image: url(" + p + ");\n    min-width: 30px;\n    height: 30px;\n    background-repeat: no-repeat;\n    background-size: 15px;\n    background-position: center;\n    background-color: transparent;\n    margin: 0;    \n}\n\n.create-new-connection div {\n    margin: auto var(--margin);\n    margin-top: 2px;\n}\n\n.create-new-connection div:nth-child(2) {\n    margin-left: 2px;\n}\n\n.connector-widget .connection-button-container {\n    margin: var(--margin) 0;\n}\n\n.connector-widget hr.divider {\n    margin: 0;\n    margin-top:20px;\n}\n\n.connector-widget button {\n    width: fit-content;\n    border: none;\n    padding: 5px 10px;\n    border: 1px solid transparent;\n    border-radius: 5px;\n}\n\n.connector-widget button.secondary {\n    background-color: transparent;\n    border: 1px solid var(--primary);\n    color: var(--primary);\n}\n\n.connector-widget button.primary {\n    background-color: var(--primary);\n    color: #fff;\n    border: 1px solid var(--primary);\n}\n\n.connector-widget .connection-button-actions .connection-name {\n    margin: auto 30px;\n    margin-left: 0;\n    width: 100%;\n    font-weight: 500;\n}\n\nbutton.danger {\n    background-color: var(--danger);\n    color: var(--white);\n    margin-left: var(--margin);\n}\n\nform#connectionForm .field-container {\n    display: inline-flex;\n    width: 100%;\n    margin: var(--margin) 0;\n}\n\nform#connectionForm label {\n    width: 50%;\n    margin: auto 0;\n}\n\nform#connectionForm .field {\n    width: -webkit-fill-available;\n    margin-left: var(--margin);\n    padding: 5px 10px;\n}\n\nform#connectionForm input:not(input[type='submit']) {\n    /* margin: 10px;\n    padding: 5px 10px; */\n}\n\n#selectConnection {\n    width: 100%;\n    padding: 6px 10px;\n    margin-bottom: var(--margin);\n}\n\n.warning-message {\n    margin-bottom: var(--margin);\n}\n\n.block {\n    margin: 30px 0px;\n    /* border: 1px solid #000; */\n    width: 600px;\n}\n\nform#connectionForm .buttons-container {\n    text-align: right;\n    margin: var(--margin) 0;\n}\n\nform#connectionForm .buttons-container button:first-child {\n    margin-right: var(--margin);\n}", ""]);
-            const h = u
+            const v = u
         },
         7517: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => l
             });
             var o = n(3645),
@@ -847,11 +865,11 @@
             e.exports = "data:image/svg+xml,%3Csvg width='14' height='14' viewBox='0 0 14 14' fill='none' xmlns='http://www.w3.org/2000/svg'%3E %3Cpath d='M14 8H8V14H6V8H0V6H6V0H8V6H14V8Z' fill='%23206EEF'/%3E %3C/svg%3E"
         },
         9941: e => {
             e.exports = "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' height='24px' viewBox='0 0 24 24' width='24px' fill='%23000000'%3E%3Cpath d='M0 0h24v24H0V0z' fill='none'/%3E%3Cpath d='M6 19c0 1.1.9 2 2 2h8c1.1 0 2-.9 2-2V7H6v12zM8 9h8v10H8V9zm7.5-5l-1-1h-5l-1 1H5v2h14V4z'/%3E%3C/svg%3E"
         },
         4147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"jupysql-plugin","version":"0.1.7","description":"Jupyterlab extension for JupySQL","private":true,"keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/ploomber/jupysql-plugin.git","bugs":{"url":"https://github.com/ploomber/jupysql-plugin.git/issues"},"license":"BSD-3-Clause","author":{"name":"Ploomber","email":"contact@ploomber.io"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/ploomber/jupysql-plugin.git.git"},"workspaces":{"packages":["jupysql_plugin","ui-tests"]},"scripts":{"build":"jlpm build:lib && jlpm build:labextension:dev","build:prod":"jlpm clean && jlpm build:lib:prod && jlpm build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc --sourceMap","build:lib:prod":"tsc","clean":"jlpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf jupysql_plugin/labextension jupysql_plugin/_version.py","clean:all":"jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache","eslint":"jlpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"jlpm build","lint":"jlpm stylelint && jlpm prettier && jlpm eslint","lint:check":"jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check","prettier":"jlpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"jlpm prettier:base --check","stylelint":"jlpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"@comment":{"dependencies":{"@lumino/widgets":"An official library to implement the frontend of the widgets: https://github.com/jupyterlab/lumino"}},"dependencies":{"@emotion/react":"^11.11.0","@emotion/styled":"^11.11.0","@jupyter-widgets/base":"^6.0.4","@jupyterlab/application":"^3.6.2","@jupyterlab/codeeditor":"^3.6.2","@jupyterlab/codemirror":"^3.6.3","@jupyterlab/completer":"^3.6.2","@jupyterlab/notebook":"^3.6.2","@jupyterlab/statedb":"^3.6.2","@lumino/widgets":"<2.0.0","@mui/icons-material":"^5.11.16","@mui/material":"^5.13.4","@types/codemirror":"^5.60.7","@types/underscore":"^1.11.4","bootstrap":"^5.2.3","react":"^18.2.0","sql-formatter":"^12.2.0","underscore":"^1.13.6"},"devDependencies":{"@babel/core":"^7.0.0","@babel/preset-env":"^7.0.0","@jupyterlab/builder":"^3.1.0","@jupyterlab/testutils":"^3.0.0","@types/bootstrap":"^5.2.6","@types/jest":"^26.0.0","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-prettier":"^3.1.4","jest":"^26.0.0","npm-run-all":"^4.1.5","prettier":"^2.1.1","rimraf":"^3.0.2","stylelint":"^14.3.0","stylelint-config-prettier":"^9.0.4","stylelint-config-recommended":"^6.0.0","stylelint-config-standard":"~24.0.0","stylelint-prettier":"^2.0.0","ts-jest":"^26.0.0","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"outputDir":"jupysql_plugin/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"jupysql-plugin","version":"0.1.8","description":"Jupyterlab extension for JupySQL","private":true,"keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/ploomber/jupysql-plugin.git","bugs":{"url":"https://github.com/ploomber/jupysql-plugin.git/issues"},"license":"BSD-3-Clause","author":{"name":"Ploomber","email":"contact@ploomber.io"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/ploomber/jupysql-plugin.git.git"},"workspaces":{"packages":["jupysql_plugin","ui-tests"]},"scripts":{"build":"jlpm build:lib && jlpm build:labextension:dev","build:prod":"jlpm clean && jlpm build:lib:prod && jlpm build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc --sourceMap","build:lib:prod":"tsc","clean":"jlpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf jupysql_plugin/labextension jupysql_plugin/_version.py","clean:all":"jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache","eslint":"jlpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"jlpm build","lint":"jlpm stylelint && jlpm prettier && jlpm eslint","lint:check":"jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check","prettier":"jlpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"jlpm prettier:base --check","stylelint":"jlpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"@comment":{"dependencies":{"@lumino/widgets":"An official library to implement the frontend of the widgets: https://github.com/jupyterlab/lumino"}},"dependencies":{"@emotion/react":"^11.11.0","@emotion/styled":"^11.11.0","@jupyter-widgets/base":"^6.0.4","@jupyterlab/application":"^3.6.2","@jupyterlab/codeeditor":"^3.6.2","@jupyterlab/codemirror":"^3.6.3","@jupyterlab/completer":"^3.6.2","@jupyterlab/notebook":"^3.6.2","@jupyterlab/statedb":"^3.6.2","@lumino/widgets":"<2.0.0","@mui/icons-material":"^5.11.16","@mui/material":"^5.13.4","@types/codemirror":"^5.60.7","@types/underscore":"^1.11.4","bootstrap":"^5.2.3","clean":"^4.0.2","react":"^17.0.2","sql-formatter":"^12.2.0","underscore":"^1.13.6"},"devDependencies":{"@babel/core":"^7.0.0","@babel/preset-env":"^7.0.0","@jupyterlab/builder":"^3.1.0","@jupyterlab/testutils":"^3.0.0","@testing-library/jest-dom":"^5.16.5","@testing-library/react":"^12.1.2","@types/bootstrap":"^5.2.6","@types/jest":"^26.0.0","@types/jest-when":"^3.5.2","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-prettier":"^3.1.4","jest":"^26.0.0","jest-when":"^3.5.2","npm-run-all":"^4.1.5","prettier":"^2.1.1","react-dom":"^17.0.2","rimraf":"^3.0.2","stylelint":"^14.3.0","stylelint-config-prettier":"^9.0.4","stylelint-config-recommended":"^6.0.0","stylelint-config-standard":"~24.0.0","stylelint-prettier":"^2.0.0","ts-jest":"^26.0.0","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"outputDir":"jupysql_plugin/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/40.4f257c905f8cbcacb158.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 40.4f257c905f8cbcacb158.js.LICENSE.txt */
+/*! For license information please see 40.2e8dd60e0a5a8bf83e3e.js.LICENSE.txt */
 "use strict";
 (self.webpackChunkjupysql_plugin = self.webpackChunkjupysql_plugin || []).push([
     [40, 122], {
         2122: (e, t, r) => {
             function n() {
                 return n = Object.assign ? Object.assign.bind() : function(e) {
                     for (var t = 1; t < arguments.length; t++) {
@@ -36,104 +36,104 @@
                 o = r(9756),
                 i = r(6271),
                 a = r(6010),
                 s = r(4780),
                 l = r(8216),
                 c = r(1657),
                 u = r(948),
-                d = r(2994),
-                f = r(8521);
+                f = r(2994),
+                d = r(8521);
             const p = ["children", "className", "color", "component", "fontSize", "htmlColor", "inheritViewBox", "titleAccess", "viewBox"],
                 m = (0, u.ZP)("svg", {
                     name: "MuiSvgIcon",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         const {
                             ownerState: r
                         } = e;
                         return [t.root, "inherit" !== r.color && t[`color${(0,l.Z)(r.color)}`], t[`fontSize${(0,l.Z)(r.fontSize)}`]]
                     }
                 })((({
                     theme: e,
                     ownerState: t
                 }) => {
-                    var r, n, o, i, a, s, l, c, u, d, f, p, m, h, y, g, Z;
+                    var r, n, o, i, a, s, l, c, u, f, d, p, m, h, y, g, b;
                     return {
                         userSelect: "none",
                         width: "1em",
                         height: "1em",
                         display: "inline-block",
                         fill: t.hasSvgAsChild ? void 0 : "currentColor",
                         flexShrink: 0,
                         transition: null == (r = e.transitions) || null == (n = r.create) ? void 0 : n.call(r, "fill", {
                             duration: null == (o = e.transitions) || null == (i = o.duration) ? void 0 : i.shorter
                         }),
                         fontSize: {
                             inherit: "inherit",
                             small: (null == (a = e.typography) || null == (s = a.pxToRem) ? void 0 : s.call(a, 20)) || "1.25rem",
                             medium: (null == (l = e.typography) || null == (c = l.pxToRem) ? void 0 : c.call(l, 24)) || "1.5rem",
-                            large: (null == (u = e.typography) || null == (d = u.pxToRem) ? void 0 : d.call(u, 35)) || "2.1875rem"
+                            large: (null == (u = e.typography) || null == (f = u.pxToRem) ? void 0 : f.call(u, 35)) || "2.1875rem"
                         } [t.fontSize],
-                        color: null != (f = null == (p = (e.vars || e).palette) || null == (m = p[t.color]) ? void 0 : m.main) ? f : {
+                        color: null != (d = null == (p = (e.vars || e).palette) || null == (m = p[t.color]) ? void 0 : m.main) ? d : {
                             action: null == (h = (e.vars || e).palette) || null == (y = h.action) ? void 0 : y.active,
-                            disabled: null == (g = (e.vars || e).palette) || null == (Z = g.action) ? void 0 : Z.disabled,
+                            disabled: null == (g = (e.vars || e).palette) || null == (b = g.action) ? void 0 : b.disabled,
                             inherit: void 0
                         } [t.color]
                     }
                 })),
                 h = i.forwardRef((function(e, t) {
                     const r = (0, c.Z)({
                             props: e,
                             name: "MuiSvgIcon"
                         }),
                         {
                             children: u,
                             className: h,
                             color: y = "inherit",
                             component: g = "svg",
-                            fontSize: Z = "medium",
-                            htmlColor: b,
+                            fontSize: b = "medium",
+                            htmlColor: Z,
                             inheritViewBox: v = !1,
                             titleAccess: x,
                             viewBox: k = "0 0 24 24"
                         } = r,
                         w = (0, o.Z)(r, p),
-                        S = i.isValidElement(u) && "svg" === u.type,
-                        O = (0, n.Z)({}, r, {
+                        O = i.isValidElement(u) && "svg" === u.type,
+                        S = (0, n.Z)({}, r, {
                             color: y,
                             component: g,
-                            fontSize: Z,
+                            fontSize: b,
                             instanceFontSize: e.fontSize,
                             inheritViewBox: v,
                             viewBox: k,
-                            hasSvgAsChild: S
+                            hasSvgAsChild: O
                         }),
-                        A = {};
-                    v || (A.viewBox = k);
-                    const P = (e => {
+                        P = {};
+                    v || (P.viewBox = k);
+                    const A = (e => {
                         const {
                             color: t,
                             fontSize: r,
                             classes: n
                         } = e, o = {
                             root: ["root", "inherit" !== t && `color${(0,l.Z)(t)}`, `fontSize${(0,l.Z)(r)}`]
                         };
-                        return (0, s.Z)(o, d.h, n)
-                    })(O);
-                    return (0, f.jsxs)(m, (0, n.Z)({
+                        return (0, s.Z)(o, f.h, n)
+                    })(S);
+                    return (0, d.jsxs)(m, (0, n.Z)({
                         as: g,
-                        className: (0, a.Z)(P.root, h),
+                        className: (0, a.Z)(A.root, h),
                         focusable: "false",
-                        color: b,
+                        color: Z,
                         "aria-hidden": !x || void 0,
                         role: x ? "img" : void 0,
                         ref: t
-                    }, A, w, S && u.props, {
-                        ownerState: O,
-                        children: [S ? u.props.children : u, x ? (0, f.jsx)("title", {
+                    }, P, w, O && u.props, {
+                        ownerState: S,
+                        children: [O ? u.props.children : u, x ? (0, d.jsx)("title", {
                             children: x
                         }) : null]
                     }))
                 }));
             h.muiName = "SvgIcon";
             const y = h
         },
@@ -304,44 +304,44 @@
                 A200: "#ff5252",
                 A400: "#ff1744",
                 A700: "#d50000"
             }
         },
         1893: (e, t, r) => {
             r.d(t, {
-                A: () => R,
-                Z: () => j
+                A: () => T,
+                Z: () => R
             });
             var n = r(2122),
                 o = r(9756),
                 i = r(1387),
                 a = r(9766),
                 s = r(646),
                 l = r(5842),
                 c = r(6523),
                 u = r(1796),
-                d = r(6115),
-                f = r(7036),
+                f = r(6115),
+                d = r(7036),
                 p = r(4518),
                 m = r(265),
                 h = r(5137),
                 y = r(6949),
                 g = r(5621),
-                Z = r(3486);
-            const b = ["mode", "contrastThreshold", "tonalOffset"],
+                b = r(3486);
+            const Z = ["mode", "contrastThreshold", "tonalOffset"],
                 v = {
                     text: {
                         primary: "rgba(0, 0, 0, 0.87)",
                         secondary: "rgba(0, 0, 0, 0.6)",
                         disabled: "rgba(0, 0, 0, 0.38)"
                     },
                     divider: "rgba(0, 0, 0, 0.12)",
                     background: {
-                        paper: d.Z.white,
-                        default: d.Z.white
+                        paper: f.Z.white,
+                        default: f.Z.white
                     },
                     action: {
                         active: "rgba(0, 0, 0, 0.54)",
                         hover: "rgba(0, 0, 0, 0.04)",
                         hoverOpacity: .04,
                         selected: "rgba(0, 0, 0, 0.08)",
                         selectedOpacity: .08,
@@ -351,26 +351,26 @@
                         focus: "rgba(0, 0, 0, 0.12)",
                         focusOpacity: .12,
                         activatedOpacity: .12
                     }
                 },
                 x = {
                     text: {
-                        primary: d.Z.white,
+                        primary: f.Z.white,
                         secondary: "rgba(255, 255, 255, 0.7)",
                         disabled: "rgba(255, 255, 255, 0.5)",
                         icon: "rgba(255, 255, 255, 0.5)"
                     },
                     divider: "rgba(255, 255, 255, 0.12)",
                     background: {
                         paper: "#121212",
                         default: "#121212"
                     },
                     action: {
-                        active: d.Z.white,
+                        active: f.Z.white,
                         hover: "rgba(255, 255, 255, 0.08)",
                         hoverOpacity: .08,
                         selected: "rgba(255, 255, 255, 0.16)",
                         selectedOpacity: .16,
                         disabled: "rgba(255, 255, 255, 0.3)",
                         disabledBackground: "rgba(255, 255, 255, 0.12)",
                         disabledOpacity: .38,
@@ -383,45 +383,45 @@
             function k(e, t, r, n) {
                 const o = n.light || n,
                     i = n.dark || 1.5 * n;
                 e[t] || (e.hasOwnProperty(r) ? e[t] = e[r] : "light" === t ? e.light = (0, u.$n)(e.main, o) : "dark" === t && (e.dark = (0, u._j)(e.main, i)))
             }
             var w = r(1445);
 
-            function S(...e) {
+            function O(...e) {
                 return [`${e[0]}px ${e[1]}px ${e[2]}px ${e[3]}px rgba(0,0,0,0.2)`, `${e[4]}px ${e[5]}px ${e[6]}px ${e[7]}px rgba(0,0,0,0.14)`, `${e[8]}px ${e[9]}px ${e[10]}px ${e[11]}px rgba(0,0,0,0.12)`].join(",")
             }
-            const O = ["none", S(0, 2, 1, -1, 0, 1, 1, 0, 0, 1, 3, 0), S(0, 3, 1, -2, 0, 2, 2, 0, 0, 1, 5, 0), S(0, 3, 3, -2, 0, 3, 4, 0, 0, 1, 8, 0), S(0, 2, 4, -1, 0, 4, 5, 0, 0, 1, 10, 0), S(0, 3, 5, -1, 0, 5, 8, 0, 0, 1, 14, 0), S(0, 3, 5, -1, 0, 6, 10, 0, 0, 1, 18, 0), S(0, 4, 5, -2, 0, 7, 10, 1, 0, 2, 16, 1), S(0, 5, 5, -3, 0, 8, 10, 1, 0, 3, 14, 2), S(0, 5, 6, -3, 0, 9, 12, 1, 0, 3, 16, 2), S(0, 6, 6, -3, 0, 10, 14, 1, 0, 4, 18, 3), S(0, 6, 7, -4, 0, 11, 15, 1, 0, 4, 20, 3), S(0, 7, 8, -4, 0, 12, 17, 2, 0, 5, 22, 4), S(0, 7, 8, -4, 0, 13, 19, 2, 0, 5, 24, 4), S(0, 7, 9, -4, 0, 14, 21, 2, 0, 5, 26, 4), S(0, 8, 9, -5, 0, 15, 22, 2, 0, 6, 28, 5), S(0, 8, 10, -5, 0, 16, 24, 2, 0, 6, 30, 5), S(0, 8, 11, -5, 0, 17, 26, 2, 0, 6, 32, 5), S(0, 9, 11, -5, 0, 18, 28, 2, 0, 7, 34, 6), S(0, 9, 12, -6, 0, 19, 29, 2, 0, 7, 36, 6), S(0, 10, 13, -6, 0, 20, 31, 3, 0, 8, 38, 7), S(0, 10, 13, -6, 0, 21, 33, 3, 0, 8, 40, 7), S(0, 10, 14, -6, 0, 22, 35, 3, 0, 8, 42, 7), S(0, 11, 14, -7, 0, 23, 36, 3, 0, 9, 44, 8), S(0, 11, 15, -7, 0, 24, 38, 3, 0, 9, 46, 8)];
-            var A = r(6067);
-            const P = {
+            const S = ["none", O(0, 2, 1, -1, 0, 1, 1, 0, 0, 1, 3, 0), O(0, 3, 1, -2, 0, 2, 2, 0, 0, 1, 5, 0), O(0, 3, 3, -2, 0, 3, 4, 0, 0, 1, 8, 0), O(0, 2, 4, -1, 0, 4, 5, 0, 0, 1, 10, 0), O(0, 3, 5, -1, 0, 5, 8, 0, 0, 1, 14, 0), O(0, 3, 5, -1, 0, 6, 10, 0, 0, 1, 18, 0), O(0, 4, 5, -2, 0, 7, 10, 1, 0, 2, 16, 1), O(0, 5, 5, -3, 0, 8, 10, 1, 0, 3, 14, 2), O(0, 5, 6, -3, 0, 9, 12, 1, 0, 3, 16, 2), O(0, 6, 6, -3, 0, 10, 14, 1, 0, 4, 18, 3), O(0, 6, 7, -4, 0, 11, 15, 1, 0, 4, 20, 3), O(0, 7, 8, -4, 0, 12, 17, 2, 0, 5, 22, 4), O(0, 7, 8, -4, 0, 13, 19, 2, 0, 5, 24, 4), O(0, 7, 9, -4, 0, 14, 21, 2, 0, 5, 26, 4), O(0, 8, 9, -5, 0, 15, 22, 2, 0, 6, 28, 5), O(0, 8, 10, -5, 0, 16, 24, 2, 0, 6, 30, 5), O(0, 8, 11, -5, 0, 17, 26, 2, 0, 6, 32, 5), O(0, 9, 11, -5, 0, 18, 28, 2, 0, 7, 34, 6), O(0, 9, 12, -6, 0, 19, 29, 2, 0, 7, 36, 6), O(0, 10, 13, -6, 0, 20, 31, 3, 0, 8, 38, 7), O(0, 10, 13, -6, 0, 21, 33, 3, 0, 8, 40, 7), O(0, 10, 14, -6, 0, 22, 35, 3, 0, 8, 42, 7), O(0, 11, 14, -7, 0, 23, 36, 3, 0, 9, 44, 8), O(0, 11, 15, -7, 0, 24, 38, 3, 0, 9, 46, 8)];
+            var P = r(6067);
+            const A = {
                     mobileStepper: 1e3,
                     fab: 1050,
                     speedDial: 1050,
                     appBar: 1100,
                     drawer: 1200,
                     modal: 1300,
                     snackbar: 1400,
                     tooltip: 1500
                 },
-                $ = ["breakpoints", "mixins", "spacing", "palette", "transitions", "typography", "shape"];
+                j = ["breakpoints", "mixins", "spacing", "palette", "transitions", "typography", "shape"];
 
-            function T(e = {}, ...t) {
+            function $(e = {}, ...t) {
                 const {
                     mixins: r = {},
-                    palette: S = {},
-                    transitions: T = {},
-                    typography: R = {}
-                } = e, j = (0, o.Z)(e, $);
+                    palette: O = {},
+                    transitions: $ = {},
+                    typography: T = {}
+                } = e, R = (0, o.Z)(e, j);
                 if (e.vars) throw new Error((0, i.Z)(18));
                 const C = function(e) {
                         const {
                             mode: t = "light",
                             contrastThreshold: r = 3,
                             tonalOffset: s = .2
-                        } = e, l = (0, o.Z)(e, b), c = e.primary || function(e = "light") {
+                        } = e, l = (0, o.Z)(e, Z), c = e.primary || function(e = "light") {
                             return "dark" === e ? {
                                 main: y.Z[200],
                                 light: y.Z[50],
                                 dark: y.Z[400]
                             } : {
                                 main: y.Z[700],
                                 light: y.Z[400],
@@ -433,145 +433,145 @@
                                 light: p.Z[50],
                                 dark: p.Z[400]
                             } : {
                                 main: p.Z[500],
                                 light: p.Z[300],
                                 dark: p.Z[700]
                             }
-                        }(t), S = e.error || function(e = "light") {
+                        }(t), O = e.error || function(e = "light") {
                             return "dark" === e ? {
                                 main: m.Z[500],
                                 light: m.Z[300],
                                 dark: m.Z[700]
                             } : {
                                 main: m.Z[700],
                                 light: m.Z[400],
                                 dark: m.Z[800]
                             }
-                        }(t), O = e.info || function(e = "light") {
+                        }(t), S = e.info || function(e = "light") {
                             return "dark" === e ? {
                                 main: g.Z[400],
                                 light: g.Z[300],
                                 dark: g.Z[700]
                             } : {
                                 main: g.Z[700],
                                 light: g.Z[500],
                                 dark: g.Z[900]
                             }
-                        }(t), A = e.success || function(e = "light") {
+                        }(t), P = e.success || function(e = "light") {
                             return "dark" === e ? {
-                                main: Z.Z[400],
-                                light: Z.Z[300],
-                                dark: Z.Z[700]
+                                main: b.Z[400],
+                                light: b.Z[300],
+                                dark: b.Z[700]
                             } : {
-                                main: Z.Z[800],
-                                light: Z.Z[500],
-                                dark: Z.Z[900]
+                                main: b.Z[800],
+                                light: b.Z[500],
+                                dark: b.Z[900]
                             }
-                        }(t), P = e.warning || function(e = "light") {
+                        }(t), A = e.warning || function(e = "light") {
                             return "dark" === e ? {
                                 main: h.Z[400],
                                 light: h.Z[300],
                                 dark: h.Z[700]
                             } : {
                                 main: "#ed6c02",
                                 light: h.Z[500],
                                 dark: h.Z[900]
                             }
                         }(t);
 
-                        function $(e) {
+                        function j(e) {
                             return (0, u.mi)(e, x.text.primary) >= r ? x.text.primary : v.text.primary
                         }
-                        const T = ({
+                        const $ = ({
                                 color: e,
                                 name: t,
                                 mainShade: r = 500,
                                 lightShade: o = 300,
                                 darkShade: a = 700
                             }) => {
                                 if (!(e = (0, n.Z)({}, e)).main && e[r] && (e.main = e[r]), !e.hasOwnProperty("main")) throw new Error((0, i.Z)(11, t ? ` (${t})` : "", r));
                                 if ("string" != typeof e.main) throw new Error((0, i.Z)(12, t ? ` (${t})` : "", JSON.stringify(e.main)));
-                                return k(e, "light", o, s), k(e, "dark", a, s), e.contrastText || (e.contrastText = $(e.main)), e
+                                return k(e, "light", o, s), k(e, "dark", a, s), e.contrastText || (e.contrastText = j(e.main)), e
                             },
-                            R = {
+                            T = {
                                 dark: x,
                                 light: v
                             };
                         return (0, a.Z)((0, n.Z)({
-                            common: (0, n.Z)({}, d.Z),
+                            common: (0, n.Z)({}, f.Z),
                             mode: t,
-                            primary: T({
+                            primary: $({
                                 color: c,
                                 name: "primary"
                             }),
-                            secondary: T({
+                            secondary: $({
                                 color: w,
                                 name: "secondary",
                                 mainShade: "A400",
                                 lightShade: "A200",
                                 darkShade: "A700"
                             }),
-                            error: T({
-                                color: S,
+                            error: $({
+                                color: O,
                                 name: "error"
                             }),
-                            warning: T({
-                                color: P,
+                            warning: $({
+                                color: A,
                                 name: "warning"
                             }),
-                            info: T({
-                                color: O,
+                            info: $({
+                                color: S,
                                 name: "info"
                             }),
-                            success: T({
-                                color: A,
+                            success: $({
+                                color: P,
                                 name: "success"
                             }),
-                            grey: f.Z,
+                            grey: d.Z,
                             contrastThreshold: r,
-                            getContrastText: $,
-                            augmentColor: T,
+                            getContrastText: j,
+                            augmentColor: $,
                             tonalOffset: s
-                        }, R[t]), l)
-                    }(S),
-                    _ = (0, s.Z)(e);
-                let E = (0, a.Z)(_, {
-                    mixins: (I = _.breakpoints, B = r, (0, n.Z)({
+                        }, T[t]), l)
+                    }(O),
+                    E = (0, s.Z)(e);
+                let _ = (0, a.Z)(E, {
+                    mixins: (I = E.breakpoints, B = r, (0, n.Z)({
                         toolbar: {
                             minHeight: 56,
                             [I.up("xs")]: {
                                 "@media (orientation: landscape)": {
                                     minHeight: 48
                                 }
                             },
                             [I.up("sm")]: {
                                 minHeight: 64
                             }
                         }
                     }, B)),
                     palette: C,
-                    shadows: O.slice(),
-                    typography: (0, w.Z)(C, R),
-                    transitions: (0, A.ZP)(T),
-                    zIndex: (0, n.Z)({}, P)
+                    shadows: S.slice(),
+                    typography: (0, w.Z)(C, T),
+                    transitions: (0, P.ZP)($),
+                    zIndex: (0, n.Z)({}, A)
                 });
                 var I, B;
-                return E = (0, a.Z)(E, j), E = t.reduce(((e, t) => (0, a.Z)(e, t)), E), E.unstable_sxConfig = (0, n.Z)({}, l.Z, null == j ? void 0 : j.unstable_sxConfig), E.unstable_sx = function(e) {
+                return _ = (0, a.Z)(_, R), _ = t.reduce(((e, t) => (0, a.Z)(e, t)), _), _.unstable_sxConfig = (0, n.Z)({}, l.Z, null == R ? void 0 : R.unstable_sxConfig), _.unstable_sx = function(e) {
                     return (0, c.Z)({
                         sx: e,
                         theme: this
                     })
-                }, E
+                }, _
             }
 
-            function R(...e) {
-                return T(...e)
+            function T(...e) {
+                return $(...e)
             }
-            const j = T
+            const R = $
         },
         6067: (e, t, r) => {
             r.d(t, {
                 Ui: () => a,
                 ZP: () => u,
                 x9: () => s
             });
@@ -637,68 +637,68 @@
                 l = '"Roboto", "Helvetica", "Arial", sans-serif';
 
             function c(e, t) {
                 const r = "function" == typeof t ? t(e) : t,
                     {
                         fontFamily: c = l,
                         fontSize: u = 14,
-                        fontWeightLight: d = 300,
-                        fontWeightRegular: f = 400,
+                        fontWeightLight: f = 300,
+                        fontWeightRegular: d = 400,
                         fontWeightMedium: p = 500,
                         fontWeightBold: m = 700,
                         htmlFontSize: h = 16,
                         allVariants: y,
                         pxToRem: g
                     } = r,
-                    Z = (0, o.Z)(r, a),
-                    b = u / 14,
-                    v = g || (e => e / h * b + "rem"),
+                    b = (0, o.Z)(r, a),
+                    Z = u / 14,
+                    v = g || (e => e / h * Z + "rem"),
                     x = (e, t, r, o, i) => {
                         return (0, n.Z)({
                             fontFamily: c,
                             fontWeight: e,
                             fontSize: v(t),
                             lineHeight: r
                         }, c === l ? {
                             letterSpacing: (a = o / t, Math.round(1e5 * a) / 1e5 + "em")
                         } : {}, i, y);
                         var a
                     },
                     k = {
-                        h1: x(d, 96, 1.167, -1.5),
-                        h2: x(d, 60, 1.2, -.5),
-                        h3: x(f, 48, 1.167, 0),
-                        h4: x(f, 34, 1.235, .25),
-                        h5: x(f, 24, 1.334, 0),
+                        h1: x(f, 96, 1.167, -1.5),
+                        h2: x(f, 60, 1.2, -.5),
+                        h3: x(d, 48, 1.167, 0),
+                        h4: x(d, 34, 1.235, .25),
+                        h5: x(d, 24, 1.334, 0),
                         h6: x(p, 20, 1.6, .15),
-                        subtitle1: x(f, 16, 1.75, .15),
+                        subtitle1: x(d, 16, 1.75, .15),
                         subtitle2: x(p, 14, 1.57, .1),
-                        body1: x(f, 16, 1.5, .15),
-                        body2: x(f, 14, 1.43, .15),
+                        body1: x(d, 16, 1.5, .15),
+                        body2: x(d, 14, 1.43, .15),
                         button: x(p, 14, 1.75, .4, s),
-                        caption: x(f, 12, 1.66, .4),
-                        overline: x(f, 12, 2.66, 1, s),
+                        caption: x(d, 12, 1.66, .4),
+                        overline: x(d, 12, 2.66, 1, s),
                         inherit: {
                             fontFamily: "inherit",
                             fontWeight: "inherit",
                             fontSize: "inherit",
                             lineHeight: "inherit",
                             letterSpacing: "inherit"
                         }
                     };
                 return (0, i.Z)((0, n.Z)({
                     htmlFontSize: h,
                     pxToRem: v,
                     fontFamily: c,
                     fontSize: u,
-                    fontWeightLight: d,
-                    fontWeightRegular: f,
+                    fontWeightLight: f,
+                    fontWeightRegular: d,
                     fontWeightMedium: p,
                     fontWeightBold: m
-                }, k), Z, {
+                }, k), b, {
                     clone: !1
                 })
             }
         },
         247: (e, t, r) => {
             r.d(t, {
                 Z: () => n
@@ -792,50 +792,50 @@
                 capitalize: () => o.Z,
                 createChainedFunction: () => i.Z,
                 createSvgIcon: () => a.Z,
                 debounce: () => s.Z,
                 deprecatedPropType: () => l,
                 isMuiElement: () => c.Z,
                 ownerDocument: () => u.Z,
-                ownerWindow: () => d.Z,
-                requirePropFactory: () => f,
+                ownerWindow: () => f.Z,
+                requirePropFactory: () => d,
                 setRef: () => p,
                 unstable_ClassNameGenerator: () => x,
                 unstable_useEnhancedEffect: () => m.Z,
                 unstable_useId: () => h.Z,
                 unsupportedProp: () => y,
                 useControlled: () => g.Z,
-                useEventCallback: () => Z.Z,
-                useForkRef: () => b.Z,
+                useEventCallback: () => b.Z,
+                useForkRef: () => Z.Z,
                 useIsFocusVisible: () => v.Z
             });
             var n = r(7078),
                 o = r(8216),
                 i = r(5893),
                 a = r(2066),
                 s = r(7144);
             const l = function(e, t) {
                 return () => null
             };
             var c = r(6798),
                 u = r(8038),
-                d = r(5340);
+                f = r(5340);
             r(2122);
-            const f = function(e, t) {
+            const d = function(e, t) {
                     return () => null
                 },
                 p = r(7960).Z;
             var m = r(8974),
                 h = r(7909);
             const y = function(e, t, r, n, o) {
                 return null
             };
             var g = r(9299),
-                Z = r(2068),
-                b = r(1705),
+                b = r(2068),
+                Z = r(1705),
                 v = r(9674);
             const x = {
                 configure: e => {
                     n.Z.configure(e)
                 }
             }
         },
@@ -990,24 +990,24 @@
                 return o.reduce(((t, r, n) => (Array.isArray(e) ? (t[r] = null != e[n] ? e[n] : e[i], i = n) : "object" == typeof e ? (t[r] = null != e[r] ? e[r] : e[i], i = r) : t[r] = e, t)), {})
             }
         },
         1796: (e, t, r) => {
             r.d(t, {
                 $n: () => g,
                 Fq: () => p,
-                H3: () => d,
+                H3: () => f,
                 LR: () => s,
-                _4: () => b,
+                _4: () => Z,
                 _j: () => h,
                 fk: () => v,
-                mi: () => f,
+                mi: () => d,
                 oo: () => i,
                 q8: () => y,
                 tB: () => a,
-                ux: () => Z,
+                ux: () => b,
                 ve: () => u,
                 vq: () => c,
                 wy: () => l,
                 zp: () => m
             });
             var n = r(1387);
 
@@ -1077,22 +1077,22 @@
                 const u = [Math.round(255 * s(0)), Math.round(255 * s(8)), Math.round(255 * s(4))];
                 return "hsla" === e.type && (c += "a", u.push(t[3])), l({
                     type: c,
                     values: u
                 })
             }
 
-            function d(e) {
+            function f(e) {
                 let t = "hsl" === (e = a(e)).type || "hsla" === e.type ? a(u(e)).values : e.values;
                 return t = t.map((t => ("color" !== e.type && (t /= 255), t <= .03928 ? t / 12.92 : ((t + .055) / 1.055) ** 2.4))), Number((.2126 * t[0] + .7152 * t[1] + .0722 * t[2]).toFixed(3))
             }
 
-            function f(e, t) {
-                const r = d(e),
-                    n = d(t);
+            function d(e, t) {
+                const r = f(e),
+                    n = f(t);
                 return (Math.max(r, n) + .05) / (Math.min(r, n) + .05)
             }
 
             function p(e, t) {
                 return e = a(e), t = o(t), "rgb" !== e.type && "hsl" !== e.type || (e.type += "a"), "color" === e.type ? e.values[3] = `/${t}` : e.values[3] = t, l(e)
             }
 
@@ -1124,37 +1124,37 @@
                 else if (-1 !== e.type.indexOf("rgb"))
                     for (let r = 0; r < 3; r += 1) e.values[r] += (255 - e.values[r]) * t;
                 else if (-1 !== e.type.indexOf("color"))
                     for (let r = 0; r < 3; r += 1) e.values[r] += (1 - e.values[r]) * t;
                 return l(e)
             }
 
-            function Z(e, t, r) {
+            function b(e, t, r) {
                 try {
                     return g(e, t)
                 } catch (t) {
                     return e
                 }
             }
 
-            function b(e, t = .15) {
-                return d(e) > .5 ? h(e, t) : g(e, t)
+            function Z(e, t = .15) {
+                return f(e) > .5 ? h(e, t) : g(e, t)
             }
 
             function v(e, t, r) {
                 try {
                     return v(e, t)
                 } catch (t) {
                     return e
                 }
             }
         },
         8362: (e, t, r) => {
             r.d(t, {
-                ZP: () => b,
+                ZP: () => Z,
                 x9: () => y
             });
             var n = r(9756),
                 o = r(2122),
                 i = r(8883),
                 a = r(646),
                 s = r(4142);
@@ -1169,16 +1169,16 @@
                     variant: t
                 } = e, r = (0, n.Z)(e, l);
                 let o = t || "";
                 return Object.keys(r).sort().forEach((t => {
                     o += "color" === t ? c(o) ? e[t] : (0, s.Z)(e[t]) : `${c(o)?t:(0,s.Z)(t)}${(0,s.Z)(e[t].toString())}`
                 })), o
             }
-            var d = r(6523);
-            const f = ["name", "slot", "skipVariantsResolver", "skipSx", "overridesResolver"],
+            var f = r(6523);
+            const d = ["name", "slot", "skipVariantsResolver", "skipSx", "overridesResolver"],
                 p = (e, t) => t.components && t.components[e] && t.components[e].styleOverrides ? t.components[e].styleOverrides : null,
                 m = (e, t) => {
                     let r = [];
                     t && t.components && t.components[e] && t.components[e].variants && (r = t.components[e].variants);
                     const n = {};
                     return r.forEach((e => {
                         const t = u(e.props);
@@ -1199,96 +1199,96 @@
                 };
 
             function y(e) {
                 return "ownerState" !== e && "theme" !== e && "sx" !== e && "as" !== e
             }
             const g = (0, a.Z)();
 
-            function Z({
+            function b({
                 defaultTheme: e,
                 theme: t,
                 themeId: r
             }) {
                 return n = t, 0 === Object.keys(n).length ? e : t[r] || t;
                 var n
             }
 
-            function b(e = {}) {
+            function Z(e = {}) {
                 const {
                     themeId: t,
                     defaultTheme: r = g,
                     rootShouldForwardProp: a = y,
                     slotShouldForwardProp: s = y
-                } = e, l = e => (0, d.Z)((0, o.Z)({}, e, {
-                    theme: Z((0, o.Z)({}, e, {
+                } = e, l = e => (0, f.Z)((0, o.Z)({}, e, {
+                    theme: b((0, o.Z)({}, e, {
                         defaultTheme: r,
                         themeId: t
                     }))
                 }));
                 return l.__mui_systemSx = !0, (e, c = {}) => {
                     (0, i.Co)(e, (e => e.filter((e => !(null != e && e.__mui_systemSx)))));
                     const {
                         name: u,
-                        slot: d,
+                        slot: f,
                         skipVariantsResolver: g,
-                        skipSx: b,
+                        skipSx: Z,
                         overridesResolver: v
-                    } = c, x = (0, n.Z)(c, f), k = void 0 !== g ? g : d && "Root" !== d || !1, w = b || !1;
-                    let S = y;
-                    "Root" === d ? S = a : d ? S = s : function(e) {
+                    } = c, x = (0, n.Z)(c, d), k = void 0 !== g ? g : f && "Root" !== f || !1, w = Z || !1;
+                    let O = y;
+                    "Root" === f ? O = a : f ? O = s : function(e) {
                         return "string" == typeof e && e.charCodeAt(0) > 96
-                    }(e) && (S = void 0);
-                    const O = (0, i.ZP)(e, (0, o.Z)({
-                            shouldForwardProp: S,
+                    }(e) && (O = void 0);
+                    const S = (0, i.ZP)(e, (0, o.Z)({
+                            shouldForwardProp: O,
                             label: void 0
                         }, x)),
-                        A = (n, ...i) => {
+                        P = (n, ...i) => {
                             const a = i ? i.map((e => "function" == typeof e && e.__emotion_real !== e ? n => e((0, o.Z)({}, n, {
-                                theme: Z((0, o.Z)({}, n, {
+                                theme: b((0, o.Z)({}, n, {
                                     defaultTheme: r,
                                     themeId: t
                                 }))
                             })) : e)) : [];
                             let s = n;
                             u && v && a.push((e => {
-                                const n = Z((0, o.Z)({}, e, {
+                                const n = b((0, o.Z)({}, e, {
                                         defaultTheme: r,
                                         themeId: t
                                     })),
                                     i = p(u, n);
                                 if (i) {
                                     const t = {};
                                     return Object.entries(i).forEach((([r, i]) => {
                                         t[r] = "function" == typeof i ? i((0, o.Z)({}, e, {
                                             theme: n
                                         })) : i
                                     })), v(e, t)
                                 }
                                 return null
                             })), u && !k && a.push((e => {
-                                const n = Z((0, o.Z)({}, e, {
+                                const n = b((0, o.Z)({}, e, {
                                     defaultTheme: r,
                                     themeId: t
                                 }));
                                 return h(e, m(u, n), n, u)
                             })), w || a.push(l);
                             const c = a.length - i.length;
                             if (Array.isArray(n) && c > 0) {
                                 const e = new Array(c).fill("");
                                 s = [...n, ...e], s.raw = [...n.raw, ...e]
                             } else "function" == typeof n && n.__emotion_real !== n && (s = e => n((0, o.Z)({}, e, {
-                                theme: Z((0, o.Z)({}, e, {
+                                theme: b((0, o.Z)({}, e, {
                                     defaultTheme: r,
                                     themeId: t
                                 }))
                             })));
-                            const d = O(s, ...a);
-                            return e.muiName && (d.muiName = e.muiName), d
+                            const f = S(s, ...a);
+                            return e.muiName && (f.muiName = e.muiName), f
                         };
-                    return O.withConfig && (A.withConfig = O.withConfig), A
+                    return S.withConfig && (P.withConfig = S.withConfig), P
                 }
             }
         },
         1512: (e, t, r) => {
             r.d(t, {
                 Z: () => s
             });
@@ -1314,38 +1314,38 @@
                         lg: 1200,
                         xl: 1536
                     },
                     unit: r = "px",
                     step: s = 5
                 } = e, l = (0, n.Z)(e, i), c = a(t), u = Object.keys(c);
 
-                function d(e) {
+                function f(e) {
                     return `@media (min-width:${"number"==typeof t[e]?t[e]:e}${r})`
                 }
 
-                function f(e) {
+                function d(e) {
                     return `@media (max-width:${("number"==typeof t[e]?t[e]:e)-s/100}${r})`
                 }
 
                 function p(e, n) {
                     const o = u.indexOf(n);
                     return `@media (min-width:${"number"==typeof t[e]?t[e]:e}${r}) and (max-width:${(-1!==o&&"number"==typeof t[u[o]]?t[u[o]]:n)-s/100}${r})`
                 }
                 return (0, o.Z)({
                     keys: u,
                     values: c,
-                    up: d,
-                    down: f,
+                    up: f,
+                    down: d,
                     between: p,
                     only: function(e) {
-                        return u.indexOf(e) + 1 < u.length ? p(e, u[u.indexOf(e) + 1]) : d(e)
+                        return u.indexOf(e) + 1 < u.length ? p(e, u[u.indexOf(e) + 1]) : f(e)
                     },
                     not: function(e) {
                         const t = u.indexOf(e);
-                        return 0 === t ? d(u[1]) : t === u.length - 1 ? f(u[t]) : p(e, u[u.indexOf(e) + 1]).replace("@media", "@media not all and")
+                        return 0 === t ? f(u[1]) : t === u.length - 1 ? d(u[t]) : p(e, u[u.indexOf(e) + 1]).replace("@media", "@media not all and")
                     },
                     unit: r
                 }, l)
             }
         },
         8373: (e, t, r) => {
             r.d(t, {
@@ -1363,50 +1363,50 @@
                         return "number" == typeof r ? `${r}px` : r
                     })).join(" ");
                 return r.mui = !0, r
             }
         },
         646: (e, t, r) => {
             r.d(t, {
-                Z: () => f
+                Z: () => d
             });
             var n = r(2122),
                 o = r(9756),
                 i = r(9766),
                 a = r(1512);
             const s = {
                 borderRadius: 4
             };
             var l = r(8373),
                 c = r(6523),
                 u = r(5842);
-            const d = ["breakpoints", "palette", "spacing", "shape"],
-                f = function(e = {}, ...t) {
+            const f = ["breakpoints", "palette", "spacing", "shape"],
+                d = function(e = {}, ...t) {
                     const {
                         breakpoints: r = {},
-                        palette: f = {},
+                        palette: d = {},
                         spacing: p,
                         shape: m = {}
-                    } = e, h = (0, o.Z)(e, d), y = (0, a.Z)(r), g = (0, l.Z)(p);
-                    let Z = (0, i.Z)({
+                    } = e, h = (0, o.Z)(e, f), y = (0, a.Z)(r), g = (0, l.Z)(p);
+                    let b = (0, i.Z)({
                         breakpoints: y,
                         direction: "ltr",
                         components: {},
                         palette: (0, n.Z)({
                             mode: "light"
-                        }, f),
+                        }, d),
                         spacing: g,
                         shape: (0, n.Z)({}, s, m)
                     }, h);
-                    return Z = t.reduce(((e, t) => (0, i.Z)(e, t)), Z), Z.unstable_sxConfig = (0, n.Z)({}, u.Z, null == h ? void 0 : h.unstable_sxConfig), Z.unstable_sx = function(e) {
+                    return b = t.reduce(((e, t) => (0, i.Z)(e, t)), b), b.unstable_sxConfig = (0, n.Z)({}, u.Z, null == h ? void 0 : h.unstable_sxConfig), b.unstable_sx = function(e) {
                         return (0, c.Z)({
                             sx: e,
                             theme: this
                         })
-                    }, Z
+                    }, b
                 }
         },
         7730: (e, t, r) => {
             r.d(t, {
                 Z: () => o
             });
             var n = r(9766);
@@ -1418,15 +1418,15 @@
         },
         1974: (e, t, r) => {
             r.d(t, {
                 hB: () => m,
                 eI: () => p,
                 NA: () => h,
                 e6: () => g,
-                o3: () => Z
+                o3: () => b
             });
             var n = r(5408),
                 o = r(4844),
                 i = r(7730);
             const a = {
                     m: "margin",
                     p: "padding"
@@ -1453,16 +1453,16 @@
                             e = l[e]
                         }
                         const [t, r] = e.split(""), n = a[t], o = s[r] || "";
                         return Array.isArray(o) ? o.map((e => n + e)) : [n + o]
                     })(e)), t[e])
                 }(),
                 u = ["m", "mt", "mr", "mb", "ml", "mx", "my", "margin", "marginTop", "marginRight", "marginBottom", "marginLeft", "marginX", "marginY", "marginInline", "marginInlineStart", "marginInlineEnd", "marginBlock", "marginBlockStart", "marginBlockEnd"],
-                d = ["p", "pt", "pr", "pb", "pl", "px", "py", "padding", "paddingTop", "paddingRight", "paddingBottom", "paddingLeft", "paddingX", "paddingY", "paddingInline", "paddingInlineStart", "paddingInlineEnd", "paddingBlock", "paddingBlockStart", "paddingBlockEnd"],
-                f = [...u, ...d];
+                f = ["p", "pt", "pr", "pb", "pl", "px", "py", "padding", "paddingTop", "paddingRight", "paddingBottom", "paddingLeft", "paddingX", "paddingY", "paddingInline", "paddingInlineStart", "paddingInlineEnd", "paddingBlock", "paddingBlockStart", "paddingBlockEnd"],
+                d = [...u, ...f];
 
             function p(e, t, r, n) {
                 var i;
                 const a = null != (i = (0, o.DW)(e, t, !1)) ? i : r;
                 return "number" == typeof a ? e => "string" == typeof e ? e : a * e : Array.isArray(a) ? e => "string" == typeof e ? e : a[e] : "function" == typeof a ? a : () => {}
             }
 
@@ -1488,22 +1488,22 @@
                 }(e, t, o, r))).reduce(i.Z, {})
             }
 
             function g(e) {
                 return y(e, u)
             }
 
-            function Z(e) {
-                return y(e, d)
-            }
-
             function b(e) {
                 return y(e, f)
             }
-            g.propTypes = {}, g.filterProps = u, Z.propTypes = {}, Z.filterProps = d, b.propTypes = {}, b.filterProps = f
+
+            function Z(e) {
+                return y(e, d)
+            }
+            g.propTypes = {}, g.filterProps = u, b.propTypes = {}, b.filterProps = f, Z.propTypes = {}, Z.filterProps = d
         },
         4844: (e, t, r) => {
             r.d(t, {
                 DW: () => i,
                 Jq: () => a,
                 ZP: () => s
             });
@@ -1541,15 +1541,15 @@
                     }))
                 };
                 return c.propTypes = {}, c.filterProps = [t], c
             }
         },
         5842: (e, t, r) => {
             r.d(t, {
-                Z: () => j
+                Z: () => R
             });
             var n = r(1974),
                 o = r(4844),
                 i = r(7730);
             const a = function(...e) {
                 const t = e.reduce(((e, t) => (t.filterProps.forEach((r => {
                         e[r] = t
@@ -1568,20 +1568,20 @@
                     transform: l
                 }),
                 u = (0, o.ZP)({
                     prop: "borderTop",
                     themeKey: "borders",
                     transform: l
                 }),
-                d = (0, o.ZP)({
+                f = (0, o.ZP)({
                     prop: "borderRight",
                     themeKey: "borders",
                     transform: l
                 }),
-                f = (0, o.ZP)({
+                d = (0, o.ZP)({
                     prop: "borderBottom",
                     themeKey: "borders",
                     transform: l
                 }),
                 p = (0, o.ZP)({
                     prop: "borderLeft",
                     themeKey: "borders",
@@ -1599,29 +1599,29 @@
                     prop: "borderRightColor",
                     themeKey: "palette"
                 }),
                 g = (0, o.ZP)({
                     prop: "borderBottomColor",
                     themeKey: "palette"
                 }),
-                Z = (0, o.ZP)({
+                b = (0, o.ZP)({
                     prop: "borderLeftColor",
                     themeKey: "palette"
                 }),
-                b = e => {
+                Z = e => {
                     if (void 0 !== e.borderRadius && null !== e.borderRadius) {
                         const t = (0, n.eI)(e.theme, "shape.borderRadius", 4, "borderRadius"),
                             r = e => ({
                                 borderRadius: (0, n.NA)(t, e)
                             });
                         return (0, s.k9)(e, e.borderRadius, r)
                     }
                     return null
                 };
-            b.propTypes = {}, b.filterProps = ["borderRadius"], a(c, u, d, f, p, m, h, y, g, Z, b);
+            Z.propTypes = {}, Z.filterProps = ["borderRadius"], a(c, u, f, d, p, m, h, y, g, b, Z);
             const v = e => {
                 if (void 0 !== e.gap && null !== e.gap) {
                     const t = (0, n.eI)(e.theme, "spacing", 8, "gap"),
                         r = e => ({
                             gap: (0, n.NA)(t, e)
                         });
                     return (0, s.k9)(e, e.gap, r)
@@ -1651,15 +1651,15 @@
                 return null
             };
 
             function w(e, t) {
                 return "grey" === t ? t : e
             }
 
-            function S(e) {
+            function O(e) {
                 return e <= 1 && 0 !== e ? 100 * e + "%" : e
             }
             k.propTypes = {}, k.filterProps = ["rowGap"], a(v, x, k, (0, o.ZP)({
                 prop: "gridColumn"
             }), (0, o.ZP)({
                 prop: "gridRow"
             }), (0, o.ZP)({
@@ -1686,56 +1686,56 @@
                 themeKey: "palette",
                 transform: w
             }), (0, o.ZP)({
                 prop: "backgroundColor",
                 themeKey: "palette",
                 transform: w
             }));
-            const O = (0, o.ZP)({
+            const S = (0, o.ZP)({
                     prop: "width",
-                    transform: S
+                    transform: O
                 }),
-                A = e => {
+                P = e => {
                     if (void 0 !== e.maxWidth && null !== e.maxWidth) {
                         const t = t => {
                             var r, n, o;
                             return {
-                                maxWidth: (null == (r = e.theme) || null == (n = r.breakpoints) || null == (o = n.values) ? void 0 : o[t]) || s.VO[t] || S(t)
+                                maxWidth: (null == (r = e.theme) || null == (n = r.breakpoints) || null == (o = n.values) ? void 0 : o[t]) || s.VO[t] || O(t)
                             }
                         };
                         return (0, s.k9)(e, e.maxWidth, t)
                     }
                     return null
                 };
-            A.filterProps = ["maxWidth"];
-            const P = (0, o.ZP)({
+            P.filterProps = ["maxWidth"];
+            const A = (0, o.ZP)({
                     prop: "minWidth",
-                    transform: S
+                    transform: O
                 }),
-                $ = (0, o.ZP)({
+                j = (0, o.ZP)({
                     prop: "height",
-                    transform: S
+                    transform: O
                 }),
-                T = (0, o.ZP)({
+                $ = (0, o.ZP)({
                     prop: "maxHeight",
-                    transform: S
+                    transform: O
                 }),
-                R = (0, o.ZP)({
+                T = (0, o.ZP)({
                     prop: "minHeight",
-                    transform: S
+                    transform: O
                 }),
-                j = ((0, o.ZP)({
+                R = ((0, o.ZP)({
                     prop: "size",
                     cssProperty: "width",
-                    transform: S
+                    transform: O
                 }), (0, o.ZP)({
                     prop: "size",
                     cssProperty: "height",
-                    transform: S
-                }), a(O, A, P, $, T, R, (0, o.ZP)({
+                    transform: O
+                }), a(S, P, A, j, $, T, (0, o.ZP)({
                     prop: "boxSizing"
                 })), {
                     border: {
                         themeKey: "borders",
                         transform: l
                     },
                     borderTop: {
@@ -1767,15 +1767,15 @@
                         themeKey: "palette"
                     },
                     borderLeftColor: {
                         themeKey: "palette"
                     },
                     borderRadius: {
                         themeKey: "shape.borderRadius",
-                        style: b
+                        style: Z
                     },
                     color: {
                         themeKey: "palette",
                         transform: w
                     },
                     bgcolor: {
                         themeKey: "palette",
@@ -1958,30 +1958,30 @@
                     right: {},
                     bottom: {},
                     left: {},
                     boxShadow: {
                         themeKey: "shadows"
                     },
                     width: {
-                        transform: S
+                        transform: O
                     },
                     maxWidth: {
-                        style: A
+                        style: P
                     },
                     minWidth: {
-                        transform: S
+                        transform: O
                     },
                     height: {
-                        transform: S
+                        transform: O
                     },
                     maxHeight: {
-                        transform: S
+                        transform: O
                     },
                     minHeight: {
-                        transform: S
+                        transform: O
                     },
                     boxSizing: {},
                     fontFamily: {
                         themeKey: "typography"
                     },
                     fontSize: {
                         themeKey: "typography"
@@ -2020,25 +2020,25 @@
                         l = o[e];
                     if (!l) return {
                         [e]: t
                     };
                     const {
                         cssProperty: c = e,
                         themeKey: u,
-                        transform: d,
-                        style: f
+                        transform: f,
+                        style: d
                     } = l;
                     if (null == t) return null;
                     if ("typography" === u && "inherit" === t) return {
                         [e]: t
                     };
                     const p = (0, i.DW)(r, u) || {};
-                    return f ? f(s) : (0, a.k9)(s, t, (t => {
-                        let r = (0, i.Jq)(p, d, t);
-                        return t === r && "string" == typeof t && (r = (0, i.Jq)(p, d, `${e}${"default"===t?"":(0,n.Z)(t)}`, t)), !1 === c ? r : {
+                    return d ? d(s) : (0, a.k9)(s, t, (t => {
+                        let r = (0, i.Jq)(p, f, t);
+                        return t === r && "string" == typeof t && (r = (0, i.Jq)(p, f, `${e}${"default"===t?"":(0,n.Z)(t)}`, t)), !1 === c ? r : {
                             [c]: r
                         }
                     }))
                 }
                 return function t(r) {
                     var n;
                     const {
@@ -2424,15 +2424,15 @@
                         null == t && (o += 1, r(`mui-${o}`))
                     }), [t]), i
                 }(e)
             }
         },
         9962: (e, t, r) => {
             r.d(t, {
-                Z: () => d
+                Z: () => f
             });
             var n = r(6271);
             let o, i = !0,
                 a = !1;
             const s = {
                 text: !0,
                 search: !0,
@@ -2457,15 +2457,15 @@
                 i = !1
             }
 
             function u() {
                 "hidden" === this.visibilityState && a && (i = !0)
             }
 
-            function d() {
+            function f() {
                 const e = n.useCallback((e => {
                         var t;
                         null != e && ((t = e.ownerDocument).addEventListener("keydown", l, !0), t.addEventListener("mousedown", c, !0), t.addEventListener("pointerdown", c, !0), t.addEventListener("touchstart", c, !0), t.addEventListener("visibilitychange", u, !0))
                     }), []),
                     t = n.useRef(!1);
                 return {
                     isFocusVisibleRef: t,
@@ -2510,43 +2510,81 @@
                 Z: () => o
             });
             const o = function() {
                 for (var e, t, r = 0, o = ""; r < arguments.length;)(e = arguments[r++]) && (t = n(e)) && (o && (o += " "), o += t);
                 return o
             }
         },
+        7418: e => {
+            var t = Object.getOwnPropertySymbols,
+                r = Object.prototype.hasOwnProperty,
+                n = Object.prototype.propertyIsEnumerable;
+            e.exports = function() {
+                try {
+                    if (!Object.assign) return !1;
+                    var e = new String("abc");
+                    if (e[5] = "de", "5" === Object.getOwnPropertyNames(e)[0]) return !1;
+                    for (var t = {}, r = 0; r < 10; r++) t["_" + String.fromCharCode(r)] = r;
+                    if ("0123456789" !== Object.getOwnPropertyNames(t).map((function(e) {
+                            return t[e]
+                        })).join("")) return !1;
+                    var n = {};
+                    return "abcdefghijklmnopqrst".split("").forEach((function(e) {
+                        n[e] = e
+                    })), "abcdefghijklmnopqrst" === Object.keys(Object.assign({}, n)).join("")
+                } catch (e) {
+                    return !1
+                }
+            }() ? Object.assign : function(e, o) {
+                for (var i, a, s = function(e) {
+                        if (null == e) throw new TypeError("Object.assign cannot be called with null or undefined");
+                        return Object(e)
+                    }(e), l = 1; l < arguments.length; l++) {
+                    for (var c in i = Object(arguments[l])) r.call(i, c) && (s[c] = i[c]);
+                    if (t) {
+                        a = t(i);
+                        for (var u = 0; u < a.length; u++) n.call(i, a[u]) && (s[a[u]] = i[a[u]])
+                    }
+                }
+                return s
+            }
+        },
         5251: (e, t, r) => {
+            r(7418);
             var n = r(6271),
-                o = Symbol.for("react.element"),
-                i = Symbol.for("react.fragment"),
-                a = Object.prototype.hasOwnProperty,
-                s = n.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,
+                o = 60103;
+            if (t.Fragment = 60107, "function" == typeof Symbol && Symbol.for) {
+                var i = Symbol.for;
+                o = i("react.element"), t.Fragment = i("react.fragment")
+            }
+            var a = n.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,
+                s = Object.prototype.hasOwnProperty,
                 l = {
                     key: !0,
                     ref: !0,
                     __self: !0,
                     __source: !0
                 };
 
             function c(e, t, r) {
                 var n, i = {},
                     c = null,
                     u = null;
-                for (n in void 0 !== r && (c = "" + r), void 0 !== t.key && (c = "" + t.key), void 0 !== t.ref && (u = t.ref), t) a.call(t, n) && !l.hasOwnProperty(n) && (i[n] = t[n]);
+                for (n in void 0 !== r && (c = "" + r), void 0 !== t.key && (c = "" + t.key), void 0 !== t.ref && (u = t.ref), t) s.call(t, n) && !l.hasOwnProperty(n) && (i[n] = t[n]);
                 if (e && e.defaultProps)
                     for (n in t = e.defaultProps) void 0 === i[n] && (i[n] = t[n]);
                 return {
                     $$typeof: o,
                     type: e,
                     key: c,
                     ref: u,
                     props: i,
-                    _owner: s.current
+                    _owner: a.current
                 }
             }
-            t.Fragment = i, t.jsx = c, t.jsxs = c
+            t.jsx = c, t.jsxs = c
         },
         8521: (e, t, r) => {
             e.exports = r(5251)
         }
     }
 ]);
```

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/520.482c287db47780739825.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/520.482c287db47780739825.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/remoteEntry.e80d3b8b00f5114eb1bb.js` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/remoteEntry.1515ab0c4408d370a1f1.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -43,42 +43,42 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        40: "4f257c905f8cbcacb158",
+        40: "2e8dd60e0a5a8bf83e3e",
         122: "83febd31f97f409ed32e",
         126: "dde4a9689e634492f076",
         171: "256ff36dbd88e97f7d85",
         211: "4b143901e7c7d43ccb73",
         222: "3135377346670d94cf92",
-        238: "248c93b1dc2fa4a4015a",
+        238: "47dc92159927183c530c",
         271: "c80d65561d8463123810",
         282: "1bb9d755cf1f2c786d16",
         338: "49da1189f91bad8b01b4",
         378: "d4abe61f25a998d75e66",
         456: "6bda2ceb2cddaccc7e9c",
         520: "482c287db47780739825",
         646: "2440cc17aba449886588",
         747: "233d2b03fe10fa309835",
         794: "a07de7512354fbf79bee",
         799: "4a0c342e3a56827de8fe",
         804: "d8cbf6a18594a5e5e734",
         846: "1e01de8e428bb8d890c8",
         906: "0dfaf4363c1e58ef89b0"
     } [e] + ".js?v=" + {
-        40: "4f257c905f8cbcacb158",
+        40: "2e8dd60e0a5a8bf83e3e",
         122: "83febd31f97f409ed32e",
         126: "dde4a9689e634492f076",
         171: "256ff36dbd88e97f7d85",
         211: "4b143901e7c7d43ccb73",
         222: "3135377346670d94cf92",
-        238: "248c93b1dc2fa4a4015a",
+        238: "47dc92159927183c530c",
         271: "c80d65561d8463123810",
         282: "1bb9d755cf1f2c786d16",
         338: "49da1189f91bad8b01b4",
         378: "d4abe61f25a998d75e66",
         456: "6bda2ceb2cddaccc7e9c",
         520: "482c287db47780739825",
         646: "2440cc17aba449886588",
@@ -143,15 +143,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([S.e(846), S.e(338), S.e(271), S.e(171)]).then((() => () => S(338))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(378), S.e(271), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@mui/material", "5.14.0", (() => Promise.all([S.e(846), S.e(804), S.e(126), S.e(40), S.e(271), S.e(211), S.e(222), S.e(456)]).then((() => () => S(7126))))), i("bootstrap", "5.3.0", (() => Promise.all([S.e(804), S.e(520)]).then((() => () => S(7520))))), i("jupysql-plugin", "0.1.7", (() => Promise.all([S.e(40), S.e(646), S.e(271), S.e(222), S.e(238)]).then((() => () => S(3238))))), i("sql-formatter", "12.2.3", (() => S.e(906).then((() => () => S(9906))))), i("underscore", "1.13.6", (() => S.e(794).then((() => () => S(7794)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([S.e(846), S.e(338), S.e(271), S.e(171)]).then((() => () => S(338))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(378), S.e(271), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@mui/material", "5.14.0", (() => Promise.all([S.e(846), S.e(804), S.e(126), S.e(40), S.e(271), S.e(211), S.e(222), S.e(456)]).then((() => () => S(7126))))), i("bootstrap", "5.3.0", (() => Promise.all([S.e(804), S.e(520)]).then((() => () => S(7520))))), i("jupysql-plugin", "0.1.8", (() => Promise.all([S.e(40), S.e(646), S.e(271), S.e(222), S.e(238)]).then((() => () => S(3238))))), i("sql-formatter", "12.2.3", (() => S.e(906).then((() => () => S(9906))))), i("underscore", "1.13.6", (() => S.e(794).then((() => () => S(7794)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/third-party-licenses.json` & `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9834558823529411%*

 * *Differences: {"'packages'": "{27: {'versionInfo': '17.0.2'}, insert: [(26, OrderedDict([('name', "*

 * *               "'object-assign'), ('versionInfo', '4.1.1'), ('licenseId', 'MIT'), "*

 * *               "('extractedText', 'The MIT License (MIT)\\n\\nCopyright (c) Sindre Sorhus "*

 * *               '<sindresorhus@gmail.com> (sindresorhus.com)\\n\\nPermission is hereby granted, '*

 * *               'free of charge, to any person obtaining a copy\\nof this software and associated '*

 * *               'documentation files (the "Software"),  […]*

```diff
@@ -153,18 +153,24 @@
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014, 2015, 2016, 2017, 2018, 2019 Kartik Chandra, Tim Radvan\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "nearley",
             "versionInfo": "2.20.1"
         },
         {
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) Sindre Sorhus <sindresorhus@gmail.com> (sindresorhus.com)\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "object-assign",
+            "versionInfo": "4.1.1"
+        },
+        {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react",
-            "versionInfo": "18.2.0"
+            "versionInfo": "17.0.2"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-is",
             "versionInfo": "18.2.0"
         },
```

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/server_handlers/dashboard.py` & `jupysql_plugin-0.1.8/jupysql_plugin/server_handlers/dashboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,25 @@
         key = UserSettings().cloud_key
         self.finish(json.dumps({"data": key}))
 
     @tornado.web.authenticated
     def post(self):
         input_data = self.get_json_body()
         user_key = input_data["api_key"]
-        settings = UserSettings()
-        settings.cloud_key = user_key
+
+        # Valid API Key by /users/me API
+        VALIDATION_API_URL = f"{BACKEND_ENDPOINT}/users/me/"
+        headers = {"access_token": user_key}
+        res = requests.get(VALIDATION_API_URL, headers=headers)
+        if res.status_code == 200:
+            settings = UserSettings()
+            settings.cloud_key = user_key
+            self.finish({"result": "success"})
+        else:
+            self.finish({"result": "fail", "detail": res.json()})
 
 
 class JobHandler(APIHandler):
     """
     Endpoint: /dashboard/job
     We need the access the file system through this endpoint, we need below files:
     1. notebook file
@@ -81,21 +90,16 @@
         # Forward request result
         self.finish(json.dumps({"deployment_result": res.json()}))
 
     def file_upload(self, upload_files, file_path):
         try:
             upload_files.append(("files", open(file_path, "rb")))
         except FileNotFoundError:
-            # self.set_status(400)
             self.finish(
-                {
-                    "deployment_result": {
-                        "detail": f"Please make sure you have such file: {file_path}"
-                    }
-                }
+                {"deployment_result": {"detail": file_path, "type": "missing file"}}
             )
             raise FileNotFoundError
 
 
 def setup_handlers(web_app):
     host_pattern = ".*$"
```

### Comparing `jupysql_plugin-0.1.7/jupysql_plugin/widgets/connector_widget.py` & `jupysql_plugin-0.1.8/jupysql_plugin/widgets/connector_widget.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/comm.ts` & `jupysql_plugin-0.1.8/src/comm.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/connector.ts` & `jupysql_plugin-0.1.8/src/connector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/customconnector.ts` & `jupysql_plugin-0.1.8/src/customconnector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/dialog.tsx` & `jupysql_plugin-0.1.8/src/dialog.tsx`

 * *Files 17% similar despite different names*

```diff
@@ -8,46 +8,71 @@
 
 
 export function showDeploymentDialog(panel: any, context: any) {
     const dialogWidget = new DialogWidget({ notebookPath: panel.context.contentsModel.path, metadata: panel.model.metadata, context: context });
     var deploymentDialog = new jupyterlabDialog({
         title: 'Deploy Notebook', body: dialogWidget, buttons: [
             {
-                label: "Cancel",
+                label: "Close",
                 caption: "",
-                className: "",
+                className: "bg-info",
                 accept: false,
                 actions: [],
                 displayType: "default",
                 iconClass: "",
                 iconLabel: "",
             }
         ]
     })
     return deploymentDialog.launch()
 }
 
+const ErrorMessageArea = (props: any): JSX.Element => {
 
-const DialogContent = (props: any): JSX.Element => {
+
+    // Special handle for missing file 
+    if (props?.message?.type == "missing file") {
+        return (
+            <div data-testid="error-message-area">
+
+                {/* <Chip label={deploymentURL} variant="outlined" onClick={() => {
+                                                    window.open(deploymentURL);
+                                                    setIsShowSnackbar(true)
+                                                    setSnakebarMessage("Deployment Success")
+                                                }} /> */}
+                {/* A requirements.txt file with dependencies is required to deploy your notebook. Please add it at {PATH}. To learn more, see the docs */}
+                <Typography variant="subtitle1" gutterBottom> A <code>{props?.message?.detail?.fileName}</code> file with dependencies is required to deploy your notebook. Please add it at <code>{props?.message?.detail?.filePath}</code>. To learn more, see the <a target="_blank" rel="noopener noreferrer" href="https://docs.cloud.ploomber.io/en/latest/dashboards/jupyterlab-plugin.html#create-sample-notebook-and-requirements-txt">docs</a>
+                </Typography>
+            </div>
+        )
+    }
+    else {
+        return (
+            <Typography variant="subtitle1" gutterBottom>{props?.message?.detail}</Typography>
+        )
+    }
+}
+
+export const DialogContent = (props: any): JSX.Element => {
     // For deployment workflow, we need:
     // 1. The path of notebook file 
     // 2. project_id value stored in notebook file
     const notebook_relative_path = props.notebook_path;
     const [projectId] = useState(props?.metadata?.get("ploomber")?.project_id || "");
 
     const [isLoadingRemoteAPI, setIsLoadingRemoteAPI] = useState(true);
     const [isLoadingDeployStatus, setIsLoadingDeployStatus] = useState(false);
     const [isShowSnackbar, setIsShowSnackbar] = useState(false)
     const [isShowFirstTimeDeployPrompt, setIsShowFirstTimeDeployPrompt] = useState(false)
 
     const [APIKey, setAPIKey] = useState("");
-    const [deploymentURL, setDeploymentURL] = useState(null);
+    const [deploymentURL, setDeploymentURL] = useState("");
     const [APIValidStatus, setAPIValidStatus] = useState("init")
-    const [deployErrorMessage, setDeployErrorMessage] = useState("")
-
+    const [deployErrorMessage, setDeployErrorMessage] = useState(null)
+    const [snakebarMessage, setSnakebarMessage] = useState("")
 
     useEffect(() => {
         fetchAPIKey()
     }, [])
 
     // When API Key is verified, init. the first time deployment flow
     useEffect(() => {
@@ -83,16 +108,21 @@
         // When the user enters the API Key, store in the config file through /dashboard/apikey API
         setIsLoadingRemoteAPI(true);
 
         const dataToSend = { 'api_key': APIKey };
         await requestAPI<any>('apikey', {
             body: JSON.stringify(dataToSend),
             method: 'POST'
-        }).then(reply => {
-            setAPIValidStatus("success")
+        }).then(response => {
+            if (response?.result == "success") {
+                setAPIValidStatus("success")
+            }
+            else {
+                setAPIValidStatus("error")
+            }
         }).catch(reason => {
             console.error(
                 `Error on POST ${dataToSend}.\n${reason}`
             );
         });
         setIsLoadingRemoteAPI(false)
     }
@@ -106,26 +136,40 @@
         setIsLoadingDeployStatus(true)
         const dataToSend = { 'notebook_path': notebook_relative_path, 'api_key': APIKey, 'project_id': projectId };
         await requestAPI<any>('job', {
             body: JSON.stringify(dataToSend),
             method: 'POST'
         }).then(reply => {
             var result = reply["deployment_result"]
-            if (result.detail || result.message) {
-                var errorMsg = result.detail || result.message
+            var errorMsg: {
+                type: string,
+                detail: any
+            } = {
+                type: "generic",
+                detail: ""
+            }
+            if (result?.type === "missing file" && result?.detail) {
+                errorMsg.type = result.type
+                errorMsg.detail = {
+                    fileName: "requirements.txt",
+                    filePath: result.detail
+                }
+                setDeployErrorMessage(errorMsg)
+            }
+            else if (result?.detail || result?.message) {
+
+                errorMsg.detail = result.detail || result.message
                 setDeployErrorMessage(errorMsg)
             } else {
-                setDeploymentURL(DEPLOYMENT_ENDPONTS.NEW_JOB + result.project_id + "/" + result.id)
-                props?.metadata.set("ploomber", { "project_id": result.project_id })
-                props.context.save()
+                setDeploymentURL(DEPLOYMENT_ENDPONTS.NEW_JOB + result?.project_id + "/" + result?.id)
+                props?.metadata?.set("ploomber", { "project_id": result?.project_id })
+                props?.context?.save()
             }
             // Write into notebook projectID
-        }).catch(reason => {
-            setDeployErrorMessage(reason)
-        });
+        })
 
         setIsLoadingDeployStatus(false)
 
     }
 
     const APITextFieldProps: { [status: string]: any } = {
         "init": {
@@ -156,15 +200,15 @@
                 : <>
                     <Grid container spacing={4} alignItems="center" direction="column">
                         {APIValidStatus !== "success" &&
                             <div>
                                 <Grid item container direction='row' alignItems="center" width={"100%"}>
                                     <Grid container direction="row" alignItems="center" spacing={1}>
                                         <Grid item xs={10}>
-                                            <TextField id="api-key"
+                                            <TextField id="api-key-input"
                                                 size="small"
                                                 onChange={(val) => { setAPIKey(val.target.value) }}
                                                 value={APIKey}
                                                 label={APITextFieldProps[APIValidStatus]["label"]}
                                                 variant={APITextFieldProps[APIValidStatus]["variant"]}
                                                 color={APITextFieldProps[APIValidStatus]["color"]}
                                                 error={APIValidStatus == "error"}
@@ -182,40 +226,41 @@
                                 </Grid>
 
                             </div>
                         }
                         {APIValidStatus == "success" &&
                             <Grid item container alignItems="center" spacing={4} direction="column">
                                 {!isShowFirstTimeDeployPrompt ? <>
-                                    {deployErrorMessage ? <Typography variant="subtitle1" gutterBottom>{deployErrorMessage}</Typography> :
+                                    {deployErrorMessage ? <ErrorMessageArea message={deployErrorMessage} /> :
                                         <>
                                             <Grid item justifyContent="center" xs={12}>
                                                 Check your deployment status here:
 
                                             </Grid>
                                             <Grid item justifyContent="center" xs={12}>
                                                 <Chip label={deploymentURL} variant="outlined" onClick={() => {
-                                                    navigator.clipboard.writeText(deploymentURL)
+                                                    window.open(deploymentURL);
                                                     setIsShowSnackbar(true)
+                                                    setSnakebarMessage("Deployment Success")
                                                 }} />
                                                 <Snackbar
                                                     open={isShowSnackbar}
                                                     onClose={() => setIsShowSnackbar(false)}
                                                     autoHideDuration={2000}
-                                                    message="Copied to clipboard"
+                                                    message={snakebarMessage}
                                                 />
                                             </Grid>
                                         </>
                                     }
                                 </> : <>
                                     <>
                                         <Typography variant="subtitle1" gutterBottom>
                                             Clicking on deploy will upload your notebook to Ploomber Cloud servers
                                         </Typography>
-                                        <Button onClick={onClickFirstTimeDeploy} variant="contained" size="small" color="primary" disabled={deploymentURL} endIcon={<CloudQueue />}>CONFIRM </Button>
+                                        <Button onClick={onClickFirstTimeDeploy} variant="contained" size="small" color="primary" disabled={deploymentURL !== ""} endIcon={<CloudQueue />}>CONFIRM </Button>
                                     </>
                                 </>}
                             </Grid>
                         }
                     </Grid>
 
                 </>}
```

### Comparing `jupysql_plugin-0.1.7/src/formatter.ts` & `jupysql_plugin-0.1.8/src/formatter.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/index.ts` & `jupysql_plugin-0.1.8/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/keywords.json` & `jupysql_plugin-0.1.8/src/keywords.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/utils/util.ts` & `jupysql_plugin-0.1.8/src/utils/util.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/widgets/connector.ts` & `jupysql_plugin-0.1.8/src/widgets/connector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/widgets/form.ts` & `jupysql_plugin-0.1.8/src/widgets/form.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/src/widgets/table.ts` & `jupysql_plugin-0.1.8/src/widgets/table.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/style/connector.css` & `jupysql_plugin-0.1.8/style/connector.css`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/.gitignore` & `jupysql_plugin-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/LICENSE` & `jupysql_plugin-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/README.md` & `jupysql_plugin-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/pyproject.toml` & `jupysql_plugin-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.7/PKG-INFO` & `jupysql_plugin-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql-plugin
-Version: 0.1.7
+Version: 0.1.8
 Summary: Jupyterlab extension for JupySQL
 Project-URL: Homepage, https://github.com/ploomber/jupysql-plugin.git
 Project-URL: Bug Tracker, https://github.com/ploomber/jupysql-plugin.git/issues
 Project-URL: Repository, https://github.com/ploomber/jupysql-plugin.git.git
 Author-email: Ploomber <contact@ploomber.io>
 License: BSD 3-Clause License
```

