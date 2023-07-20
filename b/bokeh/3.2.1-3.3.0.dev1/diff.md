# Comparing `tmp/bokeh-3.2.1.tar.gz` & `tmp/bokeh-3.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bokeh-3.2.1.tar", last modified: Thu Jul 20 09:16:44 2023, max compression
+gzip compressed data, was "bokeh-3.3.0.dev1.tar", last modified: Thu Jun 22 16:06:53 2023, max compression
```

## Comparing `bokeh-3.2.1.tar` & `bokeh-3.3.0.dev1.tar`

### file list

```diff
@@ -1,1205 +1,1205 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.291496 bokeh-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-07-20 09:05:06.000000 bokeh-3.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-07-20 09:05:06.000000 bokeh-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    12077 2023-07-20 09:16:44.291496 bokeh-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8603 2023-07-20 09:05:06.000000 bokeh-3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    10430 2023-07-20 09:05:06.000000 bokeh-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 09:16:44.291496 bokeh-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-07-20 09:05:06.000000 bokeh-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.019494 bokeh-3.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.035494 bokeh-3.2.1/src/bokeh/
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    75472 2023-07-20 09:16:28.000000 bokeh-3.2.1/src/bokeh/_sri.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.035494 bokeh-3.2.1/src/bokeh/application/
--rw-r--r--   0 runner    (1001) docker     (122)     2145 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11549 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/application.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.039494 bokeh-3.2.1/src/bokeh/application/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6919 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/code.py
--rw-r--r--   0 runner    (1001) docker     (122)     7818 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/code_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/directory.py
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/document_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     4943 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/function.py
--rw-r--r--   0 runner    (1001) docker     (122)     7975 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/script.py
--rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/server_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/application/handlers/server_request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.039494 bokeh-3.2.1/src/bokeh/client/
--rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16199 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    21727 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/client/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/client/states.py
--rw-r--r--   0 runner    (1001) docker     (122)     3299 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/client/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/client/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.043494 bokeh-3.2.1/src/bokeh/colors/
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14039 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/colors/color.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/colors/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)    13046 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/colors/named.py
--rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/colors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.043494 bokeh-3.2.1/src/bokeh/command/
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommand.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.043494 bokeh-3.2.1/src/bokeh/command/subcommands/
--rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/file_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     4658 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/sampledata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/secret.py
--rw-r--r--   0 runner    (1001) docker     (122)    37703 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/serve.py
--rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/subcommands/static.py
--rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/command/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.047494 bokeh-3.2.1/src/bokeh/core/
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.047494 bokeh-3.2.1/src/bokeh/core/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/autoload_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/autoload_nb_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/autoload_request_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/autoload_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/css_resources.html
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/doc_js.js
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/doc_nb_js.js
--rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/file.html
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/js_resources.html
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/notebook_load.html
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/plot_div.html
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/root_div.html
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/script_tag.html
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/_templates/try_run.js
--rw-r--r--   0 runner    (1001) docker     (122)    16751 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)    29845 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/has_props.py
--rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.055494 bokeh-3.2.1/src/bokeh/core/property/
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/alias.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/any.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/auto.py
--rw-r--r--   0 runner    (1001) docker     (122)    20064 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/bases.py
--rw-r--r--   0 runner    (1001) docker     (122)     6436 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/color.py
--rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/container.py
--rw-r--r--   0 runner    (1001) docker     (122)    22696 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/dataspec.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/descriptor_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    35217 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/either.py
--rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/factors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/include.py
--rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/instance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/nothing.py
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/nullable.py
--rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/numeric.py
--rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/override.py
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/pd.py
--rw-r--r--   0 runner    (1001) docker     (122)     7166 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/primitive.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/readonly.py
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/required.py
--rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/serialized.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/singletons.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/string.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2481 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/text_like.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/vectorization.py
--rw-r--r--   0 runner    (1001) docker     (122)     8905 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/visual.py
--rw-r--r--   0 runner    (1001) docker     (122)    17537 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property_aliases.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/property_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/query.py
--rw-r--r--   0 runner    (1001) docker     (122)    23292 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.055494 bokeh-3.2.1/src/bokeh/core/validation/
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/validation/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     6555 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/validation/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/validation/issue.py
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/core/validation/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.059494 bokeh-3.2.1/src/bokeh/document/
--rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16657 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    27922 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/document.py
--rw-r--r--   0 runner    (1001) docker     (122)    29934 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     4978 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/locking.py
--rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/document/modules.py
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/driving.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.059494 bokeh-3.2.1/src/bokeh/embed/
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14666 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/bundle.py
--rw-r--r--   0 runner    (1001) docker     (122)     6464 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/elements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)    12506 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    17807 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/standalone.py
--rw-r--r--   0 runner    (1001) docker     (122)    14837 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/embed/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    23182 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.063494 bokeh-3.2.1/src/bokeh/io/
--rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/doc.py
--rw-r--r--   0 runner    (1001) docker     (122)    19390 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/export.py
--rw-r--r--   0 runner    (1001) docker     (122)    21518 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/notebook.py
--rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/saving.py
--rw-r--r--   0 runner    (1001) docker     (122)     8278 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/showing.py
--rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/io/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (122)    23032 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.063494 bokeh-3.2.1/src/bokeh/model/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/model/data_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/model/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)    21302 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/model/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     8027 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/model/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.067494 bokeh-3.2.1/src/bokeh/models/
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.071494 bokeh-3.2.1/src/bokeh/models/annotations/
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/arrows.py
--rw-r--r--   0 runner    (1001) docker     (122)    13775 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.071494 bokeh-3.2.1/src/bokeh/models/annotations/html/
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/html/html_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10444 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/html/labels.py
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/html/toolbars.py
--rw-r--r--   0 runner    (1001) docker     (122)     9340 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/labels.py
--rw-r--r--   0 runner    (1001) docker     (122)    16806 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/annotations/legends.py
--rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/axes.py
--rw-r--r--   0 runner    (1001) docker     (122)     7795 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (122)    16739 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/css.py
--rw-r--r--   0 runner    (1001) docker     (122)     6881 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/dom.py
--rw-r--r--   0 runner    (1001) docker     (122)     9495 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/expressions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    24509 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/glyph.py
--rw-r--r--   0 runner    (1001) docker     (122)    54279 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/glyphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/graphics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/grids.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/labeling.py
--rw-r--r--   0 runner    (1001) docker     (122)    23128 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/layouts.py
--rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/map_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    12636 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/mappers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33674 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    17571 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.071494 bokeh-3.2.1/src/bokeh/models/renderers/
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/renderers/contour_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/renderers/glyph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/renderers/graph_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/renderers/renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/renderers/tile_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/scales.py
--rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/selections.py
--rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/selectors.py
--rw-r--r--   0 runner    (1001) docker     (122)    33223 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/sources.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/text.py
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/textures.py
--rw-r--r--   0 runner    (1001) docker     (122)    11476 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/tickers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6596 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/tiles.py
--rw-r--r--   0 runner    (1001) docker     (122)    73516 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     9422 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.075494 bokeh-3.2.1/src/bokeh/models/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/examiner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/icons.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/menus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/panes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/tooltips.py
--rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/ui/ui_element.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.075494 bokeh-3.2.1/src/bokeh/models/util/
--rw-r--r--   0 runner    (1001) docker     (122)      876 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12432 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/util/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.075494 bokeh-3.2.1/src/bokeh/models/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/buttons.py
--rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)    16135 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/inputs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/markups.py
--rw-r--r--   0 runner    (1001) docker     (122)    11229 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/pickers.py
--rw-r--r--   0 runner    (1001) docker     (122)    10242 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/sliders.py
--rw-r--r--   0 runner    (1001) docker     (122)    28151 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/models/widgets/widget.py
--rw-r--r--   0 runner    (1001) docker     (122)   113099 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/palettes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.079494 bokeh-3.2.1/src/bokeh/plotting/
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     8267 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_docstring.py
--rw-r--r--   0 runner    (1001) docker     (122)    32388 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_figure.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     5002 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_legends.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)    12625 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3813 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_stack.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    14637 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/contour.py
--rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/glyph_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/gmap.py
--rw-r--r--   0 runner    (1001) docker     (122)     5836 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/plotting/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.079494 bokeh-3.2.1/src/bokeh/protocol/
--rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    11813 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/message.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.083495 bokeh-3.2.1/src/bokeh/protocol/messages/
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/ack.py
--rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/ok.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/patch_doc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/pull_doc_reply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/pull_doc_req.py
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/push_doc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/server_info_reply.py
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/messages/server_info_req.py
--rw-r--r--   0 runner    (1001) docker     (122)     6987 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/protocol/receiver.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    24107 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.091494 bokeh-3.2.1/src/bokeh/sampledata/
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.095495 bokeh-3.2.1/src/bokeh/sampledata/_data/
--rw-r--r--   0 runner    (1001) docker     (122)    79935 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/USHolidays.ics
--rw-r--r--   0 runner    (1001) docker     (122)   106201 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)    17444 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/auto-mpg.csv
--rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/auto-mpg2.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/browsers_nov_2013.csv
--rw-r--r--   0 runner    (1001) docker     (122)    25491 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/commits.txt.gz
--rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv
--rw-r--r--   0 runner    (1001) docker     (122)    14487 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.095495 bokeh-3.2.1/src/bokeh/sampledata/_data/icons/
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/icons/chrome_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/icons/firefox_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/icons/ie_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/icons/opera_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/icons/safari_32x32.png
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/iris.csv
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/les_mis.json
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/numberly.csv
--rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/olympics2014.json
--rw-r--r--   0 runner    (1001) docker     (122)    13478 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/probly.csv
--rw-r--r--   0 runner    (1001) docker     (122)    14494 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/sample_geojson.geojson
--rw-r--r--   0 runner    (1001) docker     (122)    76453 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz
--rw-r--r--   0 runner    (1001) docker     (122)     5332 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/sprint.csv
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/unemployment1948.csv
--rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/_data/us_marriages_divorces.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/airport_routes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/airports.py
--rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/anscombe.py
--rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/antibiotics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/autompg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/autompg2.py
--rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/browsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/commits.py
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/daylight.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/degrees.py
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/gapminder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/glucose.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/haar_cascade.py
--rw-r--r--   0 runner    (1001) docker     (122)     2371 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/iris.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/les_mis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/movies_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/mtb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/olympics2014.py
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/penguins.py
--rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/perceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/population.py
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/sample_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/sample_superstore.py
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/sea_surface_temperature.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/sprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/stocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/unemployment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/unemployment1948.py
--rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/us_cities.py
--rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/us_counties.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/us_holidays.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/us_marriages_divorces.py
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/us_states.py
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sampledata/world_cities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.095495 bokeh-3.2.1/src/bokeh/server/
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/auth_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    14606 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/protocol_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/server.py
--rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/session.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.031494 bokeh-3.2.1/src/bokeh/server/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.115495 bokeh-3.2.1/src/bokeh/server/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)   211358 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-api.js
--rw-r--r--   0 runner    (1001) docker     (122)   118614 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-api.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   536907 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-gl.js
--rw-r--r--   0 runner    (1001) docker     (122)   198754 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-gl.min.js
--rw-r--r--   0 runner    (1001) docker     (122)  2750414 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-mathjax.js
--rw-r--r--   0 runner    (1001) docker     (122)  1785917 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-mathjax.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   949241 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-tables.js
--rw-r--r--   0 runner    (1001) docker     (122)   302593 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-tables.min.js
--rw-r--r--   0 runner    (1001) docker     (122)   799769 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-widgets.js
--rw-r--r--   0 runner    (1001) docker     (122)   301430 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh-widgets.min.js
--rw-r--r--   0 runner    (1001) docker     (122)  2258934 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh.js
--rw-r--r--   0 runner    (1001) docker     (122)   959905 2023-07-20 09:15:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/bokeh.min.js
--rw-r--r--   0 runner    (1001) docker     (122) 20427534 2023-07-20 09:15:55.000000 bokeh-3.2.1/src/bokeh/server/static/js/compiler.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.147495 bokeh-3.2.1/src/bokeh/server/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.151495 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/charts.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/expr.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/figure.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    19794 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/glyph_api.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/gridplot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      739 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/io.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/linalg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/models.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    63941 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/palettes.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/parser.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/plotting.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/api/themes.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/bokeh.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.151495 bokeh-3.2.1/src/bokeh/server/static/js/lib/client/
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/client/connection.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/client/session.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.155495 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/
--rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/build_views.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/class.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    42976 2023-07-20 09:14:29.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/diagnostics.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-07-20 09:14:29.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/dom_view.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    11975 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/enums.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/geometry.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/graphics.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/has_props.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/hittest.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     8908 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/kinds.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.155495 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/border.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/grid.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/logging.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/patching.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     9618 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/properties.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/property_mixins.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/resolvers.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/selection_manager.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.155495 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/settings.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/signaling.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/ui_events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/uniforms.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.163495 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-07-20 09:14:29.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/affine.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/assert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3294 2023-07-20 09:14:29.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/bbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/bitset.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      592 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/color.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/defer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/eq.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/flip_step_mode.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/interpolation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/iterator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/math.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/matrix.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/menus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/modules.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     7246 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/platform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/pretty.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/projections.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-20 09:14:29.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/random.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/refs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/slice.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/spatial.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/svg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/templating.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/throttle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/typed_array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-07-20 09:14:27.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/version.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/wheel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/zoom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/vectorization.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/view.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.167495 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/
--rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/patterns.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.167495 bokeh-3.2.1/src/bokeh/server/static/js/lib/document/
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/document/defs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/document/document.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/document/events.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/document/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.167495 bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/json.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/notebook.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/server.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/standalone.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      446 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-07-20 09:14:29.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/model.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.167495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.171495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/
--rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      900 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/band.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4135 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.175495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/label.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/span.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/title.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.175495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/
--rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      816 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.175495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-07-20 09:14:28.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.175495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/canvas/
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/canvas/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.175495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/common/
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/common/kinds.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/common/painting.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/common/resolve.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.179495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/coordinates/
--rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/coordinates/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.179495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      932 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/elements.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/html.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/index_.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    16289 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/styles.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-20 09:14:31.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/template.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.183495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.183495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.187495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.195495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/defs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4094 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.199495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/hex_tile.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.frag.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.vert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/rect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.frag.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.vert.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      930 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.199495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/math.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.199495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphics/
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphics/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.199495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/
--rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      933 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.199495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/grids/
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/grids/grid.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/grids/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.203495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/column.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4125 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      523 2023-07-20 09:14:42.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/row.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/main.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.207495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/
--rw-r--r--   0 runner    (1001) docker     (122)      891 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/stack_color_mapper.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-07-20 09:14:41.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.207495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/divider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/menu.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/section.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.207495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/figure.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/plot.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4984 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.207495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/policies/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/policies/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.211495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/random/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/random/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.211495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/range.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.211495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-07-20 09:14:33.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.211495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/continuous_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/scale.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.215495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selections/
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selections/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selections/selection.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.215495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/by_class.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/by_css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/by_id.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/by_xpath.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.215495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.219495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/base_text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/math_text.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.219495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/mathjax/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/mathjax/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/mathjax/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/providers.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/utils.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.219495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-07-20 09:14:30.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/texture.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.223495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/basic_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/datetime_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-20 09:14:38.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/util.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-20 09:14:39.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.223495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/tile_utils.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.227496 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.227496 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/
--rw-r--r--   0 runner    (1001) docker     (122)      903 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      686 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      760 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      766 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.231495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.235495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.235495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-07-20 09:14:36.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-20 09:14:44.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-07-20 09:14:35.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.235495 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/dodge.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.239496 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.239496 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      623 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-07-20 09:14:43.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/pane.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-07-20 09:14:37.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-20 09:14:32.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-20 09:14:34.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/util.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.247496 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1832 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/control.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      901 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/div.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1335 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.251496 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/
--rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4072 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/definitions.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      980 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-07-20 09:14:47.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-07-20 09:14:46.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-07-20 09:14:45.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.251496 bokeh-3.2.1/src/bokeh/server/static/js/lib/protocol/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/protocol/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/protocol/message.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/protocol/receiver.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/safely.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.255496 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/attribution.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/base.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/buttons.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/canvas.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/caret.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/clearfix.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/dialogs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/dropdown.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/examiner.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/group_box.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/icons.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/logo.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/menus.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/plots.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/tabs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/tool_button.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/toolbar.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/tooltips.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/ui.css.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.259496 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/checkbox.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/choices.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/flatpickr.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      430 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/inputs.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/nouislider.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/password_input.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/slickgrid.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/sliders.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/switch.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/widgets/tables.css.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-07-20 09:14:40.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/testing.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 09:14:23.000000 bokeh-3.2.1/src/bokeh/server/static/js/lib/version.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.271496 bokeh-3.2.1/src/bokeh/server/static/lib/
--rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.decorators.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   824027 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.dom.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.collection.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    21204 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.core.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.generator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    14892 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5251 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2016.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2016.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     6227 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    35366 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.date.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    20994 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.number.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.promise.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2739 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.error.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.object.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.string.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    21108 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2023.array.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2023.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2023.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   212834 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es5.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.es6.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.esnext.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.esnext.full.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.esnext.intl.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.scripthost.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)   273794 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.webworker.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)    31831 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/tornado.py
--rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.275496 bokeh-3.2.1/src/bokeh/server/views/
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/app_index.html
--rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/auth_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/autoload_js_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/bokeh-dev.ico
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/bokeh.ico
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/doc_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/ico_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/metadata_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/multi_root_static_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/root_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/static_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/server/views/ws.py
--rw-r--r--   0 runner    (1001) docker     (122)    26423 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.279496 bokeh-3.2.1/src/bokeh/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (122)      929 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.283496 bokeh-3.2.1/src/bokeh/sphinxext/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/bokehjs_content_epilogue.html
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/bokehjs_content_prologue.html
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/bokehjs_html_template.html
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/color_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/enum_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/example_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/gallery_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/gallery_page.rst
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/jinja_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/model_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/options_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/palette_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      481 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/palette_group_detail.html
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/prop_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/release_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/_templates/settings_detail.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_autodoc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_color.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_directive.py
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_example_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_gallery.py
--rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_jinja.py
--rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_palette.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_palette_group.py
--rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     4988 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_prop.py
--rw-r--r--   0 runner    (1001) docker     (122)     3398 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_releases.py
--rw-r--r--   0 runner    (1001) docker     (122)     8083 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_sampledata_xref.py
--rw-r--r--   0 runner    (1001) docker     (122)     4275 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokeh_sitemap.py
--rw-r--r--   0 runner    (1001) docker     (122)     9589 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/bokehjs_content.py
--rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/example_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/sample.py
--rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/sphinxext/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.287496 bokeh-3.2.1/src/bokeh/themes/
--rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/themes/_caliber.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/themes/_contrast.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/themes/_dark_minimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/themes/_light_minimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/themes/_night_sky.py
--rw-r--r--   0 runner    (1001) docker     (122)     9350 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/themes/theme.py
--rw-r--r--   0 runner    (1001) docker     (122)     8284 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/tile_providers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.291496 bokeh-3.2.1/src/bokeh/util/
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4707 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     7856 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/callback_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    18959 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2924 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/hex.py
--rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/package.py
--rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/sampledata.json
--rw-r--r--   0 runner    (1001) docker     (122)     7969 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/sampledata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11396 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/serialization.py
--rw-r--r--   0 runner    (1001) docker     (122)     5419 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)    12872 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/token.py
--rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/tornado.py
--rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-07-20 09:05:06.000000 bokeh-3.2.1/src/bokeh/util/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.035494 bokeh-3.2.1/src/bokeh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12077 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    55013 2023-07-20 09:16:44.000000 bokeh-3.2.1/src/bokeh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-20 09:16:43.000000 bokeh-3.2.1/src/bokeh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:44.291496 bokeh-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-07-20 09:05:07.000000 bokeh-3.2.1/tests/test_bokehjs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-07-20 09:05:07.000000 bokeh-3.2.1/tests/test_cross.py
--rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-07-20 09:05:07.000000 bokeh-3.2.1/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)    10468 2023-07-20 09:05:07.000000 bokeh-3.2.1/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.345097 bokeh-3.3.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-06-22 16:06:53.341096 bokeh-3.3.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8603 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10430 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 16:06:53.345097 bokeh-3.3.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.181093 bokeh-3.3.0.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.189093 bokeh-3.3.0.dev1/src/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3750 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2136 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75472 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/_sri.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.189093 bokeh-3.3.0.dev1/src/bokeh/application/
+-rw-r--r--   0 runner    (1001) docker     (122)     2145 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11549 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/application.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.193094 bokeh-3.3.0.dev1/src/bokeh/application/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6919 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/code.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7818 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/code_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10926 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/document_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4943 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7975 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4705 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5180 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/script.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5035 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/server_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/application/handlers/server_request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.193094 bokeh-3.3.0.dev1/src/bokeh/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     2373 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16199 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21727 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/client/states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3299 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/client/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/client/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.193094 bokeh-3.3.0.dev1/src/bokeh/colors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13955 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/colors/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/colors/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13046 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/colors/named.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/colors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.193094 bokeh-3.3.0.dev1/src/bokeh/command/
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommand.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.193094 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (122)     2802 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2567 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/file_output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4658 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2564 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/sampledata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37703 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/serve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3764 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/subcommands/static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7996 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/command/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.197094 bokeh-3.3.0.dev1/src/bokeh/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.197094 bokeh-3.3.0.dev1/src/bokeh/core/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6450 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_nb_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_request_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/css_resources.html
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/doc_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/doc_nb_js.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/file.html
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/js_resources.html
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/notebook_load.html
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/plot_div.html
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/root_div.html
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/script_tag.html
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/_templates/try_run.js
+-rw-r--r--   0 runner    (1001) docker     (122)    16751 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30043 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/has_props.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.201094 bokeh-3.3.0.dev1/src/bokeh/core/property/
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2782 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/alias.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/any.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20064 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/bases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6436 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22696 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/dataspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/descriptor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35100 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/either.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/factors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/include.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/instance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/nullable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/pd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7166 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/readonly.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/required.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/serialized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/singletons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2481 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/text_like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8905 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/visual.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/property_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23292 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.201094 bokeh-3.3.0.dev1/src/bokeh/core/validation/
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/validation/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6555 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/validation/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9259 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/validation/issue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/core/validation/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.201094 bokeh-3.3.0.dev1/src/bokeh/document/
+-rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16657 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27922 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/document.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29934 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4978 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/locking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/document/modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/driving.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.205094 bokeh-3.3.0.dev1/src/bokeh/embed/
+-rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14666 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6464 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3968 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12506 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17807 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14837 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/embed/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23182 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.205094 bokeh-3.3.0.dev1/src/bokeh/io/
+-rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3375 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19390 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/export.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21518 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/saving.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8278 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/showing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8360 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/io/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23032 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.205094 bokeh-3.3.0.dev1/src/bokeh/model/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/model/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4140 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/model/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21302 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8027 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/model/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.209094 bokeh-3.3.0.dev1/src/bokeh/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.209094 bokeh-3.3.0.dev1/src/bokeh/models/annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/arrows.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13775 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.209094 bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2265 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/html_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10444 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9340 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16806 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/annotations/legends.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12456 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/axes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7795 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16739 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6881 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/dom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9495 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24509 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4197 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54279 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/glyphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6435 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/grids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23128 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/map_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12636 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33674 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17571 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.209094 bokeh-3.3.0.dev1/src/bokeh/models/renderers/
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/renderers/contour_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8796 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/renderers/glyph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/renderers/graph_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4219 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/renderers/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/renderers/tile_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/scales.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/selections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3711 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33223 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/sources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/textures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11476 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6596 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73516 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9422 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.213094 bokeh-3.3.0.dev1/src/bokeh/models/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     2153 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/examiner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/panes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/tooltips.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/ui/ui_element.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.213094 bokeh-3.3.0.dev1/src/bokeh/models/util/
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12432 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/util/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.213094 bokeh-3.3.0.dev1/src/bokeh/models/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4612 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16135 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/markups.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11229 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10819 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/sliders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28151 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/models/widgets/widget.py
+-rw-r--r--   0 runner    (1001) docker     (122)   113099 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/palettes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.213094 bokeh-3.3.0.dev1/src/bokeh/plotting/
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3921 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8267 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32388 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_figure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5002 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_legends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12625 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3813 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14637 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/contour.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27693 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/glyph_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/gmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5836 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/plotting/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.217094 bokeh-3.3.0.dev1/src/bokeh/protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)     5428 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2485 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11813 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/message.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.217094 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/ack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3307 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/ok.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/patch_doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/pull_doc_reply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2334 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/pull_doc_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/push_doc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3072 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/server_info_reply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/messages/server_info_req.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6987 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/protocol/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    24107 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.221094 bokeh-3.3.0.dev1/src/bokeh/sampledata/
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.221094 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/
+-rw-r--r--   0 runner    (1001) docker     (122)    79935 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/USHolidays.ics
+-rw-r--r--   0 runner    (1001) docker     (122)   106201 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    17444 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/auto-mpg.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    17345 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/auto-mpg2.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/browsers_nov_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    25491 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/commits.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    11342 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    14487 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.225094 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/chrome_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/firefox_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/ie_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/opera_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/safari_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/iris.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/les_mis.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/numberly.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    33264 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     8630 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/olympics2014.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13478 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/probly.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    14494 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/sample_geojson.geojson
+-rw-r--r--   0 runner    (1001) docker     (122)    76453 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (122)     5332 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/sprint.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/unemployment1948.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     5387 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/us_marriages_divorces.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/airport_routes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/airports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/anscombe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/antibiotics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/autompg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/autompg2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3112 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/browsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/commits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/daylight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/degrees.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/gapminder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/glucose.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/haar_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2371 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/iris.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/les_mis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/movies_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2096 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/mtb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/olympics2014.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/penguins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/perceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/population.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/sample_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2109 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/sample_superstore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/sea_surface_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3520 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/unemployment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/unemployment1948.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/us_cities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4032 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/us_counties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/us_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/us_marriages_divorces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/us_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sampledata/world_cities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.225094 bokeh-3.3.0.dev1/src/bokeh/server/
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/auth_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6721 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14606 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/protocol_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/session.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.185093 bokeh-3.3.0.dev1/src/bokeh/server/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.237094 bokeh-3.3.0.dev1/src/bokeh/server/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)   211364 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-api.js
+-rw-r--r--   0 runner    (1001) docker     (122)   118620 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-api.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   535981 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-gl.js
+-rw-r--r--   0 runner    (1001) docker     (122)   198524 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2750420 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (122)  1785923 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-mathjax.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   949247 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-tables.js
+-rw-r--r--   0 runner    (1001) docker     (122)   302599 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-tables.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)   799629 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-widgets.js
+-rw-r--r--   0 runner    (1001) docker     (122)   301352 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-widgets.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2257297 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh.js
+-rw-r--r--   0 runner    (1001) docker     (122)   959298 2023-06-22 16:06:03.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh.min.js
+-rw-r--r--   0 runner    (1001) docker     (122) 20427534 2023-06-22 16:06:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/compiler.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.257095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.261095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/charts.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/expr.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4471 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/figure.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    19794 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/glyph_api.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/gridplot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      448 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/io.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3346 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/linalg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/models.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    63941 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/palettes.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5394 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/parser.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/plotting.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/themes.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/bokeh.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.261095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/client/
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/client/connection.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/client/session.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.261095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     5846 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/build_views.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/class.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    42976 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/diagnostics.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/dom_view.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    11975 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/enums.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/geometry.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/graphics.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/has_props.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/hittest.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     8908 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/kinds.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.265095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/border.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/grid.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/logging.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/patching.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     9618 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/properties.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/property_mixins.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/resolvers.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/selection_manager.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.265095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/settings.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/signaling.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6931 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/ui_events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/uniforms.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.269095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/affine.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/assert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3261 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/bbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1486 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/bitset.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/color.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/defer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/eq.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/flip_step_mode.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/interpolation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/iterator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/math.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/matrix.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/menus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/modules.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/platform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/pretty.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/projections.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/random.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/refs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/slice.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/spatial.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/svg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1813 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/templating.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/throttle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/typed_array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-06-22 16:05:13.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/types.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/version.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/wheel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/zoom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/vectorization.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2375 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/view.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.269095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/patterns.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.269095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/defs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4788 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/document.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6205 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/events.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.269095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/json.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/notebook.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/server.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/standalone.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/model.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.273095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.273095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1133 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/band.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4135 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.273095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2245 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/label.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      948 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3650 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1159 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/span.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/title.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.277095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.277095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-22 16:05:14.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.277095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/canvas/
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/canvas/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.277095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/common/kinds.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/common/painting.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/common/resolve.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.277095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/coordinates/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.277095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/elements.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/html.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/index_.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    16289 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/styles.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/template.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.281095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.281095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.281095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.285095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/defs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1293 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4094 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2425 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2116 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1892 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2090 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2543 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2076 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.289095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/hex_tile.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.frag.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/marker.vert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/rect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.frag.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_line.vert.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      930 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3538 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.289095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/utils/math.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.289095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphics/
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphics/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.289095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5351 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.289095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/grids/
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/grids/grid.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/grids/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.293095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/column.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-22 16:05:24.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4125 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/row.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/main.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.293095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/stack_color_mapper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.293095 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/divider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/menu.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/section.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.297096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/figure.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4499 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/plot.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4933 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.297096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/policies/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/policies/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2207 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.297096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/random/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/random/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.297096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/range.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.297096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1306 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2946 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2714 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.297096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/continuous_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/scale.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.301096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selections/
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selections/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selections/selection.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.301096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/by_class.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/by_css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/by_id.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/by_xpath.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.301096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-22 16:05:17.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.301096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/base_text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4357 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/math_text.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.301096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/mathjax/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/mathjax/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/mathjax/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/providers.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/utils.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.301096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-22 16:05:15.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/texture.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.305096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/basic_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/datetime_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      959 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-06-22 16:05:23.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/util.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-06-22 16:05:21.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.305096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2788 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2434 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2277 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/tile_utils.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.305096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.309096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      686 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.309096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1288 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.309096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/index.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.309096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-06-22 16:05:19.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-22 16:05:26.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4551 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.313096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/dodge.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.313096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.313096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-06-22 16:05:25.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/pane.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-06-22 16:05:20.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-22 16:05:16.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-22 16:05:18.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/util.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.317096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/control.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/div.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1884 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.321096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/
+-rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4072 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3920 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/definitions.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/main.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      980 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-22 16:05:28.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-22 16:05:27.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.321096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/protocol/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/protocol/message.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/protocol/receiver.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/safely.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.321096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/attribution.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/base.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/buttons.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/canvas.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/caret.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/clearfix.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/dialogs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/dropdown.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/examiner.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/group_box.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2067 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/icons.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/logo.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/menus.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/plots.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/tabs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/tool_button.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/toolbar.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/tooltips.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/ui.css.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.321096 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/checkbox.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/choices.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/flatpickr.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/inputs.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/nouislider.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/password_input.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/slickgrid.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/sliders.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/switch.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/widgets/tables.css.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-06-22 16:05:22.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/testing.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 16:05:10.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/version.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.333096 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.decorators.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   824027 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.dom.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    16886 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.dom.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.collection.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    21204 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.core.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2552 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.generator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    14892 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3199 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5251 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    10621 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4861 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2016.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2016.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     6227 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2378 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    35366 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.date.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    20994 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.number.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     8378 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.promise.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2739 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     4258 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1152 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.error.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1085 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.object.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1336 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.string.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    21108 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2023.array.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2023.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2023.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   212834 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es5.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es6.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.esnext.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.esnext.full.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.esnext.intl.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.scripthost.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)   273794 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.webworker.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    12132 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts
+-rw-r--r--   0 runner    (1001) docker     (122)    31831 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.333096 bokeh-3.3.0.dev1/src/bokeh/server/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/app_index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/auth_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/autoload_js_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/bokeh-dev.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    15086 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/bokeh.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/doc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/ico_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2571 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/metadata_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/multi_root_static_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/root_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6493 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/static_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/server/views/ws.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26423 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.337097 bokeh-3.3.0.dev1/src/bokeh/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (122)      929 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.337097 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2608 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/bokehjs_content_epilogue.html
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/bokehjs_content_prologue.html
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/bokehjs_html_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/color_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/enum_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/example_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/gallery_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/gallery_page.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/jinja_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/model_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/options_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/palette_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/palette_group_detail.html
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/prop_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/release_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/settings_detail.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_autodoc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_color.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_directive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_example_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3964 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6135 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4828 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_palette.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_palette_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12661 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4988 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_prop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3398 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_releases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8083 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_sampledata_xref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4275 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3791 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9589 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokehjs_content.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4630 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/example_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/sample.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/sphinxext/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.341096 bokeh-3.3.0.dev1/src/bokeh/themes/
+-rw-r--r--   0 runner    (1001) docker     (122)     2904 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/themes/_caliber.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/themes/_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/themes/_dark_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/themes/_light_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2382 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/themes/_night_sky.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9348 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/themes/theme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8284 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/tile_providers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.341096 bokeh-3.3.0.dev1/src/bokeh/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4707 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7856 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/callback_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18959 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2711 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2924 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2303 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/hex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3600 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/sampledata.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7969 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/sampledata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11396 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5419 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12872 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11285 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/src/bokeh/util/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.189093 bokeh-3.3.0.dev1/src/bokeh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    55013 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-22 16:06:53.000000 bokeh-3.3.0.dev1/src/bokeh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 16:06:53.341096 bokeh-3.3.0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/tests/test_bokehjs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/tests/test_cross.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10468 2023-06-22 15:57:43.000000 bokeh-3.3.0.dev1/tests/test_examples.py
```

### Comparing `bokeh-3.2.1/LICENSE.txt` & `bokeh-3.3.0.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/MANIFEST.in` & `bokeh-3.3.0.dev1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/PKG-INFO` & `bokeh-3.3.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh
-Version: 3.2.1
+Version: 3.3.0.dev1
 Summary: Interactive plots and applications in the browser from Python
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: Copyright (c) 2012 - 2023, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `bokeh-3.2.1/README.md` & `bokeh-3.3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/pyproject.toml` & `bokeh-3.3.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/setup.py` & `bokeh-3.3.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/LICENSE.txt` & `bokeh-3.3.0.dev1/src/bokeh/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/__main__.py` & `bokeh-3.3.0.dev1/src/bokeh/__main__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/_sri.json` & `bokeh-3.3.0.dev1/src/bokeh/_sri.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'3.1.1'": "OrderedDict([('bokeh-3.1.1.js', "*

 * *            "'KdEJ8o6fwmtlZEopithF7THb7kDtTMKnHlgtvUZUkxP8JVcDIudFA9IC10dk+eVU'), "*

 * *            "('bokeh-3.1.1.min.js', "*

 * *            "'sb3F9ARvaanE9P+nq6ysz4VWrawTf2ZRbPUmL29lBQqTQf/6uUWqUGRkuU/XU0LX'), "*

 * *            "('bokeh-api-3.1.1.js', "*

 * *            "'NJpyv0S9zH4ydo71Jf0+3y6sO/C47DmqlWyHHvHOFes5XJNC15nmz+SHNW8IKVPp'), "*

 * *            "('bokeh-api-3.1.1.min.js', "*

 * *            "'U2Dj0v1agwB7AL+0nBsK9+ZE3zTL/9smUoSmC5Q7d+Ed2v16W8Yvxlmt52EaMYpq'), "*

 * *            […]*

```diff
@@ -839,36 +839,36 @@
         "bokeh-mathjax-3.1.0.js": "aNziIv4SQnyzfNeKWD2Qn0a7Rhdu6rpaSVr2e8go8aKpcUqYiMCjmqOQjQ74+no7",
         "bokeh-mathjax-3.1.0.min.js": "S5/AsNgTSh+A6J/eT5Q9GuwYarFKmkMolKw1x/6v3YHpYdrUvaTXBA3jBmVPVbKl",
         "bokeh-tables-3.1.0.js": "qJhncLIBrJemVWUXO7kGdSn78JvKy877Cq6QsdIzWq6F8n+RXjkUWwxkjrcC5So4",
         "bokeh-tables-3.1.0.min.js": "dcOPaVYe5Nz32VOQUjUpicV4bE56T/r36LHVL8o2VTvS7CxyvArV5966EdM11+v7",
         "bokeh-widgets-3.1.0.js": "uqeZQEA1PP+YRbE+3WdT0zyhaKKkUpCx1Jzp5gr82pb4MY4FouUPfW0X4NuLXZaG",
         "bokeh-widgets-3.1.0.min.js": "FXG+tFUx+B3ESIZi5RWHDGJSTBAKp0Rju2qzWPCH6QMuFdYmxuge3+bgt7gnADXm"
     },
+    "3.1.1": {
+        "bokeh-3.1.1.js": "KdEJ8o6fwmtlZEopithF7THb7kDtTMKnHlgtvUZUkxP8JVcDIudFA9IC10dk+eVU",
+        "bokeh-3.1.1.min.js": "sb3F9ARvaanE9P+nq6ysz4VWrawTf2ZRbPUmL29lBQqTQf/6uUWqUGRkuU/XU0LX",
+        "bokeh-api-3.1.1.js": "NJpyv0S9zH4ydo71Jf0+3y6sO/C47DmqlWyHHvHOFes5XJNC15nmz+SHNW8IKVPp",
+        "bokeh-api-3.1.1.min.js": "U2Dj0v1agwB7AL+0nBsK9+ZE3zTL/9smUoSmC5Q7d+Ed2v16W8Yvxlmt52EaMYpq",
+        "bokeh-gl-3.1.1.js": "5/Q3liAIXvXg0rsyc+DQKgcifw+hYZ3YmdkdS7nEv9ARq0Nt/xfBj1MHJg/dh1Hy",
+        "bokeh-gl-3.1.1.min.js": "+NM/9usfv2eYRmLMFGNNB80FKu53mDYpIlWPf84N4TOftpHKcXejNcDwqbRtH7sj",
+        "bokeh-mathjax-3.1.1.js": "ivS6JeL60HddXwVfXN9N2+X0+zAMbLMocJlPP2EJIKRa7TuaeiWkgQlZ3pX4GNaL",
+        "bokeh-mathjax-3.1.1.min.js": "HBk5UWx36wzhLHzk7EYkwbNn1rcEMVfWUuSCxZYSWLpyJ7un0AckWQNTdAV4c37f",
+        "bokeh-tables-3.1.1.js": "leHIy9b4P/LSAr8VIlo4uYxbmgVeHDXF1ehi+08L/ExLVnLUFO3ncPejMXSuq1rJ",
+        "bokeh-tables-3.1.1.min.js": "gMVXRZ3HCXODiaQqF+NXwbZNAU2qGpkqtLQsUjroLLdpGzlKxCNDsccJXV4JI8QU",
+        "bokeh-widgets-3.1.1.js": "bBAXr7z/QivJN4IoOm7yRd7yprs+7jmNer9IL0h4SYaqqOpO/7+cOXbyjvWMFUCF",
+        "bokeh-widgets-3.1.1.min.js": "ONzANfOk6Go1ROG5jmeRru3YOlJ4syaxCmnP5BHZeXgWxfcTnXOh/0MGGg8rXLAf"
+    },
     "3.2.0": {
         "bokeh-3.2.0.js": "PHYD6OmUKRMMjOl1Tus3z3qRcW5Mq6buZNJaOpekE5vCxmeXrt54rBCQRf2H20I/",
         "bokeh-3.2.0.min.js": "Ys+Lcdi6xzsbsRHTsjuyl6VCJaZYvj6dmBXbsaoLbkl8jsIEBnHplYnAsJCX2Max",
         "bokeh-api-3.2.0.js": "vENnjGJA3GoZ5Jq5Is3STB6KSM978EVHFgD6mHELp3m6kAjOEid36rOOAfe10AlB",
         "bokeh-api-3.2.0.min.js": "/0JTVRKg2wdxt6Kdr/Ducndfvcs+01HbXhbngpEveSAMT0DJeL+c+AHS7il2142s",
         "bokeh-gl-3.2.0.js": "u8QPMJozxnHD/SZeMIc9W9K0+a03dTA3T4iQ2ozDNcXtGJXLBK/SHqCmLm4IId9N",
         "bokeh-gl-3.2.0.min.js": "DVkY3sm3zxOKqWwmLXOEBtFy/UsDmds7mbNs09ulutBLSBQlZzeISXJ/AHN7l1pj",
         "bokeh-mathjax-3.2.0.js": "PHTOgdzpja3kUOMvxZHbyGsCowxqmoPg78p+iLkE5RmZSobqcHxjcNL0FyY1wGA0",
         "bokeh-mathjax-3.2.0.min.js": "PZ6K6WI2/ckm32BE9L93vH1iq57hEZPeiB+hubSW/KLjUopzPkzK36oIt+MvSYVA",
         "bokeh-tables-3.2.0.js": "ezbF4iP3oacf8s6iSm2cDB6mEtvRZK2QQI531Ouc0pTsiMD7qJCFLIs8AQ41RnOp",
         "bokeh-tables-3.2.0.min.js": "egogtdPd5MX0Qu47PvYsTXHARteEF16TCWDtT2CB7XqbYKWAfF7O1w4yXlm19OT7",
         "bokeh-widgets-3.2.0.js": "TFvltWBiHL2UM+69lNeGlLsg9JLjhcQPYAr6xpK/eJi93wYR0z5pDmONfxBtCg3T",
         "bokeh-widgets-3.2.0.min.js": "/BAPGH7x8fhUAJnOp2GDAPwHQOZ9nWE0Y8uvAEexmquLXVsyV7XOzK5uZZWVXpmR"
-    },
-    "3.2.1": {
-        "bokeh-3.2.1.js": "90+a6Qm7u0jsYDEtsBWv1Dw1EW3Nku4NejRWnQecHHvoDnAoeb6OvXL+ZQ/9U4Q0",
-        "bokeh-3.2.1.min.js": "32tW/NWPQ1H368SPcnJXorq8kn7eJMrip7gweFk+W79dQRpuNlf0PwaHBuEe6YGu",
-        "bokeh-api-3.2.1.js": "7G6Zvzmv2ZWfkOiqeLUkgju1LnHOHxbdg9Y0gt9Y/hzScKVZpkWiSlA/3izgIFG5",
-        "bokeh-api-3.2.1.min.js": "dOF+X1+AfaOGNZ1lv4ww4B90OV3CMZhOg6k/FjMN+rb7qSU/z6Xf3XY1rE3IFSmc",
-        "bokeh-gl-3.2.1.js": "9aCI5oAP8Ep9gCVBvXitFN7Q5Nrz9qN02LgoGTtur4mW5ycz/eGwNp78MdEMG+sO",
-        "bokeh-gl-3.2.1.min.js": "PzqmggKvaWOn7riE4UE5B1wh1194WaA1P4ZcujS8bPmejNxPIzCTaqRDTho3CpQI",
-        "bokeh-mathjax-3.2.1.js": "KIFv+6feg6GlTBBeA/NivZFi0LudVEaGbjfcjoeofwkljqM8m+k4jttwMjLiLlCL",
-        "bokeh-mathjax-3.2.1.min.js": "wZWmpv2IIk9yLzr6mBf7gn1PIbk/OlIfroGvhMM+ZVlC7HDtDUMUEbRzOCmFsYcv",
-        "bokeh-tables-3.2.1.js": "QwB9vmjKFBREvao2UXEvsSAtVbzOEePWSvvqogKmQqvMv7dN8SKmhJejzhEC3QsM",
-        "bokeh-tables-3.2.1.min.js": "7AmdLTDm+oUSxBbwedXxAAFj91YfKo8L6DB0Kbxrv56LTAq2GVp64SPlNqt/JTwC",
-        "bokeh-widgets-3.2.1.js": "fYbyzOWtsLyX9b/IFWpLROVhDz6JbYbWrL2twHd4VDaV6CK7cmeOpq/ZF5uWDB4R",
-        "bokeh-widgets-3.2.1.min.js": "c1Sw4cxc2d9K6DXNSJfFTKAHffnFK15EkQZHlXTCTxfLIcT2dMQV1bFs5Fz9LS0B"
     }
 }
```

### Comparing `bokeh-3.2.1/src/bokeh/application/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/application.py` & `bokeh-3.3.0.dev1/src/bokeh/application/application.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/code.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/code.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/code_runner.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/code_runner.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/directory.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/directory.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/document_lifecycle.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/document_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/function.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/function.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/handler.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/lifecycle.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/notebook.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/request_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/script.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/script.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/server_lifecycle.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/server_lifecycle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/application/handlers/server_request_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/application/handlers/server_request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/client/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/client/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/client/connection.py` & `bokeh-3.3.0.dev1/src/bokeh/client/connection.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/client/session.py` & `bokeh-3.3.0.dev1/src/bokeh/client/session.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/client/states.py` & `bokeh-3.3.0.dev1/src/bokeh/client/states.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/client/util.py` & `bokeh-3.3.0.dev1/src/bokeh/client/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/client/websocket.py` & `bokeh-3.3.0.dev1/src/bokeh/client/websocket.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/colors/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/colors/color.py` & `bokeh-3.3.0.dev1/src/bokeh/colors/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 #-----------------------------------------------------------------------------
 
 # Standard library imports
 import colorsys
 from abc import ABCMeta, abstractmethod
 from math import sqrt
 from re import match
-from typing import TYPE_CHECKING, TypeVar, Union
+from typing import TYPE_CHECKING, Union
 
 # Bokeh imports
 from ..core.serialization import AnyRep, Serializable, Serializer
 from ..util.deprecation import deprecated
 
 if TYPE_CHECKING:
-    from typing_extensions import TypeAlias
+    from typing_extensions import Self, TypeAlias
 
 #-----------------------------------------------------------------------------
 # Globals and constants
 #-----------------------------------------------------------------------------
 
 __all__ = (
     'Color',
@@ -47,16 +47,14 @@
 # General API
 #-----------------------------------------------------------------------------
 
 RGBTuple = Union[tuple[int, int, int], tuple[int, int, int, float]]
 
 ColorLike: TypeAlias = Union[str, "Color", RGBTuple]
 
-Self = TypeVar("Self", bound="Color")
-
 class Color(Serializable, metaclass=ABCMeta):
     ''' A base class for representing color objects.
 
     '''
 
     def __repr__(self) -> str:
         return self.to_css()
@@ -85,23 +83,23 @@
 
         if maximum is not None:
             return min(value, maximum)
         else:
             return value
 
     @abstractmethod
-    def copy(self: Self) -> Self:
+    def copy(self) -> Self:
         ''' Copy this color.
 
         *Subclasses must implement this method.*
 
         '''
         raise NotImplementedError
 
-    def darken(self: Self, amount: float) -> Self:
+    def darken(self, amount: float) -> Self:
         ''' Darken (reduce the luminance) of this color.
 
         *Subclasses must implement this method.*
 
         Args:
             amount (float) :
                 Amount to reduce the luminance by (clamped above zero)
@@ -110,15 +108,15 @@
             Color
 
         '''
         return self.lighten(-amount)
 
     @classmethod
     @abstractmethod
-    def from_hsl(cls: type[Self], value: HSL) -> Self:
+    def from_hsl(cls, value: HSL) -> Self:
         ''' Create a new color by converting from an HSL color.
 
         *Subclasses must implement this method.*
 
         Args:
             value (HSL) :
                 A color to convert from HSL
@@ -127,30 +125,30 @@
             Color
 
         '''
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
-    def from_rgb(cls: type[Self], value: RGB) -> Self:
+    def from_rgb(cls, value: RGB) -> Self:
         ''' Create a new color by converting from an RGB color.
 
         *Subclasses must implement this method.*
 
         Args:
             value (:class:`~bokeh.colors.RGB`) :
                 A color to convert from RGB
 
         Returns:
             Color
 
         '''
         raise NotImplementedError
 
-    def lighten(self: Self, amount: float) -> Self:
+    def lighten(self, amount: float) -> Self:
         ''' Lighten (increase the luminance) of this color.
 
         *Subclasses must implement this method.*
 
         Args:
             amount (float) :
                 Amount to increase the luminance by (clamped above zero)
```

### Comparing `bokeh-3.2.1/src/bokeh/colors/groups.py` & `bokeh-3.3.0.dev1/src/bokeh/colors/groups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/colors/named.py` & `bokeh-3.3.0.dev1/src/bokeh/colors/named.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/colors/util.py` & `bokeh-3.3.0.dev1/src/bokeh/colors/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/command/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/bootstrap.py` & `bokeh-3.3.0.dev1/src/bokeh/command/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommand.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommand.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/build.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/build.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/file_output.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/file_output.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/info.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/init.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/json.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/sampledata.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/sampledata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/secret.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/secret.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/serve.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/serve.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/subcommands/static.py` & `bokeh-3.3.0.dev1/src/bokeh/command/subcommands/static.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/command/util.py` & `bokeh-3.3.0.dev1/src/bokeh/command/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/autoload_js.js` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_js.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/autoload_nb_js.js` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_nb_js.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/autoload_request_tag.html` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_request_tag.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/autoload_tag.html` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/autoload_tag.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/file.html` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/file.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/js_resources.html` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/js_resources.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/notebook_load.html` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/notebook_load.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/_templates/try_run.js` & `bokeh-3.3.0.dev1/src/bokeh/core/_templates/try_run.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/enums.py` & `bokeh-3.3.0.dev1/src/bokeh/core/enums.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/has_props.py` & `bokeh-3.3.0.dev1/src/bokeh/core/has_props.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Literal,
     NoReturn,
     TypedDict,
     TypeVar,
     Union,
     overload,
 )
+from weakref import WeakSet
 
 if TYPE_CHECKING:
     F = TypeVar("F", bound=Callable[..., Any])
     def lru_cache(arg: int | None) -> Callable[[F], F]: ...
 else:
     from functools import lru_cache
 
@@ -94,23 +95,29 @@
 #-----------------------------------------------------------------------------
 
 if TYPE_CHECKING:
     Setter: TypeAlias = Union[ClientSession, ServerSession]
 
 C = TypeVar("C", bound=type["HasProps"])
 
+_abstract_classes: WeakSet[type[HasProps]] = WeakSet()
+
 def abstract(cls: C) -> C:
     ''' A decorator to mark abstract base classes derived from |HasProps|.
 
     '''
     if not issubclass(cls, HasProps):
         raise TypeError(f"{cls.__name__} is not a subclass of HasProps")
+    _abstract_classes.add(cls)
     cls.__doc__ = append_docstring(cls.__doc__, _ABSTRACT_ADMONITION)
     return cls
 
+def is_abstract(cls: type[HasProps]) -> bool:
+    return cls in _abstract_classes
+
 def is_DataModel(cls: type[HasProps]) -> bool:
     from ..model import DataModel
     return issubclass(cls, HasProps) and getattr(cls, "__data_model__", False) and cls != DataModel
 
 def _overridden_defaults(class_dict: dict[str, Any]) -> dict[str, Any]:
     overridden_defaults: dict[str, Any] = {}
     for name, prop in tuple(class_dict.items()):
```

### Comparing `bokeh-3.2.1/src/bokeh/core/json_encoder.py` & `bokeh-3.3.0.dev1/src/bokeh/core/json_encoder.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/properties.py` & `bokeh-3.3.0.dev1/src/bokeh/core/properties.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/_sphinx.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/_sphinx.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/alias.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/alias.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/aliases.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/aliases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/any.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/any.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/auto.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/auto.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/bases.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/bases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/color.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/container.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/container.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/dataspec.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/dataspec.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/datetime.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/datetime.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/descriptor_factory.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/descriptor_factory.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/descriptors.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,16 +320,15 @@
 
         """
         if not hasattr(obj, '_property_values'):
             # Initial values should be passed in to __init__, not set directly
             class_name = obj.__class__.__name__
             raise RuntimeError(f"Cannot set a property value {self.name!r} on a {class_name} instance before HasProps.__init__")
 
-        if self.property.readonly and obj._initialized:
-            # Allow to set a value during object initialization (e.g. value -> value_throttled)
+        if self.property.readonly:
             class_name = obj.__class__.__name__
             raise RuntimeError(f"{class_name}.{self.name} is a readonly property")
 
         value = self.property.prepare_value(obj, self.name, value)
         old = self._get(obj)
         self._set(obj, old, value, setter=setter)
```

### Comparing `bokeh-3.2.1/src/bokeh/core/property/either.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/either.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/enum.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/enum.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/factors.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/factors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/include.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/include.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/instance.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/instance.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/json.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/nothing.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/nothing.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/nullable.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/nullable.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/numeric.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/numeric.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/override.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/override.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/pd.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/pd.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/primitive.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/primitive.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/readonly.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/readonly.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/required.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/required.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/serialized.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/serialized.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/singletons.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/singletons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/string.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/string.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/struct.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/struct.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/text_like.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/text_like.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/validation.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/validation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/vectorization.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/vectorization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/visual.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/visual.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property/wrappers.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,26 +463,26 @@
         """
         old = self._saved_copy()
 
         # TODO (bev) Currently this reports old differently for array vs list
         # For arrays is reports the actual old value. For lists, the old value
         # is actually the already updated value. This is because the method
         # self._saved_copy() makes a shallow copy.
-        for k in new_data:
+        for k, v in new_data.items():
             if isinstance(self[k], np.ndarray) or isinstance(new_data[k], np.ndarray):
                 data = np.append(self[k], new_data[k])
-                if rollover is not None and len(data) > rollover:
-                    data = data[len(data) - rollover:]
+                if rollover and len(data) > rollover:
+                    data = data[-rollover:]
                 # call dict.__setitem__ directly, bypass wrapped version on base class
                 dict.__setitem__(self, k, data)
             else:
                 L = self[k]
                 L.extend(new_data[k])
                 if rollover is not None:
-                    del L[:len(L) - rollover]
+                    del L[:-rollover]
 
         from ...document.events import ColumnsStreamedEvent
         self._notify_owners(old, hint=ColumnsStreamedEvent(doc, source, "data", new_data, rollover, setter))
 
     # don't wrap with notify_owner --- notifies owners explicitly
     def _patch(self, doc: Document, source: ColumnarDataSource, patches, setter: Setter | None = None) -> None:
         """ Internal implementation to handle special-casing patch events
```

### Comparing `bokeh-3.2.1/src/bokeh/core/property_aliases.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property_aliases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/property_mixins.py` & `bokeh-3.3.0.dev1/src/bokeh/core/property_mixins.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/query.py` & `bokeh-3.3.0.dev1/src/bokeh/core/query.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/serialization.py` & `bokeh-3.3.0.dev1/src/bokeh/core/serialization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/templates.py` & `bokeh-3.3.0.dev1/src/bokeh/core/templates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/types.py` & `bokeh-3.3.0.dev1/src/bokeh/core/types.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/validation/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/core/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/validation/check.py` & `bokeh-3.3.0.dev1/src/bokeh/core/validation/check.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/validation/decorators.py` & `bokeh-3.3.0.dev1/src/bokeh/core/validation/decorators.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/validation/errors.py` & `bokeh-3.3.0.dev1/src/bokeh/core/validation/errors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/validation/issue.py` & `bokeh-3.3.0.dev1/src/bokeh/core/validation/issue.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/core/validation/warnings.py` & `bokeh-3.3.0.dev1/src/bokeh/core/validation/warnings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/document/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/callbacks.py` & `bokeh-3.3.0.dev1/src/bokeh/document/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/document.py` & `bokeh-3.3.0.dev1/src/bokeh/document/document.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/events.py` & `bokeh-3.3.0.dev1/src/bokeh/document/events.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/json.py` & `bokeh-3.3.0.dev1/src/bokeh/document/json.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/locking.py` & `bokeh-3.3.0.dev1/src/bokeh/document/locking.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/models.py` & `bokeh-3.3.0.dev1/src/bokeh/document/models.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/document/modules.py` & `bokeh-3.3.0.dev1/src/bokeh/document/modules.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/driving.py` & `bokeh-3.3.0.dev1/src/bokeh/driving.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/bundle.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/bundle.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/elements.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/elements.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/notebook.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/server.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/server.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/standalone.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/standalone.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/util.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/embed/wrappers.py` & `bokeh-3.3.0.dev1/src/bokeh/embed/wrappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/events.py` & `bokeh-3.3.0.dev1/src/bokeh/events.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/ext.py` & `bokeh-3.3.0.dev1/src/bokeh/ext.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/doc.py` & `bokeh-3.3.0.dev1/src/bokeh/io/doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/export.py` & `bokeh-3.3.0.dev1/src/bokeh/io/export.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/notebook.py` & `bokeh-3.3.0.dev1/src/bokeh/io/notebook.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/output.py` & `bokeh-3.3.0.dev1/src/bokeh/io/output.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/saving.py` & `bokeh-3.3.0.dev1/src/bokeh/io/saving.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/showing.py` & `bokeh-3.3.0.dev1/src/bokeh/io/showing.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/state.py` & `bokeh-3.3.0.dev1/src/bokeh/io/state.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/util.py` & `bokeh-3.3.0.dev1/src/bokeh/io/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/io/webdriver.py` & `bokeh-3.3.0.dev1/src/bokeh/io/webdriver.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/layouts.py` & `bokeh-3.3.0.dev1/src/bokeh/layouts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/model/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/model/data_model.py` & `bokeh-3.3.0.dev1/src/bokeh/model/data_model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/model/docs.py` & `bokeh-3.3.0.dev1/src/bokeh/model/docs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/model/model.py` & `bokeh-3.3.0.dev1/src/bokeh/model/model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/model/util.py` & `bokeh-3.3.0.dev1/src/bokeh/model/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/annotation.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/annotation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/arrows.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/arrows.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/geometry.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/geometry.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/html/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/html/html_annotation.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/html_annotation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/html/labels.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/labels.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/html/toolbars.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/html/toolbars.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/labels.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/labels.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/annotations/legends.py` & `bokeh-3.3.0.dev1/src/bokeh/models/annotations/legends.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/axes.py` & `bokeh-3.3.0.dev1/src/bokeh/models/axes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/callbacks.py` & `bokeh-3.3.0.dev1/src/bokeh/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/canvas.py` & `bokeh-3.3.0.dev1/src/bokeh/models/canvas.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/coordinates.py` & `bokeh-3.3.0.dev1/src/bokeh/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/css.py` & `bokeh-3.3.0.dev1/src/bokeh/models/css.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/dom.py` & `bokeh-3.3.0.dev1/src/bokeh/models/dom.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/expressions.py` & `bokeh-3.3.0.dev1/src/bokeh/models/expressions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/filters.py` & `bokeh-3.3.0.dev1/src/bokeh/models/filters.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/formatters.py` & `bokeh-3.3.0.dev1/src/bokeh/models/formatters.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/glyph.py` & `bokeh-3.3.0.dev1/src/bokeh/models/glyph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/glyphs.py` & `bokeh-3.3.0.dev1/src/bokeh/models/glyphs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/graphics.py` & `bokeh-3.3.0.dev1/src/bokeh/models/graphics.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/graphs.py` & `bokeh-3.3.0.dev1/src/bokeh/models/graphs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/grids.py` & `bokeh-3.3.0.dev1/src/bokeh/models/grids.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/labeling.py` & `bokeh-3.3.0.dev1/src/bokeh/models/labeling.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/layouts.py` & `bokeh-3.3.0.dev1/src/bokeh/models/layouts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/map_plots.py` & `bokeh-3.3.0.dev1/src/bokeh/models/map_plots.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/mappers.py` & `bokeh-3.3.0.dev1/src/bokeh/models/mappers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/plots.py` & `bokeh-3.3.0.dev1/src/bokeh/models/plots.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ranges.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ranges.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,16 +329,16 @@
     units of a business.
 
     For 2- and 3- level factors, each factor is a tuple of strings:
 
     .. code-block:: python
 
         FactorRange(factors=[
-            ["2016", "sales"], ["2016", "marketing"], ["2016", "engineering"],
-            ["2017", "sales"], ["2017", "marketing"], ["2017", "engineering"],
+            ["2016", "sales'], ["2016", "marketing'], ["2016", "engineering"],
+            ["2017", "sales'], ["2017", "marketing'], ["2017", "engineering"],
         ])
 
     defines a range with six 2-level factors that might represent the three
     business units, grouped by year.
 
     Note that factors and sub-factors *may only be strings*.
 
@@ -371,18 +371,18 @@
     group_padding = Float(default=1.4, help="""
     How much padding to add in between top-level groups of factors. This
     property only applies when the overall range factors have either two or
     three levels. For example, with:
 
     .. code-block:: python
 
-        FactorRange(factors=[["foo", "1"], ["foo", "2"], ["bar", "1"]])
+        FactorRange(factors=[["foo", "1'], ["foo", "2'], ["bar", "1"]])
 
     The top level groups correspond to ``"foo"` and ``"bar"``, and the
-    group padding will be applied between the factors ``["foo", "2"]`` and
+    group padding will be applied between the factors ``["foo", "2']`` and
     ``["bar", "1"]``
     """)
 
     range_padding = Float(default=0, help="""
     How much padding to add around the outside of computed range bounds.
 
     When ``range_padding_units`` is set to ``"percent"``, the span of the
```

### Comparing `bokeh-3.2.1/src/bokeh/models/renderers/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/models/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/renderers/contour_renderer.py` & `bokeh-3.3.0.dev1/src/bokeh/models/renderers/contour_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/renderers/glyph_renderer.py` & `bokeh-3.3.0.dev1/src/bokeh/models/renderers/glyph_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/renderers/graph_renderer.py` & `bokeh-3.3.0.dev1/src/bokeh/models/renderers/graph_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/renderers/renderer.py` & `bokeh-3.3.0.dev1/src/bokeh/models/renderers/renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/renderers/tile_renderer.py` & `bokeh-3.3.0.dev1/src/bokeh/models/renderers/tile_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/scales.py` & `bokeh-3.3.0.dev1/src/bokeh/models/scales.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/selections.py` & `bokeh-3.3.0.dev1/src/bokeh/models/selections.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/selectors.py` & `bokeh-3.3.0.dev1/src/bokeh/models/selectors.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/sources.py` & `bokeh-3.3.0.dev1/src/bokeh/models/sources.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/text.py` & `bokeh-3.3.0.dev1/src/bokeh/models/text.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/textures.py` & `bokeh-3.3.0.dev1/src/bokeh/models/textures.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/tickers.py` & `bokeh-3.3.0.dev1/src/bokeh/models/tickers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/tiles.py` & `bokeh-3.3.0.dev1/src/bokeh/models/tiles.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/tools.py` & `bokeh-3.3.0.dev1/src/bokeh/models/tools.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/transforms.py` & `bokeh-3.3.0.dev1/src/bokeh/models/transforms.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/dialogs.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/examiner.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/examiner.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/icons.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/icons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/menus.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/menus.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/panes.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/panes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/tooltips.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/tooltips.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/ui/ui_element.py` & `bokeh-3.3.0.dev1/src/bokeh/models/ui/ui_element.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/util/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/models/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/util/structure.py` & `bokeh-3.3.0.dev1/src/bokeh/models/util/structure.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/buttons.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/groups.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/groups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/inputs.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/inputs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/markups.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/markups.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/pickers.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/pickers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/sliders.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/sliders.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     Nullable,
     Override,
     Readonly,
     Required,
     String,
     Tuple,
 )
+from ...core.property.descriptors import UnsetValueError
+from ...core.property.singletons import Undefined
 from ...core.validation import error
 from ...core.validation.errors import EQUAL_SLIDER_START_END
 from ..formatters import TickFormatter
 from .widget import Widget
 
 #-----------------------------------------------------------------------------
 # Globals and constants
@@ -65,23 +67,36 @@
 #-----------------------------------------------------------------------------
 
 @abstract
 class AbstractSlider(Widget):
     """ """
 
     def __init__(self, *args, **kwargs) -> None:
-        if 'start' in kwargs and 'end' in kwargs:
-            if kwargs['start'] == kwargs['end']:
-                raise ValueError("Slider 'start' and 'end' cannot be equal.")
-
-        if "value" in kwargs and "value_throttled" not in kwargs:
-            kwargs["value_throttled"] = kwargs["value"]
-
         super().__init__(*args, **kwargs)
 
+        try:
+            # synchronize the value of a readonly property `value_throttled`
+            self.lookup("value_throttled")._set(self, Undefined, self.value)
+        except UnsetValueError:
+            pass
+        except AttributeError:
+            # TODO Remove this when proper support for property overrides is
+            # implemented. For now this is required to make defaults' tests
+            # work, because we depend there on model instances to provide
+            # "default" values.
+            pass
+
+    # TODO value = Required(GenericType, help="""
+    # Initial or selected range.
+    # """)
+
+    # TODO value_throttled = Readonly(GenericType, help="""
+    # Initial or selected value, throttled according to report only on mouseup.
+    # """)
+
     orientation = Enum("horizontal", "vertical", help="""
     Orient the slider either horizontally (default) or vertically.
     """)
 
     title = Nullable(String, default="", help="""
     The slider's label (supports :ref:`math text <ug_styling_mathtext>`).
     """)
```

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/tables.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/tables.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/models/widgets/widget.py` & `bokeh-3.3.0.dev1/src/bokeh/models/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/palettes.py` & `bokeh-3.3.0.dev1/src/bokeh/palettes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_decorators.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_decorators.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_docstring.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_docstring.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_figure.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_figure.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_graph.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_graph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_legends.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_legends.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_plot.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_plot.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_renderer.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_renderer.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_stack.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_stack.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/_tools.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/_tools.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/contour.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/contour.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/glyph_api.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/glyph_api.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/gmap.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/gmap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/plotting/graph.py` & `bokeh-3.3.0.dev1/src/bokeh/plotting/graph.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/exceptions.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/message.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/message.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/ack.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/ack.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/error.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/error.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/ok.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/ok.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/patch_doc.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/patch_doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/pull_doc_reply.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/pull_doc_reply.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/pull_doc_req.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/pull_doc_req.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/push_doc.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/push_doc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/server_info_reply.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/server_info_reply.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/messages/server_info_req.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/messages/server_info_req.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/protocol/receiver.py` & `bokeh-3.3.0.dev1/src/bokeh/protocol/receiver.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/resources.py` & `bokeh-3.3.0.dev1/src/bokeh/resources.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/USHolidays.ics` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/USHolidays.ics`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/US_Regions_State_Boundaries.csv.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/auto-mpg.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/auto-mpg.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/auto-mpg2.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/auto-mpg2.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/browsers_nov_2013.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/browsers_nov_2013.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/commits.txt.gz` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/commits.txt.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/daylight_warsaw_2013.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/elements.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/elements.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/icons/chrome_32x32.png` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/chrome_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/icons/firefox_32x32.png` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/firefox_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/icons/ie_32x32.png` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/ie_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/icons/opera_32x32.png` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/opera_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/icons/safari_32x32.png` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/icons/safari_32x32.png`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/iris.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/iris.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/les_mis.json` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/les_mis.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/numberly.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/numberly.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/obiszow_mtb_xcm.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/olympics2014.json` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/olympics2014.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/penguins.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/penguins.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/percent-bachelors-degrees-women-usa.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/probly.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/probly.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/sample_geojson.geojson` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/sample_geojson.geojson`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/sea_surface_temperature.csv.gz`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/sprint.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/sprint.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/unemployment1948.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/unemployment1948.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/_data/us_marriages_divorces.csv` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/_data/us_marriages_divorces.csv`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/airport_routes.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/airport_routes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/airports.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/airports.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/anscombe.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/anscombe.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/antibiotics.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/antibiotics.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/autompg.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/autompg.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/autompg2.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/autompg2.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/browsers.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/browsers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/commits.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/commits.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/daylight.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/daylight.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/degrees.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/degrees.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/gapminder.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/gapminder.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/glucose.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/glucose.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/haar_cascade.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/haar_cascade.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/iris.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/les_mis.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/les_mis.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/movies_data.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/movies_data.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/mtb.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/mtb.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/olympics2014.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/olympics2014.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/penguins.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/penguins.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/perceptions.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/perceptions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/periodic_table.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/periodic_table.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/population.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/population.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/sample_geojson.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/sample_geojson.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/sample_superstore.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/sample_superstore.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/sea_surface_temperature.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/sea_surface_temperature.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/sprint.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/sprint.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/stocks.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/stocks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/unemployment.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/unemployment.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/unemployment1948.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/unemployment1948.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/us_cities.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/us_cities.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/us_counties.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/us_counties.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/us_holidays.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/us_holidays.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/us_marriages_divorces.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/us_marriages_divorces.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/us_states.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/us_states.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sampledata/world_cities.py` & `bokeh-3.3.0.dev1/src/bokeh/sampledata/world_cities.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/server/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/auth_provider.py` & `bokeh-3.3.0.dev1/src/bokeh/server/auth_provider.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/callbacks.py` & `bokeh-3.3.0.dev1/src/bokeh/server/callbacks.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/connection.py` & `bokeh-3.3.0.dev1/src/bokeh/server/connection.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/contexts.py` & `bokeh-3.3.0.dev1/src/bokeh/server/contexts.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/protocol_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/protocol_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/server.py` & `bokeh-3.3.0.dev1/src/bokeh/server/server.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/session.py` & `bokeh-3.3.0.dev1/src/bokeh/server/session.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-api.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-api.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -72,15 +72,15 @@
                 var object_1 = require(9) /* ../core/util/object */ ;
                 __esExport("keys", object_1.keys);
                 __esExport("values", object_1.values);
                 __esExport("entries", object_1.entries);
                 __esExport("size", object_1.size);
                 __esExport("extend", object_1.extend);
                 tslib_1.__exportStar(require(10) /* ../core/util/array */ , exports);
-                tslib_1.__exportStar(require(39) /* ../core/util/string */ , exports);
+                tslib_1.__exportStar(require(38) /* ../core/util/string */ , exports);
                 tslib_1.__exportStar(require(265) /* ../core/util/random */ , exports);
                 tslib_1.__exportStar(require(8) /* ../core/util/types */ , exports);
                 tslib_1.__exportStar(require(25) /* ../core/util/eq */ , exports);
                 const ndarray_1 = require(29) /* ../core/util/ndarray */ ;
                 const types_1 = require(8) /* ../core/util/types */ ;
                 const array_1 = require(10) /* ../core/util/array */ ;
                 const arrayable_1 = require(13) /* ../core/util/arrayable */ ;
@@ -2339,15 +2339,15 @@
                 const tslib_1 = require(1) /* tslib */ ;
                 const properties_1 = require(17) /* ../core/properties */ ;
                 const class_1 = require(545) /* ../core/class */ ;
                 const eq_1 = require(25) /* ../core/util/eq */ ;
                 const array_1 = require(10) /* ../core/util/array */ ;
                 const object_1 = require(9) /* ../core/util/object */ ;
                 const types_1 = require(8) /* ../core/util/types */ ;
-                const iterator_1 = require(33) /* ../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../core/util/iterator */ ;
                 const nd = tslib_1.__importStar(require(29) /* ../core/util/ndarray */ );
                 const models_1 = require(542) /* ./models */ ;
                 const legend_1 = require(253) /* ../models/annotations/legend */ ;
                 const legend_item_1 = require(254) /* ../models/annotations/legend_item */ ;
                 const figure_1 = require(410) /* ../models/plots/figure */ ;
                 const glyph_api_1 = require(546) /* ./glyph_api */ ;
                 const {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-api.min.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-api.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -57,15 +57,15 @@
                 const p = i.__importStar(t(541));
                 o.Palettes = p, o.Themes = i.__importStar(t(550)), n("Document", t(5).Document), n("sprintf", t(170).sprintf), i.__exportStar(t(542), o), n("f", t(551).f)
             },
             539: function _(r, t, e, n, a) {
                 n();
                 const i = r(1);
                 var o = r(9);
-                a("keys", o.keys), a("values", o.values), a("entries", o.entries), a("size", o.size), a("extend", o.extend), i.__exportStar(r(10), e), i.__exportStar(r(39), e), i.__exportStar(r(265), e), i.__exportStar(r(8), e), i.__exportStar(r(25), e);
+                a("keys", o.keys), a("values", o.values), a("entries", o.entries), a("size", o.size), a("extend", o.extend), i.__exportStar(r(10), e), i.__exportStar(r(38), e), i.__exportStar(r(265), e), i.__exportStar(r(8), e), i.__exportStar(r(25), e);
                 const s = r(29),
                     u = r(8),
                     p = r(10),
                     f = r(13),
                     l = r(265),
                     m = r(25),
                     h = r(11),
@@ -1239,15 +1239,15 @@
                 const o = e(1),
                     l = e(17),
                     a = e(545),
                     c = e(25),
                     _ = e(10),
                     d = e(9),
                     u = e(8),
-                    g = e(33),
+                    g = e(32),
                     h = o.__importStar(e(29)),
                     f = e(542),
                     p = e(253),
                     x = e(254),
                     m = e(410),
                     y = e(546),
                     {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-gl.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-gl.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -10946,18 +10946,17 @@
                     _get_visuals() {
                         return this.glyph.visuals;
                     }
                     draw(indices, main_glyph, transform) {
                         this._draw_impl(indices, transform, main_glyph.glglyph, this.marker_type);
                     }
                     _draw_impl(indices, transform, main_gl_glyph, marker_type) {
-                        if (main_gl_glyph.data_changed || main_gl_glyph.data_mapped) {
+                        if (main_gl_glyph.data_changed) {
                             main_gl_glyph.set_data();
                             main_gl_glyph.data_changed = false;
-                            main_gl_glyph.data_mapped = false;
                         }
                         if (this.visuals_changed) {
                             this._set_visuals();
                             this.visuals_changed = false;
                         }
                         const nmarkers = main_gl_glyph.nvertices;
                         const prev_nmarkers = this._show.length;
@@ -11107,32 +11106,28 @@
             524: /* models/glyphs/webgl/base.js */ function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 class BaseGLGlyph {
                     constructor(regl_wrapper, glyph) {
                         this.nvertices = 0;
                         this.size_changed = false;
                         this.data_changed = false;
-                        this.data_mapped = false;
                         this.visuals_changed = false;
                         this.regl_wrapper = regl_wrapper;
                         this.glyph = glyph;
                     }
                     set_data_changed() {
                         const {
                             data_size
                         } = this.glyph;
                         if (data_size != this.nvertices) {
                             this.nvertices = data_size;
                             this.size_changed = true;
                         }
                         this.data_changed = true;
                     }
-                    set_data_mapped() {
-                        this.data_mapped = true;
-                    }
                     set_visuals_changed() {
                         this.visuals_changed = true;
                     }
                     render(_ctx, indices, mainglyph) {
                         if (indices.length == 0) {
                             return;
                         }
@@ -11423,18 +11418,17 @@
                         this._miter_limit = 10.0; // Threshold for miters to be replaced by bevels.
                     }
                     _draw_impl(indices, transform, main_gl_glyph) {
                         if (this.visuals_changed) {
                             this._set_visuals();
                             this.visuals_changed = false;
                         }
-                        if (main_gl_glyph.data_changed || main_gl_glyph.data_mapped) {
-                            main_gl_glyph._set_data(main_gl_glyph.data_changed);
+                        if (main_gl_glyph.data_changed) {
+                            main_gl_glyph._set_data();
                             main_gl_glyph.data_changed = false;
-                            main_gl_glyph.data_mapped = false;
                         }
                         const line_visuals = this._get_visuals().line;
                         const line_cap = webgl_utils_1.cap_lookup[line_visuals.line_cap.value];
                         const line_join = webgl_utils_1.join_lookup[line_visuals.line_join.value];
                         const points = main_gl_glyph._points;
                         const nsegments = points.length / 2 - 3; // Points array includes extra points at each end
                         const show = this._get_show_buffer(indices, main_gl_glyph);
@@ -11465,44 +11459,37 @@
                         } else {
                             this.regl_wrapper.solid_line()(solid_props);
                         }
                     }
                     _is_dashed() {
                         return this._line_dash != null && this._line_dash.length > 0;
                     }
-                    _set_data(data_changed) {
-                        // If data_changed is false the underlying glyph data has not changed but has been mapped to
-                        // different canvas coordinates e.g. via pan or zoom. If data_changed is true the data itself
-                        // has changed, which also implies it has been mapped.
+                    _set_data() {
                         const points_array = this._set_data_points();
-                        if (data_changed) {
-                            // Points array includes extra points at each end
-                            const npoints = points_array.length / 2 - 2;
-                            if (this._show == null)
-                                this._show = new buffer_1.Uint8Buffer(this.regl_wrapper);
-                            const show_array = this._show.get_sized_array(npoints + 1);
-                            let start_finite = isFinite(points_array[2]) && isFinite(points_array[3]);
-                            for (let i = 1; i < npoints; i++) {
-                                const end_finite = isFinite(points_array[2 * i + 2]) && isFinite(points_array[2 * i + 3]);
-                                show_array[i] = (start_finite && end_finite) ? 1 : 0;
-                                start_finite = end_finite;
-                            }
-                            if (this._is_closed) {
-                                show_array[0] = show_array[npoints - 1];
-                                show_array[npoints] = show_array[1];
-                            } else {
-                                show_array[0] = 0;
-                                show_array[npoints] = 0;
-                            }
-                            this._show.update();
+                        // Points array includes extra points at each end
+                        const npoints = points_array.length / 2 - 2;
+                        if (this._show == null)
+                            this._show = new buffer_1.Uint8Buffer(this.regl_wrapper);
+                        const show_array = this._show.get_sized_array(npoints + 1);
+                        let start_finite = isFinite(points_array[2]) && isFinite(points_array[3]);
+                        for (let i = 1; i < npoints; i++) {
+                            const end_finite = isFinite(points_array[2 * i + 2]) && isFinite(points_array[2 * i + 3]);
+                            show_array[i] = (start_finite && end_finite) ? 1 : 0;
+                            start_finite = end_finite;
                         }
+                        if (this._is_closed) {
+                            show_array[0] = show_array[npoints - 1];
+                            show_array[npoints] = show_array[1];
+                        } else {
+                            show_array[0] = 0;
+                            show_array[npoints] = 0;
+                        }
+                        this._show.update();
                         if (this._is_dashed()) {
-                            const npoints = points_array.length / 2 - 2;
                             const nsegments = npoints - 1;
-                            const show_array = this._show.get_sized_array(npoints + 1);
                             if (this._length_so_far == null)
                                 this._length_so_far = new buffer_1.Float32Buffer(this.regl_wrapper);
                             const lengths_array = this._length_so_far.get_sized_array(nsegments);
                             let length = 0.0;
                             for (let i = 0; i < nsegments; i++) {
                                 lengths_array[i] = length;
                                 if (show_array[i + 1] == 1)
@@ -11756,18 +11743,17 @@
                     constructor(regl_wrapper, glyph) {
                         super(regl_wrapper, glyph);
                         this.glyph = glyph;
                     }
                     draw(indices, main_glyph, transform) {
                         // The main glyph has the data, this glyph has the visuals.
                         const main_gl_glyph = main_glyph.glglyph;
-                        if (main_gl_glyph.data_changed || main_gl_glyph.data_mapped) {
+                        if (main_gl_glyph.data_changed) {
                             main_gl_glyph.set_data();
                             main_gl_glyph.data_changed = false;
-                            main_gl_glyph.data_mapped = false;
                         }
                         if (this.visuals_changed) {
                             this._set_visuals();
                             this.visuals_changed = false;
                         }
                         const nmarkers = main_gl_glyph.nvertices;
                         const ntypes = main_gl_glyph._unique_marker_types.length;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-gl.min.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-gl.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -4913,40 +4913,40 @@
                         const s = this.nvertices,
                             e = this._centers.get_sized_array(2 * s);
                         (0, _.interleave)(this.glyph.sx, this.glyph.sy, s, r.SingleMarkerGL.missing_point, e), this._centers.update()
                     }
                 }
                 t.SXSYGlyphGL = h, h.__name__ = "SXSYGlyphGL"
             },
-            522: function _(s, a, t, e, _) {
-                e();
+            522: function _(s, t, e, _, a) {
+                _();
                 const h = s(523);
                 class i extends h.BaseMarkerGL {
-                    constructor(s, a) {
-                        super(s, a), this.glyph = a
+                    constructor(s, t) {
+                        super(s, t), this.glyph = t
                     }
                     _get_visuals() {
                         return this.glyph.visuals
                     }
-                    draw(s, a, t) {
-                        this._draw_impl(s, t, a.glglyph, this.marker_type)
+                    draw(s, t, e) {
+                        this._draw_impl(s, e, t.glglyph, this.marker_type)
                     }
-                    _draw_impl(s, a, t, e) {
-                        (t.data_changed || t.data_mapped) && (t.set_data(), t.data_changed = !1, t.data_mapped = !1), this.visuals_changed && (this._set_visuals(), this.visuals_changed = !1);
-                        const _ = t.nvertices,
+                    _draw_impl(s, t, e, _) {
+                        e.data_changed && (e.set_data(), e.data_changed = !1), this.visuals_changed && (this._set_visuals(), this.visuals_changed = !1);
+                        const a = e.nvertices,
                             h = this._show.length,
-                            i = this._show.get_sized_array(_);
-                        if (s.length < _) {
+                            i = this._show.get_sized_array(a);
+                        if (s.length < a) {
                             this._show_all = !1, i.fill(0);
-                            for (let a = 0; a < s.length; a++) i[s[a]] = 255
-                        } else this._show_all && h == _ || (this._show_all = !0, i.fill(255));
-                        this._show.update(), this._draw_one_marker_type(e, a, t)
+                            for (let t = 0; t < s.length; t++) i[s[t]] = 255
+                        } else this._show_all && h == a || (this._show_all = !0, i.fill(255));
+                        this._show.update(), this._draw_one_marker_type(_, t, e)
                     }
                 }
-                t.SingleMarkerGL = i, i.__name__ = "SingleMarkerGL"
+                e.SingleMarkerGL = i, i.__name__ = "SingleMarkerGL"
             },
             523: function _(t, e, _, s, i) {
                 s();
                 const h = t(524),
                     r = t(525),
                     a = t(526);
                 class l extends h.BaseGLGlyph {
@@ -5013,46 +5013,43 @@
                             hatch: _
                         } = this._get_visuals();
                         this._linewidths.set_from_prop(t.line_width), this._line_caps.set_from_line_cap(t.line_cap), this._line_joins.set_from_line_join(t.line_join), this._line_rgba.set_from_color(t.line_color, t.line_alpha), this._fill_rgba.set_from_color(e.fill_color, e.fill_alpha), this._have_hatch = _.doit, this._have_hatch && (this._hatch_patterns.set_from_hatch_pattern(_.hatch_pattern), this._hatch_scales.set_from_prop(_.hatch_scale), this._hatch_weights.set_from_prop(_.hatch_weight), this._hatch_rgba.set_from_color(_.hatch_color, _.hatch_alpha))
                     }
                 }
                 _.BaseMarkerGL = l, l.__name__ = "BaseMarkerGL", l.missing_point = -1e4
             },
-            524: function _(e, t, a, s, i) {
-                s();
-                class h {
-                    constructor(e, t) {
-                        this.nvertices = 0, this.size_changed = !1, this.data_changed = !1, this.data_mapped = !1, this.visuals_changed = !1, this.regl_wrapper = e, this.glyph = t
+            524: function _(e, s, t, i, h) {
+                i();
+                class a {
+                    constructor(e, s) {
+                        this.nvertices = 0, this.size_changed = !1, this.data_changed = !1, this.visuals_changed = !1, this.regl_wrapper = e, this.glyph = s
                     }
                     set_data_changed() {
                         const {
                             data_size: e
                         } = this.glyph;
                         e != this.nvertices && (this.nvertices = e, this.size_changed = !0), this.data_changed = !0
                     }
-                    set_data_mapped() {
-                        this.data_mapped = !0
-                    }
                     set_visuals_changed() {
                         this.visuals_changed = !0
                     }
-                    render(e, t, a) {
-                        if (0 == t.length) return;
+                    render(e, s, t) {
+                        if (0 == s.length) return;
                         const {
-                            width: s,
-                            height: i
-                        } = this.glyph.renderer.plot_view.canvas_view.webgl.canvas, h = {
+                            width: i,
+                            height: h
+                        } = this.glyph.renderer.plot_view.canvas_view.webgl.canvas, a = {
                             pixel_ratio: this.glyph.renderer.plot_view.canvas_view.pixel_ratio,
-                            width: s,
-                            height: i
+                            width: i,
+                            height: h
                         };
-                        this.draw(t, a, h)
+                        this.draw(s, t, a)
                     }
                 }
-                a.BaseGLGlyph = h, h.__name__ = "BaseGLGlyph"
+                t.BaseGLGlyph = a, a.__name__ = "BaseGLGlyph"
             },
             525: function _(r, t, a, e, s) {
                 e();
                 const i = r(526),
                     _ = r(21);
                 class n {
                     constructor(r) {
@@ -5239,91 +5236,86 @@
                         super._set_once(), this._angles.set_from_scalar(0), this._auxs.set_from_scalar(0)
                     }
                 }
                 r.AnnulusGL = n, n.__name__ = "AnnulusGL"
             },
             528: function _(s, i, t, _, e) {
                 _();
-                const a = s(524),
-                    h = s(525),
+                const h = s(524),
+                    a = s(525),
                     l = s(526),
                     n = s(21),
                     o = s(76);
-                class d extends a.BaseGLGlyph {
+                class r extends h.BaseGLGlyph {
                     constructor(s, i) {
                         super(s, i), this._line_dash = null, this.glyph = i, this._antialias = 1.5, this._miter_limit = 10
                     }
                     _draw_impl(s, i, t) {
-                        this.visuals_changed && (this._set_visuals(), this.visuals_changed = !1), (t.data_changed || t.data_mapped) && (t._set_data(t.data_changed), t.data_changed = !1, t.data_mapped = !1);
+                        this.visuals_changed && (this._set_visuals(), this.visuals_changed = !1), t.data_changed && (t._set_data(), t.data_changed = !1);
                         const _ = this._get_visuals().line,
                             e = l.cap_lookup[_.line_cap.value],
-                            a = l.join_lookup[_.line_join.value],
-                            h = t._points,
-                            n = h.length / 2 - 3,
+                            h = l.join_lookup[_.line_join.value],
+                            a = t._points,
+                            n = a.length / 2 - 3,
                             o = this._get_show_buffer(s, t),
-                            d = {
+                            r = {
                                 scissor: this.regl_wrapper.scissor,
                                 viewport: this.regl_wrapper.viewport,
                                 canvas_size: [i.width, i.height],
                                 pixel_ratio: i.pixel_ratio,
                                 line_color: this._color,
                                 linewidth: this._linewidth,
                                 antialias: this._antialias,
                                 miter_limit: this._miter_limit,
-                                points: h,
+                                points: a,
                                 show: o,
                                 nsegments: n,
-                                line_join: a,
+                                line_join: h,
                                 line_cap: e
                             };
                         if (this._is_dashed()) {
-                            const s = Object.assign(Object.assign({}, d), {
+                            const s = Object.assign(Object.assign({}, r), {
                                 length_so_far: this._length_so_far,
                                 dash_tex: this._dash_tex,
                                 dash_tex_info: this._dash_tex_info,
                                 dash_scale: this._dash_scale,
                                 dash_offset: this._dash_offset
                             });
                             this.regl_wrapper.dashed_line()(s)
-                        } else this.regl_wrapper.solid_line()(d)
+                        } else this.regl_wrapper.solid_line()(r)
                     }
                     _is_dashed() {
                         return null != this._line_dash && this._line_dash.length > 0
                     }
-                    _set_data(s) {
-                        const i = this._set_data_points();
-                        if (s) {
-                            const s = i.length / 2 - 2;
-                            null == this._show && (this._show = new h.Uint8Buffer(this.regl_wrapper));
-                            const t = this._show.get_sized_array(s + 1);
-                            let _ = isFinite(i[2]) && isFinite(i[3]);
-                            for (let e = 1; e < s; e++) {
-                                const s = isFinite(i[2 * e + 2]) && isFinite(i[2 * e + 3]);
-                                t[e] = _ && s ? 1 : 0, _ = s
-                            }
-                            this._is_closed ? (t[0] = t[s - 1], t[s] = t[1]) : (t[0] = 0, t[s] = 0), this._show.update()
-                        }
-                        if (this._is_dashed()) {
-                            const s = i.length / 2 - 2,
-                                t = s - 1,
-                                _ = this._show.get_sized_array(s + 1);
-                            null == this._length_so_far && (this._length_so_far = new h.Float32Buffer(this.regl_wrapper));
-                            const e = this._length_so_far.get_sized_array(t);
-                            let a = 0;
-                            for (let s = 0; s < t; s++) e[s] = a, 1 == _[s + 1] && (a += Math.sqrt((i[2 * s + 4] - i[2 * s + 2]) ** 2 + (i[2 * s + 5] - i[2 * s + 3]) ** 2));
+                    _set_data() {
+                        const s = this._set_data_points(),
+                            i = s.length / 2 - 2;
+                        null == this._show && (this._show = new a.Uint8Buffer(this.regl_wrapper));
+                        const t = this._show.get_sized_array(i + 1);
+                        let _ = isFinite(s[2]) && isFinite(s[3]);
+                        for (let e = 1; e < i; e++) {
+                            const i = isFinite(s[2 * e + 2]) && isFinite(s[2 * e + 3]);
+                            t[e] = _ && i ? 1 : 0, _ = i
+                        }
+                        if (this._is_closed ? (t[0] = t[i - 1], t[i] = t[1]) : (t[0] = 0, t[i] = 0), this._show.update(), this._is_dashed()) {
+                            const _ = i - 1;
+                            null == this._length_so_far && (this._length_so_far = new a.Float32Buffer(this.regl_wrapper));
+                            const e = this._length_so_far.get_sized_array(_);
+                            let h = 0;
+                            for (let i = 0; i < _; i++) e[i] = h, 1 == t[i + 1] && (h += Math.sqrt((s[2 * i + 4] - s[2 * i + 2]) ** 2 + (s[2 * i + 5] - s[2 * i + 3]) ** 2));
                             this._length_so_far.update()
                         }
                     }
                     _set_visuals() {
                         const s = this._get_visuals().line,
                             i = (0, n.color2rgba)(s.line_color.value, s.line_alpha.value);
                         this._color = i.map((s => s / 255)), this._linewidth = s.line_width.value, this._linewidth < 1 && (this._color[3] *= this._linewidth, this._linewidth = 1), this._line_dash = (0, o.resolve_line_dash)(s.line_dash.value), this._is_dashed() && ([this._dash_tex_info, this._dash_tex, this._dash_scale] = this.regl_wrapper.get_dash(this._line_dash), this._dash_offset = s.line_dash_offset.value)
                     }
                 }
-                t.BaseLineGL = d, d.__name__ = "BaseLineGL"
+                t.BaseLineGL = r, r.__name__ = "BaseLineGL"
             },
             529: function _(s, e, t, _, r) {
                 _();
                 const a = s(521),
                     i = s(13);
                 class c extends a.SXSYGlyphGL {
                     constructor(s, e) {
@@ -5455,46 +5447,46 @@
                     }
                     _set_once() {
                         super._set_once(), this._auxs.set_from_scalar(0)
                     }
                 }
                 e.LRTBGL = a, a.__name__ = "LRTBGL"
             },
-            533: function _(s, t, e, _, a) {
+            533: function _(s, t, e, _, i) {
                 _();
-                const i = s(523),
+                const a = s(523),
                     h = s(526);
-                class r extends i.BaseMarkerGL {
+                class r extends a.BaseMarkerGL {
                     constructor(s, t) {
                         super(s, t), this.glyph = t
                     }
                     draw(s, t, e) {
                         const _ = t.glglyph;
-                        (_.data_changed || _.data_mapped) && (_.set_data(), _.data_changed = !1, _.data_mapped = !1), this.visuals_changed && (this._set_visuals(), this.visuals_changed = !1);
-                        const a = _.nvertices,
-                            i = _._unique_marker_types.length;
+                        _.data_changed && (_.set_data(), _.data_changed = !1), this.visuals_changed && (this._set_visuals(), this.visuals_changed = !1);
+                        const i = _.nvertices,
+                            a = _._unique_marker_types.length;
                         for (const t of _._unique_marker_types) {
                             if (null == t) continue;
-                            let h = a;
+                            let h = i;
                             const r = this._show.length,
-                                l = this._show.get_sized_array(a);
-                            if (i > 1 || s.length < a) {
+                                l = this._show.get_sized_array(i);
+                            if (a > 1 || s.length < i) {
                                 this._show_all = !1, l.fill(0), h = 0;
-                                for (const e of s) 1 != i && _._marker_types.get(e) != t || (l[e] = 255, h++)
-                            } else this._show_all && r == a || (this._show_all = !0, l.fill(255));
+                                for (const e of s) 1 != a && _._marker_types.get(e) != t || (l[e] = 255, h++)
+                            } else this._show_all && r == i || (this._show_all = !0, l.fill(255));
                             this._show.update(), 0 != h && this._draw_one_marker_type(t, e, _)
                         }
                     }
                     _get_visuals() {
                         return this.glyph.visuals
                     }
                     _set_data() {
                         const s = this.nvertices,
                             t = this._centers.get_sized_array(2 * s);
-                        (0, h.interleave)(this.glyph.sx, this.glyph.sy, s, i.BaseMarkerGL.missing_point, t), this._centers.update(), this._widths.set_from_prop(this.glyph.size), this._angles.set_from_prop(this.glyph.angle), this._marker_types = this.glyph.marker, this._unique_marker_types = [...new Set(this._marker_types)]
+                        (0, h.interleave)(this.glyph.sx, this.glyph.sy, s, a.BaseMarkerGL.missing_point, t), this._centers.update(), this._widths.set_from_prop(this.glyph.size), this._angles.set_from_prop(this.glyph.angle), this._marker_types = this.glyph.marker, this._unique_marker_types = [...new Set(this._marker_types)]
                     }
                     _set_once() {
                         super._set_once(), this._heights.set_from_scalar(0), this._auxs.set_from_scalar(0)
                     }
                 }
                 e.MultiMarkerGL = r, r.__name__ = "MultiMarkerGL"
             },
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-mathjax.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-mathjax.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-mathjax.min.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-mathjax.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-tables.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-tables.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -505,15 +505,15 @@
                 const tslib_1 = require(1) /* tslib */ ;
                 const timezone_1 = tslib_1.__importDefault(require(173) /* timezone */ );
                 const Numbro = tslib_1.__importStar(require(171) /* @bokeh/numbro */ );
                 const underscore_template_1 = require(633) /* underscore.template */ ;
                 const dom_1 = require(56) /* ../../../core/dom */ ;
                 const enums_1 = require(19) /* ../../../core/enums */ ;
                 const types_1 = require(8) /* ../../../core/util/types */ ;
-                const string_1 = require(39) /* ../../../core/util/string */ ;
+                const string_1 = require(38) /* ../../../core/util/string */ ;
                 const color_1 = require(21) /* ../../../core/util/color */ ;
                 const model_1 = require(50) /* ../../../model */ ;
                 class CellFormatter extends model_1.Model {
                     constructor(attrs) {
                         super(attrs);
                     }
                     doFormat(_row, _cell, value, _columnDef, _dataContext) {
@@ -990,15 +990,15 @@
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const slick_rowselectionmodel_1 = require(636) /* @bokeh/slickgrid/plugins/slick.rowselectionmodel */ ;
                 const slick_checkboxselectcolumn_1 = require(640) /* @bokeh/slickgrid/plugins/slick.checkboxselectcolumn */ ;
                 const slick_cellexternalcopymanager_1 = require(641) /* @bokeh/slickgrid/plugins/slick.cellexternalcopymanager */ ;
                 const slickgrid_1 = require(642) /* @bokeh/slickgrid */ ;
                 const dom_1 = require(56) /* ../../../core/dom */ ;
-                const string_1 = require(39) /* ../../../core/util/string */ ;
+                const string_1 = require(38) /* ../../../core/util/string */ ;
                 const types_1 = require(8) /* ../../../core/util/types */ ;
                 const array_1 = require(10) /* ../../../core/util/array */ ;
                 const ndarray_1 = require(29) /* ../../../core/util/ndarray */ ;
                 const object_1 = require(9) /* ../../../core/util/object */ ;
                 const logging_1 = require(18) /* ../../../core/logging */ ;
                 const widget_1 = require(651) /* ../widget */ ;
                 const definitions_1 = require(630) /* ./definitions */ ;
@@ -20745,15 +20745,15 @@
                 })();
             },
             653: /* models/widgets/tables/table_column.js */ function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const cell_formatters_1 = require(632) /* ./cell_formatters */ ;
                 const cell_editors_1 = require(629) /* ./cell_editors */ ;
-                const string_1 = require(39) /* ../../../core/util/string */ ;
+                const string_1 = require(38) /* ../../../core/util/string */ ;
                 const enums_1 = require(19) /* ../../../core/enums */ ;
                 const model_1 = require(50) /* ../../../model */ ;
                 class TableColumn extends model_1.Model {
                     constructor(attrs) {
                         super(attrs);
                     }
                     toColumn() {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-tables.min.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-tables.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -355,15 +355,15 @@
                 const m = t(1),
                     _ = m.__importDefault(t(173)),
                     d = m.__importStar(t(171)),
                     f = t(633),
                     g = t(56),
                     h = t(19),
                     F = t(8),
-                    p = t(39),
+                    p = t(38),
                     b = t(21),
                     S = t(50);
                 class x extends S.Model {
                     constructor(t) {
                         super(t)
                     }
                     doFormat(t, e, r, n, a) {
@@ -664,15 +664,15 @@
                 s();
                 const n = e(1),
                     l = e(636),
                     d = e(640),
                     a = e(641),
                     h = e(642),
                     u = e(56),
-                    c = e(39),
+                    c = e(38),
                     _ = e(8),
                     m = e(10),
                     g = e(29),
                     f = e(9),
                     p = e(18),
                     w = e(651),
                     b = e(630),
@@ -9268,15 +9268,15 @@
                 })))
             },
             653: function _(t, e, i, r, l) {
                 var o;
                 r();
                 const d = t(632),
                     n = t(629),
-                    a = t(39),
+                    a = t(38),
                     s = t(19),
                     u = t(50);
                 class f extends u.Model {
                     constructor(t) {
                         super(t)
                     }
                     toColumn() {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-widgets.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-widgets.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -323,15 +323,15 @@
             },
             559: /* models/widgets/autocomplete_input.js */ function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const text_input_1 = require(560) /* ./text_input */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const math_1 = require(11) /* ../../core/util/math */ ;
                 const kinds_1 = require(20) /* ../../core/kinds */ ;
                 const dropdown_css_1 = tslib_1.__importStar(require(564) /* ../../styles/dropdown.css */ ),
                     dropdown = dropdown_css_1;
                 const SearchStrategy = (0, kinds_1.Enum)("starts_with", "includes");
                 class AutocompleteInputView extends text_input_1.TextInputView {
                     constructor() {
@@ -1004,15 +1004,15 @@
             569: /* models/widgets/checkbox_group.js */ function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const toggle_input_group_1 = require(570) /* ./toggle_input_group */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const inputs = tslib_1.__importStar(require(563) /* ../../styles/widgets/inputs.css */ );
                 class CheckboxGroupView extends toggle_input_group_1.ToggleInputGroupView {
                     get active() {
                         return new Set(this.model.active);
                     }
                     connect_signals() {
                         super.connect_signals();
@@ -1467,21 +1467,17 @@
                 const enums_1 = require(19) /* ../../core/enums */ ;
                 const dom_2 = require(56) /* ../../core/dom */ ;
                 const assert_1 = require(12) /* ../../core/util/assert */ ;
                 const flatpickr_css_1 = tslib_1.__importDefault(require(586) /* ../../styles/widgets/flatpickr.css */ );
                 const inputs = tslib_1.__importStar(require(563) /* ../../styles/widgets/inputs.css */ );
                 class PickerBaseView extends input_widget_1.InputWidgetView {
                     get picker() {
-                            (0, assert_1.assert)(this._picker != null);
-                            return this._picker;
-                        }
-                        * controls() {
-                            var _b;
-                            yield(_b = this.picker.altInput) !== null && _b !== void 0 ? _b : this.input_el;
-                        }
+                        (0, assert_1.assert)(this._picker != null);
+                        return this._picker;
+                    }
                     remove() {
                         var _b;
                         (_b = this._picker) === null || _b === void 0 ? void 0 : _b.destroy();
                         super.remove();
                     }
                     stylesheets() {
                         return [...super.stylesheets(), flatpickr_css_1.default];
@@ -15376,16 +15372,16 @@
             },
             618: /* models/widgets/radio_group.js */ function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const toggle_input_group_1 = require(570) /* ./toggle_input_group */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const inputs = tslib_1.__importStar(require(563) /* ../../styles/widgets/inputs.css */ );
                 class RadioGroupView extends toggle_input_group_1.ToggleInputGroupView {
                     connect_signals() {
                         super.connect_signals();
                         const {
                             active
                         } = this.model.properties;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh-widgets.min.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh-widgets.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25,15 +25,15 @@
  * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
  * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
  * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
  * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
  * THE POSSIBILITY OF SUCH DAMAGE.
  */
 (function(root, factory) {
-    factory(root["Bokeh"], "3.2.1");
+    factory(root["Bokeh"], "3.3.0-dev.1");
 })(this, function(Bokeh, version) {
     let define;
     return (function(modules, entry, aliases, externals) {
             const bokeh = typeof Bokeh !== "undefined" && (version != null ? Bokeh[version] : Bokeh);
             if (bokeh != null) {
                 return bokeh.register_plugin(modules, entry, aliases);
             } else {
@@ -185,15 +185,15 @@
             },
             559: function _(e, t, s, n, i) {
                 var h;
                 n();
                 const o = e(1),
                     _ = e(560),
                     u = e(56),
-                    r = e(33),
+                    r = e(32),
                     c = e(11),
                     l = e(20),
                     a = o.__importStar(e(564)),
                     m = a,
                     d = (0, l.Enum)("starts_with", "includes");
                 class p extends _.TextInputView {
                     constructor() {
@@ -677,15 +677,15 @@
             569: function _(e, t, s, n, i) {
                 var c;
                 n();
                 const o = e(1),
                     a = e(570),
                     h = e(56),
                     l = e(10),
-                    r = e(33),
+                    r = e(32),
                     d = o.__importStar(e(563));
                 class p extends a.ToggleInputGroupView {
                     get active() {
                         return new Set(this.model.active)
                     }
                     connect_signals() {
                         super.connect_signals();
@@ -1017,28 +1017,25 @@
                     date_format: [r.String, "Y-m-d"]
                 })))
             },
             577: function _(e, t, i, n, o) {
                 var s;
                 n();
                 const r = e(1),
-                    l = r.__importDefault(e(578)),
-                    a = e(562),
+                    a = r.__importDefault(e(578)),
+                    l = e(562),
                     c = e(56),
                     d = e(19),
                     h = e(56),
                     p = e(12),
                     f = r.__importDefault(e(586)),
                     g = r.__importStar(e(563));
-                class u extends a.InputWidgetView {
+                class u extends l.InputWidgetView {
                     get picker() {
                         return (0, p.assert)(null != this._picker), this._picker
-                    }* controls() {
-                        var e;
-                        yield null !== (e = this.picker.altInput) && void 0 !== e ? e : this.input_el
                     }
                     remove() {
                         var e;
                         null === (e = this._picker) || void 0 === e || e.destroy(), super.remove()
                     }
                     stylesheets() {
                         return [...super.stylesheets(), f.default]
@@ -1064,56 +1061,56 @@
                         var e;
                         super.render(), null === (e = this._picker) || void 0 === e || e.destroy(), this.input_el = (0, c.input)({
                             type: "text",
                             class: g.input,
                             disabled: this.model.disabled
                         }), this.group_el.appendChild(this.input_el);
                         const t = this.flatpickr_options;
-                        this._picker = (0, l.default)(this.input_el, t)
+                        this._picker = (0, a.default)(this.input_el, t)
                     }
                     _position(e, t) {
                         const i = null != t ? t : e._positionElement,
                             n = [...e.calendarContainer.children].reduce(((e, t) => e + (0, h.bounding_box)(t).height), 0),
                             o = e.calendarContainer.offsetWidth,
                             s = this.model.position.split(" "),
                             r = s[0],
-                            l = s.length > 1 ? s[1] : null,
-                            a = i.offsetTop,
+                            a = s.length > 1 ? s[1] : null,
+                            l = i.offsetTop,
                             c = i.offsetTop + i.offsetHeight,
                             d = i.offsetLeft,
                             p = i.offsetLeft + i.offsetWidth,
                             f = i.offsetWidth,
                             g = window.innerHeight - c,
-                            u = "above" === r || "below" !== r && g < n && a > n,
-                            _ = null != e.config.appendTo ? a + (u ? -n - 2 : i.offsetHeight + 2) : window.scrollY + a + (u ? -n - 2 : i.offsetHeight + 2);
+                            u = "above" === r || "below" !== r && g < n && l > n,
+                            _ = null != e.config.appendTo ? l + (u ? -n - 2 : i.offsetHeight + 2) : window.scrollY + l + (u ? -n - 2 : i.offsetHeight + 2);
                         if (e.calendarContainer.classList.toggle("arrowTop", !u), e.calendarContainer.classList.toggle("arrowBottom", u), e.config.inline) return;
                         let w = window.scrollX + d,
                             C = !1,
                             m = !1;
-                        "center" === l ? (w -= (o - f) / 2, C = !0) : "right" === l && (w -= o - f, m = !0), e.calendarContainer.classList.toggle("arrowLeft", !C && !m), e.calendarContainer.classList.toggle("arrowCenter", C), e.calendarContainer.classList.toggle("arrowRight", m);
+                        "center" === a ? (w -= (o - f) / 2, C = !0) : "right" === a && (w -= o - f, m = !0), e.calendarContainer.classList.toggle("arrowLeft", !C && !m), e.calendarContainer.classList.toggle("arrowCenter", C), e.calendarContainer.classList.toggle("arrowRight", m);
                         const y = window.document.body.offsetWidth - (window.scrollX + p),
                             k = w + o > window.document.body.offsetWidth,
                             b = y + o > window.document.body.offsetWidth;
                         if (e.calendarContainer.classList.toggle("rightMost", k), !e.config.static)
                             if (e.calendarContainer.style.top = `${_}px`, k)
                                 if (b) {
                                     const t = this.shadow_el.styleSheets[0],
                                         i = window.document.body.offsetWidth,
                                         n = Math.max(0, i / 2 - o / 2),
                                         s = ".flatpickr-calendar.centerMost:before",
                                         r = ".flatpickr-calendar.centerMost:after",
-                                        l = t.cssRules.length,
-                                        a = `{left:${d}px;right:auto;}`;
-                                    e.calendarContainer.classList.toggle("rightMost", !1), e.calendarContainer.classList.toggle("centerMost", !0), t.insertRule(`${s},${r}${a}`, l), e.calendarContainer.style.left = `${n}px`, e.calendarContainer.style.right = "auto"
+                                        a = t.cssRules.length,
+                                        l = `{left:${d}px;right:auto;}`;
+                                    e.calendarContainer.classList.toggle("rightMost", !1), e.calendarContainer.classList.toggle("centerMost", !0), t.insertRule(`${s},${r}${l}`, a), e.calendarContainer.style.left = `${n}px`, e.calendarContainer.style.right = "auto"
                                 } else e.calendarContainer.style.left = "auto", e.calendarContainer.style.right = `${y}px`;
                         else e.calendarContainer.style.left = `${w}px`, e.calendarContainer.style.right = "auto"
                     }
                 }
                 i.PickerBaseView = u, u.__name__ = "PickerBaseView";
-                class _ extends a.InputWidget {
+                class _ extends l.InputWidget {
                     constructor(e) {
                         super(e)
                     }
                 }
                 i.PickerBase = _, s = _, _.__name__ = "PickerBase", s.define((({
                     Boolean: e
                 }) => ({
@@ -8769,16 +8766,16 @@
             },
             618: function _(e, t, n, i, s) {
                 var o;
                 i();
                 const a = e(1),
                     l = e(570),
                     c = e(56),
-                    d = e(39),
-                    p = e(33),
+                    d = e(38),
+                    p = e(32),
                     u = a.__importStar(e(563));
                 class r extends l.ToggleInputGroupView {
                     connect_signals() {
                         super.connect_signals();
                         const {
                             active: e
                         } = this.model.properties;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -748,23 +748,23 @@
                 __esExport("documents", document_1.documents);
                 var safely_1 = require(69) /* ./safely */ ;
                 __esExport("safely", safely_1.safely);
             },
             /* version.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
-                exports.version = "3.2.1";
+                exports.version = "3.3.0-dev.1";
             },
             /* embed/index.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const document_1 = require(5) /* ../document */ ;
                 const settings_1 = require(28) /* ../core/settings */ ;
                 const logging_1 = require(18) /* ../core/logging */ ;
-                const string_1 = require(39) /* ../core/util/string */ ;
+                const string_1 = require(38) /* ../core/util/string */ ;
                 const object_1 = require(9) /* ../core/util/object */ ;
                 const types_1 = require(8) /* ../core/util/types */ ;
                 const defer_1 = require(16) /* ../core/util/defer */ ;
                 const standalone_1 = require(53) /* ./standalone */ ;
                 const server_1 = require(60) /* ./server */ ;
                 const dom_1 = require(65) /* ./dom */ ;
                 var standalone_2 = require(53) /* ./standalone */ ;
@@ -835,37 +835,37 @@
                 }
             },
             /* document/index.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 tslib_1.__exportStar(require(6) /* ./document */ , exports);
-                tslib_1.__exportStar(require(40) /* ./events */ , exports);
+                tslib_1.__exportStar(require(39) /* ./events */ , exports);
             },
             /* document/document.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const base_1 = require(7) /* ../base */ ;
                 const version_1 = require(3) /* ../version */ ;
                 const logging_1 = require(18) /* ../core/logging */ ;
                 const resolvers_1 = require(45) /* ../core/resolvers */ ;
-                const serialization_1 = require(31) /* ../core/serialization */ ;
+                const serialization_1 = require(30) /* ../core/serialization */ ;
                 const deserializer_1 = require(46) /* ../core/serialization/deserializer */ ;
                 const version_2 = require(49) /* ../core/util/version */ ;
                 const signaling_1 = require(15) /* ../core/signaling */ ;
                 const types_1 = require(8) /* ../core/util/types */ ;
                 const eq_1 = require(25) /* ../core/util/eq */ ;
                 const array_1 = require(10) /* ../core/util/array */ ;
                 const object_1 = require(9) /* ../core/util/object */ ;
                 const sets = tslib_1.__importStar(require(43) /* ../core/util/set */ );
                 const model_1 = require(50) /* ../model */ ;
                 const defs_1 = require(51) /* ./defs */ ;
                 const bokeh_events_1 = require(52) /* ../core/bokeh_events */ ;
-                const events_1 = require(40) /* ./events */ ;
+                const events_1 = require(39) /* ./events */ ;
                 deserializer_1.Deserializer.register("model", defs_1.decode_def);
                 // Dispatches events to the subscribed models
                 class EventManager {
                     constructor(document) {
                         this.subscribed_models = new Set();
                         this.document = document;
                     }
@@ -2521,23 +2521,23 @@
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const signaling_1 = require(15) /* ./signaling */ ;
                 const p = tslib_1.__importStar(require(17) /* ./properties */ );
                 const k = tslib_1.__importStar(require(20) /* ./kinds */ );
                 const assert_1 = require(12) /* ./util/assert */ ;
-                const string_1 = require(39) /* ./util/string */ ;
+                const string_1 = require(38) /* ./util/string */ ;
                 const object_1 = require(9) /* ./util/object */ ;
                 const types_1 = require(8) /* ./util/types */ ;
                 const eq_1 = require(25) /* ./util/eq */ ;
-                const serialization_1 = require(31) /* ./serialization */ ;
-                const events_1 = require(40) /* ../document/events */ ;
+                const serialization_1 = require(30) /* ./serialization */ ;
+                const events_1 = require(39) /* ../document/events */ ;
                 const eq_2 = require(25) /* ./util/eq */ ;
-                const pretty_1 = require(41) /* ./util/pretty */ ;
-                const cloneable_1 = require(30) /* ./util/cloneable */ ;
+                const pretty_1 = require(40) /* ./util/pretty */ ;
+                const cloneable_1 = require(41) /* ./util/cloneable */ ;
                 const kinds = tslib_1.__importStar(require(20) /* ./kinds */ );
                 const vectorization_1 = require(27) /* ./vectorization */ ;
                 const patching_1 = require(42) /* ./patching */ ;
                 const _qualified_names = new WeakMap();
                 class HasProps extends(0, signaling_1.Signalable)() {
                     get is_syncable() {
                         return true;
@@ -3305,18 +3305,18 @@
                 const math_1 = require(11) /* ./util/math */ ;
                 const color_1 = require(21) /* ./util/color */ ;
                 const platform_1 = require(26) /* ./util/platform */ ;
                 const types_2 = require(8) /* ./util/types */ ;
                 const vectorization_1 = require(27) /* ./vectorization */ ;
                 const settings_1 = require(28) /* ./settings */ ;
                 const ndarray_1 = require(29) /* ./util/ndarray */ ;
-                const diagnostics_1 = require(37) /* ./diagnostics */ ;
+                const diagnostics_1 = require(36) /* ./diagnostics */ ;
                 const assert_1 = require(12) /* ./util/assert */ ;
-                const serialization_1 = require(31) /* ./serialization */ ;
-                const uniforms_1 = require(38) /* ./uniforms */ ;
+                const serialization_1 = require(30) /* ./serialization */ ;
+                const uniforms_1 = require(37) /* ./uniforms */ ;
                 __esExport("Uniform", uniforms_1.Uniform);
                 __esExport("UniformScalar", uniforms_1.UniformScalar);
                 __esExport("UniformVector", uniforms_1.UniformVector);
 
                 function valueToString(value) {
                     try {
                         return JSON.stringify(value);
@@ -5752,16 +5752,15 @@
             /* core/util/ndarray.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a, _b, _c, _d, _e, _f, _g, _h, _j, _k;
                 __esModule();
                 const types_1 = require(8) /* ./types */ ;
                 const platform_1 = require(26) /* ./platform */ ;
                 const eq_1 = require(25) /* ./eq */ ;
-                const cloneable_1 = require(30) /* ./cloneable */ ;
-                const serialization_1 = require(31) /* ../serialization */ ;
+                const serialization_1 = require(30) /* ../serialization */ ;
                 const __ndarray__ = Symbol("__ndarray__");
 
                 function encode_NDArray(array, serializer) {
                     const encoded = serializer.encode(array.dtype == "object" ? Array.from(array) : array.buffer);
                     return {
                         type: "ndarray",
                         array: encoded,
@@ -5777,17 +5776,14 @@
                             this.dtype = "bool";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_a = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new BoolNDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i] == 1;
                     }
                 }
@@ -5800,17 +5796,14 @@
                             this.dtype = "uint8";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_b = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Uint8NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5823,17 +5816,14 @@
                             this.dtype = "int8";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_c = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Int8NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5846,17 +5836,14 @@
                             this.dtype = "uint16";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_d = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Uint16NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5869,17 +5856,14 @@
                             this.dtype = "int16";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_e = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Int16NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5892,17 +5876,14 @@
                             this.dtype = "uint32";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_f = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Uint32NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5915,17 +5896,14 @@
                             this.dtype = "int32";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_g = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Int32NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5938,17 +5916,14 @@
                             this.dtype = "float32";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_h = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Float32NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5961,17 +5936,14 @@
                             this.dtype = "float64";
                             this.shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : [this.length]);
                             this.dimension = this.shape.length;
                         }
                         [(_j = __ndarray__, eq_1.equals)](that, cmp) {
                             return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                         }
-                        [cloneable_1.clone](cloner) {
-                            return new Float64NDArray(this, cloner.clone(this.shape));
-                        }
                         [serialization_1.serialize](serializer) {
                             return encode_NDArray(this, serializer);
                         }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -5997,17 +5969,14 @@
                             }
                         }
                         this._shape = shape !== null && shape !== void 0 ? shape : (is_NDArray(init) ? init.shape : undefined);
                     }
                     [(_k = __ndarray__, eq_1.equals)](that, cmp) {
                         return cmp.eq(this.shape, that.shape) && cmp.arrays(this, that);
                     }
-                    [cloneable_1.clone](cloner) {
-                        return new ObjectNDArray(this, cloner.clone(this.shape));
-                    }
                     [serialization_1.serialize](serializer) {
                         return encode_NDArray(this, serializer);
                     }
                     get(i) {
                         return this[i];
                     }
                 }
@@ -6069,82 +6038,36 @@
                             return new Float64NDArray(init, shape);
                         case "object":
                             return new ObjectNDArray(init, shape);
                     }
                 }
                 exports.ndarray = ndarray;
             },
-            /* core/util/cloneable.js */
-            function _(require, module, exports, __esModule, __esExport) {
-                __esModule();
-                const object_1 = require(9) /* ./object */ ;
-                const types_1 = require(8) /* ./types */ ;
-                exports.clone = Symbol("clone");
-
-                function is_Cloneable(obj) {
-                    return (0, types_1.isObject)(obj) && exports.clone in obj;
-                }
-                exports.is_Cloneable = is_Cloneable;
-                class CloningError extends Error {}
-                exports.CloningError = CloningError;
-                CloningError.__name__ = "CloningError";
-                class Cloner {
-                    constructor() {}
-                    clone(obj) {
-                        if (is_Cloneable(obj)) {
-                            return obj[exports.clone](this);
-                        } else if ((0, types_1.isPrimitive)(obj)) {
-                            return obj;
-                        } else if ((0, types_1.isArray)(obj)) {
-                            const n = obj.length;
-                            const result = new Array(n);
-                            for (let i = 0; i < n; i++) {
-                                const value = obj[i];
-                                result[i] = this.clone(value);
-                            }
-                            return result;
-                        } else if ((0, types_1.isPlainObject)(obj)) {
-                            const result = {};
-                            for (const [key, value] of(0, object_1.entries)(obj)) {
-                                result[key] = this.clone(value);
-                            }
-                            return result;
-                        } else if (obj instanceof Map) {
-                            return new Map([...obj].map(([k, v]) => [this.clone(k), this.clone(v)]));
-                        } else if (obj instanceof Set) {
-                            return new Set([...obj].map((v) => this.clone(v)));
-                        } else
-                            throw new CloningError(`${Object.prototype.toString.call(obj)} is not cloneable`);
-                    }
-                }
-                exports.Cloner = Cloner;
-                Cloner.__name__ = "Cloner";
-            },
             /* core/serialization/index.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
-                var serializer_1 = require(32) /* ./serializer */ ;
+                var serializer_1 = require(31) /* ./serializer */ ;
                 __esExport("Serializer", serializer_1.Serializer);
                 __esExport("SerializationError", serializer_1.SerializationError);
                 __esExport("serialize", serializer_1.serialize);
-                var buffer_1 = require(34) /* ./buffer */ ;
+                var buffer_1 = require(33) /* ./buffer */ ;
                 __esExport("Buffer", buffer_1.Buffer);
                 __esExport("Base64Buffer", buffer_1.Base64Buffer);
-                tslib_1.__exportStar(require(36) /* ./reps */ , exports);
+                tslib_1.__exportStar(require(35) /* ./reps */ , exports);
             },
             /* core/serialization/serializer.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const assert_1 = require(12) /* ../util/assert */ ;
                 const object_1 = require(9) /* ../util/object */ ;
                 const types_1 = require(8) /* ../util/types */ ;
-                const iterator_1 = require(33) /* ../util/iterator */ ;
+                const iterator_1 = require(32) /* ../util/iterator */ ;
                 const platform_1 = require(26) /* ../util/platform */ ;
-                const buffer_1 = require(34) /* ./buffer */ ;
+                const buffer_1 = require(33) /* ./buffer */ ;
                 // TypedArray?
                 exports.serialize = Symbol("serialize");
 
                 function is_Serializable(obj) {
                     return (0, types_1.isObject)(obj) && exports.serialize in obj;
                 }
                 class SerializationError extends Error {}
@@ -6506,15 +6429,15 @@
                     }
                 }
                 exports.subsets = subsets;
             },
             /* core/serialization/buffer.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
-                const buffer_1 = require(35) /* ../util/buffer */ ;
+                const buffer_1 = require(34) /* ../util/buffer */ ;
                 const eq_1 = require(25) /* ../util/eq */ ;
                 class Buffer {
                     constructor(buffer) {
                         this.buffer = buffer;
                     }
                     to_base64() {
                             return (0, buffer_1.buffer_to_base64)(this.buffer);
@@ -6831,15 +6754,15 @@
                 }
                 exports.insert_text_on_position = insert_text_on_position;
             },
             /* document/events.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const eq_1 = require(25) /* ../core/util/eq */ ;
-                const serialization_1 = require(31) /* ../core/serialization */ ;
+                const serialization_1 = require(30) /* ../core/serialization */ ;
                 class DocumentEvent {
                     constructor(document) {
                         this.document = document;
                     }
                     get[Symbol.toStringTag]() {
                             return this.constructor.__name__;
                         }
@@ -7150,14 +7073,60 @@
 
                 function to_string(obj, options) {
                     const printer = new Printer(options);
                     return printer.to_string(obj);
                 }
                 exports.to_string = to_string;
             },
+            /* core/util/cloneable.js */
+            function _(require, module, exports, __esModule, __esExport) {
+                __esModule();
+                const object_1 = require(9) /* ./object */ ;
+                const types_1 = require(8) /* ./types */ ;
+                exports.clone = Symbol("clone");
+
+                function is_Cloneable(obj) {
+                    return (0, types_1.isObject)(obj) && exports.clone in obj;
+                }
+                exports.is_Cloneable = is_Cloneable;
+                class CloningError extends Error {}
+                exports.CloningError = CloningError;
+                CloningError.__name__ = "CloningError";
+                class Cloner {
+                    constructor() {}
+                    clone(obj) {
+                        if (is_Cloneable(obj)) {
+                            return obj[exports.clone](this);
+                        } else if ((0, types_1.isPrimitive)(obj)) {
+                            return obj;
+                        } else if ((0, types_1.isArray)(obj)) {
+                            const n = obj.length;
+                            const result = new Array(n);
+                            for (let i = 0; i < n; i++) {
+                                const value = obj[i];
+                                result[i] = this.clone(value);
+                            }
+                            return result;
+                        } else if ((0, types_1.isPlainObject)(obj)) {
+                            const result = {};
+                            for (const [key, value] of(0, object_1.entries)(obj)) {
+                                result[key] = this.clone(value);
+                            }
+                            return result;
+                        } else if (obj instanceof Map) {
+                            return new Map([...obj].map(([k, v]) => [this.clone(k), this.clone(v)]));
+                        } else if (obj instanceof Set) {
+                            return new Set([...obj].map((v) => this.clone(v)));
+                        } else
+                            throw new CloningError(`${Object.prototype.toString.call(obj)} is not cloneable`);
+                    }
+                }
+                exports.Cloner = Cloner;
+                Cloner.__name__ = "Cloner";
+            },
             /* core/patching.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const types_1 = require(8) /* ./util/types */ ;
                 const object_1 = require(9) /* ./util/object */ ;
                 const set_1 = require(43) /* ./util/set */ ;
@@ -7390,15 +7359,15 @@
                 __esModule();
                 const logging_1 = require(18) /* ../logging */ ;
                 const refs_1 = require(47) /* ../util/refs */ ;
                 const ndarray_1 = require(29) /* ../util/ndarray */ ;
                 const object_1 = require(9) /* ../util/object */ ;
                 const array_1 = require(10) /* ../util/array */ ;
                 const platform_1 = require(26) /* ../util/platform */ ;
-                const buffer_1 = require(35) /* ../util/buffer */ ;
+                const buffer_1 = require(34) /* ../util/buffer */ ;
                 const types_1 = require(8) /* ../util/types */ ;
                 const slice_1 = require(48) /* ../util/slice */ ;
                 const _decoders = new Map();
                 class DeserializationError extends Error {}
                 exports.DeserializationError = DeserializationError;
                 DeserializationError.__name__ = "DeserializationError";
                 class Deserializer {
@@ -7743,15 +7712,15 @@
                     return (0, types_1.isPlainObject)(obj) && "id" in obj && !("type" in obj);
                 }
                 exports.is_ref = is_ref;
             },
             /* core/util/slice.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
-                const serialization_1 = require(31) /* ../serialization */ ;
+                const serialization_1 = require(30) /* ../serialization */ ;
                 class Slice {
                     constructor({
                             start,
                             stop,
                             step
                         } = {}) {
                             this.start = start !== null && start !== void 0 ? start : null;
@@ -8047,15 +8016,15 @@
                         r = Reflect.decorate(decorators, target, key, desc);
                     else
                         for (var i = decorators.length - 1; i >= 0; i--)
                             if (d = decorators[i])
                                 r = (c < 3 ? d(r) : c > 3 ? d(target, key, r) : d(target, key)) || r;
                     return c > 3 && r && Object.defineProperty(target, key, r), r;
                 };
-                const serialization_1 = require(31) /* ./serialization */ ;
+                const serialization_1 = require(30) /* ./serialization */ ;
                 const eq_1 = require(25) /* ./util/eq */ ;
                 const kinds_1 = require(20) /* ./kinds */ ;
                 exports.KeyModifiers = (0, kinds_1.PartialStruct)({
                     shift: kinds_1.Boolean,
                     ctrl: kinds_1.Boolean,
                     alt: kinds_1.Boolean,
                 });
@@ -8532,17 +8501,14 @@
                 const signaling_1 = require(15) /* ./signaling */ ;
                 const types_1 = require(8) /* ./util/types */ ;
                 class View {
                     get ready() {
                             return this._ready;
                         }
                         * children() {}
-                    mark_finished() {
-                        this._has_finished = true;
-                    }
                     connect(signal, slot) {
                         let new_slot = this._slots.get(slot);
                         if (new_slot == null) {
                             new_slot = (args, sender) => {
                                 const promise = Promise.resolve(slot.call(this, args, sender));
                                 this._ready = this._ready.then(() => promise);
                                 if (this.root != this) {
@@ -9687,22 +9653,14 @@
                         return new BBox({
                             x: tx + x,
                             y: ty + y,
                             width,
                             height
                         });
                     }
-                    scale(factor) {
-                        return new BBox({
-                            x0: this.x0 * factor,
-                            x1: this.x1 * factor,
-                            y0: this.y0 * factor,
-                            y1: this.y1 * factor,
-                        });
-                    }
                     relativize(x, y) {
                         return [x - this.x, y - this.y];
                     }
                     contains(x, y) {
                         return this.x0 <= x && x <= this.x1 && this.y0 <= y && y <= this.y1;
                     }
                     clip(x, y) {
@@ -10235,16 +10193,16 @@
                     return connection.connect();
                 }
                 exports.pull_session = pull_session;
             },
             /* protocol/message.js */
             function _(require, module, exports, __esModule, __esExport) {
                 __esModule();
-                const serialization_1 = require(31) /* ../core/serialization */ ;
-                const string_1 = require(39) /* ../core/util/string */ ;
+                const serialization_1 = require(30) /* ../core/serialization */ ;
+                const string_1 = require(38) /* ../core/util/string */ ;
                 const assert_1 = require(12) /* ../core/util/assert */ ;
                 class Message {
                     get buffers() {
                         return this._buffers;
                     }
                     constructor(header, metadata, content) {
                         this._buffers = new Map();
@@ -12965,15 +12923,15 @@
             /* models/ranges/data_range1d.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const data_range_1 = require(94) /* ./data_range */ ;
                 const enums_1 = require(19) /* ../../core/enums */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const logging_1 = require(18) /* ../../core/logging */ ;
                 const bbox = tslib_1.__importStar(require(57) /* ../../core/util/bbox */ );
                 const util_1 = require(95) /* ../util */ ;
                 exports.auto_ranged = Symbol("auto_ranged");
 
                 function is_auto_ranged(r) {
                     return exports.auto_ranged in r;
@@ -18683,15 +18641,15 @@
                 var _a, _b, _c;
                 __esModule();
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const image_1 = require(150) /* ../../core/util/image */ ;
                 const color_1 = require(21) /* ../../core/util/color */ ;
                 const graphics_1 = require(151) /* ../../core/graphics */ ;
                 const text_1 = require(152) /* ../../core/util/text */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 const affine_1 = require(153) /* ../../core/util/affine */ ;
                 const bbox_1 = require(57) /* ../../core/util/bbox */ ;
                 const base_text_1 = require(147) /* ./base_text */ ;
                 const providers_1 = require(154) /* ./providers */ ;
                 /**
                  * Helper class for rendering MathText into Canvas
                  */
@@ -21407,15 +21365,15 @@
             },
             /* models/policies/labeling.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a, _b;
                 __esModule();
                 const model_1 = require(50) /* ../../model */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const types_2 = require(23) /* ../../core/types */ ;
                 class LabelingPolicy extends model_1.Model {
                     constructor(attrs) {
                         super(attrs);
                     }
                 }
@@ -21778,15 +21736,15 @@
             },
             /* models/formatters/datetime_tick_formatter.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const enums_1 = require(19) /* ../../core/enums */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const templating_1 = require(170) /* ../../core/util/templating */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const tick_formatter_1 = require(162) /* ./tick_formatter */ ;
                 const util_1 = require(174) /* ../tickers/util */ ;
                 const timezone_1 = tslib_1.__importDefault(require(173) /* timezone */ );
                 // Labels of time units, from finest to coarsest.
                 exports.resolution_order = [
@@ -24152,15 +24110,15 @@
                 })();
             },
             /* models/formatters/basic_tick_formatter.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tick_formatter_1 = require(162) /* ./tick_formatter */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
 
                 function unicode_replace(input) {
                     let output = "";
                     for (const c of input) {
                         if (c == "-")
                             output += "\u2212";
                         else
@@ -26069,15 +26027,15 @@
                                 } else {
                                     array = scale.v_compute(array);
                                 }
                                 this[`s${prop.attr}`] = array;
                             }
                         }
                         this._map_data();
-                        (_b = this.glglyph) === null || _b === void 0 ? void 0 : _b.set_data_mapped();
+                        (_b = this.glglyph) === null || _b === void 0 ? void 0 : _b.set_data_changed();
                     }
                     // This is where specs not included in coords are computed, e.g. radius.
                     _map_data() {}
                 }
                 exports.GlyphView = GlyphView;
                 GlyphView.__name__ = "GlyphView";
                 class Glyph extends model_1.Model {
@@ -27780,15 +27738,15 @@
             },
             /* models/formatters/customjs_tick_formatter.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tick_formatter_1 = require(162) /* ./tick_formatter */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 class CustomJSTickFormatter extends tick_formatter_1.TickFormatter {
                     constructor(attrs) {
                         super(attrs);
                     }
                     get names() {
                         return (0, object_1.keys)(this.args);
                     }
@@ -31513,21 +31471,21 @@
                 const legend_item_1 = require(254) /* ./legend_item */ ;
                 const enums_1 = require(19) /* ../../core/enums */ ;
                 const mixins = tslib_1.__importStar(require(78) /* ../../core/property_mixins */ );
                 const signaling_1 = require(15) /* ../../core/signaling */ ;
                 const side_panel_1 = require(144) /* ../../core/layout/side_panel */ ;
                 const bbox_1 = require(57) /* ../../core/util/bbox */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const graphics_1 = require(151) /* ../../core/graphics */ ;
                 const layout_1 = require(229) /* ../../core/layout */ ;
                 const {
                     max,
-                    ceil
+                    floor
                 } = Math;
                 class TextLayout extends layout_1.ContentLayoutable {
                     constructor(text) {
                         super();
                         this.text = text;
                     }
                     _content_size() {
@@ -31663,21 +31621,21 @@
                             let {
                                 ncols,
                                 nrows
                             } = this.model;
                             const n = entries.length;
                             if (vertical) {
                                 if (nrows != "auto") {} else if (ncols != "auto")
-                                    nrows = ceil(n / ncols);
+                                    nrows = floor(n / ncols);
                                 else
                                     nrows = Infinity;
                                 ncols = Infinity;
                             } else {
                                 if (ncols != "auto") {} else if (nrows != "auto")
-                                    ncols = ceil(n / nrows);
+                                    ncols = floor(n / nrows);
                                 else
                                     ncols = Infinity;
                                 nrows = Infinity;
                             }
                             return {
                                 ncols,
                                 nrows
@@ -33153,15 +33111,15 @@
                 const tslib_1 = require(1) /* tslib */ ;
                 const logging_1 = require(18) /* ../../core/logging */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
                 const build_views_1 = require(59) /* ../../core/build_views */ ;
                 const ui_element_1 = require(260) /* ../ui/ui_element */ ;
                 const enums_1 = require(19) /* ../../core/enums */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const tool_1 = require(267) /* ./tool */ ;
                 const tool_proxy_1 = require(268) /* ./tool_proxy */ ;
                 const tool_button_1 = require(269) /* ./tool_button */ ;
                 const gesture_tool_1 = require(274) /* ./gestures/gesture_tool */ ;
                 const inspect_tool_1 = require(276) /* ./inspectors/inspect_tool */ ;
@@ -35856,15 +35814,15 @@
             /* models/tools/tool_proxy.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const signaling_1 = require(15) /* ../../core/signaling */ ;
                 const model_1 = require(50) /* ../../model */ ;
                 const tool_1 = require(267) /* ./tool */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 class ToolProxy extends model_1.Model {
                     constructor(attrs) {
                         super(attrs);
                     }
                     // Operates all the tools given only one button
                     get underlying() {
                         return this.tools[0];
@@ -37344,15 +37302,15 @@
             /* models/callbacks/customjs.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const callback_1 = require(290) /* ./callback */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 const logging_1 = require(18) /* ../../core/logging */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 class CustomJS extends callback_1.Callback {
                     constructor(attrs) {
                         super(attrs);
                         this._state = null;
                     }
@@ -37575,17 +37533,14 @@
                 const dom_2 = require(56) /* ../../core/dom */ ;
                 const canvas_css_1 = tslib_1.__importDefault(require(298) /* ../../styles/canvas.css */ );
                 async function init_webgl() {
                     // We use a global invisible canvas and gl context. By having a global context,
                     // we avoid the limitation of max 16 contexts that most browsers have.
                     const canvas = document.createElement("canvas");
                     const gl = canvas.getContext("webgl", {
-                        alpha: true,
-                        antialias: false,
-                        depth: false,
                         premultipliedAlpha: true
                     });
                     // If WebGL is available, we store a reference to the ReGL wrapper on
                     // the ctx object, because that's what gets passed everywhere.
                     if (gl != null) {
                         const webgl = await (0, modules_1.load_module)(Promise.resolve().then(() => tslib_1.__importStar(require(511) /* ../glyphs/webgl */ )));
                         if (webgl != null) {
@@ -41053,15 +41008,15 @@
                 var _a;
                 __esModule();
                 const has_props_1 = require(14) /* ../../core/has_props */ ;
                 const expression_1 = require(301) /* ./expression */ ;
                 const types_1 = require(23) /* ../../core/types */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 const types_2 = require(8) /* ../../core/util/types */ ;
                 class CustomJSExpr extends expression_1.Expression {
                     constructor(attrs) {
                         super(attrs);
                     }
                     connect_signals() {
                         super.connect_signals();
@@ -41424,15 +41379,15 @@
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const filter_1 = require(219) /* ./filter */ ;
                 const types_1 = require(23) /* ../../core/types */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
                 const types_2 = require(8) /* ../../core/util/types */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 class CustomJSFilter extends filter_1.Filter {
                     constructor(attrs) {
                         super(attrs);
                     }
                     get names() {
                         return (0, object_1.keys)(this.args);
                     }
@@ -42670,15 +42625,15 @@
                 const tslib_1 = require(1) /* tslib */ ;
                 const xy_glyph_1 = require(202) /* ./xy_glyph */ ;
                 const property_mixins_1 = require(78) /* ../../core/property_mixins */ ;
                 const types_1 = require(23) /* ../../core/types */ ;
                 const enums_1 = require(19) /* ../../core/enums */ ;
                 const hittest = tslib_1.__importStar(require(210) /* ../../core/hittest */ );
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
-                const uniforms = tslib_1.__importStar(require(38) /* ../../core/uniforms */ );
+                const uniforms = tslib_1.__importStar(require(37) /* ../../core/uniforms */ );
                 const arrayable_1 = require(13) /* ../../core/util/arrayable */ ;
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 class CircleView extends xy_glyph_1.XYGlyphView {
                     async load_glglyph() {
                         const {
                             CircleGL
                         } = await Promise.resolve().then(() => tslib_1.__importStar(require(529) /* ./webgl/circle */ ));
@@ -43249,15 +43204,15 @@
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const glyph_1 = require(203) /* ./glyph */ ;
                 const utils_1 = require(209) /* ./utils */ ;
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 const property_mixins_1 = require(78) /* ../../core/property_mixins */ ;
-                const uniforms = tslib_1.__importStar(require(38) /* ../../core/uniforms */ );
+                const uniforms = tslib_1.__importStar(require(37) /* ../../core/uniforms */ );
                 const arrayable_1 = require(13) /* ../../core/util/arrayable */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
                 const {
                     abs,
                     max
                 } = Math;
@@ -43417,15 +43372,15 @@
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const glyph_1 = require(203) /* ./glyph */ ;
                 const utils_1 = require(209) /* ./utils */ ;
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 const property_mixins_1 = require(78) /* ../../core/property_mixins */ ;
                 const types_1 = require(23) /* ../../core/types */ ;
-                const uniforms = tslib_1.__importStar(require(38) /* ../../core/uniforms */ );
+                const uniforms = tslib_1.__importStar(require(37) /* ../../core/uniforms */ );
                 const arrayable_1 = require(13) /* ../../core/util/arrayable */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
                 const UNUSED = 0;
                 class HStripView extends glyph_1.GlyphView {
                     async lazy_initialize() {
                         await super.lazy_initialize();
@@ -43712,15 +43667,15 @@
                     // overriding map_data instead of _map_data because the default automatic mappings
                     // for other glyphs (with cartesian coordinates) is not useful
                     map_data() {
                         var _b;
                         [this.sx, this.sy] = this.renderer.coordinates.map_to_screen(this._x, this._y);
                         [this.svx, this.svy] = this._get_unscaled_vertices();
                         // From overridden GlyphView.map_data()
-                        (_b = this.glglyph) === null || _b === void 0 ? void 0 : _b.set_data_mapped();
+                        (_b = this.glglyph) === null || _b === void 0 ? void 0 : _b.set_data_changed();
                     }
                     _get_unscaled_vertices() {
                         const size = this.model.size;
                         const aspect_scale = this.model.aspect_scale;
                         if (this.model.orientation == "pointytop") {
                             const rscale = this.renderer.yscale;
                             const hscale = this.renderer.xscale;
@@ -45727,15 +45682,15 @@
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const xy_glyph_1 = require(202) /* ./xy_glyph */ ;
                 const property_mixins_1 = require(78) /* ../../core/property_mixins */ ;
                 const hittest = tslib_1.__importStar(require(210) /* ../../core/hittest */ );
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
-                const uniforms = tslib_1.__importStar(require(38) /* ../../core/uniforms */ );
+                const uniforms = tslib_1.__importStar(require(37) /* ../../core/uniforms */ );
                 const array_1 = require(10) /* ../../core/util/array */ ;
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 class MarkerView extends xy_glyph_1.XYGlyphView {
                     _render(ctx, indices, data) {
                         const {
                             sx,
                             sy,
@@ -46722,18 +46677,18 @@
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const xy_glyph_1 = require(202) /* ./xy_glyph */ ;
                 const mixins = tslib_1.__importStar(require(78) /* ../../core/property_mixins */ );
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
-                const uniforms_1 = require(38) /* ../../core/uniforms */ ;
+                const uniforms_1 = require(37) /* ../../core/uniforms */ ;
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 const bbox_1 = require(57) /* ../../core/util/bbox */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const affine_1 = require(153) /* ../../core/util/affine */ ;
                 const graphics_1 = require(151) /* ../../core/graphics */ ;
                 const kinds_1 = require(236) /* ../common/kinds */ ;
                 const resolve = tslib_1.__importStar(require(238) /* ../common/resolve */ );
                 const painting_1 = require(237) /* ../common/painting */ ;
                 class TextAnchorSpec extends p.DataSpec {}
                 TextAnchorSpec.__name__ = "TextAnchorSpec";
@@ -47113,15 +47068,15 @@
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const glyph_1 = require(203) /* ./glyph */ ;
                 const utils_1 = require(209) /* ./utils */ ;
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 const property_mixins_1 = require(78) /* ../../core/property_mixins */ ;
-                const uniforms = tslib_1.__importStar(require(38) /* ../../core/uniforms */ );
+                const uniforms = tslib_1.__importStar(require(37) /* ../../core/uniforms */ );
                 const arrayable_1 = require(13) /* ../../core/util/arrayable */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
                 const {
                     abs,
                     max
                 } = Math;
@@ -47281,15 +47236,15 @@
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const glyph_1 = require(203) /* ./glyph */ ;
                 const utils_1 = require(209) /* ./utils */ ;
                 const selection_1 = require(101) /* ../selections/selection */ ;
                 const property_mixins_1 = require(78) /* ../../core/property_mixins */ ;
                 const types_1 = require(23) /* ../../core/types */ ;
-                const uniforms = tslib_1.__importStar(require(38) /* ../../core/uniforms */ );
+                const uniforms = tslib_1.__importStar(require(37) /* ../../core/uniforms */ );
                 const arrayable_1 = require(13) /* ../../core/util/arrayable */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
                 const UNUSED = 0;
                 class VStripView extends glyph_1.GlyphView {
                     async lazy_initialize() {
                         await super.lazy_initialize();
@@ -49045,15 +49000,15 @@
                         composite.ctx.fillStyle = bg_color;
                         composite.ctx.fillRect(x, y, width, height);
                         for (const view of this.child_views) {
                             const region = view.export(type, hidpi);
                             const {
                                 x,
                                 y
-                            } = view.bbox.scale(composite.pixel_ratio);
+                            } = view.bbox;
                             composite.ctx.drawImage(region.canvas, x, y);
                         }
                         return composite;
                     }
                     serializable_state() {
                         return Object.assign(Object.assign({}, super.serializable_state()), {
                             children: this.child_views.map((child) => child.serializable_state())
@@ -49110,15 +49065,15 @@
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const ui_element_1 = require(260) /* ../ui/ui_element */ ;
                 const menu_item_1 = require(369) /* ./menu_item */ ;
                 const enums_1 = require(19) /* ../../core/enums */ ;
                 const build_views_1 = require(59) /* ../../core/build_views */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const menus_css_1 = tslib_1.__importStar(require(271) /* ../../styles/menus.css */ ),
                     menus = menus_css_1;
                 class MenuView extends ui_element_1.UIElementView {
                     constructor() {
                         super(...arguments);
                         this.items = new Map();
                     }
@@ -49465,15 +49420,15 @@
                 var _a;
                 __esModule();
                 const layout_dom_1 = require(367) /* ./layout_dom */ ;
                 const alignments_1 = require(370) /* ./alignments */ ;
                 const kinds_1 = require(236) /* ../common/kinds */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
                 const grid_1 = require(231) /* ../../core/layout/grid */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const {
                     max
                 } = Math;
                 class CSSGridBoxView extends layout_dom_1.LayoutDOMView {
                     connect_signals() {
                         super.connect_signals();
@@ -50372,15 +50327,15 @@
             },
             /* models/transforms/customjs_transform.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const transform_1 = require(86) /* ./transform */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 class CustomJSTransform extends transform_1.Transform {
                     constructor(attrs) {
                         super(attrs);
                     }
                     get names() {
                         return (0, object_1.keys)(this.args);
                     }
@@ -51046,15 +51001,15 @@
                 const build_views_1 = require(59) /* ../../core/build_views */ ;
                 const visuals_1 = require(75) /* ../../core/visuals */ ;
                 const logging_1 = require(18) /* ../../core/logging */ ;
                 const bokeh_events_2 = require(52) /* ../../core/bokeh_events */ ;
                 const throttle_1 = require(403) /* ../../core/util/throttle */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const canvas_2 = require(263) /* ../../core/util/canvas */ ;
                 const alignments_1 = require(230) /* ../../core/layout/alignments */ ;
                 const border_1 = require(232) /* ../../core/layout/border */ ;
                 const grid_1 = require(231) /* ../../core/layout/grid */ ;
                 const side_panel_1 = require(144) /* ../../core/layout/side_panel */ ;
                 const bbox_1 = require(57) /* ../../core/util/bbox */ ;
                 const text_1 = require(152) /* ../../core/util/text */ ;
@@ -51092,17 +51047,14 @@
                     }
                     get state() {
                         return this._state_manager;
                     }
                     set invalidate_dataranges(value) {
                         this._range_manager.invalidate_dataranges = value;
                     }
-                    get computed_renderer_views() {
-                        return this.computed_renderers.map((r) => this.renderer_views.get(r));
-                    }
                     renderer_view(renderer) {
                         const view = this.renderer_views.get(renderer);
                         if (view == null) {
                             for (const [, renderer_view] of this.renderer_views) {
                                 const view = renderer_view.renderer_view(renderer);
                                 if (view != null)
                                     return view;
@@ -51846,24 +51798,17 @@
                     repaint() {
                         this._invalidate_layout_if_needed();
                         this.paint();
                     }
                     paint() {
                         if (this.is_paused)
                             return;
-                        if (this.is_displayed) {
+                        if (this.model.visible) {
                             logging_1.logger.trace(`${this.toString()}.paint()`);
                             this._actual_paint();
-                        } else {
-                            // This is possibly the first render cycle, but plot isn't displayed,
-                            // so all renderers have to be manually marked as finished, because
-                            // their `render()` method didn't run.
-                            for (const renderer_view of this.computed_renderer_views) {
-                                renderer_view.mark_finished();
-                            }
                         }
                         if (this._needs_notify) {
                             this._needs_notify = false;
                             this.notify_finished();
                         }
                     }
                     _actual_paint() {
@@ -52762,14 +52707,15 @@
                 var _a;
                 __esModule();
                 const layout_dom_1 = require(367) /* ../layouts/layout_dom */ ;
                 const grid_box_1 = require(371) /* ../layouts/grid_box */ ;
                 const kinds_1 = require(236) /* ../common/kinds */ ;
                 const toolbar_1 = require(259) /* ../tools/toolbar */ ;
                 const action_tool_1 = require(277) /* ../tools/actions/action_tool */ ;
+                const canvas_1 = require(263) /* ../../core/util/canvas */ ;
                 const build_views_1 = require(59) /* ../../core/build_views */ ;
                 const enums_1 = require(19) /* ../../core/enums */ ;
                 class GridPlotView extends layout_dom_1.LayoutDOMView {
                     constructor() {
                         super(...arguments);
                         this._tool_views = new Map();
                     }
@@ -52877,14 +52823,47 @@
                                     return "row-reverse";
                             }
                         })();
                         this.style.append(":host", {
                             flex_direction
                         });
                     }
+                    export (type = "auto", hidpi = true) {
+                        const output_backend = (() => {
+                            switch (type) {
+                                case "auto": // TODO: actually infer the best type
+                                case "png":
+                                    return "canvas";
+                                case "svg":
+                                    return "svg";
+                            }
+                        })();
+                        const composite = new canvas_1.CanvasLayer(output_backend, hidpi);
+                        const {
+                            x,
+                            y,
+                            width,
+                            height
+                        } = this.grid_box_view.bbox.relative();
+                        composite.resize(width, height);
+                        composite.ctx.save();
+                        const bg_color = getComputedStyle(this.el).backgroundColor;
+                        composite.ctx.fillStyle = bg_color;
+                        composite.ctx.fillRect(x, y, width, height);
+                        for (const view of this.child_views) {
+                            const region = view.export(type, hidpi);
+                            const {
+                                x,
+                                y
+                            } = view.bbox;
+                            composite.ctx.drawImage(region.canvas, x, y);
+                        }
+                        composite.ctx.restore();
+                        return composite;
+                    }
                 }
                 exports.GridPlotView = GridPlotView;
                 GridPlotView.__name__ = "GridPlotView";
                 class GridPlot extends layout_dom_1.LayoutDOM {
                     constructor(attrs) {
                         super(attrs);
                     }
@@ -54147,49 +54126,32 @@
                 const wmts_tile_source_1 = require(436) /* ./wmts_tile_source */ ;
                 const renderer_1 = require(74) /* ../renderers/renderer */ ;
                 const range1d_1 = require(88) /* ../ranges/range1d */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
                 const image_1 = require(150) /* ../../core/util/image */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
-                const assert_1 = require(12) /* ../../core/util/assert */ ;
                 const attribution_css_1 = tslib_1.__importDefault(require(437) /* ../../styles/attribution.css */ );
                 class TileRendererView extends renderer_1.RendererView {
-                    constructor() {
-                        super(...arguments);
-                        this._tiles = null;
-                    }
-                    mark_finished() {
-                        super.mark_finished();
+                    initialize() {
                         this._tiles = [];
+                        super.initialize();
                     }
                     connect_signals() {
                         super.connect_signals();
                         this.connect(this.model.change, () => this.request_render());
                         this.connect(this.model.tile_source.change, () => this.request_render());
                     }
                     remove() {
                         if (this.attribution_el != null)
                             (0, dom_1.remove)(this.attribution_el);
                         super.remove();
                     }
                     get_extent() {
-                        const {
-                            x_range,
-                            y_range
-                        } = this;
-                        const x_start = x_range.start;
-                        const y_start = y_range.start;
-                        const x_end = x_range.end;
-                        const y_end = y_range.end;
-                        (0, assert_1.assert)(isFinite(x_start));
-                        (0, assert_1.assert)(isFinite(y_start));
-                        (0, assert_1.assert)(isFinite(x_end));
-                        (0, assert_1.assert)(isFinite(y_end));
-                        return [x_start, y_start, x_end, y_end];
+                        return [this.x_range.start, this.y_range.start, this.x_range.end, this.y_range.end];
                     }
                     get map_plot() {
                         return this.plot_model;
                     }
                     get map_canvas() {
                         return this.layer.ctx;
                     }
@@ -54275,16 +54237,14 @@
                             bounds,
                             loaded: false,
                             finished: false,
                             x_coord: bounds[0],
                             y_coord: bounds[3],
                         };
                         this.model.tile_source.tiles.set(cache_key, tile);
-                        if (this._tiles == null)
-                            this._tiles = [];
                         this._tiles.push(tile);
                         new image_1.ImageLoader(src, {
                             loaded: (img) => {
                                 Object.assign(tile, {
                                     img,
                                     loaded: true
                                 });
@@ -54317,15 +54277,15 @@
                             this._last_height = this.map_frame.bbox.height;
                             this._last_width = this.map_frame.bbox.width;
                         }
                     }
                     has_finished() {
                         if (!super.has_finished())
                             return false;
-                        if (this._tiles == null)
+                        if (this._tiles.length == 0)
                             return false;
                         for (const tile of this._tiles) {
                             if (!tile.finished)
                                 return false;
                         }
                         return true;
                     }
@@ -54575,15 +54535,15 @@
                 __esExport("Texture", texture_1.Texture);
             },
             /* models/textures/canvas_texture.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const texture_1 = require(441) /* ./texture */ ;
-                const string_1 = require(39) /* ../../core/util/string */ ;
+                const string_1 = require(38) /* ../../core/util/string */ ;
                 class CanvasTexture extends texture_1.Texture {
                     constructor(attrs) {
                         super(attrs);
                     }
                     get func() {
                         const code = (0, string_1.use_strict)(this.code);
                         return new Function("ctx", "color", "scale", "weight", code);
@@ -55060,22 +55020,22 @@
                 var _a;
                 __esModule();
                 const tslib_1 = require(1) /* tslib */ ;
                 const ui_element_1 = require(260) /* ./ui_element */ ;
                 const p = tslib_1.__importStar(require(17) /* ../../core/properties */ );
                 const has_props_1 = require(14) /* ../../core/has_props */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
-                const pretty_1 = require(41) /* ../../core/util/pretty */ ;
+                const pretty_1 = require(40) /* ../../core/util/pretty */ ;
                 const model_1 = require(50) /* ../../model */ ;
                 const types_1 = require(8) /* ../../core/util/types */ ;
                 const object_1 = require(9) /* ../../core/util/object */ ;
                 const array_1 = require(10) /* ../../core/util/array */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 const signaling_1 = require(15) /* ../../core/signaling */ ;
-                const diagnostics_1 = require(37) /* ../../core/diagnostics */ ;
+                const diagnostics_1 = require(36) /* ../../core/diagnostics */ ;
                 const examiner_css_1 = tslib_1.__importDefault(require(453) /* ../../styles/examiner.css */ );
                 class HTMLPrinter {
                     constructor(click, max_items, max_depth) {
                         this.visited = new WeakSet();
                         this.depth = 0;
                         this.click = click;
                         this.max_items = max_items;
@@ -60274,15 +60234,15 @@
             },
             /* models/tools/inspectors/customjs_hover.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const model_1 = require(50) /* ../../../model */ ;
                 const object_1 = require(9) /* ../../../core/util/object */ ;
-                const string_1 = require(39) /* ../../../core/util/string */ ;
+                const string_1 = require(38) /* ../../../core/util/string */ ;
                 class CustomJSHover extends model_1.Model {
                     constructor(attrs) {
                         super(attrs);
                     }
                     get values() {
                         return (0, object_1.values)(this.args);
                     }
@@ -60319,15 +60279,15 @@
                 const build_views_1 = require(59) /* ../../../core/build_views */ ;
                 const dom_1 = require(56) /* ../../../core/dom */ ;
                 const enums_1 = require(19) /* ../../../core/enums */ ;
                 const hittest = tslib_1.__importStar(require(210) /* ../../../core/hittest */ );
                 const signaling_1 = require(15) /* ../../../core/signaling */ ;
                 const assert_1 = require(12) /* ../../../core/util/assert */ ;
                 const color_1 = require(21) /* ../../../core/util/color */ ;
-                const iterator_1 = require(33) /* ../../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../../core/util/iterator */ ;
                 const object_1 = require(9) /* ../../../core/util/object */ ;
                 const templating_1 = require(170) /* ../../../core/util/templating */ ;
                 const types_1 = require(8) /* ../../../core/util/types */ ;
                 const icons_css_1 = require(272) /* ../../../styles/icons.css */ ;
                 const styles = tslib_1.__importStar(require(457) /* ../../../styles/tooltips.css */ );
                 const tooltip_1 = require(455) /* ../../ui/tooltip */ ;
                 const template_1 = require(499) /* ../../dom/template */ ;
@@ -61410,15 +61370,15 @@
             },
             /* models/dom/toggle_group.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const action_1 = require(501) /* ./action */ ;
                 const renderer_1 = require(74) /* ../renderers/renderer */ ;
-                const iterator_1 = require(33) /* ../../core/util/iterator */ ;
+                const iterator_1 = require(32) /* ../../core/util/iterator */ ;
                 class ToggleGroupView extends action_1.ActionView {
                     update(_source, i, _vars /*, formatters?: Formatters*/ ) {
                         for (const [group, j] of(0, iterator_1.enumerate)(this.model.groups)) {
                             group.visible = i == j;
                         }
                     }
                 }
@@ -61445,15 +61405,15 @@
             /* models/dom/value_of.js */
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const dom_node_1 = require(449) /* ./dom_node */ ;
                 const has_props_1 = require(14) /* ../../core/has_props */ ;
                 const dom_1 = require(56) /* ../../core/dom */ ;
-                const pretty_1 = require(41) /* ../../core/util/pretty */ ;
+                const pretty_1 = require(40) /* ../../core/util/pretty */ ;
                 class ValueOfView extends dom_node_1.DOMNodeView {
                     connect_signals() {
                         super.connect_signals();
                         const {
                             obj,
                             attr
                         } = this.model;
@@ -61526,26 +61486,26 @@
             "core/types": 23,
             "core/util/bitset": 24,
             "core/util/eq": 25,
             "core/util/platform": 26,
             "core/vectorization": 27,
             "core/settings": 28,
             "core/util/ndarray": 29,
-            "core/util/cloneable": 30,
-            "core/serialization/index": 31,
-            "core/serialization/serializer": 32,
-            "core/util/iterator": 33,
-            "core/serialization/buffer": 34,
-            "core/util/buffer": 35,
-            "core/serialization/reps": 36,
-            "core/diagnostics": 37,
-            "core/uniforms": 38,
-            "core/util/string": 39,
-            "document/events": 40,
-            "core/util/pretty": 41,
+            "core/serialization/index": 30,
+            "core/serialization/serializer": 31,
+            "core/util/iterator": 32,
+            "core/serialization/buffer": 33,
+            "core/util/buffer": 34,
+            "core/serialization/reps": 35,
+            "core/diagnostics": 36,
+            "core/uniforms": 37,
+            "core/util/string": 38,
+            "document/events": 39,
+            "core/util/pretty": 40,
+            "core/util/cloneable": 41,
             "core/patching": 42,
             "core/util/set": 43,
             "core/util/typed_array": 44,
             "core/resolvers": 45,
             "core/serialization/deserializer": 46,
             "core/util/refs": 47,
             "core/util/slice": 48,
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/bokeh.min.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/bokeh.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -532,23 +532,23 @@
             function _(e, t, o, s, l) {
                 s();
                 const r = e(1);
                 l("version", e(3).version), l("index", e(4).index), o.embed = r.__importStar(e(4)), o.protocol = r.__importStar(e(67)), o._testing = r.__importStar(e(68));
                 var _ = e(18);
                 l("logger", _.logger), l("set_log_level", _.set_log_level), l("settings", e(28).settings), l("Models", e(7).default_resolver), l("documents", e(5).documents), l("safely", e(69).safely)
             },
-            function _(n, i, o, c, e) {
-                c(), o.version = "3.2.1"
+            function _(n, e, i, o, v) {
+                o(), i.version = "3.3.0-dev.1"
             },
             function _(e, o, t, n, r) {
                 n();
                 const s = e(5),
                     d = e(28),
                     i = e(18),
-                    _ = e(39),
+                    _ = e(38),
                     c = e(9),
                     a = e(8),
                     u = e(16),
                     l = e(53),
                     m = e(60),
                     f = e(65);
                 var w = e(53);
@@ -595,36 +595,36 @@
                 }, t.embed_items = async function(e, o, t, n) {
                     return await (0, u.defer)(), k(e, o, t, n)
                 }
             },
             function _(t, _, o, r, n) {
                 r();
                 const a = t(1);
-                a.__exportStar(t(6), o), a.__exportStar(t(40), o)
+                a.__exportStar(t(6), o), a.__exportStar(t(39), o)
             },
             function _(e, t, s, o, n) {
                 o();
                 const i = e(1),
                     _ = e(7),
                     l = e(3),
                     r = e(18),
                     a = e(45),
-                    c = e(31),
+                    c = e(30),
                     d = e(46),
                     h = e(49),
                     m = e(15),
                     u = e(8),
                     f = e(25),
                     v = e(10),
                     g = e(9),
                     p = i.__importStar(e(43)),
                     w = e(50),
                     b = e(51),
                     k = e(52),
-                    y = e(40);
+                    y = e(39);
                 d.Deserializer.register("model", b.decode_def);
                 class z {
                     constructor(e) {
                         this.subscribed_models = new Set, this.document = e
                     }
                     send_event(e) {
                         if (e.publish) {
@@ -1579,23 +1579,23 @@
                 var r;
                 n();
                 const o = t(1),
                     c = t(15),
                     a = o.__importStar(t(17)),
                     h = o.__importStar(t(20)),
                     _ = t(12),
-                    l = t(39),
+                    l = t(38),
                     u = t(9),
                     f = t(8),
                     p = t(25),
-                    d = t(31),
-                    g = t(40),
+                    d = t(30),
+                    g = t(39),
                     y = t(25),
-                    m = t(41),
-                    v = t(30),
+                    m = t(40),
+                    v = t(41),
                     w = o.__importStar(t(20)),
                     b = t(27),
                     S = t(42),
                     $ = new WeakMap;
                 class j extends((0, c.Signalable)()) {
                     get is_syncable() {
                         return !0
@@ -2118,18 +2118,18 @@
                     d = e(11),
                     S = e(21),
                     p = e(26),
                     h = e(8),
                     m = e(27),
                     v = e(28),
                     f = e(29),
-                    y = e(37),
+                    y = e(36),
                     x = e(12),
-                    g = e(31),
-                    A = e(38);
+                    g = e(30),
+                    A = e(37);
 
                 function w(e) {
                     try {
                         return JSON.stringify(e)
                     } catch (t) {
                         return e.toString()
                     }
@@ -3807,299 +3807,241 @@
                     }
                     get force_webgl() {
                         return this._force_webgl
                     }
                 }
                 r.Settings = i, i.__name__ = "Settings", r.settings = new i
             },
-            function _(e, t, s, r, n) {
-                var a, i, h, u, l, o, c, p, y, _;
+            function _(t, e, s, r, n) {
+                var a, i, h, u, l, o, p, c, y, _;
                 r();
-                const A = e(8),
-                    d = e(26),
-                    g = e(25),
-                    f = e(30),
-                    m = e(31),
-                    w = Symbol("__ndarray__");
+                const A = t(8),
+                    d = t(26),
+                    g = t(25),
+                    f = t(30),
+                    m = Symbol("__ndarray__");
 
-                function N(e, t) {
+                function N(t, e) {
                     return {
                         type: "ndarray",
-                        array: t.encode("object" == e.dtype ? Array.from(e) : e.buffer),
+                        array: e.encode("object" == t.dtype ? Array.from(t) : t.buffer),
                         order: d.BYTE_ORDER,
-                        dtype: e.dtype,
-                        shape: e.shape
+                        dtype: t.dtype,
+                        shape: t.shape
                     }
                 }
                 class D extends Uint8Array {
-                    constructor(e, t) {
-                        super(e), this[a] = !0, this.dtype = "bool", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(a = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new D(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                    constructor(t, e) {
+                        super(t), this[a] = !0, this.dtype = "bool", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(a = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return 1 == this[e]
+                    get(t) {
+                        return 1 == this[t]
                     }
                 }
                 s.BoolNDArray = D, D.__name__ = "BoolNDArray";
                 class q extends Uint8Array {
-                    constructor(e, t) {
-                        super(e), this[i] = !0, this.dtype = "uint8", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(i = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new q(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                    constructor(t, e) {
+                        super(t), this[i] = !0, this.dtype = "uint8", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(i = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
                 s.Uint8NDArray = q, q.__name__ = "Uint8NDArray";
                 class b extends Int8Array {
-                    constructor(e, t) {
-                        super(e), this[h] = !0, this.dtype = "int8", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(h = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new b(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                    constructor(t, e) {
+                        super(t), this[h] = !0, this.dtype = "int8", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(h = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
                 s.Int8NDArray = b, b.__name__ = "Int8NDArray";
-                class U extends Uint16Array {
-                    constructor(e, t) {
-                        super(e), this[u] = !0, this.dtype = "uint16", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(u = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new U(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                class w extends Uint16Array {
+                    constructor(t, e) {
+                        super(t), this[u] = !0, this.dtype = "uint16", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(u = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
-                s.Uint16NDArray = U, U.__name__ = "Uint16NDArray";
-                class I extends Int16Array {
-                    constructor(e, t) {
-                        super(e), this[l] = !0, this.dtype = "int16", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(l = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new I(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                s.Uint16NDArray = w, w.__name__ = "Uint16NDArray";
+                class U extends Int16Array {
+                    constructor(t, e) {
+                        super(t), this[l] = !0, this.dtype = "int16", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(l = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
-                s.Int16NDArray = I, I.__name__ = "Int16NDArray";
-                class x extends Uint32Array {
-                    constructor(e, t) {
-                        super(e), this[o] = !0, this.dtype = "uint32", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(o = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new x(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                s.Int16NDArray = U, U.__name__ = "Int16NDArray";
+                class I extends Uint32Array {
+                    constructor(t, e) {
+                        super(t), this[o] = !0, this.dtype = "uint32", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(o = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
-                s.Uint32NDArray = x, x.__name__ = "Uint32NDArray";
-                class z extends Int32Array {
-                    constructor(e, t) {
-                        super(e), this[c] = !0, this.dtype = "int32", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(c = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new z(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                s.Uint32NDArray = I, I.__name__ = "Uint32NDArray";
+                class x extends Int32Array {
+                    constructor(t, e) {
+                        super(t), this[p] = !0, this.dtype = "int32", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(p = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
-                s.Int32NDArray = z, z.__name__ = "Int32NDArray";
-                class F extends Float32Array {
-                    constructor(e, t) {
-                        super(e), this[p] = !0, this.dtype = "float32", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(p = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new F(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                s.Int32NDArray = x, x.__name__ = "Int32NDArray";
+                class z extends Float32Array {
+                    constructor(t, e) {
+                        super(t), this[c] = !0, this.dtype = "float32", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(c = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
-                s.Float32NDArray = F, F.__name__ = "Float32NDArray";
-                class j extends Float64Array {
-                    constructor(e, t) {
-                        super(e), this[y] = !0, this.dtype = "float64", this.shape = null != t ? t : v(e) ? e.shape : [this.length], this.dimension = this.shape.length
-                    } [(y = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new j(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                s.Float32NDArray = z, z.__name__ = "Float32NDArray";
+                class F extends Float64Array {
+                    constructor(t, e) {
+                        super(t), this[y] = !0, this.dtype = "float64", this.shape = null != e ? e : B(t) ? t.shape : [this.length], this.dimension = this.shape.length
+                    } [(y = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
-                s.Float64NDArray = j, j.__name__ = "Float64NDArray";
-                class B extends Array {
+                s.Float64NDArray = F, F.__name__ = "Float64NDArray";
+                class j extends Array {
                     get shape() {
-                        var e;
-                        return null !== (e = this._shape) && void 0 !== e ? e : [this.length]
+                        var t;
+                        return null !== (t = this._shape) && void 0 !== t ? t : [this.length]
                     }
                     get dimension() {
                         return this.shape.length
                     }
-                    constructor(e, t) {
-                        const s = e instanceof ArrayBuffer ? new Float64Array(e) : e;
+                    constructor(t, e) {
+                        const s = t instanceof ArrayBuffer ? new Float64Array(t) : t;
                         if (super((0, A.isNumber)(s) ? s : s.length), this[_] = !0, this.dtype = "object", !(0, A.isNumber)(s))
-                            for (let e = 0; e < s.length; e++) this[e] = s[e];
-                        this._shape = null != t ? t : v(s) ? s.shape : void 0
-                    } [(_ = w, g.equals)](e, t) {
-                        return t.eq(this.shape, e.shape) && t.arrays(this, e)
-                    } [f.clone](e) {
-                        return new B(this, e.clone(this.shape))
-                    } [m.serialize](e) {
-                        return N(this, e)
+                            for (let t = 0; t < s.length; t++) this[t] = s[t];
+                        this._shape = null != e ? e : B(s) ? s.shape : void 0
+                    } [(_ = m, g.equals)](t, e) {
+                        return e.eq(this.shape, t.shape) && e.arrays(this, t)
+                    } [f.serialize](t) {
+                        return N(this, t)
                     }
-                    get(e) {
-                        return this[e]
+                    get(t) {
+                        return this[t]
                     }
                 }
 
-                function v(e) {
-                    return (0, A.isObject)(e) && w in e
+                function B(t) {
+                    return (0, A.isObject)(t) && m in t
                 }
-                s.ObjectNDArray = B, B.__name__ = "ObjectNDArray", s.is_NDArray = v, s.ndarray = function(e, {
-                    dtype: t,
+                s.ObjectNDArray = j, j.__name__ = "ObjectNDArray", s.is_NDArray = B, s.ndarray = function(t, {
+                    dtype: e,
                     shape: s
                 } = {}) {
-                    switch (null == t && (t = (() => {
+                    switch (null == e && (e = (() => {
                             switch (!0) {
-                                case e instanceof Uint8Array:
+                                case t instanceof Uint8Array:
                                     return "uint8";
-                                case e instanceof Int8Array:
+                                case t instanceof Int8Array:
                                     return "int8";
-                                case e instanceof Uint16Array:
+                                case t instanceof Uint16Array:
                                     return "uint16";
-                                case e instanceof Int16Array:
+                                case t instanceof Int16Array:
                                     return "int16";
-                                case e instanceof Uint32Array:
+                                case t instanceof Uint32Array:
                                     return "uint32";
-                                case e instanceof Int32Array:
+                                case t instanceof Int32Array:
                                     return "int32";
-                                case e instanceof Float32Array:
+                                case t instanceof Float32Array:
                                     return "float32";
-                                case e instanceof ArrayBuffer:
-                                case e instanceof Float64Array:
+                                case t instanceof ArrayBuffer:
+                                case t instanceof Float64Array:
                                     return "float64";
                                 default:
                                     return "object"
                             }
-                        })()), t) {
+                        })()), e) {
                         case "bool":
-                            return new D(e, s);
+                            return new D(t, s);
                         case "uint8":
-                            return new q(e, s);
+                            return new q(t, s);
                         case "int8":
-                            return new b(e, s);
+                            return new b(t, s);
                         case "uint16":
-                            return new U(e, s);
+                            return new w(t, s);
                         case "int16":
-                            return new I(e, s);
+                            return new U(t, s);
                         case "uint32":
-                            return new x(e, s);
+                            return new I(t, s);
                         case "int32":
-                            return new z(e, s);
+                            return new x(t, s);
                         case "float32":
-                            return new F(e, s);
+                            return new z(t, s);
                         case "float64":
-                            return new j(e, s);
+                            return new F(t, s);
                         case "object":
-                            return new B(e, s)
+                            return new j(t, s)
                     }
                 }
             },
-            function _(n, e, t, o, r) {
-                o();
-                const i = n(9),
-                    c = n(8);
-
-                function l(n) {
-                    return (0, c.isObject)(n) && t.clone in n
-                }
-                t.clone = Symbol("clone"), t.is_Cloneable = l;
-                class s extends Error {}
-                t.CloningError = s, s.__name__ = "CloningError";
-                class a {
-                    constructor() {}
-                    clone(n) {
-                        if (l(n)) return n[t.clone](this);
-                        if ((0, c.isPrimitive)(n)) return n;
-                        if ((0, c.isArray)(n)) {
-                            const e = n.length,
-                                t = new Array(e);
-                            for (let o = 0; o < e; o++) {
-                                const e = n[o];
-                                t[o] = this.clone(e)
-                            }
-                            return t
-                        }
-                        if ((0, c.isPlainObject)(n)) {
-                            const e = {};
-                            for (const [t, o] of(0, i.entries)(n)) e[t] = this.clone(o);
-                            return e
-                        }
-                        if (n instanceof Map) return new Map([...n].map((([n, e]) => [this.clone(n), this.clone(e)])));
-                        if (n instanceof Set) return new Set([...n].map((n => this.clone(n))));
-                        throw new s(`${Object.prototype.toString.call(n)} is not cloneable`)
-                    }
-                }
-                t.Cloner = a, a.__name__ = "Cloner"
-            },
             function _(r, e, i, a, f) {
                 a();
                 const o = r(1);
-                var l = r(32);
+                var l = r(31);
                 f("Serializer", l.Serializer), f("SerializationError", l.SerializationError), f("serialize", l.serialize);
-                var t = r(34);
-                f("Buffer", t.Buffer), f("Base64Buffer", t.Base64Buffer), o.__exportStar(r(36), i)
+                var t = r(33);
+                f("Buffer", t.Buffer), f("Base64Buffer", t.Base64Buffer), o.__exportStar(r(35), i)
             },
             function _(e, r, t, n, i) {
                 n();
                 const s = e(12),
                     a = e(9),
                     o = e(8),
-                    c = e(33),
+                    c = e(32),
                     l = e(26),
-                    u = e(34);
+                    u = e(33);
                 t.serialize = Symbol("serialize");
                 class f extends Error {}
                 t.SerializationError = f, f.__name__ = "SerializationError";
                 class y {
                     constructor(e) {
                         this.value = e
                     }
@@ -4322,15 +4264,15 @@
                     return !1
                 }, t.combinations = y, t.subsets = function*(n) {
                     for (const o of (0, i.range)(n.length + 1)) yield* y(n, o)
                 }
             },
             function _(e, f, r, s, t) {
                 s();
-                const u = e(35),
+                const u = e(34),
                     _ = e(25);
                 class a {
                     constructor(e) {
                         this.buffer = e
                     }
                     to_base64() {
                         return (0, u.buffer_to_base64)(this.buffer)
@@ -4541,15 +4483,15 @@
                     const n = [];
                     return n.push(e.slice(0, t)), n.push(r), n.push(e.slice(t)), n.join("")
                 }
             },
             function _(e, t, s, n, a) {
                 n();
                 const i = e(25),
-                    r = e(31);
+                    r = e(30);
                 class d {
                     constructor(e) {
                         this.document = e
                     }
                     get[Symbol.toStringTag]() {
                         return this.constructor.__name__
                     } [i.equals](e, t) {
@@ -4741,14 +4683,51 @@
                         return `ArrayBuffer(#${t.byteLength})`
                     }
                 }
                 i.Printer = u, u.__name__ = "Printer", i.to_string = function(t, r) {
                     return new u(r).to_string(t)
                 }
             },
+            function _(n, e, t, o, r) {
+                o();
+                const i = n(9),
+                    c = n(8);
+
+                function l(n) {
+                    return (0, c.isObject)(n) && t.clone in n
+                }
+                t.clone = Symbol("clone"), t.is_Cloneable = l;
+                class s extends Error {}
+                t.CloningError = s, s.__name__ = "CloningError";
+                class a {
+                    constructor() {}
+                    clone(n) {
+                        if (l(n)) return n[t.clone](this);
+                        if ((0, c.isPrimitive)(n)) return n;
+                        if ((0, c.isArray)(n)) {
+                            const e = n.length,
+                                t = new Array(e);
+                            for (let o = 0; o < e; o++) {
+                                const e = n[o];
+                                t[o] = this.clone(e)
+                            }
+                            return t
+                        }
+                        if ((0, c.isPlainObject)(n)) {
+                            const e = {};
+                            for (const [t, o] of(0, i.entries)(n)) e[t] = this.clone(o);
+                            return e
+                        }
+                        if (n instanceof Map) return new Map([...n].map((([n, e]) => [this.clone(n), this.clone(e)])));
+                        if (n instanceof Set) return new Set([...n].map((n => this.clone(n))));
+                        throw new s(`${Object.prototype.toString.call(n)} is not cloneable`)
+                    }
+                }
+                t.Cloner = a, a.__name__ = "Cloner"
+            },
             function _(t, r, n, e, o) {
                 e();
                 const s = t(1),
                     u = t(8),
                     c = t(9),
                     l = t(43),
                     i = s.__importStar(t(44));
@@ -4872,15 +4851,15 @@
                 n();
                 const i = e(18),
                     d = e(47),
                     o = e(29),
                     a = e(9),
                     c = e(10),
                     _ = e(26),
-                    u = e(35),
+                    u = e(34),
                     l = e(8),
                     f = e(48),
                     h = new Map;
                 class y extends Error {}
                 t.DeserializationError = y, y.__name__ = "DeserializationError";
                 class p {
                     static register(e, r) {
@@ -5128,15 +5107,15 @@
                 const f = n(8);
                 t.is_ref = function(n) {
                     return (0, f.isPlainObject)(n) && "id" in n && !("type" in n)
                 }
             },
             function _(t, s, e, l, n) {
                 l();
-                const i = t(31);
+                const i = t(30);
                 class c {
                     constructor({
                         start: t,
                         stop: s,
                         step: e
                     } = {}) {
                         this.start = null != t ? t : null, this.stop = null != s ? s : null, this.step = null != e ? e : null
@@ -5362,15 +5341,15 @@
                     var a, _ = arguments.length,
                         l = _ < 3 ? t : null === n ? n = Object.getOwnPropertyDescriptor(t, s) : n;
                     if ("object" == typeof Reflect && "function" == typeof Reflect.decorate) l = Reflect.decorate(e, t, s, n);
                     else
                         for (var o = e.length - 1; o >= 0; o--)(a = e[o]) && (l = (_ < 3 ? a(l) : _ > 3 ? a(t, s, l) : a(t, s)) || l);
                     return _ > 3 && l && Object.defineProperty(t, s, l), l
                 };
-                const U = e(31),
+                const U = e(30),
                     T = e(25),
                     I = e(20);
 
                 function w(e) {
                     return t => {
                         t.prototype.event_name = e
                     }
@@ -5648,17 +5627,14 @@
                 s();
                 const o = t(15),
                     r = t(8);
                 class h {
                     get ready() {
                         return this._ready
                     }* children() {}
-                    mark_finished() {
-                        this._has_finished = !0
-                    }
                     connect(t, e) {
                         let i = this._slots.get(e);
                         return null == i && (i = (t, i) => {
                             const s = Promise.resolve(e.call(this, t, i));
                             this._ready = this._ready.then((() => s)), this.root != this && (this.root._ready = this.root._ready.then((() => this._ready)))
                         }, this._slots.set(e, i)), t.connect(i, this)
                     }
@@ -6457,22 +6433,14 @@
                         return new c({
                             x: t + i,
                             y: e + r,
                             width: n,
                             height: h
                         })
                     }
-                    scale(t) {
-                        return new c({
-                            x0: this.x0 * t,
-                            x1: this.x1 * t,
-                            y0: this.y0 * t,
-                            y1: this.y1 * t
-                        })
-                    }
                     relativize(t, e) {
                         return [t - this.x, e - this.y]
                     }
                     contains(t, e) {
                         return this.x0 <= t && t <= this.x1 && this.y0 <= e && e <= this.y1
                     }
                     clip(t, e) {
@@ -6820,16 +6788,16 @@
                 }
                 n.ClientConnection = d, d.__name__ = "ClientConnection", n.pull_session = function(e, s, n) {
                     return new d(e, s, n).connect()
                 }
             },
             function _(e, s, t, r, n) {
                 r();
-                const i = e(31),
-                    a = e(39),
+                const i = e(30),
+                    a = e(38),
                     h = e(12);
                 class f {
                     get buffers() {
                         return this._buffers
                     }
                     constructor(e, s, t) {
                         this._buffers = new Map, this.header = e, this.metadata = s, this.content = t
@@ -8773,15 +8741,15 @@
             },
             function _(t, i, n, e, a) {
                 var s;
                 e();
                 const l = t(1),
                     _ = t(94),
                     o = t(19),
-                    r = t(33),
+                    r = t(32),
                     d = t(18),
                     h = l.__importStar(t(57)),
                     u = t(95);
                 n.auto_ranged = Symbol("auto_ranged"), n.is_auto_ranged = function(t) {
                     return n.auto_ranged in t
                 };
                 class g extends _.DataRange {
@@ -12435,15 +12403,15 @@
                 var h, o, r;
                 s();
                 const a = t(8),
                     l = t(150),
                     _ = t(21),
                     c = t(151),
                     d = t(152),
-                    u = t(39),
+                    u = t(38),
                     g = t(153),
                     x = t(57),
                     p = t(147),
                     f = t(154);
                 class m extends p.BaseTextView {
                     constructor() {
                         super(...arguments), this._position = {
@@ -14406,15 +14374,15 @@
                 r.TickFormatter = m, m.__name__ = "TickFormatter"
             },
             function _(e, n, s, t, i) {
                 var l, r;
                 t();
                 const c = e(50),
                     o = e(9),
-                    a = e(39),
+                    a = e(38),
                     u = e(8),
                     d = e(23);
                 class _ extends c.Model {
                     constructor(e) {
                         super(e)
                     }
                 }
@@ -14686,15 +14654,15 @@
                 })
             },
             function _(t, e, o, n, r) {
                 var s;
                 n();
                 const i = t(1),
                     c = t(19),
-                    _ = t(33),
+                    _ = t(32),
                     u = t(170),
                     l = t(8),
                     m = t(162),
                     a = t(174),
                     d = i.__importDefault(t(173));
                 o.resolution_order = ["microseconds", "milliseconds", "seconds", "minsec", "minutes", "hourmin", "hours", "days", "months", "years"], o.tm_index_for_resolution = new Map;
                 for (const t of o.resolution_order) o.tm_index_for_resolution.set(t, 0);
@@ -15915,15 +15883,15 @@
                     formatter: () => new o.BasicTickFormatter
                 })
             },
             function _(i, t, e, n, o) {
                 var r;
                 n();
                 const s = i(162),
-                    c = i(39);
+                    c = i(38);
 
                 function _(i) {
                     let t = "";
                     for (const e of i) t += "-" == e ? "\u2212" : e;
                     return t
                 }
                 e.unicode_replace = _;
@@ -16960,16 +16928,16 @@
                     f = e(18),
                     p = e(23),
                     g = e(8),
                     y = e(204),
                     v = e(13),
                     w = e(25),
                     x = e(205),
-                    m = e(96),
-                    b = e(101),
+                    b = e(96),
+                    m = e(101),
                     S = e(208),
                     {
                         abs: z,
                         ceil: $
                     } = Math;
                 class k extends h.View {
                     constructor() {
@@ -17117,15 +17085,15 @@
                             sy1: n
                         } = e, [a, r] = this.renderer.coordinates.x_scale.r_invert(t, s), [o, l] = this.renderer.coordinates.y_scale.r_invert(i, n), _ = [...this.index.indices({
                             x0: a,
                             x1: r,
                             y0: o,
                             y1: l
                         })];
-                        return new b.Selection({
+                        return new m.Selection({
                             indices: _
                         })
                     }
                     _project_data() {}* _iter_visuals() {
                         for (const e of this.visuals)
                             for (const t of e)(t instanceof o.VectorSpec || t instanceof o.ScalarSpec) && (yield t)
                     }
@@ -17170,15 +17138,15 @@
                         this._data_size = t.count;
                         for (const s of this.model)
                             if ((s instanceof o.VectorSpec || s instanceof o.ScalarSpec) && !r.has(s))
                                 if (s instanceof o.BaseCoordinateSpec) {
                                     const i = s.array(e);
                                     let r = t.select(i);
                                     const l = "x" == s.dimension ? n : a;
-                                    if (l instanceof m.FactorRange)
+                                    if (l instanceof b.FactorRange)
                                         if (s instanceof o.CoordinateSpec) r = l.v_synthetic(r);
                                         else if (s instanceof o.CoordinateSeqSpec)
                                         for (let e = 0; e < r.length; e++) r[e] = l.v_synthetic(r[e]);
                                     let _;
                                     _ = s instanceof o.CoordinateSeqSpec ? y.RaggedArray.from(r, Float64Array) : r, this._configure(`_${s.attr}`, {
                                         value: _
                                     })
@@ -17220,15 +17188,15 @@
                                 const n = "x" == e.dimension ? s : i;
                                 let a = t[`_${e.attr}`];
                                 if (a instanceof y.RaggedArray) {
                                     const e = n.v_compute(a.array);
                                     a = new y.RaggedArray(a.offsets, e)
                                 } else a = n.v_compute(a);
                                 this[`s${e.attr}`] = a
-                            } this._map_data(), null === (e = this.glglyph) || void 0 === e || e.set_data_mapped()
+                            } this._map_data(), null === (e = this.glglyph) || void 0 === e || e.set_data_changed()
                     }
                     _map_data() {}
                 }
                 s.GlyphView = k, k.__name__ = "GlyphView";
                 class A extends d.Model {
                     constructor(e) {
                         super(e)
@@ -18352,15 +18320,15 @@
                 e(), i("BasicTickFormatter", t(185).BasicTickFormatter), i("CategoricalTickFormatter", t(166).CategoricalTickFormatter), i("DatetimeTickFormatter", t(169).DatetimeTickFormatter), i("CustomJSTickFormatter", t(223).CustomJSTickFormatter), i("LogTickFormatter", t(187).LogTickFormatter), i("MercatorTickFormatter", t(190).MercatorTickFormatter), i("NumeralTickFormatter", t(224).NumeralTickFormatter), i("PrintfTickFormatter", t(225).PrintfTickFormatter), i("TickFormatter", t(162).TickFormatter)
             },
             function _(t, e, s, n, r) {
                 var c;
                 n();
                 const i = t(162),
                     a = t(9),
-                    o = t(39);
+                    o = t(38);
                 class u extends i.TickFormatter {
                     constructor(t) {
                         super(t)
                     }
                     get names() {
                         return (0, a.keys)(this.args)
                     }
@@ -21120,21 +21088,21 @@
                     a = t(254),
                     c = t(19),
                     h = l.__importStar(t(78)),
                     _ = t(15),
                     d = t(144),
                     u = t(57),
                     b = t(10),
-                    g = t(33),
+                    g = t(32),
                     p = t(8),
                     m = t(151),
                     f = t(229),
                     {
                         max: x,
-                        ceil: w
+                        floor: w
                     } = Math;
                 class y extends f.ContentLayoutable {
                     constructor(t) {
                         super(), this.text = t
                     }
                     _content_size() {
                         return new f.Sizeable(this.text.size())
@@ -22326,15 +22294,15 @@
                 const n = t(1),
                     a = t(18),
                     r = t(56),
                     c = t(59),
                     h = t(260),
                     _ = t(19),
                     u = t(10),
-                    v = t(33),
+                    v = t(32),
                     p = t(9),
                     d = t(8),
                     f = t(267),
                     g = t(268),
                     b = t(269),
                     m = t(274),
                     w = t(276),
@@ -24236,15 +24204,15 @@
             },
             function _(t, o, e, s, n) {
                 var i;
                 s();
                 const l = t(15),
                     r = t(50),
                     c = t(267),
-                    a = t(33);
+                    a = t(32);
                 class u extends r.Model {
                     constructor(t) {
                         super(t)
                     }
                     get underlying() {
                         return this.tools[0]
                     }
@@ -25275,15 +25243,15 @@
             },
             function _(require, module, exports, __esModule, __esExport) {
                 var _a;
                 __esModule();
                 const callback_1 = require(290),
                     object_1 = require(9),
                     array_1 = require(10),
-                    string_1 = require(39),
+                    string_1 = require(38),
                     logging_1 = require(18),
                     types_1 = require(8);
                 class CustomJS extends callback_1.Callback {
                     constructor(t) {
                         super(t), this._state = null
                     }
                     connect_signals() {
@@ -25430,59 +25398,56 @@
                 r(), s("Canvas", a(294).Canvas), s("CartesianFrame", a(157).CartesianFrame)
             },
             function _(e, t, s, i, a) {
                 var r;
                 i();
                 const l = e(1),
                     n = e(28),
-                    h = e(18),
-                    o = e(56),
+                    o = e(18),
+                    h = e(56),
                     _ = e(19),
-                    p = e(295),
-                    c = e(155),
+                    c = e(295),
+                    p = e(155),
                     u = e(263),
                     d = e(260),
                     b = e(56),
                     v = l.__importDefault(e(298));
                 const w = (() => {
                     let t;
                     return async () => void 0 !== t ? t : t = await async function() {
                         const t = document.createElement("canvas"),
                             s = t.getContext("webgl", {
-                                alpha: !0,
-                                antialias: !1,
-                                depth: !1,
                                 premultipliedAlpha: !0
                             });
                         if (null != s) {
-                            const i = await (0, c.load_module)(Promise.resolve().then((() => l.__importStar(e(511)))));
+                            const i = await (0, p.load_module)(Promise.resolve().then((() => l.__importStar(e(511)))));
                             if (null != i) {
                                 const e = i.get_regl(s);
                                 if (e.has_webgl) return {
                                     canvas: t,
                                     regl_wrapper: e
                                 };
-                                h.logger.trace("WebGL is supported, but not the required extensions")
-                            } else h.logger.trace("WebGL is supported, but bokehjs(.min).js bundle is not available")
-                        } else h.logger.trace("WebGL is not supported");
+                                o.logger.trace("WebGL is supported, but not the required extensions")
+                            } else o.logger.trace("WebGL is supported, but bokehjs(.min).js bundle is not available")
+                        } else o.logger.trace("WebGL is not supported");
                         return null
                     }()
                 })();
                 class g extends d.UIElementView {
                     constructor() {
                         super(...arguments), this.webgl = null, this._size = new b.InlineStyleSheet, this.plot_views = []
                     }
                     initialize() {
-                        super.initialize(), this.underlays_el = (0, o.div)({
+                        super.initialize(), this.underlays_el = (0, h.div)({
                             class: "bk-layer"
-                        }), this.primary = this.create_layer(), this.overlays = this.create_layer(), this.overlays_el = (0, o.div)({
+                        }), this.primary = this.create_layer(), this.overlays = this.create_layer(), this.overlays_el = (0, h.div)({
                             class: "bk-layer"
-                        }), this.events_el = (0, o.div)({
+                        }), this.events_el = (0, h.div)({
                             class: ["bk-layer", "bk-events"]
-                        }), this.ui_event_bus = new p.UIEventBus(this)
+                        }), this.ui_event_bus = new c.UIEventBus(this)
                     }
                     get layers() {
                         return [this.underlays_el, this.primary, this.overlays, this.overlays_el, this.events_el]
                     }
                     async lazy_initialize() {
                         if (await super.lazy_initialize(), "webgl" == this.model.output_backend && (this.webgl = await w(), n.settings.force_webgl && null == this.webgl)) throw new Error("webgl is not available")
                     }
@@ -25491,15 +25456,15 @@
                     }
                     stylesheets() {
                         return [...super.stylesheets(), v.default, this._size]
                     }
                     render() {
                         super.render();
                         const e = [this.underlays_el, this.primary.el, this.overlays.el, this.overlays_el, this.events_el];
-                        (0, o.append)(this.shadow_el, ...e)
+                        (0, h.append)(this.shadow_el, ...e)
                     }
                     add_underlay(e) {
                         this.underlays_el.appendChild(e)
                     }
                     add_overlay(e) {
                         this.overlays_el.appendChild(e)
                     }
@@ -25541,26 +25506,26 @@
                         if (null != t) {
                             const {
                                 width: s,
                                 height: i
                             } = this.bbox;
                             t.canvas.width = this.pixel_ratio * s, t.canvas.height = this.pixel_ratio * i;
                             const [a, r, l, n] = e, {
-                                xview: h,
-                                yview: o
-                            } = this.bbox, _ = h.compute(a), p = o.compute(r + n), c = this.pixel_ratio;
-                            t.regl_wrapper.set_scissor(c * _, c * p, c * l, c * n), this._clear_webgl()
+                                xview: o,
+                                yview: h
+                            } = this.bbox, _ = o.compute(a), c = h.compute(r + n), p = this.pixel_ratio;
+                            t.regl_wrapper.set_scissor(p * _, p * c, p * l, p * n), this._clear_webgl()
                         }
                     }
                     blit_webgl(e) {
                         const {
                             webgl: t
                         } = this;
                         if (null != t && t.canvas.width * t.canvas.height > 0) {
-                            if (h.logger.debug("Blitting WebGL canvas"), e.restore(), e.drawImage(t.canvas, 0, 0), e.save(), this.model.hidpi) {
+                            if (o.logger.debug("Blitting WebGL canvas"), e.restore(), e.drawImage(t.canvas, 0, 0), e.save(), this.model.hidpi) {
                                 const t = this.pixel_ratio;
                                 e.scale(t, t), e.translate(.5, .5)
                             }
                             this._clear_webgl()
                         }
                     }
                     _clear_webgl() {
@@ -27115,15 +27080,15 @@
                 var o;
                 t();
                 const a = e(14),
                     c = e(301),
                     i = e(23),
                     u = e(10),
                     l = e(9),
-                    h = e(39),
+                    h = e(38),
                     g = e(8);
                 class v extends c.Expression {
                     constructor(e) {
                         super(e)
                     }
                     connect_signals() {
                         super.connect_signals();
@@ -27392,15 +27357,15 @@
             function _(e, n, r, s, t) {
                 var i;
                 s();
                 const o = e(219),
                     u = e(23),
                     c = e(9),
                     a = e(8),
-                    l = e(39);
+                    l = e(38);
                 class f extends o.Filter {
                     constructor(e) {
                         super(e)
                     }
                     get names() {
                         return (0, c.keys)(this.args)
                     }
@@ -28290,15 +28255,15 @@
                 const n = s(1),
                     d = s(202),
                     h = s(78),
                     c = s(23),
                     _ = s(19),
                     o = n.__importStar(s(210)),
                     u = n.__importStar(s(17)),
-                    l = n.__importStar(s(38)),
+                    l = n.__importStar(s(37)),
                     x = s(13),
                     y = s(101);
                 class m extends d.XYGlyphView {
                     async load_glglyph() {
                         const {
                             CircleGL: i
                         } = await Promise.resolve().then((() => n.__importStar(s(529))));
@@ -28713,15 +28678,15 @@
                 var r;
                 i();
                 const _ = t(1),
                     a = t(203),
                     o = t(209),
                     d = t(101),
                     c = t(78),
-                    h = _.__importStar(t(38)),
+                    h = _.__importStar(t(37)),
                     l = t(13),
                     p = t(10),
                     u = _.__importStar(t(17)),
                     {
                         abs: y,
                         max: f
                     } = Math;
@@ -28844,15 +28809,15 @@
                 s();
                 const a = t(1),
                     _ = t(203),
                     o = t(209),
                     l = t(101),
                     h = t(78),
                     c = t(23),
-                    d = a.__importStar(t(38)),
+                    d = a.__importStar(t(37)),
                     p = t(13),
                     y = t(10),
                     u = a.__importStar(t(17));
                 class f extends _.GlyphView {
                     async lazy_initialize() {
                         await super.lazy_initialize();
                         const {
@@ -29076,15 +29041,15 @@
                             const i = this._x[r],
                                 n = this._y[r];
                             e.add_rect(i - s, n - t, i + s, n + t)
                         }
                     }
                     map_data() {
                         var e;
-                        [this.sx, this.sy] = this.renderer.coordinates.map_to_screen(this._x, this._y), [this.svx, this.svy] = this._get_unscaled_vertices(), null === (e = this.glglyph) || void 0 === e || e.set_data_mapped()
+                        [this.sx, this.sy] = this.renderer.coordinates.map_to_screen(this._x, this._y), [this.svx, this.svy] = this._get_unscaled_vertices(), null === (e = this.glglyph) || void 0 === e || e.set_data_changed()
                     }
                     _get_unscaled_vertices() {
                         const e = this.model.size,
                             t = this.model.aspect_scale;
                         if ("pointytop" == this.model.orientation) {
                             const s = this.renderer.yscale,
                                 i = this.renderer.xscale,
@@ -30646,15 +30611,15 @@
                 var r;
                 i();
                 const a = e(1),
                     _ = e(202),
                     c = e(78),
                     o = a.__importStar(e(210)),
                     h = a.__importStar(e(17)),
-                    l = a.__importStar(e(38)),
+                    l = a.__importStar(e(37)),
                     x = e(10),
                     d = e(101);
                 class y extends _.XYGlyphView {
                     _render(e, t, s) {
                         const {
                             sx: i,
                             sy: n,
@@ -31275,18 +31240,18 @@
             function _(t, e, s, i, a) {
                 var n;
                 i();
                 const r = t(1),
                     o = t(202),
                     l = r.__importStar(t(78)),
                     c = r.__importStar(t(17)),
-                    h = t(38),
+                    h = t(37),
                     _ = t(101),
                     d = t(57),
-                    u = t(33),
+                    u = t(32),
                     x = t(153),
                     f = t(151),
                     g = t(236),
                     p = r.__importStar(t(238)),
                     y = t(237);
                 class b extends c.DataSpec {}
                 b.__name__ = "TextAnchorSpec";
@@ -31589,15 +31554,15 @@
                 var _;
                 s();
                 const r = t(1),
                     a = t(203),
                     o = t(209),
                     d = t(101),
                     c = t(78),
-                    h = r.__importStar(t(38)),
+                    h = r.__importStar(t(37)),
                     x = t(13),
                     l = t(10),
                     p = r.__importStar(t(17)),
                     {
                         abs: u,
                         max: f
                     } = Math;
@@ -31720,15 +31685,15 @@
                 s();
                 const a = t(1),
                     _ = t(203),
                     o = t(209),
                     l = t(101),
                     c = t(78),
                     h = t(23),
-                    d = a.__importStar(t(38)),
+                    d = a.__importStar(t(37)),
                     p = t(13),
                     x = t(10),
                     u = a.__importStar(t(17));
                 class f extends _.GlyphView {
                     async lazy_initialize() {
                         await super.lazy_initialize();
                         const {
@@ -32942,15 +32907,15 @@
                         const r = getComputedStyle(this.el).backgroundColor;
                         s.ctx.fillStyle = r, s.ctx.fillRect(l, n, a, o);
                         for (const i of this.child_views) {
                             const l = i.export(t, e),
                                 {
                                     x: n,
                                     y: a
-                                } = i.bbox.scale(s.pixel_ratio);
+                                } = i.bbox;
                             s.ctx.drawImage(l.canvas, n, a)
                         }
                         return s
                     }
                     serializable_state() {
                         return Object.assign(Object.assign({}, super.serializable_state()), {
                             children: this.child_views.map((t => t.serializable_state()))
@@ -32998,15 +32963,15 @@
                 var n;
                 i();
                 const a = e(1),
                     l = e(260),
                     o = e(369),
                     d = e(19),
                     m = e(59),
-                    u = e(33),
+                    u = e(32),
                     c = a.__importStar(e(271)),
                     h = c;
                 class _ extends l.UIElementView {
                     constructor() {
                         super(...arguments), this.items = new Map
                     }
                     stylesheets() {
@@ -33290,15 +33255,15 @@
                 var o;
                 t();
                 const a = n(367),
                     l = n(370),
                     r = n(236),
                     c = n(56),
                     _ = n(231),
-                    u = n(33),
+                    u = n(32),
                     d = n(8),
                     {
                         max: p
                     } = Math;
                 class g extends a.LayoutDOMView {
                     connect_signals() {
                         super.connect_signals();
@@ -33947,15 +33912,15 @@
                 e(), n("CustomJSTransform", r(391).CustomJSTransform), n("Dodge", r(392).Dodge), n("Interpolator", r(394).Interpolator), n("Jitter", r(395).Jitter), n("LinearInterpolator", r(397).LinearInterpolator), n("StepInterpolator", r(398).StepInterpolator), n("Transform", r(86).Transform)
             },
             function _(r, t, s, n, e) {
                 var a;
                 n();
                 const u = r(86),
                     o = r(9),
-                    m = r(39);
+                    m = r(38);
                 class _ extends u.Transform {
                     constructor(r) {
                         super(r)
                     }
                     get names() {
                         return (0, o.keys)(this.args)
                     }
@@ -34479,15 +34444,15 @@
                     m = e(59),
                     b = e(75),
                     v = e(18),
                     f = e(52),
                     w = e(403),
                     y = e(8),
                     x = e(10),
-                    z = e(33),
+                    z = e(32),
                     k = e(263),
                     S = e(230),
                     M = e(232),
                     $ = e(231),
                     q = e(144),
                     V = e(57),
                     O = e(152),
@@ -34514,17 +34479,14 @@
                     }
                     get state() {
                         return this._state_manager
                     }
                     set invalidate_dataranges(e) {
                         this._range_manager.invalidate_dataranges = e
                     }
-                    get computed_renderer_views() {
-                        return this.computed_renderers.map((e => this.renderer_views.get(e)))
-                    }
                     renderer_view(e) {
                         const t = this.renderer_views.get(e);
                         if (null == t)
                             for (const [, t] of this.renderer_views) {
                                 const i = t.renderer_view(e);
                                 if (null != i) return i
                             }
@@ -35025,20 +34987,15 @@
                         } = this.layout;
                         this._inner_bbox.equals(c) || (this._inner_bbox = c, this._needs_paint = !0), this._needs_paint && this.paint()
                     }
                     repaint() {
                         this._invalidate_layout_if_needed(), this.paint()
                     }
                     paint() {
-                        if (!this.is_paused) {
-                            if (this.is_displayed) v.logger.trace(`${this.toString()}.paint()`), this._actual_paint();
-                            else
-                                for (const e of this.computed_renderer_views) e.mark_finished();
-                            this._needs_notify && (this._needs_notify = !1, this.notify_finished())
-                        }
+                        this.is_paused || (this.model.visible && (v.logger.trace(`${this.toString()}.paint()`), this._actual_paint()), this._needs_notify && (this._needs_notify = !1, this.notify_finished()))
                     }
                     _actual_paint() {
                         var e;
                         const {
                             document: t
                         } = this.model;
                         if (null != t) {
@@ -35576,25 +35533,26 @@
                 class l extends _.GMapPlot {
                     constructor(e) {
                         super(e)
                     }
                 }
                 t.GMap = l, p = l, l.__name__ = "GMap", p.prototype.default_view = i
             },
-            function _(i, o, e, t, s) {
+            function _(i, t, e, o, s) {
                 var l;
-                t();
+                o();
                 const r = i(367),
                     n = i(371),
                     a = i(236),
                     c = i(259),
                     _ = i(277),
-                    d = i(59),
-                    h = i(19);
-                class u extends r.LayoutDOMView {
+                    d = i(263),
+                    h = i(59),
+                    u = i(19);
+                class b extends r.LayoutDOMView {
                     constructor() {
                         super(...arguments), this._tool_views = new Map
                     }
                     get toolbar_view() {
                         return this.child_views.find((i => i.model == this.model.toolbar))
                     }
                     get grid_box_view() {
@@ -35607,57 +35565,57 @@
                             location: i
                         })
                     }
                     initialize() {
                         super.initialize(), this._update_location();
                         const {
                             children: i,
-                            rows: o,
+                            rows: t,
                             cols: e,
-                            spacing: t
+                            spacing: o
                         } = this.model;
                         this._grid_box = new n.GridBox({
                             children: i,
-                            rows: o,
+                            rows: t,
                             cols: e,
-                            spacing: t,
+                            spacing: o,
                             sizing_mode: "inherit"
                         })
                     }
                     async lazy_initialize() {
                         await super.lazy_initialize(), await this.build_tool_views()
                     }
                     connect_signals() {
                         super.connect_signals();
                         const {
                             toolbar: i,
-                            toolbar_location: o,
+                            toolbar_location: t,
                             children: e,
-                            rows: t,
+                            rows: o,
                             cols: s,
                             spacing: l
                         } = this.model.properties;
-                        this.on_change(o, (() => {
+                        this.on_change(t, (() => {
                             this._update_location(), this.rebuild()
-                        })), this.on_change([i, e, t, s, l], (() => {
+                        })), this.on_change([i, e, o, s, l], (() => {
                             this.rebuild()
                         })), this.on_change(this.model.toolbar.properties.tools, (async () => {
                             await this.build_tool_views()
                         })), this.mouseenter.connect((() => {
                             this.toolbar_view.set_visibility(!0)
                         })), this.mouseleave.connect((() => {
                             this.toolbar_view.set_visibility(!1)
                         }))
                     }
                     remove() {
-                        (0, d.remove_views)(this._tool_views), super.remove()
+                        (0, h.remove_views)(this._tool_views), super.remove()
                     }
                     async build_tool_views() {
                         const i = this.model.toolbar.tools.filter((i => i instanceof _.ActionTool));
-                        await (0, d.build_views)(this._tool_views, i, {
+                        await (0, h.build_views)(this._tool_views, i, {
                             parent: this
                         })
                     }* children() {
                         yield* super.children(), yield* this._tool_views.values()
                     }
                     get child_models() {
                         return [this.model.toolbar, this._grid_box]
@@ -35668,44 +35626,74 @@
                             outer: "flex"
                         }
                     }
                     _update_layout() {
                         super._update_layout();
                         const {
                             location: i
-                        } = this.model.toolbar, o = (() => {
+                        } = this.model.toolbar, t = (() => {
                             switch (i) {
                                 case "above":
                                     return "column";
                                 case "below":
                                     return "column-reverse";
                                 case "left":
                                     return "row";
                                 case "right":
                                     return "row-reverse"
                             }
                         })();
                         this.style.append(":host", {
-                            flex_direction: o
+                            flex_direction: t
                         })
                     }
+                    export (i = "auto", t = !0) {
+                        const e = (() => {
+                                switch (i) {
+                                    case "auto":
+                                    case "png":
+                                        return "canvas";
+                                    case "svg":
+                                        return "svg"
+                                }
+                            })(),
+                            o = new d.CanvasLayer(e, t),
+                            {
+                                x: s,
+                                y: l,
+                                width: r,
+                                height: n
+                            } = this.grid_box_view.bbox.relative();
+                        o.resize(r, n), o.ctx.save();
+                        const a = getComputedStyle(this.el).backgroundColor;
+                        o.ctx.fillStyle = a, o.ctx.fillRect(s, l, r, n);
+                        for (const e of this.child_views) {
+                            const s = e.export(i, t),
+                                {
+                                    x: l,
+                                    y: r
+                                } = e.bbox;
+                            o.ctx.drawImage(s.canvas, l, r)
+                        }
+                        return o.ctx.restore(), o
+                    }
                 }
-                e.GridPlotView = u, u.__name__ = "GridPlotView";
-                class b extends r.LayoutDOM {
+                e.GridPlotView = b, b.__name__ = "GridPlotView";
+                class w extends r.LayoutDOM {
                     constructor(i) {
                         super(i)
                     }
                 }
-                e.GridPlot = b, l = b, b.__name__ = "GridPlot", l.prototype.default_view = u, l.define((({
+                e.GridPlot = w, l = w, w.__name__ = "GridPlot", l.prototype.default_view = b, l.define((({
                     Array: i,
-                    Ref: o,
+                    Ref: t,
                     Nullable: e
                 }) => ({
-                    toolbar: [o(c.Toolbar), () => new c.Toolbar],
-                    toolbar_location: [e(h.Location), "above"],
+                    toolbar: [t(c.Toolbar), () => new c.Toolbar],
+                    toolbar_location: [e(u.Location), "above"],
                     children: [i((0, a.GridChild)(r.LayoutDOM)), []],
                     rows: [e(a.TracksSizing), null],
                     cols: [e(a.TracksSizing), null],
                     spacing: [a.GridSpacing, 0]
                 })))
             },
             function _(e, t, s, i, a) {
@@ -36574,42 +36562,34 @@
                 r.QUADKEYTileSource = c, c.__name__ = "QUADKEYTileSource"
             },
             function _(t, e, i, s, _) {
                 var n;
                 s();
                 const a = t(1),
                     h = t(432),
-                    r = t(436),
-                    o = t(74),
+                    o = t(436),
+                    r = t(74),
                     l = t(88),
                     d = t(56),
                     m = t(150),
                     c = t(10),
                     u = t(8),
-                    p = t(12),
-                    b = a.__importDefault(t(437));
-                class g extends o.RendererView {
-                    constructor() {
-                        super(...arguments), this._tiles = null
-                    }
-                    mark_finished() {
-                        super.mark_finished(), this._tiles = []
+                    p = a.__importDefault(t(437));
+                class g extends r.RendererView {
+                    initialize() {
+                        this._tiles = [], super.initialize()
                     }
                     connect_signals() {
                         super.connect_signals(), this.connect(this.model.change, (() => this.request_render())), this.connect(this.model.tile_source.change, (() => this.request_render()))
                     }
                     remove() {
                         null != this.attribution_el && (0, d.remove)(this.attribution_el), super.remove()
                     }
                     get_extent() {
-                        const {
-                            x_range: t,
-                            y_range: e
-                        } = this, i = t.start, s = e.start, _ = t.end, n = e.end;
-                        return (0, p.assert)(isFinite(i)), (0, p.assert)(isFinite(s)), (0, p.assert)(isFinite(_)), (0, p.assert)(isFinite(n)), [i, s, _, n]
+                        return [this.x_range.start, this.y_range.start, this.x_range.end, this.y_range.end]
                     }
                     get map_plot() {
                         return this.plot_model
                     }
                     get map_canvas() {
                         return this.layer.ctx
                     }
@@ -36643,40 +36623,40 @@
                                 }
                             });
                             const a = (0, d.div)();
                             a.innerHTML = t;
                             const h = this.attribution_el.attachShadow({
                                 mode: "open"
                             });
-                            new d.InlineStyleSheet(b.default).install(h), h.appendChild(a), this.attribution_el.title = a.textContent.replace(/\s*\n\s*/g, " "), this.plot_view.canvas_view.add_event(this.attribution_el)
+                            new d.InlineStyleSheet(p.default).install(h), h.appendChild(a), this.attribution_el.title = a.textContent.replace(/\s*\n\s*/g, " "), this.plot_view.canvas_view.add_event(this.attribution_el)
                         }
                     }
                     _map_data() {
                         this.initial_extent = this.get_extent();
                         const t = this.model.tile_source.get_level_by_extent(this.initial_extent, this.map_frame.bbox.height, this.map_frame.bbox.width),
                             e = this.model.tile_source.snap_to_zoom_level(this.initial_extent, this.map_frame.bbox.height, this.map_frame.bbox.width, t);
                         this.x_range.start = e[0], this.y_range.start = e[1], this.x_range.end = e[2], this.y_range.end = e[3], this.x_range instanceof l.Range1d && (this.x_range.reset_start = e[0], this.x_range.reset_end = e[2]), this.y_range instanceof l.Range1d && (this.y_range.reset_start = e[1], this.y_range.reset_end = e[3]), this._update_attribution()
                     }
                     _create_tile(t, e, i, s, _ = !1) {
                         const n = this.model.tile_source.tile_xyz_to_quadkey(t, e, i),
                             a = this.model.tile_source.tile_xyz_to_key(t, e, i);
                         if (this.model.tile_source.tiles.has(a)) return;
-                        const [h, r, o] = this.model.tile_source.normalize_xyz(t, e, i), l = this.model.tile_source.get_image_url(h, r, o), d = {
+                        const [h, o, r] = this.model.tile_source.normalize_xyz(t, e, i), l = this.model.tile_source.get_image_url(h, o, r), d = {
                             img: void 0,
                             tile_coords: [t, e, i],
-                            normalized_coords: [h, r, o],
+                            normalized_coords: [h, o, r],
                             quadkey: n,
                             cache_key: a,
                             bounds: s,
                             loaded: !1,
                             finished: !1,
                             x_coord: s[0],
                             y_coord: s[3]
                         };
-                        this.model.tile_source.tiles.set(a, d), null == this._tiles && (this._tiles = []), this._tiles.push(d), new m.ImageLoader(l, {
+                        this.model.tile_source.tiles.set(a, d), this._tiles.push(d), new m.ImageLoader(l, {
                             loaded: t => {
                                 Object.assign(d, {
                                     img: t,
                                     loaded: !0
                                 }), _ ? (d.finished = !0, this.notify_finished()) : this.request_render()
                             },
                             failed() {
@@ -36696,15 +36676,15 @@
                                 start: i[1],
                                 end: i[3]
                             }), this.extent = i, this._last_height = this.map_frame.bbox.height, this._last_width = this.map_frame.bbox.width
                         }
                     }
                     has_finished() {
                         if (!super.has_finished()) return !1;
-                        if (null == this._tiles) return !1;
+                        if (0 == this._tiles.length) return !1;
                         for (const t of this._tiles)
                             if (!t.finished) return !1;
                         return !0
                     }
                     _render() {
                         null == this.map_initialized && (this._set_data(), this._map_data(), this.map_initialized = !0), this._enforce_aspect_ratio(), this._update(), null != this.prefetch_timer && clearTimeout(this.prefetch_timer), this.prefetch_timer = setTimeout(this._prefetch_tiles.bind(this), 500), this.has_finished() && this.notify_finished()
                     }
@@ -36713,16 +36693,16 @@
                         if (null != e && e.loaded) {
                             const [
                                 [t],
                                 [i]
                             ] = this.coordinates.map_to_screen([e.bounds[0]], [e.bounds[3]]), [
                                 [s],
                                 [_]
-                            ] = this.coordinates.map_to_screen([e.bounds[2]], [e.bounds[1]]), n = s - t, a = _ - i, h = t, r = i, o = this.map_canvas.imageSmoothingEnabled;
-                            this.map_canvas.imageSmoothingEnabled = this.model.smoothing, this.map_canvas.drawImage(e.img, h, r, n, a), this.map_canvas.imageSmoothingEnabled = o, e.finished = !0
+                            ] = this.coordinates.map_to_screen([e.bounds[2]], [e.bounds[1]]), n = s - t, a = _ - i, h = t, o = i, r = this.map_canvas.imageSmoothingEnabled;
+                            this.map_canvas.imageSmoothingEnabled = this.model.smoothing, this.map_canvas.drawImage(e.img, h, o, n, a), this.map_canvas.imageSmoothingEnabled = r, e.finished = !0
                         }
                     }
                     _set_rect() {
                         const t = this.plot_model.outline_line_width,
                             e = this.map_frame.bbox.left + t / 2,
                             i = this.map_frame.bbox.top + t / 2,
                             s = this.map_frame.bbox.width - t,
@@ -36761,59 +36741,59 @@
                             max_zoom: i
                         } = t;
                         let s = this.get_extent();
                         const _ = this.extent[2] - this.extent[0] < s[2] - s[0],
                             n = this.map_frame.bbox.height,
                             a = this.map_frame.bbox.width;
                         let h = t.get_level_by_extent(s, n, a),
-                            r = !1;
-                        h < e ? (s = this.extent, h = e, r = !0) : h > i && (s = this.extent, h = i, r = !0), r && (this.x_range.setv({
+                            o = !1;
+                        h < e ? (s = this.extent, h = e, o = !0) : h > i && (s = this.extent, h = i, o = !0), o && (this.x_range.setv({
                             start: s[0],
                             end: s[2]
                         }), this.y_range.setv({
                             start: s[1],
                             end: s[3]
                         })), this.extent = s;
-                        const o = t.get_tiles_by_extent(s, h),
+                        const r = t.get_tiles_by_extent(s, h),
                             l = [],
                             d = [],
                             m = [],
                             u = [];
-                        for (const e of o) {
+                        for (const e of r) {
                             const [i, s, n] = e, a = t.tile_xyz_to_key(i, s, n), h = t.tiles.get(a);
                             if (null != h && h.loaded) d.push(a);
                             else if (this.model.render_parents) {
-                                const [e, a, h] = t.get_closest_parent_by_tile_xyz(i, s, n), r = t.tile_xyz_to_key(e, a, h), o = t.tiles.get(r);
-                                if (null != o && o.loaded && !(0, c.includes)(m, r) && m.push(r), _) {
+                                const [e, a, h] = t.get_closest_parent_by_tile_xyz(i, s, n), o = t.tile_xyz_to_key(e, a, h), r = t.tiles.get(o);
+                                if (null != r && r.loaded && !(0, c.includes)(m, o) && m.push(o), _) {
                                     const e = t.children_by_tile_xyz(i, s, n);
                                     for (const [i, s, _] of e) {
                                         const e = t.tile_xyz_to_key(i, s, _);
                                         t.tiles.has(e) && u.push(e)
                                     }
                                 }
                             }
                             null == h && l.push(e)
                         }
                         this._render_tiles(m), this._render_tiles(u), this._render_tiles(d), null != this.render_timer && clearTimeout(this.render_timer), this.render_timer = setTimeout((() => this._fetch_tiles(l)), 65)
                     }
                 }
                 i.TileRendererView = g, g.__name__ = "TileRendererView";
-                class f extends o.Renderer {
+                class b extends r.Renderer {
                     constructor(t) {
                         super(t)
                     }
                 }
-                i.TileRenderer = f, n = f, f.__name__ = "TileRenderer", n.prototype.default_view = g, n.define((({
+                i.TileRenderer = b, n = b, b.__name__ = "TileRenderer", n.prototype.default_view = g, n.define((({
                     Boolean: t,
                     Number: e,
                     Ref: i
                 }) => ({
                     alpha: [e, 1],
                     smoothing: [t, !0],
-                    tile_source: [i(h.TileSource), () => new r.WMTSTileSource],
+                    tile_source: [i(h.TileSource), () => new o.WMTSTileSource],
                     render_parents: [t, !0]
                 }))), n.override({
                     level: "image"
                 })
             },
             function _(t, e, r, o, s) {
                 o();
@@ -36849,15 +36829,15 @@
             function _(e, t, u, a, r) {
                 a(), r("CanvasTexture", e(440).CanvasTexture), r("ImageURLTexture", e(442).ImageURLTexture), r("Texture", e(441).Texture)
             },
             function _(t, e, n, c, s) {
                 var r;
                 c();
                 const o = t(441),
-                    a = t(39);
+                    a = t(38);
                 class u extends o.Texture {
                     constructor(t) {
                         super(t)
                     }
                     get func() {
                         const t = (0, a.use_strict)(this.code);
                         return new Function("ctx", "color", "scale", "weight", t)
@@ -37173,22 +37153,22 @@
                 var i;
                 n();
                 const a = t(1),
                     l = t(260),
                     r = a.__importStar(t(17)),
                     c = t(14),
                     d = t(56),
-                    p = t(41),
+                    p = t(40),
                     h = t(50),
                     u = t(8),
                     f = t(9),
                     _ = t(10),
-                    v = t(33),
+                    v = t(32),
                     g = t(15),
-                    m = t(37),
+                    m = t(36),
                     b = a.__importDefault(t(453));
                 class y {
                     constructor(t, e, s) {
                         this.visited = new WeakSet, this.depth = 0, this.click = t, this.max_items = e, this.max_depth = s
                     }
                     to_html(t) {
                         if ((0, u.isObject)(t)) {
@@ -40813,15 +40793,15 @@
                 }))), n.register_alias("crosshair", (() => new p))
             },
             function _(e, s, t, r, n) {
                 var o;
                 r();
                 const a = e(50),
                     u = e(9),
-                    c = e(39);
+                    c = e(38);
                 class i extends a.Model {
                     constructor(e) {
                         super(e)
                     }
                     get values() {
                         return (0, u.values)(this.args)
                     }
@@ -40848,15 +40828,15 @@
                     l = e(59),
                     a = e(56),
                     c = e(19),
                     _ = r.__importStar(e(210)),
                     d = e(15),
                     p = e(12),
                     u = e(21),
-                    h = e(33),
+                    h = e(32),
                     m = e(9),
                     y = e(170),
                     f = e(8),
                     v = e(272),
                     x = r.__importStar(e(457)),
                     w = e(455),
                     g = e(499),
@@ -41653,15 +41633,15 @@
                 t.Index = a, o = a, a.__name__ = "Index", o.prototype.default_view = _
             },
             function _(e, o, r, t, n) {
                 var s;
                 t();
                 const u = e(501),
                     i = e(74),
-                    p = e(33);
+                    p = e(32);
                 class g extends u.ActionView {
                     update(e, o, r) {
                         for (const [e, r] of(0, p.enumerate)(this.model.groups)) e.visible = o == r
                     }
                 }
                 r.ToggleGroupView = g, g.__name__ = "ToggleGroupView";
                 class _ extends u.Action {
@@ -41678,15 +41658,15 @@
             },
             function _(e, t, n, s, o) {
                 var r;
                 s();
                 const i = e(449),
                     a = e(14),
                     l = e(56),
-                    c = e(41);
+                    c = e(40);
                 class p extends i.DOMNodeView {
                     connect_signals() {
                         super.connect_signals();
                         const {
                             obj: e,
                             attr: t
                         } = this.model;
@@ -41749,26 +41729,26 @@
             "core/types": 23,
             "core/util/bitset": 24,
             "core/util/eq": 25,
             "core/util/platform": 26,
             "core/vectorization": 27,
             "core/settings": 28,
             "core/util/ndarray": 29,
-            "core/util/cloneable": 30,
-            "core/serialization/index": 31,
-            "core/serialization/serializer": 32,
-            "core/util/iterator": 33,
-            "core/serialization/buffer": 34,
-            "core/util/buffer": 35,
-            "core/serialization/reps": 36,
-            "core/diagnostics": 37,
-            "core/uniforms": 38,
-            "core/util/string": 39,
-            "document/events": 40,
-            "core/util/pretty": 41,
+            "core/serialization/index": 30,
+            "core/serialization/serializer": 31,
+            "core/util/iterator": 32,
+            "core/serialization/buffer": 33,
+            "core/util/buffer": 34,
+            "core/serialization/reps": 35,
+            "core/diagnostics": 36,
+            "core/uniforms": 37,
+            "core/util/string": 38,
+            "document/events": 39,
+            "core/util/pretty": 40,
+            "core/util/cloneable": 41,
             "core/patching": 42,
             "core/util/set": 43,
             "core/util/typed_array": 44,
             "core/resolvers": 45,
             "core/serialization/deserializer": 46,
             "core/util/refs": 47,
             "core/util/slice": 48,
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/compiler.js` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/compiler.js`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/charts.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/charts.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/figure.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/figure.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/glyph_api.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/glyph_api.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/gridplot.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/gridplot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/io.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/io.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/linalg.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/linalg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/palettes.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/palettes.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/parser.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/parser.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/api/themes.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/api/themes.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/client/connection.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/client/connection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/client/session.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/client/session.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/bokeh_events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/build_views.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/build_views.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/css.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/css.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/dom.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/dom_view.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/dom_view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/enums.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/enums.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/geometry.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/geometry.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/graphics.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/graphics.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/has_props.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/has_props.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/hittest.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/hittest.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/kinds.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/kinds.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/alignments.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/border.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/border.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/grid.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/grid.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/layoutable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/side_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/layout/types.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/layout/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/logging.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/logging.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/patching.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/patching.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/properties.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/properties.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/property_mixins.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/property_mixins.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/selection_manager.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/selection_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/deserializer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/reps.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/serialization/serializer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/signaling.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/signaling.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/types.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/ui_events.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/ui_events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/uniforms.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/uniforms.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/affine.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/affine.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/algorithms.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/array.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/arrayable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/bbox.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/bbox.d.ts`

 * *Files 5% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     get aspect(): number;
     get hcenter(): number;
     get vcenter(): number;
     get area(): number;
     round(): BBox;
     relative(): BBox;
     translate(tx: number, ty: number): BBox;
-    scale(factor: number): BBox;
     relativize(x: number, y: number): [number, number];
     contains(x: number, y: number): boolean;
     clip(x: number, y: number): [number, number];
     grow_by(size: number): BBox;
     shrink_by(size: number): BBox;
     union(that: Rect): BBox;
     intersection(that: Rect): BBox | null;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/bitset.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/bitset.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/canvas.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/cloneable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/color.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/color.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/eq.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/eq.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/image.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/iterator.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/iterator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/math.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/math.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/matrix.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/matrix.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/menus.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/menus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/ndarray.d.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import type { NDDataType, Arrayable } from "../types";
 import type { Equatable, Comparator } from "./eq";
 import { equals } from "./eq";
-import type { Cloner, Cloneable } from "./cloneable";
-import { clone } from "./cloneable";
 import type { Serializable, Serializer } from "../serialization";
 import { serialize } from "../serialization";
 declare const __ndarray__: unique symbol;
-export interface NDArrayType<T, U = T> extends Arrayable<U>, Equatable, Cloneable, Serializable {
+export interface NDArrayType<T, U = T> extends Arrayable<U>, Equatable, Serializable {
     readonly [__ndarray__]: boolean;
     readonly dtype: NDDataType;
     readonly shape: number[];
     readonly dimension: number;
     get(i: number): T;
     [i: number]: U;
 }
@@ -18,115 +16,105 @@
 export declare class BoolNDArray extends Uint8Array implements NDArrayType<boolean, number> {
     readonly [__ndarray__] = true;
     readonly dtype: "bool";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): boolean;
 }
 export declare class Uint8NDArray extends Uint8Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "uint8";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class Int8NDArray extends Int8Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "int8";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class Uint16NDArray extends Uint16Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "uint16";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class Int16NDArray extends Int16Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "int16";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class Uint32NDArray extends Uint32Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "uint32";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class Int32NDArray extends Int32Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "int32";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class Float32NDArray extends Float32Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "float32";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class Float64NDArray extends Float64Array implements NDArrayType<number> {
     readonly [__ndarray__] = true;
     readonly dtype: "float64";
     readonly shape: number[];
     readonly dimension: number;
     constructor(init: Init<number>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): number;
 }
 export declare class ObjectNDArray<T = unknown> extends Array<T> implements NDArrayType<T> {
     readonly [__ndarray__] = true;
     readonly dtype: "object";
     private _shape?;
     get shape(): number[];
     get dimension(): number;
     constructor(init_: Init<T>, shape?: number[]);
     [equals](that: this, cmp: Comparator): boolean;
-    [clone](cloner: Cloner): this;
     [serialize](serializer: Serializer): unknown;
     get(i: number): T;
 }
 export type NDArray = BoolNDArray | Uint8NDArray | Int8NDArray | Uint16NDArray | Int16NDArray | Uint32NDArray | Int32NDArray | Float32NDArray | Float64NDArray | ObjectNDArray;
 export declare function is_NDArray(v: unknown): v is NDArray;
 export type NDArrayTypes = {
     bool: {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/object.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/pretty.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/pretty.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/projections.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/projections.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/ragged_array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/random.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/random.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/svg.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/svg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/svg_colors.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/templating.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/templating.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/text.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/types.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/util/zoom.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/util/zoom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/vectorization.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/vectorization.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/view.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/view.d.ts`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     readonly parent: View | null;
     readonly root: View;
     readonly owner: ViewManager;
     protected _ready: Promise<void>;
     get ready(): Promise<void>;
     children(): IterViews;
     protected _has_finished: boolean;
-    mark_finished(): void;
     connect<Args, Sender extends object>(signal: Signal<Args, Sender>, slot: Slot<Args, Sender>): boolean;
     disconnect<Args, Sender extends object>(signal: Signal<Args, Sender>, slot: Slot<Args, Sender>): boolean;
     constructor(options: View.Options);
     initialize(): void;
     lazy_initialize(): Promise<void>;
     protected _removed: boolean;
     remove(): void;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/fill.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/hatch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/image.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/line.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/text.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/core/visuals/visual.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/document/defs.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/defs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/document/document.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/document.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/document/events.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/document/events.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/embed/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/embed/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/model.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/model.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/arrow.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/arrow_head.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/band.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/band.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/base_color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/box_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/contour_color_bar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/data_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/label.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/label_set.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/text_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/html/title.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/label.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/label.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/label_set.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/legend.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/legend_item.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/poly_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/slope.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/span.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/span.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/text_annotation.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/title.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/title.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/toolbar_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/upper_lower.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/annotations/whisker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/axis.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/categorical_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/continuous_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/datetime_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/linear_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/log_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/axes/mercator_axis.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/callback.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/customjs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/open_url.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/callbacks/set_value.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/canvas/canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/canvas/cartesian_frame.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/common/kinds.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/common/kinds.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/common/resolve.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/common/resolve.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/coordinates/coordinate_mapping.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/action.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/color_ref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/dom_element.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/dom_node.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/elements.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/elements.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/html.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/html.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/index_.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/index_.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/placeholder.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/styles.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/styles.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/stylesheets.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/template.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/template.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/text.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/toggle_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/value_of.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/dom/value_ref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/coordinate_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/cumsum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/customjs_expr.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/expression.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/maximum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/minimum.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/polar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/expressions/stack.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/all_indices.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/boolean_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/customjs_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/difference_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/group_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/index_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/intersection_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/inversion_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/symmetric_difference_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/filters/union_filter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/basic_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/categorical_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/customjs_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/datetime_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/log_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/mercator_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/numeral_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/printf_tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/formatters/tick_formatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/annular_wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/annulus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/arc.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/area.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/bezier.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/block.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/center_rotatable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/circle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/ellipse.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/glyph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/harea.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/harea_step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hex_tile.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hspan.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/hstrip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_base.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_rgba.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_stack.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/image_url.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/lrtb.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/multi_line.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/multi_polygons.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/patch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/patches.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/quad.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/quadratic.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/ray.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/rect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/scatter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/segment.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/spline.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/utils.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/varea.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/varea_step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/vbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/vspan.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/vstrip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annular_wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/annulus.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base.d.ts`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 };
 export declare abstract class BaseGLGlyph {
     protected readonly regl_wrapper: ReglWrapper;
     readonly glyph: GlyphView;
     protected nvertices: number;
     protected size_changed: boolean;
     protected data_changed: boolean;
-    protected data_mapped: boolean;
     protected visuals_changed: boolean;
     constructor(regl_wrapper: ReglWrapper, glyph: GlyphView);
     set_data_changed(): void;
-    set_data_mapped(): void;
     set_visuals_changed(): void;
     render(_ctx: Context2d, indices: number[], mainglyph: GlyphView): void;
     abstract draw(indices: number[], mainglyph: GlyphView, trans: Transform): void;
 }
 export type Transform = {
     pixel_ratio: number;
     width: number;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_line.d.ts`

 * *Files 12% similar despite different names*

```diff
@@ -25,12 +25,12 @@
     protected _dash_offset?: number;
     constructor(regl_wrapper: ReglWrapper, glyph: GlyphView);
     abstract draw(_indices: number[], main_glyph: GlyphView, transform: Transform): void;
     protected _draw_impl(indices: number[], transform: Transform, main_gl_glyph: BaseLineGL): void;
     protected abstract _get_show_buffer(indices: number[], main_gl_glyph: BaseLineGL): Uint8Buffer;
     protected abstract _get_visuals(): LineGLVisuals;
     protected _is_dashed(): boolean;
-    protected _set_data(data_changed: boolean): void;
+    protected _set_data(): void;
     protected abstract _set_data_points(): Float32Array;
     protected _set_visuals(): void;
 }
 //# sourceMappingURL=base_line.d.ts.map
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/base_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/buffer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/circle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/dash_cache.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/line_gl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/lrtb.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/multi_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/regl_wrap.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/single_marker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/step.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/sxsy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/types.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/webgl_utils.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/webgl/wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/wedge.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/glyphs/xy_glyph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphics/decoration.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphics/marking.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/graph_hit_test_policy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/layout_provider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/graphs/static_layout_provider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/grids/grid.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/grids/grid.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/alignments.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/column.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/column.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/css_grid_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/flex_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/grid_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/group_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/hbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/layout_dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/row.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/row.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/scroll_box.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/spacer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/tab_panel.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/tabs.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/layouts/vbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_marker_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/categorical_pattern_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/continuous_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/eqhist_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/linear_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/log_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/scanning_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/mappers/weighted_stack_color_mapper.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/action.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/check_action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/divider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/divider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/menu.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/menu.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/menu_item.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/menus/section.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/menus/section.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/figure.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/figure.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/gmap.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/gmap_plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/gmap_plot_canvas.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/grid_plot.d.ts`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import { LayoutDOM, LayoutDOMView } from "../layouts/layout_dom";
 import type { GridBoxView } from "../layouts/grid_box";
 import { GridBox } from "../layouts/grid_box";
 import { TracksSizing } from "../common/kinds";
 import type { ToolbarView } from "../tools/toolbar";
 import { Toolbar } from "../tools/toolbar";
 import type { UIElement } from "../ui/ui_element";
+import { CanvasLayer } from "../../core/util/canvas";
 import type { IterViews } from "../../core/build_views";
 import { Location } from "../../core/enums";
 import type * as p from "../../core/properties";
 export declare class GridPlotView extends LayoutDOMView {
     model: GridPlot;
     protected _grid_box: GridBox;
     get toolbar_view(): ToolbarView;
@@ -21,14 +22,15 @@
     remove(): void;
     private readonly _tool_views;
     build_tool_views(): Promise<void>;
     children(): IterViews;
     get child_models(): UIElement[];
     protected _intrinsic_display(): FullDisplay;
     _update_layout(): void;
+    export(type?: "auto" | "png" | "svg", hidpi?: boolean): CanvasLayer;
 }
 export declare namespace GridPlot {
     type Attrs = p.AttrsOf<Props>;
     type Props = LayoutDOM.Props & {
         toolbar: p.Property<Toolbar>;
         toolbar_location: p.Property<Location | null>;
         children: p.Property<[LayoutDOM, number, number, number?, number?][]>;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/plot.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/plot.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/plot_canvas.d.ts`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     get state(): StateManager;
     set invalidate_dataranges(value: boolean);
     protected _is_paused?: number;
     protected lod_started: boolean;
     protected _initial_state: StateInfo;
     protected throttled_paint: () => void;
     computed_renderers: Renderer[];
-    get computed_renderer_views(): RendererView[];
     renderer_view<T extends Renderer>(renderer: T): T["__view_type__"] | undefined;
     get auto_ranged_renderers(): (RendererView & AutoRanged)[];
     get base_font_size(): number | null;
     readonly renderer_views: ViewStorage<Renderer>;
     readonly tool_views: ViewStorage<Tool>;
     children(): IterViews;
     get is_paused(): boolean;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/range_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/plots/state_manager.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/policies/labeling.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/random/park_miller_lcg.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/random/random_generator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/data_range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/data_range1d.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/factor_range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/range.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/range.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ranges/range1d.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/contour_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/data_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/glyph_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/graph_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/guide_renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/renderers/renderer.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/categorical_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/linear_interpolation_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/linear_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/log_scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/scales/scale.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/scales/scale.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selections/interaction_policy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selections/selection.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selections/selection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/selectors/selector.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/ajax_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/cds_view.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/column_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/columnar_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/geojson_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/server_sent_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/sources/web_data_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/base_text.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/base_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/math_text.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/math_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/plain_text.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/text/providers.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/text/providers.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/canvas_texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/image_url_texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/textures/texture.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/textures/texture.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/adaptive_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/binned_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/categorical_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/composite_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/continuous_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/days_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/fixed_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/log_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/mercator_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/months_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/single_interval_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tickers/years_ticker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/bbox_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/mercator_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/quadkey_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/tile_renderer.d.ts`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     bounds: Bounds;
     finished: boolean;
     x_coord: number;
     y_coord: number;
 };
 export declare class TileRendererView extends RendererView {
     model: TileRenderer;
-    protected _tiles: TileData[] | null;
+    protected _tiles: TileData[];
     protected extent: Extent;
     protected initial_extent: Extent;
     protected _last_height?: number;
     protected _last_width?: number;
     protected map_initialized?: boolean;
     protected render_timer?: number;
     protected prefetch_timer?: number;
     protected attribution_el?: HTMLElement;
-    mark_finished(): void;
+    initialize(): void;
     connect_signals(): void;
     remove(): void;
     get_extent(): Extent;
     private get map_plot();
     private get map_canvas();
     private get map_frame();
     private get x_range();
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/tms_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tiles/wmts_tile_source.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/action_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/copy_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/custom_action.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/examine_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/fullscreen_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/help_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/plot_action_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/redo_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/reset_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/save_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/undo_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_base_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_in_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/actions/zoom_out_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/click_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/box_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/freehand_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/line_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/line_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/point_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/poly_draw_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/poly_edit_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/edit/poly_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/box_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/box_zoom_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/gesture_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/lasso_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/pan_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/poly_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/range_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/region_select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/select_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/tap_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_pan_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/gestures/wheel_zoom_tool.d.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import { GestureTool, GestureToolView } from "./gesture_tool";
 import type * as p from "../../../core/properties";
 import type { PinchEvent, ScrollEvent } from "../../../core/ui_events";
 import { Dimensions } from "../../../core/enums";
-declare const ZoomTogether: import("../../../core/kinds").Kinds.Enum<"none" | "all" | "cross">;
+declare const ZoomTogether: import("core/kinds").Kinds.Enum<"none" | "all" | "cross">;
 type ZoomTogether = typeof ZoomTogether["__type__"];
 export declare class WheelZoomToolView extends GestureToolView {
     model: WheelZoomTool;
     _pinch(ev: PinchEvent): void;
     _scroll(ev: ScrollEvent): void;
 }
 export declare namespace WheelZoomTool {
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/crosshair_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/customjs_hover.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/hover_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/inspectors/inspect_tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/on_off_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/tool.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/tool.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/tool_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/tool_proxy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/tools/toolbar.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/customjs_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/jitter.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/linear_interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/range_transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/step_interpolator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/transforms/transform.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/dialog.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/examiner.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/builtin_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/svg_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/icons/tabler_icon.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/pane.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/pane.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/tooltip.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/ui/ui_element.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/abstract_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/abstract_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/autocomplete_input.d.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import { TextInput, TextInputView } from "./text_input";
 import type { StyleSheetLike } from "../../core/dom";
 import type * as p from "../../core/properties";
 type SearchStrategy = typeof SearchStrategy["__type__"];
-declare const SearchStrategy: import("../../core/kinds").Kinds.Enum<"includes" | "starts_with">;
+declare const SearchStrategy: import("core/kinds").Kinds.Enum<"includes" | "starts_with">;
 export declare class AutocompleteInputView extends TextInputView {
     model: AutocompleteInput;
     protected _open: boolean;
     protected _last_value: string;
     protected _hover_index: number;
     protected menu: HTMLElement;
     stylesheets(): StyleSheetLike[];
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/base_date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/base_datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/button.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/checkbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/checkbox_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/checkbox_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/color_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/control.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/control.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_range_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/date_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/datetime_range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/div.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/div.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/dropdown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/file_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/help_button.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/index.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/index.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/input_widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/markup.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multi_choice.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multiple_date_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multiple_datetime_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/multiselect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/numeric_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/oriented_control.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/paragraph.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/password_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/picker_base.d.ts`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import type { StyleSheetLike } from "../../core/dom";
 import { CalendarPosition } from "../../core/enums";
 import type * as p from "../../core/properties";
 export declare abstract class PickerBaseView extends InputWidgetView {
     model: PickerBase;
     protected _picker?: flatpickr.Instance;
     get picker(): flatpickr.Instance;
-    controls(): Generator<import("./input_widget").HTMLInputElementLike, void, unknown>;
     remove(): void;
     stylesheets(): StyleSheetLike[];
     connect_signals(): void;
     protected get flatpickr_options(): flatpickr.Options.Options;
     protected abstract _on_change(selected: Date[]): void;
     render(): void;
     protected _position(self: flatpickr.Instance, custom_el: HTMLElement | undefined): void;
```

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/pretext.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/radio_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/radio_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/range_slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/selectbox.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/slider.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/spinner.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/switch.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_editors.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/cell_formatters.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/data_cube.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/data_table.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/row_aggregators.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/table_column.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/tables/table_widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/text_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/text_like_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/textarea_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/time_picker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle_button_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle_input.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/toggle_input_group.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/models/widgets/widget.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/protocol/message.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/protocol/message.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/protocol/receiver.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/protocol/receiver.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/js/lib/styles/icons.css.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/js/lib/styles/icons.css.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.decorators.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.decorators.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.decorators.legacy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.dom.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.dom.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.dom.iterable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.dom.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.collection.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.collection.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.core.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.core.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.generator.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.generator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.promise.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.proxy.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.reflect.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.symbol.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2015.symbol.wellknown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2016.array.include.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2016.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2016.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2016.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2016.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.intl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.object.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.string.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2017.typedarrays.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.asyncgenerator.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.asynciterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.intl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.promise.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2018.regexp.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.array.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.intl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.object.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.string.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2019.symbol.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.bigint.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.date.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.date.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.intl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.number.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.number.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.promise.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.string.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2020.symbol.wellknown.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.intl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.promise.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.promise.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.string.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2021.weakref.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.array.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.error.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.error.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.intl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.object.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.object.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.regexp.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.sharedmemory.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2022.string.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2022.string.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2023.array.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2023.array.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2023.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2023.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es2023.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es2023.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es5.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es5.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.es6.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.es6.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.esnext.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.esnext.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.esnext.full.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.esnext.full.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.esnext.intl.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.esnext.intl.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.scripthost.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.scripthost.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.webworker.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.webworker.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.webworker.importscripts.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts` & `bokeh-3.3.0.dev1/src/bokeh/server/static/lib/lib.webworker.iterable.d.ts`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/tornado.py` & `bokeh-3.3.0.dev1/src/bokeh/server/tornado.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/urls.py` & `bokeh-3.3.0.dev1/src/bokeh/server/urls.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/util.py` & `bokeh-3.3.0.dev1/src/bokeh/server/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/app_index.html` & `bokeh-3.3.0.dev1/src/bokeh/server/views/app_index.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/auth_request_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/auth_request_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/autoload_js_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/autoload_js_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/bokeh-dev.ico` & `bokeh-3.3.0.dev1/src/bokeh/server/views/bokeh-dev.ico`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/bokeh.ico` & `bokeh-3.3.0.dev1/src/bokeh/server/views/bokeh.ico`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/doc_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/doc_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/ico_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/ico_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/metadata_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/multi_root_static_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/multi_root_static_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/root_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/root_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/session_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/session_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/static_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/static_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/server/views/ws.py` & `bokeh-3.3.0.dev1/src/bokeh/server/views/ws.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/settings.py` & `bokeh-3.3.0.dev1/src/bokeh/settings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/bokehjs_codepen_init.html`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/_templates/gallery_page.rst` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/gallery_page.rst`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/_templates/release_detail.rst` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/_templates/release_detail.rst`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_autodoc.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_autodoc.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_color.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_color.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_dataframe.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_dataframe.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_directive.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_directive.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_enum.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_enum.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_example_metadata.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_example_metadata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_gallery.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_gallery.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_jinja.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_jinja.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_model.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_model.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_options.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_options.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_palette.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_palette.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_palette_group.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_palette_group.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_plot.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_plot.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_prop.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_prop.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_releases.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_releases.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_roles.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_roles.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_sampledata_xref.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_sampledata_xref.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_settings.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_settings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokeh_sitemap.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokeh_sitemap.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/bokehjs_content.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/bokehjs_content.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/example_handler.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/example_handler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/sample.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/sample.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/templates.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/templates.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/sphinxext/util.py` & `bokeh-3.3.0.dev1/src/bokeh/sphinxext/util.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/themes/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/themes/_caliber.py` & `bokeh-3.3.0.dev1/src/bokeh/themes/_caliber.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/themes/_contrast.py` & `bokeh-3.3.0.dev1/src/bokeh/themes/_contrast.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/themes/_dark_minimal.py` & `bokeh-3.3.0.dev1/src/bokeh/themes/_dark_minimal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/themes/_light_minimal.py` & `bokeh-3.3.0.dev1/src/bokeh/themes/_light_minimal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/themes/_night_sky.py` & `bokeh-3.3.0.dev1/src/bokeh/themes/_night_sky.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/themes/theme.py` & `bokeh-3.3.0.dev1/src/bokeh/themes/theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         values that specify the new property defaults for that type.
 
         Take note of the fact that YAML interprets the value `None` as
         a string, which is not usually what you want. To give `None` as a
         value in YAML, use `!!null`. To give 'None' as a value in json,
         use `null`.
 
-        Here is an example theme in YAML format that sets various visual
-        properties for all figures, grids, and titles:
+       Here is an example theme in YAML format that sets various visual
+       properties for all figures, grids, and titles:
 
         .. code-block:: yaml
 
             attrs:
                 Plot:
                     background_fill_color: '#2F2F2F'
                     border_fill_color: '#2F2F2F'
```

### Comparing `bokeh-3.2.1/src/bokeh/tile_providers.py` & `bokeh-3.3.0.dev1/src/bokeh/tile_providers.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/transform.py` & `bokeh-3.3.0.dev1/src/bokeh/transform.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/__init__.py` & `bokeh-3.3.0.dev1/src/bokeh/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/browser.py` & `bokeh-3.3.0.dev1/src/bokeh/util/browser.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/callback_manager.py` & `bokeh-3.3.0.dev1/src/bokeh/util/callback_manager.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/compiler.py` & `bokeh-3.3.0.dev1/src/bokeh/util/compiler.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/dataclasses.py` & `bokeh-3.3.0.dev1/src/bokeh/util/dataclasses.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/datatypes.py` & `bokeh-3.3.0.dev1/src/bokeh/util/datatypes.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/dependencies.py` & `bokeh-3.3.0.dev1/src/bokeh/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/deprecation.py` & `bokeh-3.3.0.dev1/src/bokeh/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/functions.py` & `bokeh-3.3.0.dev1/src/bokeh/util/functions.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/hex.py` & `bokeh-3.3.0.dev1/src/bokeh/util/hex.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/logconfig.py` & `bokeh-3.3.0.dev1/src/bokeh/util/logconfig.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/options.py` & `bokeh-3.3.0.dev1/src/bokeh/util/options.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/package.py` & `bokeh-3.3.0.dev1/src/bokeh/util/package.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/paths.py` & `bokeh-3.3.0.dev1/src/bokeh/util/paths.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/sampledata.json` & `bokeh-3.3.0.dev1/src/bokeh/util/sampledata.json`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/sampledata.py` & `bokeh-3.3.0.dev1/src/bokeh/util/sampledata.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/serialization.py` & `bokeh-3.3.0.dev1/src/bokeh/util/serialization.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/strings.py` & `bokeh-3.3.0.dev1/src/bokeh/util/strings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/terminal.py` & `bokeh-3.3.0.dev1/src/bokeh/util/terminal.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/token.py` & `bokeh-3.3.0.dev1/src/bokeh/util/token.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/tornado.py` & `bokeh-3.3.0.dev1/src/bokeh/util/tornado.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/version.py` & `bokeh-3.3.0.dev1/src/bokeh/util/version.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh/util/warnings.py` & `bokeh-3.3.0.dev1/src/bokeh/util/warnings.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/src/bokeh.egg-info/PKG-INFO` & `bokeh-3.3.0.dev1/src/bokeh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bokeh
-Version: 3.2.1
+Version: 3.3.0.dev1
 Summary: Interactive plots and applications in the browser from Python
 Author: Bokeh Team
 Author-email: info@bokeh.org
 License: Copyright (c) 2012 - 2023, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `bokeh-3.2.1/src/bokeh.egg-info/SOURCES.txt` & `bokeh-3.3.0.dev1/src/bokeh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/tests/test_bokehjs.py` & `bokeh-3.3.0.dev1/tests/test_bokehjs.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/tests/test_cross.py` & `bokeh-3.3.0.dev1/tests/test_cross.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/tests/test_defaults.py` & `bokeh-3.3.0.dev1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `bokeh-3.2.1/tests/test_examples.py` & `bokeh-3.3.0.dev1/tests/test_examples.py`

 * *Files identical despite different names*

