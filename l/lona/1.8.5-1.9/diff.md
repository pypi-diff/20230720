# Comparing `tmp/lona-1.8.5.tar.gz` & `tmp/lona-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lona-1.8.5.tar", last modified: Wed Dec 15 11:49:00 2021, max compression
+gzip compressed data, was "lona-1.9.tar", last modified: Fri Jan 28 19:34:54 2022, max compression
```

## Comparing `lona-1.8.5.tar` & `lona-1.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.506688 lona-1.8.5/
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1071 2020-09-08 19:30:05.000000 lona-1.8.5/LICENSE.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)      181 2021-09-15 13:54:46.000000 lona-1.8.5/MANIFEST.in
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4380 2021-12-15 11:49:00.506688 lona-1.8.5/PKG-INFO
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2832 2021-10-04 16:21:33.000000 lona-1.8.5/README.rst
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.490688 lona-1.8.5/bin/
--rwxr-xr-x   0 fsc       (1000) fsc       (1000)      160 2021-04-26 12:26:21.000000 lona-1.8.5/bin/lona
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.494688 lona-1.8.5/lona/
--rw-r--r--   0 fsc       (1000) fsc       (1000)      238 2021-12-15 11:19:48.000000 lona-1.8.5/lona/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      152 2021-09-15 14:03:36.000000 lona-1.8.5/lona/__main__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      456 2021-07-15 08:55:51.000000 lona-1.8.5/lona/_json.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    12072 2021-11-24 12:57:34.000000 lona-1.8.5/lona/app.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.498688 lona-1.8.5/lona/client/
--rw-r--r--   0 fsc       (1000) fsc       (1000)     9332 2021-11-09 17:42:41.000000 lona-1.8.5/lona/client/context.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5257 2021-10-04 16:21:33.000000 lona-1.8.5/lona/client/dom-renderer.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)    16035 2021-10-04 16:21:33.000000 lona-1.8.5/lona/client/dom-updater.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)     9513 2021-11-04 21:23:57.000000 lona-1.8.5/lona/client/input-events.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1015 2021-08-09 06:36:12.000000 lona-1.8.5/lona/client/job-queue.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1749 2021-07-15 08:55:51.000000 lona-1.8.5/lona/client/lona.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2047 2021-07-15 08:55:51.000000 lona-1.8.5/lona/client/widget-data-updater.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)      645 2021-09-17 17:36:27.000000 lona-1.8.5/lona/client/window-shim.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)    12583 2021-11-09 17:42:41.000000 lona-1.8.5/lona/client/window.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2087 2021-11-02 17:17:07.000000 lona-1.8.5/lona/client_pre_compiler.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.498688 lona-1.8.5/lona/command_line/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-04-28 08:10:35.000000 lona-1.8.5/lona/command_line/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2768 2021-10-04 16:21:33.000000 lona-1.8.5/lona/command_line/collect_static.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5349 2021-11-24 09:58:43.000000 lona-1.8.5/lona/command_line/handle_command_line.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     3245 2021-11-02 20:26:04.000000 lona-1.8.5/lona/command_line/run_server.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      594 2021-09-15 14:02:28.000000 lona-1.8.5/lona/command_line/terminal.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1018 2021-10-04 16:21:33.000000 lona-1.8.5/lona/connection.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)       85 2021-10-04 16:21:33.000000 lona-1.8.5/lona/default_routes.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2560 2021-12-05 20:38:56.000000 lona-1.8.5/lona/default_settings.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1758 2021-10-04 16:21:33.000000 lona-1.8.5/lona/default_views.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      241 2021-11-24 10:23:27.000000 lona-1.8.5/lona/errors.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.498688 lona-1.8.5/lona/events/
--rw-r--r--   0 fsc       (1000) fsc       (1000)       52 2021-09-17 17:36:27.000000 lona-1.8.5/lona/events/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1302 2021-11-22 10:01:10.000000 lona-1.8.5/lona/events/event_types.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2116 2021-11-22 10:01:10.000000 lona-1.8.5/lona/events/input_event.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      267 2021-10-04 16:21:33.000000 lona-1.8.5/lona/events/view_event.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      119 2020-10-07 06:20:40.000000 lona-1.8.5/lona/exceptions.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.498688 lona-1.8.5/lona/html/
--rw-r--r--   0 fsc       (1000) fsc       (1000)      316 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     3816 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/abstract_node.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     6142 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/attribute_dict.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4157 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/attribute_list.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.502688 lona-1.8.5/lona/html/data_binding/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-02-05 16:46:07.000000 lona-1.8.5/lona/html/data_binding/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     8487 2021-11-04 21:23:57.000000 lona-1.8.5/lona/html/data_binding/inputs.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4030 2021-11-02 17:17:07.000000 lona-1.8.5/lona/html/data_binding/select.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2140 2021-11-16 19:55:44.000000 lona-1.8.5/lona/html/document.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    10057 2021-11-02 17:17:07.000000 lona-1.8.5/lona/html/node.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2420 2021-09-17 17:36:27.000000 lona-1.8.5/lona/html/node_event_list.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5963 2021-11-11 10:21:34.000000 lona-1.8.5/lona/html/node_list.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     3672 2021-11-02 17:17:07.000000 lona-1.8.5/lona/html/nodes.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5670 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/parsing.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      772 2021-09-17 17:36:27.000000 lona-1.8.5/lona/html/patches.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     3073 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/selector.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1912 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/text_node.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2237 2021-10-04 16:21:33.000000 lona-1.8.5/lona/html/widget.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    13098 2021-11-22 14:37:19.000000 lona-1.8.5/lona/html/widget_data.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2223 2021-11-11 10:21:34.000000 lona-1.8.5/lona/html/widgets.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1546 2021-10-04 16:21:33.000000 lona-1.8.5/lona/imports.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     6466 2021-12-15 11:08:37.000000 lona-1.8.5/lona/logging.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5928 2021-10-04 16:21:33.000000 lona-1.8.5/lona/middleware_controller.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.502688 lona-1.8.5/lona/middlewares/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-07-15 13:23:46.000000 lona-1.8.5/lona/middlewares/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      964 2021-11-02 17:17:07.000000 lona-1.8.5/lona/middlewares/lona_messages.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2618 2021-10-04 16:21:33.000000 lona-1.8.5/lona/middlewares/sessions.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5017 2021-11-22 10:01:10.000000 lona-1.8.5/lona/protocol.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4094 2021-11-02 17:17:07.000000 lona-1.8.5/lona/pytest.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1034 2021-09-15 14:02:28.000000 lona-1.8.5/lona/request.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4280 2021-11-11 19:11:11.000000 lona-1.8.5/lona/response_parser.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     5764 2021-11-11 10:21:34.000000 lona-1.8.5/lona/routing.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    18407 2021-11-11 10:21:34.000000 lona-1.8.5/lona/server.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1748 2021-08-09 06:36:12.000000 lona-1.8.5/lona/server_state.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1738 2021-10-04 16:21:33.000000 lona-1.8.5/lona/settings.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.502688 lona-1.8.5/lona/shell/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-04-15 06:55:45.000000 lona-1.8.5/lona/shell/__init__.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.502688 lona-1.8.5/lona/shell/commands/
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-04-15 06:55:45.000000 lona-1.8.5/lona/shell/commands/__init__.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      805 2021-04-26 12:26:21.000000 lona-1.8.5/lona/shell/commands/lona_connections.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      933 2021-11-24 09:58:43.000000 lona-1.8.5/lona/shell/commands/lona_info.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1144 2021-10-04 16:21:33.000000 lona-1.8.5/lona/shell/commands/lona_middlewares.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1860 2021-10-04 16:21:33.000000 lona-1.8.5/lona/shell/commands/lona_routes.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      879 2021-04-26 12:26:21.000000 lona-1.8.5/lona/shell/commands/lona_server_state.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1398 2021-09-17 17:36:27.000000 lona-1.8.5/lona/shell/commands/lona_settings.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1969 2021-09-17 17:36:27.000000 lona-1.8.5/lona/shell/commands/lona_static_files.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2021 2021-09-17 17:36:27.000000 lona-1.8.5/lona/shell/commands/lona_templates.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     9182 2021-10-04 16:21:33.000000 lona-1.8.5/lona/shell/commands/lona_views.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      574 2021-04-15 06:55:45.000000 lona-1.8.5/lona/shell/shell.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.490688 lona-1.8.5/lona/static/
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.502688 lona-1.8.5/lona/static/lona/
--rw-r--r--   0 fsc       (1000) fsc       (1000)       57 2021-09-15 13:54:46.000000 lona-1.8.5/lona/static/lona/style.css
--rw-r--r--   0 fsc       (1000) fsc       (1000)     7843 2021-11-02 17:17:07.000000 lona-1.8.5/lona/static_file_loader.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      577 2021-10-04 16:21:33.000000 lona-1.8.5/lona/static_files.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.490688 lona-1.8.5/lona/templates/
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.506688 lona-1.8.5/lona/templates/lona/
--rw-r--r--   0 fsc       (1000) fsc       (1000)       30 2021-08-04 18:06:00.000000 lona-1.8.5/lona/templates/lona/403.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)       30 2020-09-08 19:30:05.000000 lona-1.8.5/lona/templates/lona/404.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)       35 2020-09-08 19:30:05.000000 lona-1.8.5/lona/templates/lona/500.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-09-15 13:54:46.000000 lona-1.8.5/lona/templates/lona/footer.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)      660 2021-09-15 13:54:46.000000 lona-1.8.5/lona/templates/lona/frontend.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)      140 2021-09-15 13:54:46.000000 lona-1.8.5/lona/templates/lona/frontend.js
--rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-09-15 13:54:46.000000 lona-1.8.5/lona/templates/lona/header.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)      207 2021-03-04 08:15:28.000000 lona-1.8.5/lona/templates/lona/script_tags.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)      144 2020-12-08 20:10:22.000000 lona-1.8.5/lona/templates/lona/style_tags.html
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4029 2021-12-05 20:38:56.000000 lona-1.8.5/lona/templating.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)      451 2021-09-15 14:02:28.000000 lona-1.8.5/lona/unique_ids.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    10043 2021-11-11 10:21:34.000000 lona-1.8.5/lona/view.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4161 2021-11-11 10:21:34.000000 lona-1.8.5/lona/view_loader.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    26660 2021-11-24 10:23:27.000000 lona-1.8.5/lona/view_runtime.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)    12979 2021-11-02 17:17:07.000000 lona-1.8.5/lona/view_runtime_controller.py
--rw-r--r--   0 fsc       (1000) fsc       (1000)     1307 2021-09-17 17:36:27.000000 lona-1.8.5/lona/worker_pool.py
-drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2021-12-15 11:49:00.494688 lona-1.8.5/lona.egg-info/
--rw-r--r--   0 fsc       (1000) fsc       (1000)     4380 2021-12-15 11:49:00.000000 lona-1.8.5/lona.egg-info/PKG-INFO
--rw-r--r--   0 fsc       (1000) fsc       (1000)     2639 2021-12-15 11:49:00.000000 lona-1.8.5/lona.egg-info/SOURCES.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)        1 2021-12-15 11:49:00.000000 lona-1.8.5/lona.egg-info/dependency_links.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)       31 2021-12-15 11:49:00.000000 lona-1.8.5/lona.egg-info/entry_points.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)       48 2021-12-15 11:49:00.000000 lona-1.8.5/lona.egg-info/requires.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)        5 2021-12-15 11:49:00.000000 lona-1.8.5/lona.egg-info/top_level.txt
--rw-r--r--   0 fsc       (1000) fsc       (1000)      600 2021-12-15 11:49:00.506688 lona-1.8.5/setup.cfg
--rwxr-xr-x   0 fsc       (1000) fsc       (1000)      636 2021-10-04 16:21:33.000000 lona-1.8.5/setup.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.909571 lona-1.9/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1071 2020-09-08 19:30:05.000000 lona-1.9/LICENSE.txt
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      181 2021-09-15 13:54:46.000000 lona-1.9/MANIFEST.in
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     4466 2022-01-28 19:34:54.909571 lona-1.9/PKG-INFO
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2906 2022-01-25 14:45:31.000000 lona-1.9/README.rst
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.897571 lona-1.9/bin/
+-rwxr-xr-x   0 fsc       (1000) fsc       (1000)      160 2021-04-26 12:26:21.000000 lona-1.9/bin/lona
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.901571 lona-1.9/lona/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      428 2022-01-28 18:51:49.000000 lona-1.9/lona/__init__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      152 2022-01-26 22:07:00.000000 lona-1.9/lona/__main__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      456 2021-07-15 08:55:51.000000 lona-1.9/lona/_json.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    12118 2022-01-28 07:40:46.000000 lona-1.9/lona/app.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.901571 lona-1.9/lona/client/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     9332 2021-11-09 17:42:41.000000 lona-1.9/lona/client/context.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     5257 2021-10-04 16:21:33.000000 lona-1.9/lona/client/dom-renderer.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    16035 2021-10-04 16:21:33.000000 lona-1.9/lona/client/dom-updater.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    10988 2022-01-10 13:20:17.000000 lona-1.9/lona/client/input-events.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1015 2021-08-09 06:36:12.000000 lona-1.9/lona/client/job-queue.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1749 2021-07-15 08:55:51.000000 lona-1.9/lona/client/lona.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2047 2021-07-15 08:55:51.000000 lona-1.9/lona/client/widget-data-updater.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      645 2021-09-17 17:36:27.000000 lona-1.9/lona/client/window-shim.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    12583 2021-11-09 17:42:41.000000 lona-1.9/lona/client/window.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2143 2022-01-28 07:39:59.000000 lona-1.9/lona/client_pre_compiler.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.905571 lona-1.9/lona/command_line/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-04-28 08:10:35.000000 lona-1.9/lona/command_line/__init__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2771 2022-01-19 08:43:40.000000 lona-1.9/lona/command_line/collect_static.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     5349 2021-11-24 09:58:43.000000 lona-1.9/lona/command_line/handle_command_line.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     3241 2022-01-19 08:43:40.000000 lona-1.9/lona/command_line/run_server.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      594 2021-09-15 14:02:28.000000 lona-1.9/lona/command_line/terminal.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      881 2022-01-28 07:39:59.000000 lona-1.9/lona/connection.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       85 2021-10-04 16:21:33.000000 lona-1.9/lona/default_routes.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2560 2021-12-05 20:38:56.000000 lona-1.9/lona/default_settings.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1759 2022-01-19 08:43:40.000000 lona-1.9/lona/default_views.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      241 2021-11-24 10:23:27.000000 lona-1.9/lona/errors.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.905571 lona-1.9/lona/events/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       52 2021-09-17 17:36:27.000000 lona-1.9/lona/events/__init__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1401 2022-01-10 13:20:17.000000 lona-1.9/lona/events/event_types.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2527 2022-01-10 13:20:17.000000 lona-1.9/lona/events/input_event.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      287 2022-01-28 07:39:59.000000 lona-1.9/lona/events/view_event.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      119 2020-10-07 06:20:40.000000 lona-1.9/lona/exceptions.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.905571 lona-1.9/lona/html/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      368 2022-01-10 13:20:17.000000 lona-1.9/lona/html/__init__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     4137 2022-01-10 13:20:17.000000 lona-1.9/lona/html/abstract_node.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     6142 2022-01-19 08:43:40.000000 lona-1.9/lona/html/attribute_dict.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     4157 2021-10-04 16:21:33.000000 lona-1.9/lona/html/attribute_list.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.905571 lona-1.9/lona/html/data_binding/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-02-05 16:46:07.000000 lona-1.9/lona/html/data_binding/__init__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     8423 2022-01-10 13:20:17.000000 lona-1.9/lona/html/data_binding/inputs.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     3966 2022-01-10 13:20:17.000000 lona-1.9/lona/html/data_binding/select.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2140 2021-11-16 19:55:44.000000 lona-1.9/lona/html/document.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    10516 2022-01-10 13:20:17.000000 lona-1.9/lona/html/node.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2420 2021-09-17 17:36:27.000000 lona-1.9/lona/html/node_event_list.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     5963 2021-11-11 10:21:34.000000 lona-1.9/lona/html/node_list.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     3672 2021-11-02 17:17:07.000000 lona-1.9/lona/html/nodes.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     5670 2021-10-04 16:21:33.000000 lona-1.9/lona/html/parsing.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      772 2021-09-17 17:36:27.000000 lona-1.9/lona/html/patches.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     3093 2022-01-28 07:39:59.000000 lona-1.9/lona/html/selector.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1912 2021-10-04 16:21:33.000000 lona-1.9/lona/html/text_node.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2237 2021-10-04 16:21:33.000000 lona-1.9/lona/html/widget.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    13098 2021-11-22 14:37:19.000000 lona-1.9/lona/html/widget_data.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2223 2021-11-11 10:21:34.000000 lona-1.9/lona/html/widgets.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1546 2021-10-04 16:21:33.000000 lona-1.9/lona/imports.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     6466 2021-12-15 11:08:37.000000 lona-1.9/lona/logging.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     5928 2021-10-04 16:21:33.000000 lona-1.9/lona/middleware_controller.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.909571 lona-1.9/lona/middlewares/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-07-15 13:23:46.000000 lona-1.9/lona/middlewares/__init__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      965 2022-01-19 08:43:40.000000 lona-1.9/lona/middlewares/lona_messages.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2619 2022-01-19 08:43:40.000000 lona-1.9/lona/middlewares/sessions.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     5048 2022-01-10 13:20:17.000000 lona-1.9/lona/protocol.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     6556 2022-01-28 07:39:59.000000 lona-1.9/lona/pytest.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1034 2021-09-15 14:02:28.000000 lona-1.9/lona/request.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     4244 2022-01-19 08:43:40.000000 lona-1.9/lona/response_parser.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     5764 2021-11-11 10:21:34.000000 lona-1.9/lona/routing.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    25250 2022-01-28 07:39:59.000000 lona-1.9/lona/server.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1748 2021-08-09 06:36:12.000000 lona-1.9/lona/server_state.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1738 2021-10-04 16:21:33.000000 lona-1.9/lona/settings.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.909571 lona-1.9/lona/shell/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-04-15 06:55:45.000000 lona-1.9/lona/shell/__init__.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.909571 lona-1.9/lona/shell/commands/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-04-15 06:55:45.000000 lona-1.9/lona/shell/commands/__init__.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      806 2022-01-19 08:43:40.000000 lona-1.9/lona/shell/commands/lona_connections.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      933 2021-11-24 09:58:43.000000 lona-1.9/lona/shell/commands/lona_info.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1145 2022-01-19 08:43:40.000000 lona-1.9/lona/shell/commands/lona_middlewares.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1864 2022-01-19 08:43:40.000000 lona-1.9/lona/shell/commands/lona_routes.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      879 2021-04-26 12:26:21.000000 lona-1.9/lona/shell/commands/lona_server_state.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1398 2021-09-17 17:36:27.000000 lona-1.9/lona/shell/commands/lona_settings.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1972 2022-01-19 08:43:40.000000 lona-1.9/lona/shell/commands/lona_static_files.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1967 2022-01-19 08:43:40.000000 lona-1.9/lona/shell/commands/lona_templates.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     9187 2022-01-19 08:43:40.000000 lona-1.9/lona/shell/commands/lona_views.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      574 2021-04-15 06:55:45.000000 lona-1.9/lona/shell/shell.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.893571 lona-1.9/lona/static/
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.909571 lona-1.9/lona/static/lona/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       57 2021-09-15 13:54:46.000000 lona-1.9/lona/static/lona/style.css
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     7799 2022-01-28 07:39:59.000000 lona-1.9/lona/static_file_loader.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      577 2021-10-04 16:21:33.000000 lona-1.9/lona/static_files.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.893571 lona-1.9/lona/templates/
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.909571 lona-1.9/lona/templates/lona/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       30 2021-08-04 18:06:00.000000 lona-1.9/lona/templates/lona/403.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       30 2020-09-08 19:30:05.000000 lona-1.9/lona/templates/lona/404.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       35 2020-09-08 19:30:05.000000 lona-1.9/lona/templates/lona/500.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-09-15 13:54:46.000000 lona-1.9/lona/templates/lona/footer.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      660 2021-09-15 13:54:46.000000 lona-1.9/lona/templates/lona/frontend.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      140 2021-09-15 13:54:46.000000 lona-1.9/lona/templates/lona/frontend.js
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        0 2021-09-15 13:54:46.000000 lona-1.9/lona/templates/lona/header.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      207 2021-03-04 08:15:28.000000 lona-1.9/lona/templates/lona/script_tags.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      144 2020-12-08 20:10:22.000000 lona-1.9/lona/templates/lona/style_tags.html
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     4033 2022-01-19 08:43:40.000000 lona-1.9/lona/templating.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      451 2021-09-15 14:02:28.000000 lona-1.9/lona/unique_ids.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    10810 2022-01-28 07:39:59.000000 lona-1.9/lona/view.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     4162 2022-01-19 08:43:40.000000 lona-1.9/lona/view_loader.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    26739 2022-01-28 07:39:59.000000 lona-1.9/lona/view_runtime.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)    13451 2022-01-28 07:39:59.000000 lona-1.9/lona/view_runtime_controller.py
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     1307 2022-01-18 10:43:20.000000 lona-1.9/lona/worker_pool.py
+drwxr-xr-x   0 fsc       (1000) fsc       (1000)        0 2022-01-28 19:34:54.901571 lona-1.9/lona.egg-info/
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     4466 2022-01-28 19:34:54.000000 lona-1.9/lona.egg-info/PKG-INFO
+-rw-r--r--   0 fsc       (1000) fsc       (1000)     2639 2022-01-28 19:34:54.000000 lona-1.9/lona.egg-info/SOURCES.txt
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        1 2022-01-28 19:34:54.000000 lona-1.9/lona.egg-info/dependency_links.txt
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       31 2022-01-28 19:34:54.000000 lona-1.9/lona.egg-info/entry_points.txt
+-rw-r--r--   0 fsc       (1000) fsc       (1000)       48 2022-01-28 19:34:54.000000 lona-1.9/lona.egg-info/requires.txt
+-rw-r--r--   0 fsc       (1000) fsc       (1000)        5 2022-01-28 19:34:54.000000 lona-1.9/lona.egg-info/top_level.txt
+-rw-r--r--   0 fsc       (1000) fsc       (1000)      600 2022-01-28 19:34:54.913571 lona-1.9/setup.cfg
+-rwxr-xr-x   0 fsc       (1000) fsc       (1000)      634 2022-01-25 14:45:31.000000 lona-1.9/setup.py
```

### Comparing `lona-1.8.5/LICENSE.txt` & `lona-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/PKG-INFO` & `lona-1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: lona
-Version: 1.8.5
+Version: 1.9
 Summary: Write responsive web apps in full python
 Home-page: https://github.com/lona-web-org/lona
 Author: Florian Scherf
-Author-email: f.scherf@pengutronix.de
+Author-email: mail@florianscherf.de
 License: MIT
 Description: .. image:: doc/content/logo.svg
             :alt: Lona logo
             :height: 200px
             :width: 200px
         .. image:: https://img.shields.io/pypi/l/lona.svg
             :alt: license MIT
@@ -36,14 +36,16 @@
         
         **Documentation:** `lona-web.org <http://lona-web.org>`_
         
         **Changelog:** `lona-web.org/changelog <http://lona-web.org/changelog.html>`_
         
         **Reddit:** `reddit.com/r/lona_web_org/ <https://www.reddit.com/r/lona_web_org/>`_
         
+        **Discord:** `discord.com/lona-web.org <https://discord.gg/WBf5PVACsj>`_
+        
         Web is a solved problem in Python since ages, but traditionally Python handles
         only the server side. If you want to have client side interaction like
         click events or you want update content live, you have to write an additional
         Javascript application.
         
         Lona handles the server side and the client side, and provides a simple,
         pythonic API to write self contained views.
```

### Comparing `lona-1.8.5/README.rst` & `lona-1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 **Documentation:** `lona-web.org <http://lona-web.org>`_
 
 **Changelog:** `lona-web.org/changelog <http://lona-web.org/changelog.html>`_
 
 **Reddit:** `reddit.com/r/lona_web_org/ <https://www.reddit.com/r/lona_web_org/>`_
 
+**Discord:** `discord.com/lona-web.org <https://discord.gg/WBf5PVACsj>`_
+
 Web is a solved problem in Python since ages, but traditionally Python handles
 only the server side. If you want to have client side interaction like
 click events or you want update content live, you have to write an additional
 Javascript application.
 
 Lona handles the server side and the client side, and provides a simple,
 pythonic API to write self contained views.
```

### Comparing `lona-1.8.5/lona/app.py` & `lona-1.9/lona/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,27 +79,28 @@
             self,
             # 1 = lona.MATCH_ALL  https://github.com/python/mypy/issues/10026
             raw_pattern: str | Literal[1],
             name: str = '',
             interactive: bool = True,
             http_pass_through: bool = False,
             frontend_view: None | str | LonaView = None,
-    ) -> Callable[[type[LonaView]], None]:
+    ) -> Callable[[type[LonaView]], type[LonaView]]:
 
-        def decorator(view_class: type[LonaView]) -> None:
+        def decorator(view_class: type[LonaView]) -> type[LonaView]:
             self.routes.append(
                 Route(
                     raw_pattern=raw_pattern,
                     view=view_class,
                     name=name,
                     interactive=interactive,
                     http_pass_through=http_pass_through,
                     frontend_view=frontend_view,
                 ),
             )
+            return view_class
 
         return decorator
 
     # middleware
     @overload
     def middleware(self) -> Callable[[type], None]:
         ...
@@ -411,16 +412,16 @@
         )
 
         # setup worker pool
         worker_pool = WorkerPool(
             settings=self.server.settings,
         )
 
-        self.server.set_loop(loop)
-        self.server.set_worker_pool(worker_pool)
+        self.server._loop = loop
+        self.server._worker_pool = worker_pool
 
     def run(
             self,
             loop: None | AbstractEventLoop = None,
             parse_command_line: bool = True,
             **args: Any,
     ) -> None:
```

### Comparing `lona-1.8.5/lona/client/context.js` & `lona-1.9/lona/client/context.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/client/dom-renderer.js` & `lona-1.9/lona/client/dom-renderer.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/client/dom-updater.js` & `lona-1.9/lona/client/dom-updater.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/client/input-events.js` & `lona-1.9/lona/client/input-events.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -41,14 +41,16 @@
         return value;
     };
 
     this._clear_input_events = function(node) {
         node.onclick = undefined;
         node.oninput = undefined;
         node.onchange = undefined;
+        node.onfocus = undefined;
+        node.onblur = undefined;
     };
 
     this._patch_link = function(node) {
         var lona_window = this.lona_window;
 
         node.onclick = function(event) {
             event.preventDefault();
@@ -219,14 +221,60 @@
 
             };
 
             return false;
         };
     };
 
+    this._patch_onfocus = function(node, event_type) {
+        var input_event_handler = this;
+        var lona_window = this.lona_window;
+
+        node.onfocus = function(event) {
+            event.preventDefault();
+
+            try {
+                input_event_handler.fire_input_event(
+                    node,
+                    Lona.protocol.INPUT_EVENT_TYPE.FOCUS,
+                    undefined,
+                );
+
+            } catch (error) {
+                lona_window.crash(error);
+
+            };
+
+            return false;
+        };
+    };
+
+    this._patch_onblur = function(node, event_type) {
+        var input_event_handler = this;
+        var lona_window = this.lona_window;
+
+        node.onblur = function(event) {
+            event.preventDefault();
+
+            try {
+                input_event_handler.fire_input_event(
+                    node,
+                    Lona.protocol.INPUT_EVENT_TYPE.BLUR,
+                    undefined,
+                );
+
+            } catch (error) {
+                lona_window.crash(error);
+
+            };
+
+            return false;
+        };
+    };
+
     this._parse_data_lona_events = function(node) {
         var event_types = {};
 
         if (!node.hasAttribute('data-lona-events')) {
             return event_types;
         };
 
@@ -281,14 +329,22 @@
             } else if (key == Lona.protocol.INPUT_EVENT_TYPE.CHANGE) {
                 _this._patch_onchange(node, event_type);
 
                 // onsubmit
             } else if (key == Lona.protocol.INPUT_EVENT_TYPE.SUBMIT) {
                 _this._patch_onsubmit(node, event_type);
 
+                // onfocus
+            } else if (key == Lona.protocol.INPUT_EVENT_TYPE.FOCUS) {
+                _this._patch_onfocus(node, event_type);
+
+                // onblur
+            } else if (key == Lona.protocol.INPUT_EVENT_TYPE.BLUR) {
+                _this._patch_onblur(node, event_type);
+
             };
         });
     };
 
     this.fire_input_event = function(node, event_type, data) {
         var _this = this;
```

### Comparing `lona-1.8.5/lona/client/job-queue.js` & `lona-1.9/lona/client/job-queue.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/client/lona.js` & `lona-1.9/lona/client/lona.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/client/widget-data-updater.js` & `lona-1.9/lona/client/widget-data-updater.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/client/window-shim.js` & `lona-1.9/lona/client/window-shim.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/client/window.js` & `lona-1.9/lona/client/window.js`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/command_line/collect_static.py` & `lona-1.9/lona/command_line/collect_static.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,27 +76,27 @@
     # clean
     if args.clean:
         for name in os.listdir(args.destination):
             path = os.path.join(args.destination, name)
             _rm(path)
 
     # copy node static files
-    for static_file in server.static_file_loader.static_files[::-1]:
+    for static_file in server._static_file_loader.static_files[::-1]:
         if not static_file.enabled:
             continue
 
         destination = os.path.join(
             args.destination,
             static_file.url,
         )
 
         _cp(static_file.path, destination)
 
     # copy static files from static directories
-    for static_dir in server.static_file_loader.static_dirs[::-1]:
+    for static_dir in server._static_file_loader.static_dirs[::-1]:
         for name in os.listdir(static_dir):
             source = os.path.join(static_dir, name)
             destination = os.path.join(args.destination, name)
 
             _cp(source, destination)
 
     # copy client
@@ -107,8 +107,8 @@
 
     destination = os.path.join(
         args.destination,
         client_url,
     )
 
     _mkdir(os.path.dirname(destination))
-    _cp(server.client_pre_compiler.resolve(), destination)
+    _cp(server._client_pre_compiler.resolve(), destination)
```

### Comparing `lona-1.8.5/lona/command_line/handle_command_line.py` & `lona-1.9/lona/command_line/handle_command_line.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/command_line/run_server.py` & `lona-1.9/lona/command_line/run_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     async def shutdown(app):
         server = app['lona_server']
 
         await server.loop.run_in_executor(None, server.worker_pool.shutdown)
 
     app.on_shutdown.append(shutdown)
 
-    server.set_loop(loop)
-    server.set_worker_pool(worker_pool)
+    server._loop = loop
+    server._worker_pool = worker_pool
 
     # run server
     if args.shell:
         async def start_shell(server):
             def _start_shell():
                 embed_kwargs = {
                     'locals': {
```

### Comparing `lona-1.8.5/lona/command_line/terminal.py` & `lona-1.9/lona/command_line/terminal.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/connection.py` & `lona-1.9/lona/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,13 +29,7 @@
 
         # this exception gets handled by aiohttp internally and can be ignored
         with contextlib.suppress(ConnectionResetError):
             return self.server.run_coroutine_sync(
                 self.websocket.send_str(string),
                 wait=wait,
             )
-
-    async def close(self):
-        if not self.interactive:
-            raise NotInteractiveError
-
-        await self.websocket.close()
```

### Comparing `lona-1.8.5/lona/default_settings.py` & `lona-1.9/lona/default_settings.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/default_views.py` & `lona-1.9/lona/default_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         }
 
     def handle_request(self, request, **extra_context):
         view_setting = request.server.settings.get(self.VIEW_SETTING, '')
 
         if view_setting:
             try:
-                view_class = request.server.view_loader.load(view_setting)
+                view_class = request.server._view_loader.load(view_setting)
 
                 view = view_class(
                     server=self.server,
                     view_runtime=self._view_runtime,
                     request=request,
                 )
```

### Comparing `lona-1.8.5/lona/events/event_types.py` & `lona-1.9/lona/events/event_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,8 +45,10 @@
         if self._input_delay:
             return f'{self._symbol.value}:{self._input_delay}'
 
         return str(self._symbol.value)
 
 
 CLICK = EventType('CLICK', INPUT_EVENT_TYPE.CLICK)
+FOCUS = EventType('FOCUS', INPUT_EVENT_TYPE.FOCUS)
+BLUR = EventType('BLUR', INPUT_EVENT_TYPE.BLUR)
 CHANGE = ChangeEventType('CHANGE', INPUT_EVENT_TYPE.CHANGE)
```

### Comparing `lona-1.8.5/lona/events/input_event.py` & `lona-1.9/lona/events/input_event.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,14 +34,26 @@
 
         elif payload[1] == INPUT_EVENT_TYPE.CHANGE:
             self.type = INPUT_EVENT_TYPE.CHANGE
             self.name = 'change'
             self.data = payload[2]
             self.node_info = payload[3:]
 
+        elif payload[1] == INPUT_EVENT_TYPE.FOCUS:
+            self.type = INPUT_EVENT_TYPE.FOCUS
+            self.name = 'focus'
+            self.data = payload[2]
+            self.node_info = payload[3:]
+
+        elif payload[1] == INPUT_EVENT_TYPE.BLUR:
+            self.type = INPUT_EVENT_TYPE.BLUR
+            self.name = 'blur'
+            self.data = payload[2]
+            self.node_info = payload[3:]
+
         # find node
         # node info contains a lona node id
         if self.node_info[0]:
             self.nodes = document.get_node(node_id=self.node_info[0])
 
             if self.nodes:
                 self.node = self.nodes[0]
```

### Comparing `lona-1.8.5/lona/html/abstract_node.py` & `lona-1.9/lona/html/abstract_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -92,21 +92,33 @@
     # input events ############################################################
     def handle_change(self, input_event):
         return input_event
 
     def handle_click(self, input_event):
         return input_event
 
+    def handle_focus(self, input_event):
+        return input_event
+
+    def handle_blur(self, input_event):
+        return input_event
+
     def handle_input_event(self, input_event):
         if input_event.name == 'change':
             return self.handle_change(input_event)
 
         elif input_event.name == 'click':
             return self.handle_click(input_event)
 
+        elif input_event.name == 'focus':
+            return self.handle_focus(input_event)
+
+        elif input_event.name == 'blur':
+            return self.handle_blur(input_event)
+
         return input_event
 
     # queries #################################################################
     def iter_nodes(self, node=None):
         if node is None:
             node = self
```

### Comparing `lona-1.8.5/lona/html/attribute_dict.py` & `lona-1.9/lona/html/attribute_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,26 +195,26 @@
 
                 # boolean properties
                 if key in BOOLEAN_ATTRIBUTES:
                     if value is not False:
                         string.append(key)
 
                 else:
-                    string.append(f'{key}="{value}"')
+                    string.append(f'{key}="{html.escape(value)}"')
 
-            return html.escape(' '.join(string))
+            return ' '.join(string)
 
     def to_sub_attribute_string(self):
         with self._node.lock:
             string = []
 
             for key, value in self._attributes.items():
-                string.append(f'{key}: {value}')
+                string.append(f'{key}: {html.escape(value)}')
 
-            return html.escape('; '.join(string))
+            return '; '.join(string)
 
     def __repr__(self):
         return f'<AttributeDict({self._attributes!r})>'
 
 
 class StyleDict(AttributeDict):
     PATCH_TYPE = PATCH_TYPE.STYLE
```

### Comparing `lona-1.8.5/lona/html/attribute_list.py` & `lona-1.9/lona/html/attribute_list.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/data_binding/inputs.py` & `lona-1.9/lona/html/data_binding/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,19 @@
                 issuer=(input_event.connection, input_event.window_id),
             )
 
             self._check_validity()
 
             input_event = self.handle_change(input_event)
 
-        elif input_event.name == 'click':
-            input_event = self.handle_click(input_event)
+            if self.bubble_up:
+                return input_event
 
         else:
-            return input_event
-
-        if self.bubble_up:
-            return input_event
+            return super().handle_input_event(input_event)
 
     # properties ##############################################################
     # value
     @property
     def value(self):
         return self.attributes.get(self.INPUT_ATTRIBUTE_NAME, '')
```

### Comparing `lona-1.8.5/lona/html/data_binding/select.py` & `lona-1.9/lona/html/data_binding/select.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 
     def handle_input_event(self, input_event):
         if input_event.name == 'change':
             self.value = input_event.data
 
             input_event = self.handle_change(input_event)
 
-        elif input_event.name == 'click':
-            input_event = self.handle_click(input_event)
+            if self.bubble_up:
+                return input_event
 
         else:
-            return input_event
-
-        if self.bubble_up:
-            return input_event
+            return super().handle_input_event(input_event)
 
     # properties ##############################################################
     # disabled
     @property
     def disabled(self):
         return 'disabled' in self.attributes
```

### Comparing `lona-1.8.5/lona/html/document.py` & `lona-1.9/lona/html/document.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/node.py` & `lona-1.9/lona/html/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,26 @@
 
             elif name == 'handle-click':  # '_' was replaced to '-' above
                 if not callable(value):
                     raise TypeError('handle_click has to be a function')
 
                 self.handle_click = value
 
+            elif name == 'handle-focus':  # '_' was replaced to '-' above
+                if not callable(value):
+                    raise TypeError('handle_focus has to be a function')
+
+                self.handle_focus = value
+
+            elif name == 'handle-blur':  # '_' was replaced to '-' above
+                if not callable(value):
+                    raise TypeError('handle_blur has to be a function')
+
+                self.handle_blur = value
+
             # misc attributes
             else:
                 self._attributes[name] = value
 
     # node attributes  ########################################################
     # id_list
     @property
```

### Comparing `lona-1.8.5/lona/html/node_event_list.py` & `lona-1.9/lona/html/node_event_list.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/node_list.py` & `lona-1.9/lona/html/node_list.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/nodes.py` & `lona-1.9/lona/html/nodes.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/parsing.py` & `lona-1.9/lona/html/parsing.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/patches.py` & `lona-1.9/lona/html/patches.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/selector.py` & `lona-1.9/lona/html/selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, raw_selector_string):
         self.raw_selector_string = raw_selector_string
 
         self.check_raw_selector_string()
         self.parse_selector()
 
     def __repr__(self):
-        return f'<{self.__class__.__name__}({self.selectors!r})>'
+        return f'<{self.__class__.__name__}({self.selectors!r})>'  # pragma: no cover
 
     def check_raw_selector_string(self):
         match = UNSUPPORTED_CHARACTERS.search(self.raw_selector_string)
 
         if match:
             raise ValueError(
                 f'unsupported selector feature: {match.group()!r}',
```

### Comparing `lona-1.8.5/lona/html/text_node.py` & `lona-1.9/lona/html/text_node.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/widget.py` & `lona-1.9/lona/html/widget.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/widget_data.py` & `lona-1.9/lona/html/widget_data.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/html/widgets.py` & `lona-1.9/lona/html/widgets.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/imports.py` & `lona-1.9/lona/imports.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/logging.py` & `lona-1.9/lona/logging.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/middleware_controller.py` & `lona-1.9/lona/middleware_controller.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/middlewares/lona_messages.py` & `lona-1.9/lona/middlewares/lona_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,14 @@
             return data
 
         if method == METHOD.PING:
             data.connection.send_str(encode_pong(), wait=False)
 
             return
 
-        data.server.view_runtime_controller.handle_lona_message(
+        data.server._view_runtime_controller.handle_lona_message(
             connection=data.connection,
             window_id=window_id,
             view_runtime_id=view_runtime_id,
             method=method,
             payload=payload,
         )
```

### Comparing `lona-1.8.5/lona/middlewares/sessions.py` & `lona-1.9/lona/middlewares/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             acquire,
             data.server.settings.SESSIONS_KEY_GENERATOR,
         )
 
     def handle_connection(self, data):
         http_request = data.connection.http_request
         settings = data.server.settings
-        router = data.server.router
+        router = data.server._router
 
         def get_session_key():
             if settings.SESSIONS_KEY_NAME not in http_request.cookies:
                 return ''
 
             return http_request.cookies[settings.SESSIONS_KEY_NAME]
```

### Comparing `lona-1.8.5/lona/protocol.py` & `lona-1.9/lona/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     PONG = 206
 
 
 class INPUT_EVENT_TYPE(Enum):
     CLICK = 301
     CHANGE = 302
     CUSTOM = 303
+    FOCUS = 304
+    BLUR = 305
 
 
 class NODE_TYPE(Enum):
     NODE = 401
     TEXT_NODE = 402
     WIDGET = 403
```

### Comparing `lona-1.8.5/lona/request.py` & `lona-1.9/lona/request.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/response_parser.py` & `lona-1.9/lona/response_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,23 +114,23 @@
 
             if 'context' in template_context:
                 template_context = template_context['context']
 
             # template file
             if 'template' in raw_response_dict:
                 response_dict['text'] = \
-                    self.server.templating_engine.render_template(
+                    self.server.render_template(
                         raw_response_dict['template'],
                         template_context,
                     )
 
             # template string
             else:
                 response_dict['text'] = \
-                    self.server.templating_engine.render_string(
+                    self.server.render_string(
                         raw_response_dict['template_string'],
                         template_context,
                     )
 
         # json response
         elif 'json' in raw_response_dict:
             logger.debug("'%s' is a json view", view_name)
```

### Comparing `lona-1.8.5/lona/routing.py` & `lona-1.9/lona/routing.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/server_state.py` & `lona-1.9/lona/server_state.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/settings.py` & `lona-1.9/lona/settings.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/shell/commands/lona_connections.py` & `lona-1.9/lona/shell/commands/lona_connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,13 @@
         argument_parser.parse_args(argv[1:])
 
         server = self.repl.locals['server']
 
         # write connections
         rows = [['User', 'URL']]
 
-        for connection in server.websocket_connections:
+        for connection in server._websocket_connections:
             rows.append(
                 [repr(connection.user), connection.http_request.url.path],
             )
 
         write_table(rows, self.repl.write)
```

### Comparing `lona-1.8.5/lona/shell/commands/lona_info.py` & `lona-1.9/lona/shell/commands/lona_info.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/shell/commands/lona_middlewares.py` & `lona-1.9/lona/shell/commands/lona_middlewares.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             prog='lona_middlewares',
             description=self.__doc__,
         )
 
         argument_parser.parse_args(argv[1:])
 
         server = self.repl.locals['server']
-        middleware_controller = server.middleware_controller
+        middleware_controller = server._middleware_controller
 
         # list middlewares
         hook_names = [
             'on_startup',
             'on_shutdown',
             'handle_connection',
             'handle_websocket_message',
```

### Comparing `lona-1.8.5/lona/shell/commands/lona_routes.py` & `lona-1.9/lona/shell/commands/lona_routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,22 +26,22 @@
         arguments = vars(argument_parser.parse_args(argv[1:]))
 
         server = self.repl.locals['server']
 
         # resolve
         if arguments['resolve']:
             path = arguments['resolve']
-            match, route, match_info = server.router.resolve(path)
+            match, route, match_info = server._router.resolve(path)
 
             if not match:
                 self.repl.write('No match')
 
                 return
 
-            route_id = server.router.routes.index(route)
+            route_id = server._router.routes.index(route)
 
             rows = [
                 ['Route ID', route_id],
                 ['Route', repr(route)],
                 ['Match info', repr(match_info)],
             ]
 
@@ -50,23 +50,23 @@
             return
 
         # show given route
         if arguments['route-id']:
             try:
                 route_id = int(arguments['route-id'])
 
-                self.repl.write(repr(server.router.routes[route_id]) + '\n')
+                self.repl.write(repr(server._router.routes[route_id]) + '\n')
 
                 return
 
             except Exception:
                 self.repl.write_error('invalid route id\n')
 
                 return 1
 
         # show all routes
         rows = [['Route ID', 'Route']]
 
-        for index, route in enumerate(server.router.routes):
+        for index, route in enumerate(server._router.routes):
             rows.append([index, repr(route)])
 
         write_table(rows, self.repl.write)
```

### Comparing `lona-1.8.5/lona/shell/commands/lona_server_state.py` & `lona-1.9/lona/shell/commands/lona_server_state.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/shell/commands/lona_settings.py` & `lona-1.9/lona/shell/commands/lona_settings.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/shell/commands/lona_static_files.py` & `lona-1.9/lona/shell/commands/lona_static_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,34 +36,34 @@
 
         args = argument_parser.parse_args(argv[1:])
 
         server = self.repl.locals['server']
 
         # resolve
         if args.resolve:
-            abs_path = server.static_file_loader.resolve_path(args.resolve)
+            abs_path = server._static_file_loader.resolve_path(args.resolve)
 
             if not abs_path:
                 return 1
 
             self.repl.write(f'{abs_path}\n')
 
             return
 
         # list directories
         if args.list_directories:
-            for static_dir in server.static_file_loader.static_dirs:
+            for static_dir in server._static_file_loader.static_dirs:
                 self.repl.write(f'{static_dir}\n')
 
             return
 
         # list static files
         static_files = {}
 
-        for static_dir in server.static_file_loader.static_dirs:
+        for static_dir in server._static_file_loader.static_dirs:
             for root, _dirs, files in os.walk(static_dir):
                 for _file in files:
                     name = os.path.join(root, _file)
 
                     if name in static_files:
                         continue
```

### Comparing `lona-1.8.5/lona/shell/commands/lona_templates.py` & `lona-1.9/lona/shell/commands/lona_templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,34 +38,34 @@
         args = argument_parser.parse_args(argv[1:])
 
         server = self.repl.locals['server']
 
         # resolve
         if args.resolve:
             try:
-                template = server.templating_engine.get_template(args.resolve)
+                template = server.get_template(args.resolve)
 
             except TemplateNotFound:
                 return 1
 
             self.repl.write(f'{template.filename}\n')
 
             return
 
         # list directories
         if args.list_directories:
-            for static_dir in server.templating_engine.template_dirs:
+            for static_dir in server.template_dirs:
                 self.repl.write(f'{static_dir}\n')
 
             return
 
         # list static files
         templates = {}
 
-        for template_dir in server.templating_engine.template_dirs:
+        for template_dir in server.template_dirs:
             for root, _dirs, files in os.walk(template_dir):
                 for _file in files:
                     name = os.path.join(root, _file)
 
                     if name in templates:
                         continue
```

### Comparing `lona-1.8.5/lona/shell/commands/lona_views.py` & `lona-1.9/lona/shell/commands/lona_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     NAME = 'lona_views'
 
     def __init__(self, repl):
         self.repl = repl
 
     def complete(self, text, state, line_buffer):
         server = self.repl.locals['server']
-        controller = server.view_runtime_controller
+        controller = server._view_runtime_controller
 
         view_runtime_ids = []
 
         for view_runtime in controller.iter_view_runtimes():
             view_runtime_ids.append(view_runtime.view_runtime_id)
 
         view_runtime_ids = sorted(view_runtime_ids)
@@ -121,15 +121,15 @@
         if arguments['runtime-id']:
             return self.show_view_info(arguments)
 
         return self.list_views(arguments)
 
     def show_view_memory(self, arguments):
         server = self.repl.locals['server']
-        controller = server.view_runtime_controller
+        controller = server._view_runtime_controller
 
         if not arguments['runtime-id']:
             self.repl.write_error('no runtime id given')
 
             return 1
 
         try:
@@ -165,15 +165,15 @@
                 rows.append([key, pformat(value)])
 
             write_table(rows, self.repl.write)
             self.repl.write('\n\n')
 
     def show_view_info(self, arguments):
         server = self.repl.locals['server']
-        controller = server.view_runtime_controller
+        controller = server._view_runtime_controller
 
         try:
             view_runtime = controller.get_view_runtime(
                 view_runtime_id=arguments['runtime-id'],
             )
 
         except Exception:
@@ -260,27 +260,27 @@
             for line in traceback.format_list(frame_summary_list):
                 self.repl.write(line)
 
         self.repl.write('\n')
 
     def list_views(self, arguments):
         server = self.repl.locals['server']
-        controller = server.view_runtime_controller
+        controller = server._view_runtime_controller
 
         rows = [
             ['Runtime ID', 'Thread ID', 'Flags', 'User', 'Route ID',
              'URL', 'State'],
         ]
 
         for view_runtime in controller.iter_view_runtimes():
             # find route id
             route = view_runtime.route
 
             if route:
-                route_id = server.router.routes.index(view_runtime.route)
+                route_id = server._router.routes.index(view_runtime.route)
 
                 url = route.format_string.format(
                     **view_runtime.request.match_info)
 
             else:
                 # in case of 404 or 500 responses the runtime
                 # may have no route set
```

### Comparing `lona-1.8.5/lona/shell/shell.py` & `lona-1.9/lona/shell/shell.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/static_file_loader.py` & `lona-1.9/lona/static_file_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 from lona.static_files import StyleSheet, StaticFile, Script
 from lona.imports import get_all_subclasses, get_file
 from lona.html.abstract_node import AbstractNode
 
 # avoid import cycles
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from lona.server import LonaServer
 
 
 logger = logging.getLogger('lona.static_file_loader')
 
 
 class StaticFileLoader:
@@ -42,24 +42,24 @@
         logger.debug('%d stylesheets discovered', len(self.stylesheets))
         logger.debug('%d scripts discovered', len(self.scripts))
 
         # render html files
         logger.debug('rendering html files')
 
         # stylesheets
-        self.style_tags_html: str = self.server.templating_engine.render_template(  # NOQA: LN001
+        self.style_tags_html: str = self.server.render_template(
             self.server.settings.STATIC_FILES_STYLE_TAGS_TEMPLATE,
             {
                 'stylesheets': [i for i in self.stylesheets
                                 if i.enabled and i.link],
             },
         )
 
         # scripts
-        self.script_tags_html: str = self.server.templating_engine.render_template(  # NOQA: LN001
+        self.script_tags_html: str = self.server.render_template(
             self.server.settings.STATIC_FILES_SCRIPT_TAGS_TEMPLATE,
             {
                 'scripts': [i for i in self.scripts
                             if i.enabled and i.link],
             },
         )
 
@@ -68,15 +68,15 @@
         node_classes = [AbstractNode] + list(get_all_subclasses(AbstractNode))
         logger.debug('%d node classes discovered', len(node_classes))
 
         for node_class in node_classes:
             yield node_class, iter(node_class.STATIC_FILES)
 
         logger.debug('discover view classes')
-        view_classes = self.server.view_loader.get_all_views()
+        view_classes = self.server._view_loader.get_all_views()
         logger.debug('%d view classes discovered', len(view_classes))
 
         for view_class in view_classes:
             if not hasattr(view_class, 'STATIC_FILES'):
                 continue
 
             yield view_class, iter(view_class.STATIC_FILES)
@@ -214,15 +214,15 @@
 
         if client_url.startswith('/'):
             client_url = client_url[1:]
 
         if rel_path == client_url:
             logger.debug('returning javascript client')
 
-            return self.server.client_pre_compiler.resolve()
+            return self.server._client_pre_compiler.resolve()
 
         # searching in static dirs
         for static_dir in self.static_dirs:
             abs_path = os.path.join(static_dir, rel_path)
 
             logger.debug("trying '%s'", abs_path)
```

### Comparing `lona-1.8.5/lona/static_files.py` & `lona-1.9/lona/static_files.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/templates/lona/frontend.html` & `lona-1.9/lona/templates/lona/frontend.html`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona/templating.py` & `lona-1.9/lona/templating.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,36 +17,36 @@
 
 class Namespace:
     def __init__(self, server, templating_engine):
         self.server = server
         self.templating_engine = templating_engine
 
     def load_stylesheets(self):
-        return self.server.static_file_loader.style_tags_html
+        return self.server._static_file_loader.style_tags_html
 
     def load_scripts(self):
-        return self.server.static_file_loader.script_tags_html
+        return self.server._static_file_loader.script_tags_html
 
     def _import(self, *args, **kwargs):
         return self.server.acquire(*args, **kwargs)
 
     def resolve_url(self, *args, **kwargs):
-        return self.server.router.reverse(*args, **kwargs)
+        return self.server._router.reverse(*args, **kwargs)
 
     def load_static_file(self, path):
         logger.debug('resolving static file path %s', path)
 
         if path.startswith('/'):
             path = path[1:]
 
         if path in self.templating_engine.static_path_cache:
             logger.debug('%s is cached', path)
 
         else:
-            resolved_path = self.server.static_file_loader.resolve_path(path)
+            resolved_path = self.server._static_file_loader.resolve_path(path)
 
             if not resolved_path:
                 logger.error("static file '%s' was not found", path)
 
                 return ''
 
             self.templating_engine.static_path_cache.append(path)
```

### Comparing `lona-1.8.5/lona/view.py` & `lona-1.9/lona/view.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 from typing import TYPE_CHECKING, overload, TypeVar, Union, cast
 from collections.abc import Awaitable, Callable
 import threading
 import asyncio
 
 from typing_extensions import Literal
-from jinja2.nodes import Template
 
 from lona.view_runtime import VIEW_RUNTIME_STATE, ViewRuntime
 from lona.html.abstract_node import AbstractNode
 from lona.events.input_event import InputEvent
 from lona.static_files import StaticFile
 from lona.connection import Connection
 from lona.request import Request
 
 # avoid import cycles
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from lona.events.view_event import ViewEvent
     from lona.server import LonaServer
 
 T = TypeVar('T')
 V = TypeVar('V', bound='LonaView')
 H = Union[None, AbstractNode, str]
 
@@ -98,16 +97,16 @@
         finally:
             self._view_runtime.state = VIEW_RUNTIME_STATE.RUNNING
 
     # html ####################################################################
     def show(
             self,
             html: H = None,
-            template: None | str | Template = None,
-            template_string: None | str | Template = None,
+            template: None | str = None,
+            template_string: None | str = None,
             title: None | str = None,
             template_context: None | dict = None,
     ) -> None:
         self._assert_not_main_thread()
         self._assert_view_is_interactive()
         self._assert_view_is_running()
 
@@ -116,23 +115,23 @@
             template_context = template_context or {}
 
             if 'template_context' in template_context:
                 template_context = template_context['template_context']
 
             # string based templates
             if template_string:
-                html = self._server.templating_engine.render_string(
+                html = self._server.render_string(
                     template_string=template_string,
                     template_context=template_context,
                 )
 
             # file based templates
             else:
-                html = self._server.templating_engine.render_template(
-                    template_name=template,
+                html = self._server.render_template(
+                    template_name=cast(str, template),
                     template_context=template_context,
                 )
 
         with self._view_runtime.document.lock:
             html = html or self._view_runtime.document.html
             data = self._view_runtime.document.apply(html)
 
@@ -157,15 +156,15 @@
     ) -> None:
         self._assert_not_main_thread()
         self._assert_view_is_interactive()
         self._assert_view_is_running()
 
         # broadcast
         if broadcast:
-            for connection in self.server.websocket_connections.copy():
+            for connection in self.server._websocket_connections.copy():
                 if not filter_connections(connection):
                     continue
 
                 connection.send_str(string, wait=wait)
 
         # view local
         else:
@@ -249,17 +248,47 @@
     def await_change(self, *nodes, html=None):
         return self._await_specific_input_event(
             *nodes,
             event_type='change',
             html=html,
         )
 
+    @overload
+    def await_focus(self, *nodes: AbstractNode, html: H = None) -> InputEvent:
+        ...
+
+    @overload
+    def await_focus(self, __nodes: list[AbstractNode], html: H = None) -> InputEvent:  # NOQA: LN001
+        ...
+
+    def await_focus(self, *nodes, html=None):
+        return self._await_specific_input_event(
+            *nodes,
+            event_type='focus',
+            html=html,
+        )
+
+    @overload
+    def await_blur(self, *nodes: AbstractNode, html: H = None) -> InputEvent:
+        ...
+
+    @overload
+    def await_blur(self, __nodes: list[AbstractNode], html: H = None) -> InputEvent:  # NOQA: LN001
+        ...
+
+    def await_blur(self, *nodes, html=None):
+        return self._await_specific_input_event(
+            *nodes,
+            event_type='blur',
+            html=html,
+        )
+
     # view events #############################################################
     def fire_view_event(self, name: str, data: dict | None = None) -> None:
-        self.server.view_runtime_controller.fire_view_event(
+        self.server._view_runtime_controller.fire_view_event(
             name=name,
             data=data,
             view_classes=[self.__class__],
         )
 
     # runtime #################################################################
     @overload
```

### Comparing `lona-1.8.5/lona/view_loader.py` & `lona-1.9/lona/view_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     def setup(self):
         # views
         logger.debug('loading views from routes')
 
         self._cache = {}
 
-        for route in self.server.router.routes:
+        for route in self.server._router.routes:
             self._cache_view(
                 route=route,
                 view=route.view,
             )
 
             if route.frontend_view:
                 self._cache_view(
```

### Comparing `lona-1.8.5/lona/view_runtime.py` & `lona-1.9/lona/view_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from lona.unique_ids import generate_unique_id
 from lona.events.input_event import InputEvent
 from lona.imports import get_object_repr
 from lona.html.document import Document
 from lona.request import Request
 
 # avoid import cycles
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from lona.server import LonaServer
 
 
 logger = logging.getLogger('lona.view_runtime')
 input_events_logger = logging.getLogger('lona.input_events')
 
 
@@ -81,15 +81,15 @@
 
         if frontend:
             self.view = self.server.settings.CORE_FRONTEND_VIEW
 
             if route and route.frontend_view:
                 self.view = route.frontend_view
 
-        self.view_class = self.server.view_loader.load(self.view)
+        self.view_class = self.server._view_loader.load(self.view)
         self.name = repr(self.view_class)
 
         self.view = self.view_class(
             server=self.server,
             view_runtime=self,
             request=self.request,
         )
@@ -114,14 +114,16 @@
         self.started_at = None
         self.stopped_at = None
 
         self.pending_input_events = {
             'event': None,
             'click': None,
             'change': None,
+            'focus': None,
+            'blur': None,
         }
 
     # state ###################################################################
     @property
     def state(self):
         if self.is_stopped:
             if self.stop_reason is not None:
@@ -152,15 +154,15 @@
             send_view_stop: bool = False,
             connections: dict | None = None,
     ) -> Dict[str, Any]:
 
         if send_view_start:
             self.send_view_start(connections=connections)
 
-        view_class = self.server.view_loader.load(view_name)
+        view_class = self.server._view_loader.load(view_name)
 
         view = view_class(
             server=self.server,
             view_runtime=self,
             request=self.request,
         )
 
@@ -181,15 +183,15 @@
 
         return cast(Dict[str, Any], response_dict)
 
     # middlewares #############################################################
     def run_middlewares(self, connection, window_id, url):
         try:
             handled, raw_response_dict, middleware = \
-                self.server.middleware_controller.handle_request(
+                self.server._middleware_controller.handle_request(
                     view=self.view,
                     request=self.request,
                 )
 
             if handled:
                 if not raw_response_dict:
                     raw_response_dict = ''
@@ -412,15 +414,15 @@
         # clean up
         if clean_up:
             # drop all connections
             self.connections = {}
 
             # multi user views have no start_connection
             if self.start_connection:
-                self.server.view_runtime_controller.remove_view_runtime(self)
+                self.server._view_runtime_controller.remove_view_runtime(self)
 
     def issue_500_error(self, exception):
         # stop the runtime but don't run cleanup code to get the
         # output of the 500 handle through
         self.stop(reason=exception, clean_up=False)
 
         self.run_error_view(
@@ -598,15 +600,15 @@
                 )
 
                 connection.send_str(message)
 
     def handle_raw_response_dict(self, raw_response_dict, connections=None):
         connections = connections or self.connections
 
-        response_dict = self.server.response_parser.render_response_dict(
+        response_dict = self.server._response_parser.render_response_dict(
             raw_response_dict=raw_response_dict,
             view_name=self.name,
         )
 
         if response_dict['redirect']:
             self.send_redirect(
                 response_dict['redirect'],
@@ -679,15 +681,15 @@
                 raise RuntimeError(
                     '%r returned an unexpected type (%r)',
                     handler,
                     return_value,
                 )
 
             if isinstance(return_value, dict):
-                response_parser = self.server.response_parser
+                response_parser = self.server._response_parser
 
                 response_dict = response_parser.parse_event_response_dict(
                     return_value,
                 )
 
                 self.handle_raw_response_dict(response_dict)
```

### Comparing `lona-1.8.5/lona/view_runtime_controller.py` & `lona-1.9/lona/view_runtime_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import contextlib
 import logging
 
 from yarl import URL
 
+from lona.view_runtime import VIEW_RUNTIME_STATE, ViewRuntime
 from lona.protocol import encode_http_redirect, METHOD
 from lona.events.view_event import ViewEvent
-from lona.view_runtime import ViewRuntime
 from lona.exceptions import ServerStop
 from lona.view import LonaView
 
 input_events_logger = logging.getLogger('lona.input_events')
 view_events_logger = logging.getLogger('lona.view_events')
 views_logger = logging.getLogger('lona.views')
 
@@ -147,15 +147,15 @@
     def handle_view_message(self, connection, window_id, view_runtime_id,
                             method, payload):
 
         url, post_data = payload
 
         # resolve url
         url_object = URL(url)
-        match, route, match_info = self.server.router.resolve(url_object.path)
+        match, route, match_info = self.server._router.resolve(url_object.path)
 
         # route is not interactive; issue a http redirect
         if(connection.interactive and
            match and
            (route.http_pass_through or not route.interactive)):
 
             views_logger.debug(
@@ -206,17 +206,15 @@
                 return
 
         # start new view runtime ##############################################
         # remove previous running runtime
         if connection.interactive and running_view_runtime:
             views_logger.debug('removing previous runtime')
 
-            self.server.view_runtime_controller.remove_view_runtime(
-                view_runtime=running_view_runtime,
-            )
+            self.remove_view_runtime(view_runtime=running_view_runtime)
 
         # start nev runtime
         views_logger.debug('trying to start a new view runtime')
 
         frontend = False
 
         if not connection.interactive and match and route.interactive:
@@ -354,15 +352,15 @@
 
         if not isinstance(return_value, (dict, type(None))):
             exception = ValueError(f'{repr(view_runtime.view.on_view_event)} returned an unexpected type ({repr(return_value)})')
 
             view_runtime.issue_500_error(exception)
 
         if isinstance(return_value, dict):
-            response_parser = self.server.response_parser
+            response_parser = self.server._response_parser
 
             try:
                 response_dict = response_parser.parse_event_response_dict(
                     return_value,
                 )
 
                 view_runtime.handle_raw_response_dict(response_dict)
@@ -417,7 +415,26 @@
             )
 
             self.server.run_function_async(
                 self.run_view_event_hook,
                 view_runtime,
                 view_event,
             )
+
+    # public api ##############################################################
+    def get_views(
+        self,
+        view_class: type[LonaView],
+    ) -> list[LonaView]:
+
+        views: list[LonaView] = []
+
+        for view_runtime in self.iter_view_runtimes():
+            if view_runtime.view_class is not view_class:
+                continue
+
+            if view_runtime.state == VIEW_RUNTIME_STATE.NOT_STARTED:
+                continue
+
+            views.append(view_runtime.view)
+
+        return views
```

### Comparing `lona-1.8.5/lona/worker_pool.py` & `lona-1.9/lona/worker_pool.py`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/lona.egg-info/PKG-INFO` & `lona-1.9/lona.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.1
 Name: lona
-Version: 1.8.5
+Version: 1.9
 Summary: Write responsive web apps in full python
 Home-page: https://github.com/lona-web-org/lona
 Author: Florian Scherf
-Author-email: f.scherf@pengutronix.de
+Author-email: mail@florianscherf.de
 License: MIT
 Description: .. image:: doc/content/logo.svg
             :alt: Lona logo
             :height: 200px
             :width: 200px
         .. image:: https://img.shields.io/pypi/l/lona.svg
             :alt: license MIT
@@ -36,14 +36,16 @@
         
         **Documentation:** `lona-web.org <http://lona-web.org>`_
         
         **Changelog:** `lona-web.org/changelog <http://lona-web.org/changelog.html>`_
         
         **Reddit:** `reddit.com/r/lona_web_org/ <https://www.reddit.com/r/lona_web_org/>`_
         
+        **Discord:** `discord.com/lona-web.org <https://discord.gg/WBf5PVACsj>`_
+        
         Web is a solved problem in Python since ages, but traditionally Python handles
         only the server side. If you want to have client side interaction like
         click events or you want update content live, you have to write an additional
         Javascript application.
         
         Lona handles the server side and the client side, and provides a simple,
         pythonic API to write self contained views.
```

### Comparing `lona-1.8.5/lona.egg-info/SOURCES.txt` & `lona-1.9/lona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/setup.cfg` & `lona-1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `lona-1.8.5/setup.py` & `lona-1.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     include_package_data=True,
     name='lona',
     version=VERSION_STRING,
     author='Florian Scherf',
     url='https://github.com/lona-web-org/lona',
-    author_email='f.scherf@pengutronix.de',
+    author_email='mail@florianscherf.de',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'aiohttp>=3,<4',
         'jinja2',
         'rlpython',
         'typing-extensions',
```

