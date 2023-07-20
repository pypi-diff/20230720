# Comparing `tmp/datacraft-0.7.2.tar.gz` & `tmp/datacraft-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacraft-0.7.2.tar", last modified: Thu Jul 20 16:31:48 2023, max compression
+gzip compressed data, was "datacraft-0.7.3.tar", last modified: Thu Jul 20 20:55:01 2023, max compression
```

## Comparing `datacraft-0.7.2.tar` & `datacraft-0.7.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 16:31:48.025290 datacraft-0.7.2/
--rw-rw-rw-   0        0        0     1080 2022-07-20 19:48:53.000000 datacraft-0.7.2/LICENSE.txt
--rw-rw-rw-   0        0        0       16 2022-07-20 19:48:53.000000 datacraft-0.7.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6009 2023-07-20 16:31:48.025290 datacraft-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     5104 2022-11-23 22:16:24.000000 datacraft-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 16:31:47.497080 datacraft-0.7.2/datacraft/
--rw-rw-rw-   0        0        0     2350 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/__init__.py
--rw-rw-rw-   0        0        0     1569 2023-07-20 16:21:23.000000 datacraft-0.7.2/datacraft/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:31:47.558761 datacraft-0.7.2/datacraft/_registered_types/
--rw-rw-rw-   0        0        0      308 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/__init__.py
--rw-rw-rw-   0        0        0     1254 2022-11-12 14:37:56.000000 datacraft-0.7.2/datacraft/_registered_types/calculate.py
--rw-rw-rw-   0        0        0     3883 2022-11-12 15:07:20.000000 datacraft-0.7.2/datacraft/_registered_types/char_class.py
--rw-rw-rw-   0        0        0     4350 2022-11-12 15:11:51.000000 datacraft-0.7.2/datacraft/_registered_types/combine.py
--rw-rw-rw-   0        0        0     3311 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/common.py
--rw-rw-rw-   0        0        0      377 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/config_ref.py
--rw-rw-rw-   0        0        0     4907 2023-07-20 15:43:51.000000 datacraft-0.7.2/datacraft/_registered_types/csv.py
--rw-rw-rw-   0        0        0     6746 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/date.py
--rw-rw-rw-   0        0        0     1890 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/distribution.py
--rw-rw-rw-   0        0        0      231 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/entrypoint.py
--rw-rw-rw-   0        0        0     2616 2022-11-12 18:01:56.000000 datacraft-0.7.2/datacraft/_registered_types/geo.py
--rw-rw-rw-   0        0        0     4721 2022-11-12 18:02:04.000000 datacraft-0.7.2/datacraft/_registered_types/nested.py
--rw-rw-rw-   0        0        0     3319 2022-11-12 18:02:31.000000 datacraft-0.7.2/datacraft/_registered_types/network.py
--rw-rw-rw-   0        0        0     4659 2022-11-12 18:03:00.000000 datacraft-0.7.2/datacraft/_registered_types/range_suppliers.py
--rw-rw-rw-   0        0        0     3670 2022-11-12 18:03:18.000000 datacraft-0.7.2/datacraft/_registered_types/refs.py
--rw-rw-rw-   0        0        0     4076 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/replace.py
--rw-rw-rw-   0        0        0     2600 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:31:47.585893 datacraft-0.7.2/datacraft/_registered_types/schema/
--rw-rw-rw-   0        0        0        0 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/calculate.schema.json
--rw-rw-rw-   0        0        0     2282 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/char_class.schema.json
--rw-rw-rw-   0        0        0      931 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/combine-list.schema.json
--rw-rw-rw-   0        0        0      857 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/combine.schema.json
--rw-rw-rw-   0        0        0      429 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/configref.schema.json
--rw-rw-rw-   0        0        0     2577 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/csv.schema.json
--rw-rw-rw-   0        0        0     3816 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/schema/date.epoch.schema.json
--rw-rw-rw-   0        0        0     4030 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/schema/date.schema.json
--rw-rw-rw-   0        0        0     4149 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/definitions.json
--rw-rw-rw-   0        0        0      592 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/distribution.schema.json
--rw-rw-rw-   0        0        0      860 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/geo.lat.schema.json
--rw-rw-rw-   0        0        0      869 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/geo.long.schema.json
--rw-rw-rw-   0        0        0     1189 2022-11-30 01:52:43.000000 datacraft-0.7.2/datacraft/_registered_types/schema/geo.pair.schema.json
--rw-rw-rw-   0        0        0      913 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/ip.precise.schema.json
--rw-rw-rw-   0        0        0     1353 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/ip.schema.json
--rw-rw-rw-   0        0        0      804 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/nested.schema.json
--rw-rw-rw-   0        0        0      794 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/net.mac.schema.json
--rw-rw-rw-   0        0        0     1145 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/range.schema.json
--rw-rw-rw-   0        0        0      706 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/ref.schema.json
--rw-rw-rw-   0        0        0      959 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/schema/replace.schema.json
--rw-rw-rw-   0        0        0     2222 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/schema/sample.schema.json
--rw-rw-rw-   0        0        0     1438 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/templated.schema.json
--rw-rw-rw-   0        0        0     2387 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/unicode_range.schema.json
--rw-rw-rw-   0        0        0      660 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/uuid.schema.json
--rw-rw-rw-   0        0        0      912 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/values.schema.json
--rw-rw-rw-   0        0        0     2478 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/weighted_csv.schema.json
--rw-rw-rw-   0        0        0      723 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/_registered_types/schema/weighted_ref.schema.json
--rw-rw-rw-   0        0        0     1266 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/schemas.py
--rw-rw-rw-   0        0        0     1518 2022-11-12 18:04:13.000000 datacraft-0.7.2/datacraft/_registered_types/templated.py
--rw-rw-rw-   0        0        0     1377 2022-11-12 18:04:21.000000 datacraft-0.7.2/datacraft/_registered_types/unicode_range.py
--rw-rw-rw-   0        0        0     1155 2022-11-12 18:04:38.000000 datacraft-0.7.2/datacraft/_registered_types/uuid_handler.py
--rw-rw-rw-   0        0        0     1142 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/_registered_types/values.py
--rw-rw-rw-   0        0        0     4838 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/builder.py
--rw-rw-rw-   0        0        0     5494 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/casters.py
--rw-rw-rw-   0        0        0    17043 2023-07-20 16:21:23.000000 datacraft-0.7.2/datacraft/cli.py
--rw-rw-rw-   0        0        0     3486 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/defaults.py
--rw-rw-rw-   0        0        0     5072 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/distributions.py
--rw-rw-rw-   0        0        0      631 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/entrypoints.py
--rw-rw-rw-   0        0        0      565 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/exceptions.py
--rw-rw-rw-   0        0        0     7183 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/loader.py
--rw-rw-rw-   0        0        0      768 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/logging_handler.py
--rw-rw-rw-   0        0        0    13593 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/outputs.py
--rw-rw-rw-   0        0        0    10327 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/preprocessor.py
--rw-rw-rw-   0        0        0        0 2022-12-04 16:45:17.000000 datacraft-0.7.2/datacraft/py.typed
--rw-rw-rw-   0        0        0     7248 2022-12-04 16:45:17.000000 datacraft-0.7.2/datacraft/registries.py
--rw-rw-rw-   0        0        0      875 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/schemas.py
--rw-rw-rw-   0        0        0     2684 2023-07-20 16:23:20.000000 datacraft-0.7.2/datacraft/server.py
--rw-rw-rw-   0        0        0     6479 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/spec_formatters.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:31:47.601893 datacraft-0.7.2/datacraft/supplier/
--rw-rw-rw-   0        0        0        0 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/__init__.py
--rw-rw-rw-   0        0        0     1907 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/calculate.py
--rw-rw-rw-   0        0        0     1438 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/combine.py
--rw-rw-rw-   0        0        0    13592 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/common.py
--rw-rw-rw-   0        0        0     8925 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/csv.py
--rw-rw-rw-   0        0        0     5203 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/supplier/date.py
--rw-rw-rw-   0        0        0      234 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/exceptions.py
--rw-rw-rw-   0        0        0     4747 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/key_suppliers.py
--rw-rw-rw-   0        0        0     5747 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/supplier/model.py
--rw-rw-rw-   0        0        0     2875 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/network.py
--rw-rw-rw-   0        0        0     2774 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/supplier/ranges.py
--rw-rw-rw-   0        0        0      758 2022-11-23 22:16:24.000000 datacraft-0.7.2/datacraft/supplier/strings.py
--rw-rw-rw-   0        0        0     1014 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/templated.py
--rw-rw-rw-   0        0        0      766 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/unicode.py
--rw-rw-rw-   0        0        0     1229 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/supplier/uuid.py
--rw-rw-rw-   0        0        0    40659 2023-07-20 15:49:29.000000 datacraft-0.7.2/datacraft/suppliers.py
--rw-rw-rw-   0        0        0     2301 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/template_engines.py
--rw-rw-rw-   0        0        0     1942 2023-07-20 15:43:51.000000 datacraft-0.7.2/datacraft/usage.py
--rw-rw-rw-   0        0        0     3022 2022-07-20 19:48:53.000000 datacraft-0.7.2/datacraft/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:31:47.537239 datacraft-0.7.2/datacraft.egg-info/
--rw-rw-rw-   0        0        0     6009 2023-07-20 16:31:47.000000 datacraft-0.7.2/datacraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4658 2023-07-20 16:31:47.000000 datacraft-0.7.2/datacraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 16:31:47.000000 datacraft-0.7.2/datacraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2023-07-20 16:31:47.000000 datacraft-0.7.2/datacraft.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      280 2023-07-20 16:31:47.000000 datacraft-0.7.2/datacraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 16:31:47.000000 datacraft-0.7.2/datacraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2022-07-20 19:48:53.000000 datacraft-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0     1393 2023-07-20 16:31:48.036286 datacraft-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0       93 2022-07-20 19:48:53.000000 datacraft-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 16:31:48.023300 datacraft-0.7.2/tests/
--rw-rw-rw-   0        0        0     2516 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_buffering.py
--rw-rw-rw-   0        0        0    18868 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_builder.py
--rw-rw-rw-   0        0        0     2393 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_calculate.py
--rw-rw-rw-   0        0        0     4598 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_casters.py
--rw-rw-rw-   0        0        0     2826 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_char_class.py
--rw-rw-rw-   0        0        0     4594 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_combine.py
--rw-rw-rw-   0        0        0     1063 2023-07-20 15:51:03.000000 datacraft-0.7.2/tests/test_counts.py
--rw-rw-rw-   0        0        0     6213 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_csv.py
--rw-rw-rw-   0        0        0     6238 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_date.py
--rw-rw-rw-   0        0        0      552 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_defaults.py
--rw-rw-rw-   0        0        0     3169 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_distributions.py
--rw-rw-rw-   0        0        0      399 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_entrypoints.py
--rw-rw-rw-   0        0        0     1344 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_generate.py
--rw-rw-rw-   0        0        0     4203 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_geo.py
--rw-rw-rw-   0        0        0     2659 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_key_suppliers.py
--rw-rw-rw-   0        0        0     3367 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_loader.py
--rw-rw-rw-   0        0        0      199 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_logging_handler.py
--rw-rw-rw-   0        0        0     8347 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_main.py
--rw-rw-rw-   0        0        0      410 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_model.py
--rw-rw-rw-   0        0        0     3745 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_nested.py
--rw-rw-rw-   0        0        0     4578 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_network.py
--rw-rw-rw-   0        0        0     4207 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_outputs.py
--rw-rw-rw-   0        0        0    11848 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_preprocessor.py
--rw-rw-rw-   0        0        0     1763 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_random_range.py
--rw-rw-rw-   0        0        0     2323 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_range_supplier.py
--rw-rw-rw-   0        0        0     1352 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_refs.py
--rw-rw-rw-   0        0        0     3537 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_registry.py
--rw-rw-rw-   0        0        0     2462 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_replace.py
--rw-rw-rw-   0        0        0     1468 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_schemas.py
--rw-rw-rw-   0        0        0     5059 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_schemas_data.py
--rw-rw-rw-   0        0        0     2460 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_select_list.py
--rw-rw-rw-   0        0        0     1194 2023-07-20 16:22:56.000000 datacraft-0.7.2/tests/test_server.py
--rw-rw-rw-   0        0        0     2834 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_spec_formatters.py
--rw-rw-rw-   0        0        0      502 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_strings.py
--rw-rw-rw-   0        0        0      372 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_template_engine.py
--rw-rw-rw-   0        0        0     1324 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_templated.py
--rw-rw-rw-   0        0        0     1738 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_unicode_range.py
--rw-rw-rw-   0        0        0     1748 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_usage.py
--rw-rw-rw-   0        0        0     1052 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_uuid.py
--rw-rw-rw-   0        0        0     4154 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_values.py
--rw-rw-rw-   0        0        0     2146 2022-07-20 19:48:53.000000 datacraft-0.7.2/tests/test_weighted_csv.py
--rw-rw-rw-   0        0        0     1400 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_weighted_ref.py
--rw-rw-rw-   0        0        0      931 2022-11-23 22:16:24.000000 datacraft-0.7.2/tests/test_yaml_specs.py
+drwxrwxrwx   0        0        0        0 2023-07-20 20:55:01.398528 datacraft-0.7.3/
+-rw-rw-rw-   0        0        0     1080 2022-07-20 19:48:53.000000 datacraft-0.7.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       16 2022-07-20 19:48:53.000000 datacraft-0.7.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6009 2023-07-20 20:55:01.398528 datacraft-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2022-11-23 22:16:24.000000 datacraft-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 20:55:01.255030 datacraft-0.7.3/datacraft/
+-rw-rw-rw-   0        0        0     2350 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/__init__.py
+-rw-rw-rw-   0        0        0     1603 2023-07-20 20:45:51.000000 datacraft-0.7.3/datacraft/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 20:55:01.297319 datacraft-0.7.3/datacraft/_registered_types/
+-rw-rw-rw-   0        0        0      308 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/__init__.py
+-rw-rw-rw-   0        0        0     1254 2022-11-12 14:37:56.000000 datacraft-0.7.3/datacraft/_registered_types/calculate.py
+-rw-rw-rw-   0        0        0     3883 2022-11-12 15:07:20.000000 datacraft-0.7.3/datacraft/_registered_types/char_class.py
+-rw-rw-rw-   0        0        0     4350 2022-11-12 15:11:51.000000 datacraft-0.7.3/datacraft/_registered_types/combine.py
+-rw-rw-rw-   0        0        0     3311 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/common.py
+-rw-rw-rw-   0        0        0      377 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/config_ref.py
+-rw-rw-rw-   0        0        0     4907 2023-07-20 15:43:51.000000 datacraft-0.7.3/datacraft/_registered_types/csv.py
+-rw-rw-rw-   0        0        0     6746 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/date.py
+-rw-rw-rw-   0        0        0     1890 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/distribution.py
+-rw-rw-rw-   0        0        0      231 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/entrypoint.py
+-rw-rw-rw-   0        0        0     2616 2022-11-12 18:01:56.000000 datacraft-0.7.3/datacraft/_registered_types/geo.py
+-rw-rw-rw-   0        0        0     4721 2022-11-12 18:02:04.000000 datacraft-0.7.3/datacraft/_registered_types/nested.py
+-rw-rw-rw-   0        0        0     3319 2022-11-12 18:02:31.000000 datacraft-0.7.3/datacraft/_registered_types/network.py
+-rw-rw-rw-   0        0        0     4659 2022-11-12 18:03:00.000000 datacraft-0.7.3/datacraft/_registered_types/range_suppliers.py
+-rw-rw-rw-   0        0        0     3670 2022-11-12 18:03:18.000000 datacraft-0.7.3/datacraft/_registered_types/refs.py
+-rw-rw-rw-   0        0        0     4076 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/replace.py
+-rw-rw-rw-   0        0        0     2600 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-20 20:55:01.330821 datacraft-0.7.3/datacraft/_registered_types/schema/
+-rw-rw-rw-   0        0        0        0 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/calculate.schema.json
+-rw-rw-rw-   0        0        0     2282 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/char_class.schema.json
+-rw-rw-rw-   0        0        0      931 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/combine-list.schema.json
+-rw-rw-rw-   0        0        0      857 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/combine.schema.json
+-rw-rw-rw-   0        0        0      429 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/configref.schema.json
+-rw-rw-rw-   0        0        0     2577 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/csv.schema.json
+-rw-rw-rw-   0        0        0     3816 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/schema/date.epoch.schema.json
+-rw-rw-rw-   0        0        0     4030 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/schema/date.schema.json
+-rw-rw-rw-   0        0        0     4149 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/definitions.json
+-rw-rw-rw-   0        0        0      592 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/distribution.schema.json
+-rw-rw-rw-   0        0        0      860 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/geo.lat.schema.json
+-rw-rw-rw-   0        0        0      869 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/geo.long.schema.json
+-rw-rw-rw-   0        0        0     1189 2022-11-30 01:52:43.000000 datacraft-0.7.3/datacraft/_registered_types/schema/geo.pair.schema.json
+-rw-rw-rw-   0        0        0      913 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/ip.precise.schema.json
+-rw-rw-rw-   0        0        0     1353 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/ip.schema.json
+-rw-rw-rw-   0        0        0      804 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/nested.schema.json
+-rw-rw-rw-   0        0        0      794 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/net.mac.schema.json
+-rw-rw-rw-   0        0        0     1145 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/range.schema.json
+-rw-rw-rw-   0        0        0      706 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/ref.schema.json
+-rw-rw-rw-   0        0        0      959 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/schema/replace.schema.json
+-rw-rw-rw-   0        0        0     2222 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/schema/sample.schema.json
+-rw-rw-rw-   0        0        0     1438 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/templated.schema.json
+-rw-rw-rw-   0        0        0     2387 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/unicode_range.schema.json
+-rw-rw-rw-   0        0        0      660 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/uuid.schema.json
+-rw-rw-rw-   0        0        0      912 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/values.schema.json
+-rw-rw-rw-   0        0        0     2478 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/weighted_csv.schema.json
+-rw-rw-rw-   0        0        0      723 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/_registered_types/schema/weighted_ref.schema.json
+-rw-rw-rw-   0        0        0     1266 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/schemas.py
+-rw-rw-rw-   0        0        0     1518 2022-11-12 18:04:13.000000 datacraft-0.7.3/datacraft/_registered_types/templated.py
+-rw-rw-rw-   0        0        0     1377 2022-11-12 18:04:21.000000 datacraft-0.7.3/datacraft/_registered_types/unicode_range.py
+-rw-rw-rw-   0        0        0     1155 2022-11-12 18:04:38.000000 datacraft-0.7.3/datacraft/_registered_types/uuid_handler.py
+-rw-rw-rw-   0        0        0     1142 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/_registered_types/values.py
+-rw-rw-rw-   0        0        0     4838 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/builder.py
+-rw-rw-rw-   0        0        0     5494 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/casters.py
+-rw-rw-rw-   0        0        0    17165 2023-07-20 20:45:57.000000 datacraft-0.7.3/datacraft/cli.py
+-rw-rw-rw-   0        0        0     3486 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/defaults.py
+-rw-rw-rw-   0        0        0     5072 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/distributions.py
+-rw-rw-rw-   0        0        0      631 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/entrypoints.py
+-rw-rw-rw-   0        0        0      565 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/exceptions.py
+-rw-rw-rw-   0        0        0     7183 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/loader.py
+-rw-rw-rw-   0        0        0      768 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/logging_handler.py
+-rw-rw-rw-   0        0        0    13593 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/outputs.py
+-rw-rw-rw-   0        0        0    10327 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/preprocessor.py
+-rw-rw-rw-   0        0        0        0 2022-12-04 16:45:17.000000 datacraft-0.7.3/datacraft/py.typed
+-rw-rw-rw-   0        0        0     7248 2022-12-04 16:45:17.000000 datacraft-0.7.3/datacraft/registries.py
+-rw-rw-rw-   0        0        0      875 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/schemas.py
+-rw-rw-rw-   0        0        0     2867 2023-07-20 20:50:59.000000 datacraft-0.7.3/datacraft/server.py
+-rw-rw-rw-   0        0        0     6479 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/spec_formatters.py
+drwxrwxrwx   0        0        0        0 2023-07-20 20:55:01.347038 datacraft-0.7.3/datacraft/supplier/
+-rw-rw-rw-   0        0        0        0 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/__init__.py
+-rw-rw-rw-   0        0        0     1907 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/calculate.py
+-rw-rw-rw-   0        0        0     1438 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/combine.py
+-rw-rw-rw-   0        0        0    13592 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/common.py
+-rw-rw-rw-   0        0        0     8925 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/csv.py
+-rw-rw-rw-   0        0        0     5203 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/supplier/date.py
+-rw-rw-rw-   0        0        0      234 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/exceptions.py
+-rw-rw-rw-   0        0        0     4747 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/key_suppliers.py
+-rw-rw-rw-   0        0        0     5747 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/supplier/model.py
+-rw-rw-rw-   0        0        0     2875 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/network.py
+-rw-rw-rw-   0        0        0     2774 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/supplier/ranges.py
+-rw-rw-rw-   0        0        0      758 2022-11-23 22:16:24.000000 datacraft-0.7.3/datacraft/supplier/strings.py
+-rw-rw-rw-   0        0        0     1014 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/templated.py
+-rw-rw-rw-   0        0        0      766 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/unicode.py
+-rw-rw-rw-   0        0        0     1229 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/supplier/uuid.py
+-rw-rw-rw-   0        0        0    40659 2023-07-20 15:49:29.000000 datacraft-0.7.3/datacraft/suppliers.py
+-rw-rw-rw-   0        0        0     2301 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/template_engines.py
+-rw-rw-rw-   0        0        0     1942 2023-07-20 15:43:51.000000 datacraft-0.7.3/datacraft/usage.py
+-rw-rw-rw-   0        0        0     3022 2022-07-20 19:48:53.000000 datacraft-0.7.3/datacraft/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 20:55:01.273470 datacraft-0.7.3/datacraft.egg-info/
+-rw-rw-rw-   0        0        0     6009 2023-07-20 20:55:01.000000 datacraft-0.7.3/datacraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4658 2023-07-20 20:55:01.000000 datacraft-0.7.3/datacraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 20:55:01.000000 datacraft-0.7.3/datacraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2023-07-20 20:55:01.000000 datacraft-0.7.3/datacraft.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      280 2023-07-20 20:55:01.000000 datacraft-0.7.3/datacraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-20 20:55:01.000000 datacraft-0.7.3/datacraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2022-07-20 19:48:53.000000 datacraft-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1393 2023-07-20 20:55:01.406520 datacraft-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0       93 2022-07-20 19:48:53.000000 datacraft-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 20:55:01.397527 datacraft-0.7.3/tests/
+-rw-rw-rw-   0        0        0     2516 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_buffering.py
+-rw-rw-rw-   0        0        0    18868 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_builder.py
+-rw-rw-rw-   0        0        0     2393 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_calculate.py
+-rw-rw-rw-   0        0        0     4598 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_casters.py
+-rw-rw-rw-   0        0        0     2826 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_char_class.py
+-rw-rw-rw-   0        0        0     4594 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_combine.py
+-rw-rw-rw-   0        0        0     1063 2023-07-20 15:51:03.000000 datacraft-0.7.3/tests/test_counts.py
+-rw-rw-rw-   0        0        0     6213 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_csv.py
+-rw-rw-rw-   0        0        0     6238 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_date.py
+-rw-rw-rw-   0        0        0      552 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_defaults.py
+-rw-rw-rw-   0        0        0     3169 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_distributions.py
+-rw-rw-rw-   0        0        0      399 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_entrypoints.py
+-rw-rw-rw-   0        0        0     1344 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_generate.py
+-rw-rw-rw-   0        0        0     4203 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_geo.py
+-rw-rw-rw-   0        0        0     2659 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_key_suppliers.py
+-rw-rw-rw-   0        0        0     3367 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_loader.py
+-rw-rw-rw-   0        0        0      199 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_logging_handler.py
+-rw-rw-rw-   0        0        0     8347 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_main.py
+-rw-rw-rw-   0        0        0      410 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_model.py
+-rw-rw-rw-   0        0        0     3745 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_nested.py
+-rw-rw-rw-   0        0        0     4578 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_network.py
+-rw-rw-rw-   0        0        0     4207 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_outputs.py
+-rw-rw-rw-   0        0        0    11848 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_preprocessor.py
+-rw-rw-rw-   0        0        0     1763 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_random_range.py
+-rw-rw-rw-   0        0        0     2323 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_range_supplier.py
+-rw-rw-rw-   0        0        0     1352 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_refs.py
+-rw-rw-rw-   0        0        0     3537 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_registry.py
+-rw-rw-rw-   0        0        0     2462 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_replace.py
+-rw-rw-rw-   0        0        0     1468 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_schemas.py
+-rw-rw-rw-   0        0        0     5059 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_schemas_data.py
+-rw-rw-rw-   0        0        0     2460 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_select_list.py
+-rw-rw-rw-   0        0        0     1225 2023-07-20 20:53:04.000000 datacraft-0.7.3/tests/test_server.py
+-rw-rw-rw-   0        0        0     2834 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_spec_formatters.py
+-rw-rw-rw-   0        0        0      502 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_strings.py
+-rw-rw-rw-   0        0        0      372 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_template_engine.py
+-rw-rw-rw-   0        0        0     1324 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_templated.py
+-rw-rw-rw-   0        0        0     1738 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_unicode_range.py
+-rw-rw-rw-   0        0        0     1748 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_usage.py
+-rw-rw-rw-   0        0        0     1052 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_uuid.py
+-rw-rw-rw-   0        0        0     4154 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_values.py
+-rw-rw-rw-   0        0        0     2146 2022-07-20 19:48:53.000000 datacraft-0.7.3/tests/test_weighted_csv.py
+-rw-rw-rw-   0        0        0     1400 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_weighted_ref.py
+-rw-rw-rw-   0        0        0      931 2022-11-23 22:16:24.000000 datacraft-0.7.3/tests/test_yaml_specs.py
```

### Comparing `datacraft-0.7.2/LICENSE.txt` & `datacraft-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/PKG-INFO` & `datacraft-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacraft
-Version: 0.7.2
+Version: 0.7.3
 Summary: Data Generation Through Specification
 Home-page: https://github.com/bbux-dev/datacraft
 Author: Brian Buxton
 Author-email: bbux-dev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `datacraft-0.7.2/README.md` & `datacraft-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/__init__.py` & `datacraft-0.7.3/datacraft/__init__.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/__main__.py` & `datacraft-0.7.3/datacraft/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             from . import server
             using_template_or_formatter = args.template or args.format
             records_per_file = args.records_per_file
             if records_per_file is None:
                 records_per_file = 1
             server.run(generator,
                        args.endpoint,
+                       args.port,
                        data_is_json=(not using_template_or_formatter),
                        count_supplier=suppliers.count_supplier(count=records_per_file),
                        delay=args.server_delay)
         except ModuleNotFoundError:
             _log.warning('--server mode requires flask, pip/conda install flask and rerun command')
     else:
         _log.info('Starting Processing...')
```

### Comparing `datacraft-0.7.2/datacraft/_registered_types/calculate.py` & `datacraft-0.7.3/datacraft/_registered_types/calculate.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/char_class.py` & `datacraft-0.7.3/datacraft/_registered_types/char_class.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/combine.py` & `datacraft-0.7.3/datacraft/_registered_types/combine.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/common.py` & `datacraft-0.7.3/datacraft/_registered_types/common.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/csv.py` & `datacraft-0.7.3/datacraft/_registered_types/csv.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/date.py` & `datacraft-0.7.3/datacraft/_registered_types/date.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/distribution.py` & `datacraft-0.7.3/datacraft/_registered_types/distribution.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/geo.py` & `datacraft-0.7.3/datacraft/_registered_types/geo.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/nested.py` & `datacraft-0.7.3/datacraft/_registered_types/nested.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/network.py` & `datacraft-0.7.3/datacraft/_registered_types/network.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/range_suppliers.py` & `datacraft-0.7.3/datacraft/_registered_types/range_suppliers.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/refs.py` & `datacraft-0.7.3/datacraft/_registered_types/refs.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/replace.py` & `datacraft-0.7.3/datacraft/_registered_types/replace.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/sample.py` & `datacraft-0.7.3/datacraft/_registered_types/sample.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/calculate.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/calculate.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/char_class.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/char_class.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/combine-list.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/combine-list.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/combine.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/combine.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/csv.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/csv.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/date.epoch.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/date.epoch.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/date.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/date.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/definitions.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/definitions.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/distribution.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/distribution.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/geo.lat.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/geo.lat.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/geo.long.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/geo.long.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/geo.pair.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/geo.pair.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/ip.precise.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/ip.precise.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/ip.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/ip.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/nested.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/nested.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/net.mac.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/net.mac.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/range.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/range.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/ref.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/ref.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/replace.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/replace.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/sample.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/sample.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/templated.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/templated.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/unicode_range.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/unicode_range.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/uuid.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/uuid.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/values.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/values.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/weighted_csv.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/weighted_csv.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schema/weighted_ref.schema.json` & `datacraft-0.7.3/datacraft/_registered_types/schema/weighted_ref.schema.json`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/schemas.py` & `datacraft-0.7.3/datacraft/_registered_types/schemas.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/templated.py` & `datacraft-0.7.3/datacraft/_registered_types/templated.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/unicode_range.py` & `datacraft-0.7.3/datacraft/_registered_types/unicode_range.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/uuid_handler.py` & `datacraft-0.7.3/datacraft/_registered_types/uuid_handler.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/_registered_types/values.py` & `datacraft-0.7.3/datacraft/_registered_types/values.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/builder.py` & `datacraft-0.7.3/datacraft/builder.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/casters.py` & `datacraft-0.7.3/datacraft/casters.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/cli.py` & `datacraft-0.7.3/datacraft/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,16 @@
     parser.add_argument('--defaults', help='Path to defaults overrides')
     parser.add_argument("-sd", "--set-defaults", dest='set_defaults', metavar="KEY=VALUE", nargs='+',
                         help="Set a number of key-value pairs to override defaults with")
     parser.add_argument("--server", action='store_true',
                         help="Run a flask http server with the generated content")
     parser.add_argument("--server-endpoint", dest='endpoint', default='/data',
                         help="End point to host data service on")
+    parser.add_argument("--server-port", dest='port', default=5000, type=int,
+                        help="Server port")
     parser.add_argument('--server-delay', type=float, dest='server_delay',
                         help="Number of seconds before response is returned")
     parser.add_argument("--suppress-output", dest='suppress_output', action='store_true',
                         help="Silent mode, no output other than logging produced, set --log-level off to turn off "
                              "logging")
     parser.add_argument("--var-file", dest='var_file',
                         help="JSON or YAML file with variables to apply to the spec before consuming")
```

### Comparing `datacraft-0.7.2/datacraft/defaults.py` & `datacraft-0.7.3/datacraft/defaults.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/distributions.py` & `datacraft-0.7.3/datacraft/distributions.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/entrypoints.py` & `datacraft-0.7.3/datacraft/entrypoints.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/exceptions.py` & `datacraft-0.7.3/datacraft/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/loader.py` & `datacraft-0.7.3/datacraft/loader.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/logging_handler.py` & `datacraft-0.7.3/datacraft/logging_handler.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/outputs.py` & `datacraft-0.7.3/datacraft/outputs.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/preprocessor.py` & `datacraft-0.7.3/datacraft/preprocessor.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/registries.py` & `datacraft-0.7.3/datacraft/registries.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/schemas.py` & `datacraft-0.7.3/datacraft/schemas.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/server.py` & `datacraft-0.7.3/datacraft/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,21 @@
     """
     Light weight Flask server
     """
 
     def __init__(self,
                  generator: Generator,
                  endpoint: str,
+                 port: int,
                  data_is_json: bool,
                  count_supplier: datacraft.ValueSupplierInterface,
                  delay: float = None):
         self.generator = generator
         self.endpoint = endpoint
+        self.port = port
         self.data_is_json = data_is_json
         self.count_supplier = count_supplier
         self.delay = delay
         self.call_number = 0
 
     def callback(self):
         """
@@ -53,29 +55,33 @@
         # cannot return list without jsonifying it
         return flask.jsonify(data)
 
     def run(self):
         """ run the Flask app """
         app = flask.Flask(__name__)
         _log.info('Adding endpoint to server: %s', self.endpoint)
-        app.add_url_rule(self.endpoint, view_func=self.callback, methods=['POST', 'GET'])
-        app.run()
+        app.add_url_rule(self.endpoint,
+                         view_func=self.callback,
+                         methods=['POST', 'GET'])
+        app.run(port=self.port)
 
 
 def run(generator: Generator,
         endpoint: str,
+        port: int,
         data_is_json: bool,
         count_supplier: datacraft.ValueSupplierInterface,
         delay: float = None):
     """
     Runs a light weight Flask server with data returned by the provided generator served at each subsequent call to
     the provided endpoint. End point should start with /. When StopIteration encountered, returns a 204 status code.
 
     Args:
         generator: that provides response data as dictionary
         endpoint: to serve data on i.e. /data
+        port: to serve data on e.g. 8080
         data_is_json: if the data should be returned as JSON, default is as string
         count_supplier: supplies the number of values to generate for each call
         delay: number of seconds to pause between request and response
     """
-    server = _Server(generator, endpoint, data_is_json, count_supplier, delay)
+    server = _Server(generator, endpoint, port, data_is_json, count_supplier, delay)
     server.run()
```

### Comparing `datacraft-0.7.2/datacraft/spec_formatters.py` & `datacraft-0.7.3/datacraft/spec_formatters.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/calculate.py` & `datacraft-0.7.3/datacraft/supplier/calculate.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/combine.py` & `datacraft-0.7.3/datacraft/supplier/combine.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/common.py` & `datacraft-0.7.3/datacraft/supplier/common.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/csv.py` & `datacraft-0.7.3/datacraft/supplier/csv.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/date.py` & `datacraft-0.7.3/datacraft/supplier/date.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/key_suppliers.py` & `datacraft-0.7.3/datacraft/supplier/key_suppliers.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/model.py` & `datacraft-0.7.3/datacraft/supplier/model.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/network.py` & `datacraft-0.7.3/datacraft/supplier/network.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/ranges.py` & `datacraft-0.7.3/datacraft/supplier/ranges.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/strings.py` & `datacraft-0.7.3/datacraft/supplier/strings.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/templated.py` & `datacraft-0.7.3/datacraft/supplier/templated.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/unicode.py` & `datacraft-0.7.3/datacraft/supplier/unicode.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/supplier/uuid.py` & `datacraft-0.7.3/datacraft/supplier/uuid.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/suppliers.py` & `datacraft-0.7.3/datacraft/suppliers.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/template_engines.py` & `datacraft-0.7.3/datacraft/template_engines.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/usage.py` & `datacraft-0.7.3/datacraft/usage.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft/utils.py` & `datacraft-0.7.3/datacraft/utils.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/datacraft.egg-info/PKG-INFO` & `datacraft-0.7.3/datacraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacraft
-Version: 0.7.2
+Version: 0.7.3
 Summary: Data Generation Through Specification
 Home-page: https://github.com/bbux-dev/datacraft
 Author: Brian Buxton
 Author-email: bbux-dev@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `datacraft-0.7.2/datacraft.egg-info/SOURCES.txt` & `datacraft-0.7.3/datacraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/setup.cfg` & `datacraft-0.7.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 6163 7261 6674 0d0a 7665   = datacraft..ve
-00000020: 7273 696f 6e20 3d20 302e 372e 320d 0a64  rsion = 0.7.2..d
+00000020: 7273 696f 6e20 3d20 302e 372e 330d 0a64  rsion = 0.7.3..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2044 6174  escription = Dat
 00000040: 6120 4765 6e65 7261 7469 6f6e 2054 6872  a Generation Thr
 00000050: 6f75 6768 2053 7065 6369 6669 6361 7469  ough Specificati
 00000060: 6f6e 0d0a 6c6f 6e67 5f64 6573 6372 6970  on..long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `datacraft-0.7.2/tests/test_buffering.py` & `datacraft-0.7.3/tests/test_buffering.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_builder.py` & `datacraft-0.7.3/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_calculate.py` & `datacraft-0.7.3/tests/test_calculate.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_casters.py` & `datacraft-0.7.3/tests/test_casters.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_char_class.py` & `datacraft-0.7.3/tests/test_char_class.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_combine.py` & `datacraft-0.7.3/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_counts.py` & `datacraft-0.7.3/tests/test_counts.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_csv.py` & `datacraft-0.7.3/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_date.py` & `datacraft-0.7.3/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_defaults.py` & `datacraft-0.7.3/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_distributions.py` & `datacraft-0.7.3/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_generate.py` & `datacraft-0.7.3/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_geo.py` & `datacraft-0.7.3/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_key_suppliers.py` & `datacraft-0.7.3/tests/test_key_suppliers.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_loader.py` & `datacraft-0.7.3/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_main.py` & `datacraft-0.7.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_nested.py` & `datacraft-0.7.3/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_network.py` & `datacraft-0.7.3/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_outputs.py` & `datacraft-0.7.3/tests/test_outputs.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_preprocessor.py` & `datacraft-0.7.3/tests/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_random_range.py` & `datacraft-0.7.3/tests/test_random_range.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_range_supplier.py` & `datacraft-0.7.3/tests/test_range_supplier.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_refs.py` & `datacraft-0.7.3/tests/test_refs.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_registry.py` & `datacraft-0.7.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_replace.py` & `datacraft-0.7.3/tests/test_replace.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_schemas.py` & `datacraft-0.7.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_schemas_data.py` & `datacraft-0.7.3/tests/test_schemas_data.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_select_list.py` & `datacraft-0.7.3/tests/test_select_list.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_server.py` & `datacraft-0.7.3/tests/test_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 def test_server(mocker, one):
     mocker.patch('datacraft.server.flask.Flask.run', return_value=None)
 
     spec = {"test:uuid": {}}
 
     gen = datacraft.parse_spec(spec).generator(1)
 
-    datacraft.server.run(gen, endpoint='/test', data_is_json=True, count_supplier=one, )
+    datacraft.server.run(gen, endpoint='/test', port=None, data_is_json=True, count_supplier=one)
 
 
 def test_server_callback_stop_iteration(mocker, one):
     mocker.patch('flask.jsonify', return_value=None)
     spec = {"test:uuid": {}}
 
     gen = datacraft.parse_spec(spec).generator(1)
 
-    server = datacraft.server._Server(gen, endpoint='/test', data_is_json=True, count_supplier=one)
+    server = datacraft.server._Server(gen, endpoint='/test', port=None, data_is_json=True, count_supplier=one)
 
     # two calls should trigger the StopIteration
     server.callback()
     server.callback()
 
 
 def test_server_callback(mocker, one):
     spec = {"test:values": 42}
 
     processor = datacraft.outputs.processor(format_name='json-pretty')
     gen = datacraft.parse_spec(spec).generator(1, processor=processor)
 
-    server = datacraft.server._Server(gen, endpoint='/test', data_is_json=False, count_supplier=one)
+    server = datacraft.server._Server(gen, endpoint='/test', port=None, data_is_json=False, count_supplier=one)
 
     record = server.callback()
     assert record == json.dumps({'test': 42}, indent=4)
```

### Comparing `datacraft-0.7.2/tests/test_spec_formatters.py` & `datacraft-0.7.3/tests/test_spec_formatters.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_templated.py` & `datacraft-0.7.3/tests/test_templated.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_unicode_range.py` & `datacraft-0.7.3/tests/test_unicode_range.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_usage.py` & `datacraft-0.7.3/tests/test_usage.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_uuid.py` & `datacraft-0.7.3/tests/test_uuid.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_values.py` & `datacraft-0.7.3/tests/test_values.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_weighted_csv.py` & `datacraft-0.7.3/tests/test_weighted_csv.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_weighted_ref.py` & `datacraft-0.7.3/tests/test_weighted_ref.py`

 * *Files identical despite different names*

### Comparing `datacraft-0.7.2/tests/test_yaml_specs.py` & `datacraft-0.7.3/tests/test_yaml_specs.py`

 * *Files identical despite different names*

