# Comparing `tmp/pygwalker-0.2.0a3.tar.gz` & `tmp/pygwalker-0.2.0a4.tar.gz`

## Comparing `pygwalker-0.2.0a3.tar` & `pygwalker-0.2.0a4.tar`

### file list

```diff
@@ -1,110 +1,111 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/index.html
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/package.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/postcss.config.js
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/tailwind.config.js
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/tsconfig.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/vite.config.ts
--rw-r--r--   0        0        0   133942 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/yarn.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/index.css
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/index.tsx
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/defaultTab.tsx
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/loadingIcon.tsx
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/modal.tsx
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/options.tsx
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/button/base.ts
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/button/default.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/button/primary.tsx
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/codeExportModal/index.tsx
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/codeExportModal/saveConfigButton.tsx
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/initModal/index.tsx
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/dataSource/index.ts
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/interfaces/index.ts
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/notify/index.tsx
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/store/common.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/store/communication.ts
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/tools/exportTool.tsx
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/tools/loginTool.tsx
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/tools/saveTool.tsx
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/communication.ts
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/graphicWalkerParser.ts
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/save.ts
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/screenshot.ts
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/userConfig.ts
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/_constants.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/_typing.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/__init__.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/gwalker.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/html.py
--rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/pygwalker.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/walker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/communications/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/communications/base.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/communications/hacker_comm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/base.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/modin_parser.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/pandas_parser.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/polars_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/__init__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/check_update.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/data_parsers.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/fname_encodings.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/format_invoke_walk_code.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/global_var.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/preview_image.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/render.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/spec.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/tip_tools.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/upload_data.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/index.html
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/preview.html
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/preview_list.html
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/pygwalker_iframe.html
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/walk.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  1935613 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/defaultTab.d.ts
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/loadingIcon.d.ts
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/modal.d.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/button/base.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/button/default.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/button/primary.d.ts
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/codeExportModal/index.d.ts
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/initModal/index.d.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/dataSource/index.d.ts
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/notify/index.d.ts
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/store/common.d.ts
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/store/communication.d.ts
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/tools/exportTool.d.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/tools/loginTool.d.ts
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/tools/saveTool.d.ts
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/communication.d.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/graphicWalkerParser.d.ts
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/save.d.ts
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/screenshot.d.ts
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/userConfig.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/display.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/encode.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/randoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/__main__.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/config.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/defaults.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/__init__.py
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/compile.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/develop.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/LICENSE
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/README.md
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0    14582 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/index.html
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/package.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/postcss.config.js
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/tailwind.config.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/tsconfig.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/vite.config.ts
+-rw-r--r--   0        0        0   133942 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/yarn.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/index.css
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/index.tsx
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/defaultTab.tsx
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/loadingIcon.tsx
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/modal.tsx
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/options.tsx
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/button/base.ts
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/button/default.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/button/primary.tsx
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/codeExportModal/index.tsx
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/codeExportModal/saveConfigButton.tsx
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/components/initModal/index.tsx
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/dataSource/index.ts
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/notify/index.tsx
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/store/common.ts
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/store/communication.ts
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/tools/exportTool.tsx
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/tools/loginTool.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/tools/saveTool.tsx
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/utils/communication.ts
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/utils/graphicWalkerParser.ts
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/utils/save.ts
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/utils/screenshot.ts
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/app/src/utils/userConfig.ts
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/_constants.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/_typing.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/api/__init__.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/api/gwalker.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/api/html.py
+-rw-r--r--   0        0        0    10441 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/api/pygwalker.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/api/walker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/communications/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/communications/base.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/communications/hacker_comm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/data_parsers/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/data_parsers/base.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/data_parsers/modin_parser.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/data_parsers/pandas_parser.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/data_parsers/polars_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/check_update.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/data_parsers.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/fname_encodings.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/format_invoke_walk_code.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/global_var.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/preview_image.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/render.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/spec.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/tip_tools.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/services/upload_data.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/preview.html
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/preview_list.html
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/pygwalker_iframe.html
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/walk.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  1935527 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/defaultTab.d.ts
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/loadingIcon.d.ts
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/modal.d.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/button/base.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/button/default.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/button/primary.d.ts
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/codeExportModal/index.d.ts
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/components/initModal/index.d.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/dataSource/index.d.ts
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/notify/index.d.ts
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/store/common.d.ts
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/store/communication.d.ts
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/tools/exportTool.d.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/tools/loginTool.d.ts
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/tools/saveTool.d.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/utils/communication.d.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/utils/graphicWalkerParser.d.ts
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/utils/save.d.ts
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/utils/screenshot.d.ts
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/templates/dist/utils/userConfig.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/utils/display.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/utils/encode.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/utils/execute_env_check.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker/utils/randoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker_utils/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker_utils/__main__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker_utils/config.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pygwalker_utils/defaults.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/scripts/__init__.py
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/scripts/compile.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/scripts/develop.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/LICENSE
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/README.md
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0    14582 2020-02-02 00:00:00.000000 pygwalker-0.2.0a4/PKG-INFO
```

### Comparing `pygwalker-0.2.0a3/app/package.json` & `pygwalker-0.2.0a4/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/tsconfig.json` & `pygwalker-0.2.0a4/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/vite.config.ts` & `pygwalker-0.2.0a4/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/yarn.lock` & `pygwalker-0.2.0a4/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/index.tsx` & `pygwalker-0.2.0a4/app/src/index.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -25,34 +25,34 @@
 import { getLoginTool } from './tools/loginTool';
 import { domToPng } from "./utils/screenshot"
 
 // @ts-ignore
 import style from './index.css?inline'
 
 
-const initChart = async (gwRef: React.MutableRefObject<IGWHandler | null>, total: number, gid: string) => {
-    if (total !== 0) {
+const initChart = async (gwRef: React.MutableRefObject<IGWHandler | null>, total: number, props: IAppProps) => {
+    if (props.needInitChart && props.env === "jupyter_widgets" && total !== 0) {
         commonStore.initModalOpen = true;
         commonStore.setInitModalInfo({
             title: "Recover Charts",
             curIndex: 0,
             total: total,
         });
         for await (const chart of gwRef.current?.exportChartList("data-url")!) {
             const singleChart = await domToPng(chart.data.container()!);
             await communicationStore.comm?.sendMsg("save_chart", {...chart.data, singleChart});
             commonStore.setInitModalInfo({
                 title: "Recover Charts",
                 curIndex: chart.index + 1,
                 total: chart.total,
             });
-            hidePreview(gid);
+            hidePreview(props.id);
         }
     }
-    commonStore.initModalOpen = false;
+    commonStore.setInitModalOpen(false);
 }
 
 /** App does not consider props.storeRef */
 const App: React.FC<IAppProps> = observer((propsIn) => {
   const storeRef = React.useRef<IGlobalStore|null>(null);
   const gwRef = React.useRef<IGWHandler|null>(null);
   const {dataSource, ...props} = propsIn;
@@ -93,16 +93,16 @@
         storeRef?.current?.commonStore?.updateTempSTDDS({
           name: 'Dataset',
           rawFields: rawFields,
           dataSource: data,
         } as IDataSetInfo);
         storeRef?.current?.commonStore?.commitTempDS();
       }
-      if (!props.needLoadDatas && props.env === "jupyter_widgets") {
-        setTimeout(() => { initChart(gwRef, specList.length, props.id) }, 0);
+      if (!props.needLoadDatas) {
+        setTimeout(() => { initChart(gwRef, specList.length, props) }, 0);
       }
   }, [storeRef])
 
   useEffect(() => {
     setData({ data: dataSource, rawFields, visSpec });
   }, [dataSource, rawFields, visSpec]);
 
@@ -112,19 +112,15 @@
 
   const updateDataSource = useCallback(async () => {
 
     // TODO: don't always update visSpec when appending data
     await loadDataSource(dataSourceProps).then(ds => {
       const data = ds;
       setData({ data, rawFields, visSpec });
-      if (props.env === "jupyter_widgets") {
-        initChart(gwRef, specList.length, props.id);
-      } else {
-        commonStore.setInitModalOpen(false);
-      }
+      initChart(gwRef, specList.length, props);
     }).catch(e => {
       console.error('Load DataSource Error', e);
     });
   }, [dataSource, dataSourceProps, rawFields, visSpec, setData]);
 
   useEffect(() => {
     if (storeRef.current) {
```

### Comparing `pygwalker-0.2.0a3/app/src/components/defaultTab.tsx` & `pygwalker-0.2.0a4/app/src/components/defaultTab.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/loadingIcon.tsx` & `pygwalker-0.2.0a4/app/src/components/loadingIcon.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/modal.tsx` & `pygwalker-0.2.0a4/app/src/components/modal.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/options.tsx` & `pygwalker-0.2.0a4/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/button/default.tsx` & `pygwalker-0.2.0a4/app/src/components/button/default.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/button/primary.tsx` & `pygwalker-0.2.0a4/app/src/components/button/primary.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/codeExportModal/index.tsx` & `pygwalker-0.2.0a4/app/src/components/codeExportModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/codeExportModal/saveConfigButton.tsx` & `pygwalker-0.2.0a4/app/src/components/codeExportModal/saveConfigButton.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/components/initModal/index.tsx` & `pygwalker-0.2.0a4/app/src/components/initModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/dataSource/index.ts` & `pygwalker-0.2.0a4/app/src/dataSource/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/interfaces/index.ts` & `pygwalker-0.2.0a4/app/src/interfaces/index.ts`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     hashcode?: string;
     visSpec?: string;
     userConfig?: IUserConfig;
     env?: string;
     needLoadDatas?: boolean;
     specType?: string;
     showCloudTool: boolean;
+    needInitChart: boolean;
 }
 
 export interface IDataSourceProps {
     tunnelId: string;
     dataSourceId: string;
 }
```

### Comparing `pygwalker-0.2.0a3/app/src/notify/index.tsx` & `pygwalker-0.2.0a4/app/src/notify/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/store/common.ts` & `pygwalker-0.2.0a4/app/src/store/common.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/tools/exportTool.tsx` & `pygwalker-0.2.0a4/app/src/tools/exportTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/tools/loginTool.tsx` & `pygwalker-0.2.0a4/app/src/tools/loginTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/tools/saveTool.tsx` & `pygwalker-0.2.0a4/app/src/tools/saveTool.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -59,19 +59,19 @@
         // if exportChart is undefined, it means that the chart is not reload, so we think dont need to save.
         if (gwRef.current?.exportChart === undefined) {
             saveSuccess();
             return;
         }
         const chartData = await gwRef.current?.exportChart!("data-url");
         const singleChart = await domToPng(chartData.container()!);
-        await communicationStore.comm?.sendMsg("save_chart", {...chartData, singleChart});
-        hidePreview(props.id);
-        await communicationStore.comm?.sendMsg("update_vis_spec", {
-            "content": encodeSpec(storeRef.current?.vizStore.exportViewSpec()!),
+        await communicationStore.comm?.sendMsg("update_spec", {
+            "visSpec": encodeSpec(storeRef.current?.vizStore.exportViewSpec()!),
+            "chartData": {...chartData, singleChart}
         });
+        hidePreview(props.id);
         saveSuccess();
         saveJupyterNotebook();
     }
 
     useEffect(() => {
         let locker = false;
         document.addEventListener("keydown", (event) => {
```

### Comparing `pygwalker-0.2.0a3/app/src/utils/communication.ts` & `pygwalker-0.2.0a4/app/src/utils/communication.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/utils/graphicWalkerParser.ts` & `pygwalker-0.2.0a4/app/src/utils/graphicWalkerParser.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/app/src/utils/save.ts` & `pygwalker-0.2.0a4/app/src/utils/save.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/__init__.py` & `pygwalker-0.2.0a4/pygwalker/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from pygwalker.utils.randoms import rand_str as __rand_str
 from pygwalker_utils.config import get_config as __get_config
 
-__version__ = "0.2.0a3"
+__version__ = "0.2.0a4"
 __hash__ = __rand_str()
 
 from pygwalker.api.walker import walk
 from pygwalker.api.gwalker import GWalker
 from pygwalker.api.html import to_html
 from pygwalker.data_parsers.base import FieldSpec
```

### Comparing `pygwalker-0.2.0a3/pygwalker/_typing.py` & `pygwalker-0.2.0a4/pygwalker/_typing.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/api/gwalker.py` & `pygwalker-0.2.0a4/pygwalker/api/gwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/api/html.py` & `pygwalker-0.2.0a4/pygwalker/api/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         "",
         "",
         hideDataSourceConfig,
         themeKey,
         dark,
         False,
         False,
+        False,
         **kwargs
     )
 
     try:
         html = walker.to_html()
     except Exception as e:
         logging.error(traceback.format_exc())
```

### Comparing `pygwalker-0.2.0a3/pygwalker/api/pygwalker.py` & `pygwalker-0.2.0a4/pygwalker/api/pygwalker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Dict, Any, Optional, Union
 import html as m_html
 import urllib
+import json
 
 from typing_extensions import Literal
 import ipywidgets
 
 from pygwalker_utils.config import get_config
 from pygwalker.utils.display import display_html, display_on_streamlit
 from pygwalker.utils.randoms import rand_str
@@ -36,14 +37,15 @@
         spec: str,
         source_invoke_code: str,
         hidedata_source_config: bool,
         theme_key: Literal['vega', 'g2'],
         dark: Literal['media', 'light', 'dark'],
         show_cloud_tool: bool,
         use_preview: bool,
+        store_chart_data: bool,
         **kwargs
     ):
         if gid is None:
             self.gid = GlobalVarManager.get_global_gid()
         else:
             self.gid = gid
         self.origin_data_source = origin_data_source
@@ -51,30 +53,53 @@
         self.spec = spec
         self.source_invoke_code = source_invoke_code
         self.hidedata_source_config = hidedata_source_config
         self.theme_key = theme_key
         self.dark = dark
         self.data_source_id = rand_str()
         self.other_props = kwargs
-        self.vis_spec, self.spec_type = get_spec_json(spec)
         self.tunnel_id = "tunnel!"
         self.show_cloud_tool = show_cloud_tool
         self.use_preview = use_preview
-        self._chart_map = self._init_chart_map()
+        self.store_chart_data = store_chart_data
+        self._init_spec(spec)
 
-    def _init_chart_map(self) -> Dict[str, ChartData]:
-        return {}
+    def _init_spec(self, spec: Dict[str, Any]):
+        spec_obj, spec_type = get_spec_json(spec)
+        self.vis_spec = spec_obj["config"]
+        self.spec_type = spec_type
+        self._chart_map = self._parse_chart_map_dict(spec_obj["chart_map"])
+
+    def _get_chart_map_dict(self, chart_map: Dict[str, ChartData]) -> Dict[str, Any]:
+        return {
+            key: value.dict(by_alias=True)
+            for key, value in chart_map.items()
+        }
+
+    def _parse_chart_map_dict(self, chart_map_dict: Dict[str, Any]) -> Dict[str, ChartData]:
+        return {
+            key: ChartData.parse_obj(value)
+            for key, value in chart_map_dict.items()
+        }
 
     def to_html(self) -> str:
         props = self._get_props()
         return self._get_render_iframe(props)
 
     def display_on_streamlit(self):
         display_on_streamlit(self.to_html())
 
+    def display_on_convert_html(self):
+        """
+        Display on jupyter-nbconvert html.
+        """
+        props = self._get_props("jupyter")
+        iframe_html = self._get_render_iframe(props)
+        display_html(iframe_html)
+
     def display_on_jupyter(self):
         """
         Display on jupyter notebook/lab.
         If share has large data loading, only sample data can be displayed when reload.
         After that, it will be changed to python for data calculation,
         and only a small amount of data will be output to the front end to complete the analysis of big data.
         """
@@ -122,14 +147,15 @@
             layout=ipywidgets.Layout(display='block')
         )
 
         self._init_callback(comm, preview_tool)
 
         display_html(html_widgets)
         preview_tool.init_display()
+        preview_tool.render(self._chart_map)
 
     @property
     def chart_list(self) -> List[str]:
         """
         Get the list of saved charts.
         """
         return list(self._chart_map.keys())
@@ -200,30 +226,35 @@
                 records=self.origin_data_source,
                 sample_data_count=0,
                 data_source_id=self.data_source_id
             )
             return {}
 
         def get_latest_vis_spec(_):
-            vis_spec, _ = get_spec_json(self.spec)
-            return {"visSpec": vis_spec}
-
-        def update_spec(data: Dict[str, Any]):
-            with open(self.spec, "w", encoding="utf-8") as f:
-                f.write(data["content"])
+            spec_obj, _ = get_spec_json(self.spec)
+            return {"visSpec": spec_obj["config"]}
 
         def save_chart_endpoint(data: Dict[str, Any]):
             chart_data = ChartData.parse_obj(data)
             self._chart_map[data["title"]] = chart_data
             if self.use_preview:
                 preview_tool.render(self._chart_map)
 
+        def update_spec(data: Dict[str, Any]):
+            spec_obj = {"config": data["visSpec"], "chart_map": {}}
+            save_chart_endpoint(data["chartData"])
+            if self.store_chart_data:
+                spec_obj["chart_map"] = self._get_chart_map_dict(self._chart_map)
+
+            with open(self.spec, "w", encoding="utf-8") as f:
+                f.write(json.dumps(spec_obj))
+
         comm.register("request_data", reuqest_data_callback)
         comm.register("get_latest_vis_spec", get_latest_vis_spec)
-        comm.register("update_vis_spec", update_spec)
+        comm.register("update_spec", update_spec)
         comm.register("save_chart", save_chart_endpoint)
 
     def _get_props(
         self,
         env: str = "",
         data_source: Optional[Dict[str, Any]] = None,
         need_load_datas: bool = False
@@ -248,14 +279,15 @@
                 'tunnelId': self.tunnel_id,
                 'dataSourceId': self.data_source_id,
             },
             "env": env,
             "specType": self.spec_type,
             "needLoadDatas": need_load_datas,
             "showCloudTool": self.show_cloud_tool,
+            "needInitChart": not (self.store_chart_data and self._chart_map),
             **self.other_props,
         }
 
     def _get_render_iframe(self, props: Dict[str, Any]) -> str:
         html = render_gwalker_html(self.gid, props)
         srcdoc = m_html.escape(html)
         return render_gwalker_iframe(self.gid, srcdoc)
```

### Comparing `pygwalker-0.2.0a3/pygwalker/api/walker.py` & `pygwalker-0.2.0a4/pygwalker/api/walker.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing_extensions import Literal
 
 from .pygwalker import PygWalker
 from pygwalker.data_parsers.base import FieldSpec, BaseDataParser
 from pygwalker._typing import DataFrame
 from pygwalker.services.data_parsers import get_parser
 from pygwalker.services.format_invoke_walk_code import get_formated_spec_params_code_from_frame
+from pygwalker.utils.execute_env_check import check_convert
 
 
 def walk(
     df: Union[DataFrame, Any],
     gid: Union[int, str] = None,
     *,
     custom_data_parser: Optional[BaseDataParser] = None,
@@ -20,14 +21,15 @@
     hideDataSourceConfig: bool = True,
     themeKey: Literal['vega', 'g2'] = 'g2',
     dark: Literal['media', 'light', 'dark'] = 'media',
     return_html: bool = False,
     spec: str = "",
     show_cloud_tool: bool = False,
     use_preview: bool = False,
+    store_chart_data: bool = False,
     **kwargs
 ):
     """Walk through pandas.DataFrame df with Graphic Walker
 
     Args:
         - df (pl.DataFrame | pd.DataFrame, optional): dataframe.
         - gid (Union[int, str], optional): GraphicWalker container div's id ('gwalker-{gid}')
@@ -38,14 +40,15 @@
         - hideDataSourceConfig (bool, optional): Hide DataSource import and export button (True) or not (False). Default to True
         - themeKey ('vega' | 'g2'): theme type.
         - dark (Literal['media' | 'light' | 'dark']): 'media': auto detect OS theme.
         - return_html (bool, optional): Directly return a html string. Defaults to False.
         - spec (str): chart config data. config id, json, remote file url
         - show_cloud_tool(bool): Whether to use kanaries cloud function, Default to False.
         - use_preview(bool): Whether to use preview function, Default to False.
+        - store_chart_data(bool): Whether to save chart to disk, only work when spec is json file, Default to False.
     """
     if fieldSpecs is None:
         fieldSpecs = {}
 
     source_invoke_code = get_formated_spec_params_code_from_frame(
         inspect.stack()[1].frame
     )
@@ -62,23 +65,28 @@
         spec,
         source_invoke_code,
         hideDataSourceConfig,
         themeKey,
         dark,
         show_cloud_tool,
         use_preview,
+        store_chart_data,
         **kwargs
     )
 
     if return_html:
         return walker.to_html()
 
+    if check_convert():
+        env = "JupyterConvert"
+
     env_display_map = {
         "Streamlit": walker.display_on_streamlit,
         "JupyterWidget": walker.display_on_jupyter_use_widgets,
-        "Jupyter": walker.display_on_jupyter
+        "Jupyter": walker.display_on_jupyter,
+        "JupyterConvert": walker.display_on_convert_html,
     }
 
     display_func = env_display_map.get(env, lambda: None)
     display_func()
 
     return walker
```

### Comparing `pygwalker-0.2.0a3/pygwalker/communications/base.py` & `pygwalker-0.2.0a4/pygwalker/communications/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/communications/hacker_comm.py` & `pygwalker-0.2.0a4/pygwalker/communications/hacker_comm.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import uuid
 import json
 import time
 
 from ipywidgets import Text, Layout, Box
 
 from .base import BaseCommunication
+from pygwalker.utils.encode import DataFrameEncoder
 
 
 class HackerCommunication(BaseCommunication):
     """
     Hacker communication class.
     Since it is not a long running service for multiple users,
     some expired buffers and locks will not be cleaned up.
@@ -53,15 +54,15 @@
         msg = {
             "gid": self.gid,
             "rid": rid,
             "action": action,
             "data": data
         }
         with self._send_msg_lock:
-            self._html_widget.value = json.dumps(msg)
+            self._html_widget.value = json.dumps(msg, cls=DataFrameEncoder)
             self._html_widget.placeholder = str(self.__increase)
             self.__increase += 1
             time.sleep(0.1)
 
     def get_widgets(self) -> Box:
         return Box(
             children=[self._html_widget, self._kernel_widget],
```

### Comparing `pygwalker-0.2.0a3/pygwalker/data_parsers/base.py` & `pygwalker-0.2.0a4/pygwalker/data_parsers/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/data_parsers/modin_parser.py` & `pygwalker-0.2.0a4/pygwalker/data_parsers/modin_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/data_parsers/pandas_parser.py` & `pygwalker-0.2.0a4/pygwalker/data_parsers/pandas_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/data_parsers/polars_parser.py` & `pygwalker-0.2.0a4/pygwalker/data_parsers/polars_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/services/check_update.py` & `pygwalker-0.2.0a4/pygwalker/services/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/services/data_parsers.py` & `pygwalker-0.2.0a4/pygwalker/services/data_parsers.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/services/format_invoke_walk_code.py` & `pygwalker-0.2.0a4/pygwalker/services/format_invoke_walk_code.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/services/preview_image.py` & `pygwalker-0.2.0a4/pygwalker/services/preview_image.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/services/render.py` & `pygwalker-0.2.0a4/pygwalker/services/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/services/spec.py` & `pygwalker-0.2.0a4/pygwalker/services/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib import request
-from typing import Tuple
+from typing import Tuple, Dict, Any
 import json
 import os
 
 from pygwalker_utils.config import get_config
 from pygwalker.errors import InvalidConfigIdError, PrivacyError
 
 
@@ -43,15 +43,15 @@
         int(config_id, 16)
     except ValueError:
         return False
 
     return True
 
 
-def get_spec_json(spec: str) -> Tuple[str, str]:
+def _get_spec_json_from_diff_source(spec: str) -> Tuple[str, str]:
     if not spec or _is_json(spec):
         return spec, "json_string"
 
     if spec.startswith(("http:", "https:")):
         if get_config("privacy")[0] == "offline":
             raise PrivacyError("Due to privacy policy, you can't use this spec offline")
         return _get_spec_from_url(spec), "json_http"
@@ -67,7 +67,24 @@
     file_exist = os.path.exists(spec)
     if file_exist:
         return _get_sepc_from_local(spec), "json_file"
     else:
         with open(spec, "w", encoding="utf-8") as f:
             f.write("")
         return "", "json_file"
+
+
+def get_spec_json(spec: str) -> Tuple[Dict[str, Any], str]:
+    spec, spec_type = _get_spec_json_from_diff_source(spec)
+
+    if not spec:
+        return {"chart_map": {}, "config": ""}, spec_type
+
+    try:
+        spec_obj = json.loads(spec)
+    except json.decoder.JSONDecodeError as e:
+        raise ValueError("spec is not a valid json") from e
+
+    if isinstance(spec_obj, list):
+        return {"chart_map": {}, "config": spec}, spec_type
+
+    return spec_obj, spec_type
```

### Comparing `pygwalker-0.2.0a3/pygwalker/services/tip_tools.py` & `pygwalker-0.2.0a4/pygwalker/services/tip_tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from threading import Thread
 import time
 
 from pygwalker.utils.display import display_html
 
 WIDGETS_TIPS = """
 <div style="">
-If you are using pygwalker on Jupyter and it can't display properly, please execute code to fix it: `pip install "pygwalker[notebook]" --pre`.(close after 15 seconds)
+If you are using pygwalker on Jupyter Notebook(version<7) and it can't display properly, please execute code to fix it: `pip install "pygwalker[notebook]" --pre`.(close after 15 seconds)
 <div>
 """
 
 TIPS_MAP = {
     "widgets": WIDGETS_TIPS
 }
```

### Comparing `pygwalker-0.2.0a3/pygwalker/services/upload_data.py` & `pygwalker-0.2.0a4/pygwalker/services/upload_data.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/preview.html` & `pygwalker-0.2.0a4/pygwalker/templates/preview.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/preview_list.html` & `pygwalker-0.2.0a4/pygwalker/templates/preview_list.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/pygwalker_iframe.html` & `pygwalker-0.2.0a4/pygwalker/templates/pygwalker_iframe.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/walk.js` & `pygwalker-0.2.0a4/pygwalker/templates/walk.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.2.0a4/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -83495,33 +83495,33 @@
         setTimeout((() => {
             var t;
             null == (t = window.parent.document.getElementById(`pygwalker-preview-${e}`)) || t.remove()
         }), 500)
     }
     const kXe = async (e, t, n) => {
         var r, i;
-        if (0 !== t) {
+        if (n.needInitChart && "jupyter_widgets" === n.env && 0 !== t) {
             kGe.initModalOpen = !0, kGe.setInitModalInfo({
                 title: "Recover Charts",
                 curIndex: 0,
                 total: t
             });
             for await (const t of null == (r = e.current) ? void 0 : r.exportChartList("data-url")) {
                 const e = await xXe(t.data.container());
                 await (null == (i = AGe.comm) ? void 0 : i.sendMsg("save_chart", {
                     ...t.data,
                     singleChart: e
                 })), kGe.setInitModalInfo({
                     title: "Recover Charts",
                     curIndex: t.index + 1,
                     total: t.total
-                }), _Xe(n)
+                }), _Xe(n.id)
             }
         }
-        kGe.initModalOpen = !1
+        kGe.setInitModalOpen(!1)
     }, SXe = bm((e => {
         var t;
         const n = xe.useRef(null),
             r = xe.useRef(null),
             {
                 dataSource: i,
                 ...o
@@ -83580,16 +83580,16 @@
                     dsId: "dataSource-0"
                 }],
                 specList: m
             }) : (null == (s = null == (a = null == n ? void 0 : n.current) ? void 0 : a.commonStore) || s.updateTempSTDDS({
                 name: "Dataset",
                 rawFields: d,
                 dataSource: u
-            }), null == (c = null == (l = null == n ? void 0 : n.current) ? void 0 : l.commonStore) || c.commitTempDS()), o.needLoadDatas || "jupyter_widgets" !== o.env || setTimeout((() => {
-                kXe(r, m.length, o.id)
+            }), null == (c = null == (l = null == n ? void 0 : n.current) ? void 0 : l.commonStore) || c.commitTempDS()), o.needLoadDatas || setTimeout((() => {
+                kXe(r, m.length, o)
             }), 0)
         }), [n]);
         ye.useEffect((() => {
             g({
                 data: i,
                 rawFields: l,
                 visSpec: a
@@ -83625,15 +83625,15 @@
                     window.addEventListener("message", a)
                 }))
             }(s).then((e => {
                 g({
                     data: e,
                     rawFields: l,
                     visSpec: a
-                }), "jupyter_widgets" === o.env ? kXe(r, m.length, o.id) : kGe.setInitModalOpen(!1)
+                }), kXe(r, m.length, o)
             })).catch((e => {
                 console.error("Load DataSource Error", e)
             }))
         }), [i, s, l, a, g]);
         ye.useEffect((() => {
             if (n.current) try {
                 b()
@@ -83659,30 +83659,31 @@
                         type: "success",
                         title: "Tips",
                         message: "save success."
                     }, 4e3), setTimeout((() => {
                         i(!1)
                     }), 500)
                 }, s = async () => {
-                    var s, l, c, u, d;
+                    var s, l, c, u;
                     if ("json_file" !== e.specType) return void o({
                         type: "warning",
                         title: "Tips",
                         message: "spec params is not 'json_file', save is not supported."
                     }, 4e3);
                     if (r) return;
                     if (i(!0), void 0 === (null == (s = t.current) ? void 0 : s.exportChart)) return void a();
-                    const f = await (null == (l = t.current) ? void 0 : l.exportChart("data-url")),
-                        p = await xXe(f.container());
-                    await (null == (c = AGe.comm) ? void 0 : c.sendMsg("save_chart", {
-                        ...f,
-                        singleChart: p
-                    })), _Xe(e.id), await (null == (d = AGe.comm) ? void 0 : d.sendMsg("update_vis_spec", {
-                            content: jGe(null == (u = n.current) ? void 0 : u.vizStore.exportViewSpec())
-                        })), a(),
+                    const d = await (null == (l = t.current) ? void 0 : l.exportChart("data-url")),
+                        f = await xXe(d.container());
+                    await (null == (u = AGe.comm) ? void 0 : u.sendMsg("update_spec", {
+                        visSpec: jGe(null == (c = n.current) ? void 0 : c.vizStore.exportViewSpec()),
+                        chartData: {
+                            ...d,
+                            singleChart: f
+                        }
+                    })), _Xe(e.id), a(),
                         function() {
                             const e = window.parent.document;
                             e.body.dispatchEvent(new KeyboardEvent("keydown", {
                                 key: "s",
                                 keyCode: 83,
                                 metaKey: !0
                             })), e.body.dispatchEvent(new KeyboardEvent("keydown", {
```

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/dist/interfaces/index.d.ts` & `pygwalker-0.2.0a4/pygwalker/templates/dist/interfaces/index.d.ts`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     hashcode?: string;
     visSpec?: string;
     userConfig?: IUserConfig;
     env?: string;
     needLoadDatas?: boolean;
     specType?: string;
     showCloudTool: boolean;
+    needInitChart: boolean;
 }
 export interface IDataSourceProps {
     tunnelId: string;
     dataSourceId: string;
 }
 export interface IUserConfig {
     [key: string]: any;
```

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/dist/tools/saveTool.d.ts` & `pygwalker-0.2.0a4/pygwalker/templates/dist/tools/saveTool.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/templates/dist/utils/communication.d.ts` & `pygwalker-0.2.0a4/pygwalker/templates/dist/utils/communication.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker/utils/display.py` & `pygwalker-0.2.0a4/pygwalker/utils/display.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker_utils/__main__.py` & `pygwalker-0.2.0a4/pygwalker_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pygwalker_utils/config.py` & `pygwalker-0.2.0a4/pygwalker_utils/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/scripts/test-init.py` & `pygwalker-0.2.0a4/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/scripts/test-init.sh` & `pygwalker-0.2.0a4/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/.gitignore` & `pygwalker-0.2.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/LICENSE` & `pygwalker-0.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/README.md` & `pygwalker-0.2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/pyproject.toml` & `pygwalker-0.2.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a3/PKG-INFO` & `pygwalker-0.2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwalker
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: pygwalker: Combining Jupyter Notebook with a Tableau-like UI
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: "Asm.Def" <woojson@zju.edu.cn>
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygwalker Version: 0.2.0a3 Summary: pygwalker:
+Metadata-Version: 2.1 Name: pygwalker Version: 0.2.0a4 Summary: pygwalker:
 Combining Jupyter Notebook with a Tableau-like UI Project-URL: homepage, https:
 //github.com/Kanaries/pygwalker Project-URL: repository, https://github.com/
 Kanaries/pygwalker Author-email: "Asm.Def"
 zju.edu.cn> License-File: LICENSE Keywords: data-analysis,data-
 exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist: astor
```

