# Comparing `tmp/Clone-ChatGPT-1.2.4.tar.gz` & `tmp/Clone-ChatGPT-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-jttsm9iz/Clone-ChatGPT-1.2.4.tar", last modified: Mon Jun 26 04:47:44 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-viwja12j/Clone-ChatGPT-1.2.9.tar", last modified: Thu Jul 20 12:27:43 2023, max compression
```

## Comparing `Clone-ChatGPT-1.2.4.tar` & `Clone-ChatGPT-1.2.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-26 04:47:43.000000 Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:47:43.000000 Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 04:47:43.000000 Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-26 04:47:43.000000 Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 04:47:43.000000 Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/requirements_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/bots/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/bots/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/bots/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/cloud_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/exts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/exts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/exts/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/exts/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/exts/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/11/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/migrations/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/migrations/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/migrations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/migrations/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/openai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/openai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:47:44.000000 Clone-ChatGPT-1.2.4/src/pandora/turbo/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/turbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/turbo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-26 04:47:28.000000 Clone-ChatGPT-1.2.4/src/pandora/turbo/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/requirements_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/bots/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/bots/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/cloud_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/exts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/exts/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/exts/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/exts/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/migrations/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/migrations/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/migrations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/migrations/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/openai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/openai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:43.000000 Clone-ChatGPT-1.2.9/src/pandora/turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/turbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/turbo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-07-20 12:27:32.000000 Clone-ChatGPT-1.2.9/src/pandora/turbo/chat.py
```

### Comparing `Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/PKG-INFO` & `Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Clone-ChatGPT
-Version: 1.2.4
+Version: 1.2.9
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/lannychan/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/lannychan/pandora
 Project-URL: Tracker, https://github.com/lannychan/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Clone-ChatGPT Version: 1.2.4 Summary: A command-
+Metadata-Version: 2.1 Name: Clone-ChatGPT Version: 1.2.9 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/lannychan/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/lannychan/pandora Project-URL: Tracker, https://github.com/
 lannychan/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
```

### Comparing `Clone-ChatGPT-1.2.4/Clone_ChatGPT.egg-info/SOURCES.txt` & `Clone-ChatGPT-1.2.9/Clone_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/LICENSE` & `Clone-ChatGPT-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/PKG-INFO` & `Clone-ChatGPT-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Clone-ChatGPT
-Version: 1.2.4
+Version: 1.2.9
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/lannychan/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/lannychan/pandora
 Project-URL: Tracker, https://github.com/lannychan/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Clone-ChatGPT Version: 1.2.4 Summary: A command-
+Metadata-Version: 2.1 Name: Clone-ChatGPT Version: 1.2.9 Summary: A command-
 line interface to ChatGPT Home-page: https://github.com/lannychan/pandora
 Author: Neo Peng Author-email: pengzhile@gmail.com Project-URL: Source, https:/
 /github.com/lannychan/pandora Project-URL: Tracker, https://github.com/
 lannychan/pandora/issues Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo
 gpt-3.5-turbo-0301 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask Classifier: Intended Audience :: Developers
```

### Comparing `Clone-ChatGPT-1.2.4/README.md` & `Clone-ChatGPT-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/setup.py` & `Clone-ChatGPT-1.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url='https://github.com/lannychan/pandora',
     packages=find_packages('src'),
     package_dir={'pandora': 'src/pandora'},
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'api': requirements_api,
-        'cloud': ['chatgpt-cloud~=0.6.1'],
+        'cloud': ['pandora-cloud~=0.6.2'],
     },
     entry_points={
         'console_scripts': [
             'pandora = pandora.launcher:run',
             'pandora-cloud = pandora.cloud_launcher:run',
         ]
     },
```

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/bots/legacy.py` & `Clone-ChatGPT-1.2.9/src/pandora/bots/legacy.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/bots/server.py` & `Clone-ChatGPT-1.2.9/src/pandora/bots/server.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/cloud_launcher.py` & `Clone-ChatGPT-1.2.9/src/pandora/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/exts/config.py` & `Clone-ChatGPT-1.2.9/src/pandora/exts/config.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/exts/hooks.py` & `Clone-ChatGPT-1.2.9/src/pandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/exts/token.py` & `Clone-ChatGPT-1.2.9/src/pandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/apple-touch-icon.png` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/favicon-16x16.png` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/favicon-32x32.png` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Signifier-Regular.otf` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Buch.otf` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/Sohne-Halbfett.otf` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Buch.otf` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/static/images/2022/11/ChatGPT.jpg` & `Clone-ChatGPT-1.2.9/src/pandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/flask/templates/chat.html` & `Clone-ChatGPT-1.2.9/src/pandora/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/launcher.py` & `Clone-ChatGPT-1.2.9/src/pandora/launcher.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/migrations/migrate.py` & `Clone-ChatGPT-1.2.9/src/pandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/migrations/models.py` & `Clone-ChatGPT-1.2.9/src/pandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/migrations/scripts/20230308_01_7ctOr.sql` & `Clone-ChatGPT-1.2.9/src/pandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/openai/api.py` & `Clone-ChatGPT-1.2.9/src/pandora/openai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             yield await self.__process_sse_except(resp)
             return
 
         async for utf8_line in resp.aiter_lines():
             if 'data: [DONE]' == utf8_line[0:12]:
                 break
 
-            if 'data: {' == utf8_line[0:7]:
+            if 'data: {"message":' == utf8_line[0:17]:
                 yield json.loads(utf8_line[6:])
 
     @staticmethod
     async def __process_sse_except(resp):
         result = b''
         async for line in resp.aiter_bytes():
             result += line
```

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/openai/auth.py` & `Clone-ChatGPT-1.2.9/src/pandora/openai/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import re
 from datetime import datetime as dt
 from urllib.parse import urlparse, parse_qs
 
 import requests
 from certifi import where
 
+from ..exts.config import default_api_prefix
+
 
 class Auth0:
     def __init__(self, email: str, password: str, proxy: str = None, use_cache: bool = True, mfa: str = None):
         self.session_token = None
         self.email = email
         self.password = password
         self.use_cache = use_cache
@@ -39,28 +41,41 @@
     def auth(self, login_local=True) -> str:
         if self.use_cache and self.access_token and self.expires and self.expires > dt.now():
             return self.access_token
 
         if not self.__check_email(self.email) or not self.password:
             raise Exception('invalid email or password.')
 
-        return self.__part_two()
+        return self.__part_one()
 
     def get_refresh_token(self):
         return self.refresh_token
 
-    def __part_two(self) -> str:
+    def __part_one(self) -> str:
+        url = '{}/auth/preauth'.format(default_api_prefix())
+        resp = self.session.get(url, allow_redirects=False, **self.req_kwargs)
+
+        if resp.status_code == 200:
+            json = resp.json()
+            if 'preauth_cookie' not in json or not json['preauth_cookie']:
+                raise Exception('Get preauth cookie failed.')
+
+            return self.__part_two(json['preauth_cookie'])
+        else:
+            raise Exception('Error request preauth.')
+
+    def __part_two(self, preauth: str) -> str:
         code_challenge = 'w6n3Ix420Xhhu-Q5-mOOEyuPZmAsJHUbBpO8Ub7xBCY'
         code_verifier = 'yGrXROHx_VazA0uovsxKfE263LMFcrSrdm4SlC-rob8'
 
         url = 'https://auth0.openai.com/authorize?client_id=pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh&audience=https%3A%2F' \
               '%2Fapi.openai.com%2Fv1&redirect_uri=com.openai.chat%3A%2F%2Fauth0.openai.com%2Fios%2Fcom.openai.chat' \
               '%2Fcallback&scope=openid%20email%20profile%20offline_access%20model.request%20model.read' \
               '%20organization.read%20offline&response_type=code&code_challenge={}' \
-              '&code_challenge_method=S256&prompt=login'.format(code_challenge)
+              '&code_challenge_method=S256&prompt=login&preauth_cookie={}'.format(code_challenge, preauth)
         return self.__part_three(code_verifier, url)
 
     def __part_three(self, code_verifier, url: str) -> str:
         headers = {
             'User-Agent': self.user_agent,
             'Referer': 'https://ios.chat.openai.com/',
         }
```

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/openai/utils.py` & `Clone-ChatGPT-1.2.9/src/pandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/turbo/base.py` & `Clone-ChatGPT-1.2.9/src/pandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `Clone-ChatGPT-1.2.4/src/pandora/turbo/chat.py` & `Clone-ChatGPT-1.2.9/src/pandora/turbo/chat.py`

 * *Files identical despite different names*

