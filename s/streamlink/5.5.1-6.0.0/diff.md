# Comparing `tmp/streamlink-5.5.1.tar.gz` & `tmp/streamlink-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-5.5.1.tar", last modified: Mon May  8 00:33:07 2023, max compression
+gzip compressed data, was "streamlink-6.0.0.tar", last modified: Thu Jul 20 12:43:24 2023, max compression
```

## Comparing `streamlink-5.5.1.tar` & `streamlink-6.0.0.tar`

### file list

```diff
@@ -1,575 +1,627 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.068640 streamlink-5.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 00:32:02.000000 streamlink-5.5.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    75916 2023-05-08 00:32:02.000000 streamlink-5.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 00:32:02.000000 streamlink-5.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-08 00:32:02.000000 streamlink-5.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-08 00:33:07.068640 streamlink-5.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-08 00:32:02.000000 streamlink-5.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.952640 streamlink-5.5.1/completions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.960640 streamlink-5.5.1/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-05-08 00:32:50.000000 streamlink-5.5.1/completions/bash/streamlink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.960640 streamlink-5.5.1/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)    33215 2023-05-08 00:32:50.000000 streamlink-5.5.1/completions/zsh/_streamlink
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-08 00:32:02.000000 streamlink-5.5.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_applications.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.952640 streamlink-5.5.1/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (123)    37912 2023-05-08 00:32:56.000000 streamlink-5.5.1/docs/_build/man/streamlink.1
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_man.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/icon-ffmpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/icon-python.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/opengraph-image.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.964640 streamlink-5.5.1/docs/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/_templates/sidebar/github-buttons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/api_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/applications.rst
--rw-r--r--   0 runner    (1001) docker     (123)    75916 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.968640 streamlink-5.5.1/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugin-sideloading.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.968640 streamlink-5.5.1/docs/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugins/crunchyroll.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugins/twitch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/donate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_html_template_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/ext_releaseref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24181 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/players.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs/thirdparty.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 00:32:02.000000 streamlink-5.5.1/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-08 00:32:02.000000 streamlink-5.5.1/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-08 00:32:02.000000 streamlink-5.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 00:33:07.072640 streamlink-5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-08 00:32:02.000000 streamlink-5.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.952640 streamlink-5.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.076640 streamlink-5.5.1/src/streamlink/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-08 00:33:07.076640 streamlink-5.5.1/src/streamlink/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/packages/requests_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/plugin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/useragents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink/plugin/api/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/validate/_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/api/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.004640 streamlink-5.5.1/src/streamlink/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/app17.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/btv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/htv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/qq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/streann.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/stv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/welt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/plugins/zhanqi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25474 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.008640 streamlink-5.5.1/src/streamlink/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    34203 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/dash_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    32100 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20611 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/segmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/stream/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.012640 streamlink-5.5.1/src/streamlink/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.972640 streamlink-5.5.1/src/streamlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 00:33:06.000000 streamlink-5.5.1/src/streamlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.012640 streamlink-5.5.1/src/streamlink_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44541 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32105 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.016640 streamlink-5.5.1/src/streamlink_cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/output/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.016640 streamlink-5.5.1/src/streamlink_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/player.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-08 00:32:02.000000 streamlink-5.5.1/src/streamlink_cli/utils/versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.020640 streamlink-5.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.020640 streamlink-5.5.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.020640 streamlink-5.5.1/tests/cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/output/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/output/test_playeroutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_cmdline_player_fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_cmdline_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_main_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_main_setup_config_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/test_streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/cli/utils/test_versioncheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/mixins/stream_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.024640 streamlink-5.5.1/tests/plugin/override/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/override/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/testplugin_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugin/testplugin_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.056640 streamlink-5.5.1/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_app17.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_btv.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_htv.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_huya.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_indihometv.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nos.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_qq.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_streann.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_stv.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_telemadrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_welt.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/plugins/test_zhanqi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.056640 streamlink-5.5.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:06.956640 streamlink-5.5.1/tests/resources/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.056640 streamlink-5.5.1/tests/resources/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/custom
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/primary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/primary.testplugin
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/secondary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/cli/config/secondary.testplugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.060640 streamlink-5.5.1/tests/resources/dash/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_10.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_11_static.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_3.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_8.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_9.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_nested_baseurls.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_no_segment_list_or_template.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_segment_list.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_segments_byterange.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_segments_dynamic_number.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_static_no_publish_time.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/dash/test_timeline_ids.mpd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.060640 streamlink-5.5.1/tests/resources/hls/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_1.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_2.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_date.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_master.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/resources/hls/test_master_twitch_vod.m3u8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.064640 streamlink-5.5.1/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_dash_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_hls_filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    18847 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_stream_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_stream_to_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/stream/test_stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/test_api_http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    48733 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-08 00:32:02.000000 streamlink-5.5.1/tests/test_api_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_plugin_userinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/test_streamlink_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.068640 streamlink-5.5.1/tests/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/testutils/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/testutils/test_handshake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 00:33:07.068640 streamlink-5.5.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-08 00:32:03.000000 streamlink-5.5.1/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.782695 streamlink-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 12:42:25.000000 streamlink-6.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-07-20 12:42:25.000000 streamlink-6.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-20 12:42:25.000000 streamlink-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 12:42:25.000000 streamlink-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-20 12:43:24.778695 streamlink-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-20 12:42:25.000000 streamlink-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.666692 streamlink-6.0.0/completions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.674692 streamlink-6.0.0/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-20 12:43:08.000000 streamlink-6.0.0/completions/bash/streamlink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.674692 streamlink-6.0.0/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)    34901 2023-07-20 12:43:09.000000 streamlink-6.0.0/completions/zsh/_streamlink
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-20 12:42:25.000000 streamlink-6.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_applications.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.666692 streamlink-6.0.0/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    39501 2023-07-20 12:43:15.000000 streamlink-6.0.0/docs/_build/man/streamlink.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_man.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/icon-ffmpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/icon-python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/opengraph-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/sidebar/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/_templates/sidebar/github-buttons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.678692 streamlink-6.0.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/session.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/streamlink.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api/webbrowser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/api_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/applications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81057 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugin-sideloading.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/docs/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugins/crunchyroll.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugins/twitch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/donate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_html_template_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/ext_releaseref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/players.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs/thirdparty.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 12:42:25.000000 streamlink-6.0.0/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-07-20 12:42:25.000000 streamlink-6.0.0/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-20 12:42:25.000000 streamlink-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:43:24.782695 streamlink-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-20 12:42:25.000000 streamlink-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.670692 streamlink-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.782695 streamlink-6.0.0/src/streamlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 12:43:24.782695 streamlink-6.0.0/src/streamlink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/packages/requests_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink/plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/useragents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.686693 streamlink-6.0.0/src/streamlink/plugin/api/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/validate/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/api/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.718693 streamlink-6.0.0/src/streamlink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33839 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/plugins/zhanqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25638 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.722693 streamlink-6.0.0/src/streamlink/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34111 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/dash_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20613 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/stream/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.726693 streamlink-6.0.0/src/streamlink/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.726693 streamlink-6.0.0/src/streamlink/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.726693 streamlink-6.0.0/src/streamlink/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19550 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.730693 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49431 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61703 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/dom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26108 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27656 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/input_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130730 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107545 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62134 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/devtools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/cdp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/chromium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink/webbrowser/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.682692 streamlink-6.0.0/src/streamlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18161 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 12:43:24.000000 streamlink-6.0.0/src/streamlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.730693 streamlink-6.0.0/src/streamlink_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47629 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31600 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.730693 streamlink-6.0.0/src/streamlink_cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/output/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.734694 streamlink-6.0.0/src/streamlink_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-20 12:42:25.000000 streamlink-6.0.0/src/streamlink_cli/utils/versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.734694 streamlink-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/output/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/output/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_cmdline_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_main_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_main_setup_config_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_plugin_args_and_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/test_streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/cli/utils/test_versioncheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.738694 streamlink-6.0.0/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/mixins/stream_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.742694 streamlink-6.0.0/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.742694 streamlink-6.0.0/tests/plugin/override/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/override/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/testplugin_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugin/testplugin_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34427 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/plugins/test_zhanqi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.670692 streamlink-6.0.0/tests/resources/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/resources/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/custom
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/primary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/primary.testplugin
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/secondary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/cli/config/secondary.testplugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.770694 streamlink-6.0.0/tests/resources/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_10.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_11_static.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_3.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_8.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_9.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_nested_baseurls.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_no_segment_list_or_template.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_segment_list.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_segments_byterange.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_segments_dynamic_number.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_static_no_publish_time.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/dash/test_timeline_ids.mpd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.774695 streamlink-6.0.0/tests/resources/hls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_1.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_2.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_date.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_master.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/resources/hls/test_master_twitch_vod.m3u8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.774695 streamlink-6.0.0/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21610 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_dash_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39039 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_hls_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_stream_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_stream_to_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/stream/test_stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_api_http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48165 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_api_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16043 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_plugin_userinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23565 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/test_streamlink_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.774695 streamlink-6.0.0/tests/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/testutils/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/testutils/test_handshake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.778695 streamlink-6.0.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.778695 streamlink-6.0.0/tests/webbrowser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:43:24.778695 streamlink-6.0.0/tests/webbrowser/cdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39456 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/cdp/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/test_chromium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-20 12:42:25.000000 streamlink-6.0.0/tests/webbrowser/test_webbrowser.py
```

### Comparing `streamlink-5.5.1/CHANGELOG.md` & `streamlink-6.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,42 @@
 # Changelog
 
+## streamlink 6.0.0 (2023-07-20)
+
+Breaking changes:
+
+- BREAKING: dropped support for Python 3.7 ([#5302](https://github.com/streamlink/streamlink/pull/5302))
+- BREAKING: [turned `--player` CLI argument into a player-path-only argument](https://streamlink.github.io/migrations.html#player-path-only-player-cli-argument) ([#5305](https://github.com/streamlink/streamlink/issues/5305), [#5310](https://github.com/streamlink/streamlink/pull/5310))  
+  Its value won't be interpreted as a command line string anymore, so paths with whitespace don't require additional quotation. Custom player arguments now always need to be set via `--player-args`.
+- BREAKING: [removed deprecated `{filename}` variable from `--player-args`](https://streamlink.github.io/migrations.html#filename-variable-in-player-args) ([#5310](https://github.com/streamlink/streamlink/pull/5310))
+- BREAKING/API: [removed support for the deprecated `Plugin.can_handle_url()` / `Plugin.priority()` classmethods](https://streamlink.github.io/migrations.html#plugin-can-handle-url-and-plugin-priority) ([#5403](https://github.com/streamlink/streamlink/pull/5403))
+- BREAKING/API: [removed deprecated compatibility wrapper for the `Plugin` constructor](https://streamlink.github.io/migrations.html#plugin-init-self-url-compatibility-wrapper) ([#5402](https://github.com/streamlink/streamlink/pull/5402))
+- BREAKING/API: [removed deprecated global plugin arguments](https://streamlink.github.io/migrations.html#global-plugin-arguments) ([#5033](https://github.com/streamlink/streamlink/pull/5033))
+- BREAKING/API: [removed deprecated `streamlink.plugin.api.validate.text`](https://streamlink.github.io/migrations.html#plugin-api-validate-text) ([#5404](https://github.com/streamlink/streamlink/pull/5404))
+- BREAKING/API: [fixed/changed signatures of `HTTPStream`, `HLSStream` and `HLSStream.parse_variant_playlist()`](https://streamlink.github.io/migrations.html#httpstream-and-hlsstream-signature-changes) ([#5429](https://github.com/streamlink/streamlink/pull/5429))
+- BREAKING/packaging: new signing key [`44448A298D5C3618`](https://keyserver.ubuntu.com/pks/lookup?search=44448A298D5C3618&fingerprint=on&op=index) ([#5449](https://github.com/streamlink/streamlink/pull/5449))
+
+Release highlights:
+
+- Added: experimental `streamlink.webbrowser` API for extracting data from websites using the system's Chromium-based web browser ([#5380](https://github.com/streamlink/streamlink/issues/5380), [#5381](https://github.com/streamlink/streamlink/pull/5381), [#5386](https://github.com/streamlink/streamlink/pull/5386), [#5388](https://github.com/streamlink/streamlink/pull/5388), [#5410](https://github.com/streamlink/streamlink/pull/5410))  
+  See the [`--webbrowser`, `--webbrowser-executable` and related CLI arguments](https://streamlink.github.io/cli.html#web-browser-options) for more
+- Added: client-integrity token support to Twitch plugin using the `streamlink.webbrowser` API (currently only used as a fallback when acquiring the access token fails) ([#5414](https://github.com/streamlink/streamlink/pull/5414))
+- Added: `{playertitleargs}` variable to `--player-args` ([#5310](https://github.com/streamlink/streamlink/pull/5310))
+- Added: `with_{video,audio}_only` parameters to `DASHStream.parse_manifest()` ([#5340](https://github.com/streamlink/streamlink/pull/5340))
+- Changed: HLS streams to stop early on missing `EXT-X-ENDLIST` tag when polling the playlist doesn't yield new segments for twice its targetduration value ([#5330](https://github.com/streamlink/streamlink/pull/5330))
+- Fixed: regex of optional protocol plugin parameters ([#5367](https://github.com/streamlink/streamlink/pull/5367))
+- Fixed plugins: lrt ([#5444](https://github.com/streamlink/streamlink/pull/5444)), mediavitrina ([#5376](https://github.com/streamlink/streamlink/pull/5376)), mitele ([#5436](https://github.com/streamlink/streamlink/pull/5436)), NRK ([#5408](https://github.com/streamlink/streamlink/pull/5408)), pluzz ([#5369](https://github.com/streamlink/streamlink/pull/5369)), rtvs ([#5443](https://github.com/streamlink/streamlink/pull/5443)), showroom ([#5390](https://github.com/streamlink/streamlink/pull/5390)), turkuvaz ([#5374](https://github.com/streamlink/streamlink/pull/5374)), vimeo ([#5335](https://github.com/streamlink/streamlink/pull/5335)), youtube ([#5351](https://github.com/streamlink/streamlink/pull/5351))
+- Docs: added migrations page for further guidance on resolving breaking changes ([#5433](https://github.com/streamlink/streamlink/pull/5433))
+- Docs: split up, updated and improved API docs ([#5398](https://github.com/streamlink/streamlink/pull/5398))
+- Build: moved project metadata to pyproject.toml (PEP621) ([#5438](https://github.com/streamlink/streamlink/pull/5438))
+- Dependencies: added `trio` ([#5386](https://github.com/streamlink/streamlink/pull/5386)), `trio-websocket` and `typing-extensions` ([#5388](https://github.com/streamlink/streamlink/pull/5388)), and removed `importlib_metadata` ([#5302](https://github.com/streamlink/streamlink/pull/5302))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.5.1...6.0.0)
+
+
 ## streamlink 5.5.1 (2023-05-08)
 
 Patch release:
 
 - Fixed: shifting time offset when reloading HLS playlists ([#5321](https://github.com/streamlink/streamlink/pull/5321))
 - Fixed: import of `create_urllib3_context` on `urllib3 <2.0.0` ([#5333](https://github.com/streamlink/streamlink/pull/5333))
 - Fixed: Vimeo plugin ([#5331](https://github.com/streamlink/streamlink/pull/5331))
```

### Comparing `streamlink-5.5.1/LICENSE` & `streamlink-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/PKG-INFO` & `streamlink-6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.5.1
+Version: 6.0.0
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
-Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
+Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
 Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center"><a href="https://streamlink.github.io/">Streamlink<br><img height="150" alt="Streamlink" src="https://raw.githubusercontent.com/streamlink/streamlink/master/icon.svg"></a></h1>
 
 <p align="center">
   <a href="https://streamlink.github.io/install.html"><img alt="Supported Python versions" src="https://img.shields.io/pypi/pyversions/streamlink.svg?style=flat-square&maxAge=86400"></a>
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.5.1 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.0.0 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
-into a video player of choice. Home-page: https://github.com/streamlink/
-streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
-Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
-Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
-URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
-https://streamlink.github.io/latest/donate.html Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: BSD License
-Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
-Desktop Classifier: Operating System :: POSIX Classifier: Operating System ::
-MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Internet :: WWW/
-HTTP Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
-Multimedia :: Video Classifier: Topic :: Utilities Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown License-File: LICENSE
+into a video player of choice. Author: Streamlink Author-email:
+streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
+//github.com/streamlink/streamlink Project-URL: Documentation, https://
+streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
+streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
+Project-URL: Funding, https://streamlink.github.io/latest/donate.html
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: BSD License Classifier: Environment :: Console Classifier:
+Intended Audience :: End Users/Desktop Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
+:: Windows Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Multimedia :: Sound/Audio Classifier: Topic :: Multimedia :: Video Classifier:
+Topic :: Utilities Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE
                                ****** Streamlink
                               [Streamlink] ******
   [Supported_Python_versions] [Latest_release] [License] [Open_issues] [Build
                         status] [Overall_code_coverage]
  A Python library and command-line interface which pipes streams from various
                          services into a video player.
     Avoid resource-heavy and unoptimized websites, and still enjoy streamed
```

### Comparing `streamlink-5.5.1/README.md` & `streamlink-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/completions/bash/streamlink` & `streamlink-6.0.0/completions/bash/streamlink`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOMATICALLY GENERATED by `shtab`
 
 
 
-_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '--no-config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-interface' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '-f' '--force' '--progress' '--force-progress' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--dash-manifest-reload-attempts' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-disable-reruns' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
+_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '--no-config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-interface' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '-f' '--force' '--progress' '--force-progress' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--dash-manifest-reload-attempts' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--webbrowser' '--webbrowser-executable' '--webbrowser-timeout' '--webbrowser-cdp-host' '--webbrowser-cdp-port' '--webbrowser-cdp-timeout' '--webbrowser-headless' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-disable-reruns' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--twitch-purge-client-integrity' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
 
 
 
 _shtab_streamlink_cli__l_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___loglevel_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___fs_safe_rules_choices=('POSIX' 'Windows')
 _shtab_streamlink_cli___progress_choices=('yes' 'force' 'no')
@@ -58,14 +58,15 @@
 _shtab_streamlink_cli___crunchyroll_purge_credentials_nargs=0
 _shtab_streamlink_cli___niconico_purge_credentials_nargs=0
 _shtab_streamlink_cli___pixiv_purge_credentials_nargs=0
 _shtab_streamlink_cli___twitch_disable_ads_nargs=0
 _shtab_streamlink_cli___twitch_disable_hosting_nargs=0
 _shtab_streamlink_cli___twitch_disable_reruns_nargs=0
 _shtab_streamlink_cli___twitch_low_latency_nargs=0
+_shtab_streamlink_cli___twitch_purge_client_integrity_nargs=0
 _shtab_streamlink_cli___yupptv_purge_credentials_nargs=0
 _shtab_streamlink_cli___zattoo_purge_credentials_nargs=0
 
 
 # $1=COMP_WORDS[1]
 _shtab_compgen_files() {
   compgen -f -- $1  # files
```

### Comparing `streamlink-5.5.1/completions/zsh/_streamlink` & `streamlink-6.0.0/completions/zsh/_streamlink`

 * *Files 4% similar despite different names*

```diff
@@ -107,68 +107,48 @@
   {-4,--ipv4}"[
         Resolve address names to IPv4 only. This option overrides --ipv6.
         ]"
   {-6,--ipv6}"[
         Resolve address names to IPv6 only. This option overrides --ipv4.
         ]"
   {-p,--player}"[
-        Player to feed stream data to. By default, VLC will be used if it can be
-        found in its default location.
+        The player executable that will be launched (unless a different output method was chosen).
 
-        This is a shell-like syntax to support using a specific player\:
+        Either set an absolute or relative path to the player executable, or just set the executable\'s name
+        if it can be resolved from the paths of the system\'s \`PATH\` environment variable.
 
-          \%(prog)s --player\=vlc \<url\> \[stream\]
+        In addition to setting the player executable path, custom player arguments can be set via --player-args.
 
-        Absolute or relative paths can also be passed via this option in the
-        event the player\'s executable can not be resolved\:
+        Note\: In the past, --player allowed defining additional player arguments, which as a consequence required wrapping
+        player paths that contained spaces in quotation marks. This is unsupported since release \`6.0.0\`.
 
-          \%(prog)s --player\=\/path\/to\/vlc \<url\> \[stream\]
-          \%(prog)s --player\=.\/vlc-player\/vlc \<url\> \[stream\]
-
-        To use a player that is located in a path with spaces you must quote the
-        parameter or its value\:
-
-          \%(prog)s \"--player\=\/path\/with spaces\/vlc\" \<url\> \[stream\]
-          \%(prog)s --player \"C\:\\path\\with spaces\\mpc-hc64.exe\" \<url\> \[stream\]
-
-        Options may also be passed to the player. For example\:
-
-          \%(prog)s --player \"vlc --file-caching\=5000\" \<url\> \[stream\]
-
-        As an alternative to this, see the --player-args parameter, which does
-        not log any custom player arguments.
+        Default is VLC player, if available.
         ]:player:"
   {-a,--player-args}"[
-        This option allows you to customize the default arguments which are put
-        together with the value of --player to create a command to execute.
-
-        It\'s usually enough to only use --player instead of this unless you need
-        to add arguments after the player\'s input argument or if you don\'t want
-        any of the player arguments to be logged.
+        This option allows the arguments which are used to launch the player process to be customized.
 
-        The value can contain formatting variables surrounded by curly braces,
-        \`\{\` and \`\}\`. If you need to include a brace character, it can be escaped
-        by doubling, e.g. \`\{\{\` and \`\}\}\`.
+        The value can contain formatting variables surrounded by curly braces, \`\{\` and \`\}\`.
+        Curly brace characters can be escaped by doubling, e.g. \`\{\{\` and \`\}\}\`.
 
-        Formatting variables available\:
+        Available formatting variables\:
 
-        \{playerinput\}
-            This is the input that the player will use. For standard input (stdin),
-            it is \`-\` (dash), but it can also be a URL, depending on the options used.
+        \`\{playerinput\}\`
+            This is the input argument that the player will receive. For standard input (stdin),
+            it is \`-\` (dash), but it can also be a file path or URL, depending on the options used.
+            If unset, then the player input argument will be appended to the parsed player arguments list.
 
-        \{filename\}
-            The old fallback variable name with the same functionality.
+        \`\{playertitleargs\}\`
+            The automatically generated player title arguments, if a supported player was found. See --title for more.
+            If unset, automatically generated player title arguments will be prepended to the parsed player arguments list.
 
         Example\:
 
-          \%(prog)s -p vlc -a \"--play-and-exit \{playerinput\}\" \<url\> \[stream\]
+          \%(prog)s -p vlc -a \"--play-and-exit --no-one-instance\" \<url\> \[stream\]
 
-        Note\: When neither of the variables are found, \`\{playerinput\}\`
-        will be appended to the whole parameter value, to ensure that the player
-        always receives an input argument.
+        Default is \"\".
         ]:player_args:"
   {-v,--verbose-player}"[
         Allow the player to display its console output.
         ]"
   {-n,--player-fifo,--fifo}"[
         Make the player read the stream through a named pipe instead of the
         stdin pipe.
@@ -652,14 +632,56 @@
         ]:http_ssl_cert_crt_key:"
   "--http-timeout[
         General timeout used by all HTTP requests except the ones covered by
         other options.
 
         Default is 20.0.
         ]:http_timeout:"
+  "--webbrowser[
+        Enable or disable support for Streamlink\'s webbrowser API.
+
+        Streamlink\'s webbrowser API allows plugins which implement it to launch a web browser and extract data from websites
+        which they otherwise couldn\'t do via the regular HTTP session in Python due to specific JavaScript restrictions.
+
+        The web browser is run isolated and in a clean environment without access to regular user data.
+
+        Streamlink currently only supports Chromium-based web browsers using the Chrome Devtools Protocol (CDP).
+        This includes Chromium itself, Google Chrome, Microsoft Edge, Brave, Vivaldi, and others, but full support for
+        third party Chromium forks is not guaranteed. If you encounter any issues, please try Chromium or Google Chrome instead.
+
+        Default is true.
+        ]:webbrowser:"
+  "--webbrowser-executable[
+        Path to the web browser\'s executable.
+
+        By default, it is looked up automatically according to the rules of the used webbrowser API implementation.
+        This usually involves a list of known executable names and fallback paths on all supported operating systems.
+        ]:webbrowser_executable:"
+  "--webbrowser-timeout[
+        The maximum amount of time which the web browser can take to launch and execute.
+        ]:webbrowser_timeout:"
+  "--webbrowser-cdp-host[
+        Host for the web browser\'s inter-process communication interface (CDP specific).
+
+        Default is 127.0.0.1.
+        ]:webbrowser_cdp_host:"
+  "--webbrowser-cdp-port[
+        Port for the web browser\'s inter-process communication interface (CDP specific).
+
+        Tries to find a free port by default.
+        ]:webbrowser_cdp_port:"
+  "--webbrowser-cdp-timeout[
+        The maximum amount of time for waiting on a single CDP command response.
+        ]:webbrowser_cdp_timeout:"
+  "--webbrowser-headless[
+        Whether to launch the web browser in headless mode or not.
+        When enabled, it stays completely hidden and doesn\'t require a desktop environment to run.
+
+        Default is true.
+        ]:webbrowser_headless:"
   "--afreeca-username[The username used to register with afreecatv.com.]:afreeca_username:"
   "--afreeca-password[A afreecatv.com account password to use with --afreeca-username.]:afreeca_password:"
   "--afreeca-purge-credentials[Purge cached AfreecaTV credentials to initiate a new session and reauthenticate.]"
   "--bbciplayer-username[The username used to register with bbc.co.uk.]:bbciplayer_username:"
   "--bbciplayer-password[A bbc.co.uk account password to use with --bbciplayer-username.]:bbciplayer_password:"
   "--bbciplayer-hd[Prefer HD streams over local SD streams, some live programmes may not be broadcast in HD.]"
   "--clubbingtv-username[The username used to register with Clubbing TV.]:clubbingtv_username:"
@@ -729,14 +751,15 @@
         Useful for adding authentication data that can prevent ads. See the plugin-specific documentation for more information.
     ]:twitch_api_header:"
   "*--twitch-access-token-param[
         A parameter to add to the API request for acquiring the streaming access token.
 
         Can be repeated to add multiple parameters.
     ]:twitch_access_token_param:"
+  "--twitch-purge-client-integrity[Purge cached Twitch client-integrity token and acquire a new one.]"
   "--ustream-password[A password to access password protected UStream.tv channels.]:ustream_password:"
   "--ustvnow-username[Your USTV Now account username]:ustvnow_username:"
   "--ustvnow-password[Your USTV Now account password]:ustvnow_password:"
   "--wwenetwork-email[The email associated with your WWE Network account, required to access any WWE Network stream.]:wwenetwork_email:"
   "--wwenetwork-password[A WWE Network account password to use with --wwenetwork-email.]:wwenetwork_password:"
   "--yupptv-boxid[The yupptv.com boxid that\'s used in the BoxId cookie.]:yupptv_boxid:"
   "--yupptv-yuppflixtoken[The yupptv.com yuppflixtoken that\'s used in the YuppflixToken cookie.]:yupptv_yuppflixtoken:"
@@ -758,15 +781,15 @@
 
 _shtab_streamlink_cli() {
   local context state line curcontext="$curcontext" one_or_more='(-)*' remainder='(*)'
 
   if ((${_shtab_streamlink_cli_options[(I)${(q)one_or_more}*]} + ${_shtab_streamlink_cli_options[(I)${(q)remainder}*]} == 0)); then  # noqa: E501
     _shtab_streamlink_cli_options+=(': :_shtab_streamlink_cli_commands' '*::: :->streamlink')
   fi
-  _arguments -C $_shtab_streamlink_cli_options
+  _arguments -C -s $_shtab_streamlink_cli_options
 
   case $state in
     streamlink)
       words=($line[1] "${words[@]}")
       (( CURRENT += 1 ))
       curcontext="${curcontext%:*:*}:_shtab_streamlink_cli-$line[1]:"
       case $line[1] in
```

### Comparing `streamlink-5.5.1/docs/Makefile` & `streamlink-6.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_build/man/streamlink.1` & `streamlink-6.0.0/docs/_build/man/streamlink.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "STREAMLINK" "1" "May 08, 2023" "5.5.1" "Streamlink"
+.TH "STREAMLINK" "1" "Jul 20, 2023" "6.0.0" "Streamlink"
 .SH NAME
 streamlink \- extracts streams from various services and pipes them into a video player of choice
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -267,122 +267,70 @@
 .TP
 .B \-\-ipv6
 Resolve address names to IPv6 only. This option overrides \fI\%\-\-ipv4\fP\&.
 .UNINDENT
 .SS Player options
 .INDENT 0.0
 .TP
-.B \-p COMMAND
+.B \-p PATH
 .TP
-.B \-\-player COMMAND
-Player to feed stream data to. By default, VLC will be used if it can be
-found in its default location.
+.B \-\-player PATH
+The player executable that will be launched (unless a different output method was chosen).
 .sp
-This is a shell\-like syntax to support using a specific player:
-.INDENT 7.0
-.INDENT 3.5
+Either set an absolute or relative path to the player executable, or just set the executable\(aqs name
+if it can be resolved from the paths of the system\(aqs \fBPATH\fP environment variable.
 .sp
-.nf
-.ft C
-streamlink \-\-player=vlc <url> [stream]
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
+In addition to setting the player executable path, custom player arguments can be set via \fI\%\-\-player\-args\fP\&.
 .sp
-Absolute or relative paths can also be passed via this option in the
-event the player\(aqs executable can not be resolved:
-.INDENT 7.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-streamlink \-\-player=/path/to/vlc <url> [stream]
-streamlink \-\-player=./vlc\-player/vlc <url> [stream]
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.sp
-To use a player that is located in a path with spaces you must quote the
-parameter or its value:
-.INDENT 7.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-streamlink \(dq\-\-player=/path/with spaces/vlc\(dq <url> [stream]
-streamlink \-\-player \(dqC:\epath\ewith spaces\empc\-hc64.exe\(dq <url> [stream]
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.sp
-Options may also be passed to the player. For example:
+\fBNOTE:\fP
 .INDENT 7.0
 .INDENT 3.5
-.sp
-.nf
-.ft C
-streamlink \-\-player \(dqvlc \-\-file\-caching=5000\(dq <url> [stream]
-.ft P
-.fi
+In the past, \fI\%\-\-player\fP allowed defining additional player arguments, which as a consequence required wrapping
+player paths that contained spaces in quotation marks. This is unsupported since release \fB6.0.0\fP\&.
 .UNINDENT
 .UNINDENT
 .sp
-As an alternative to this, see the \fI\%\-\-player\-args\fP parameter, which does
-not log any custom player arguments.
+Default is: \fBVLC player, if available\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-a ARGUMENTS
 .TP
 .B \-\-player\-args ARGUMENTS
-This option allows you to customize the default arguments which are put
-together with the value of \fI\%\-\-player\fP to create a command to execute.
-.sp
-It\(aqs usually enough to only use \fI\%\-\-player\fP instead of this unless you need
-to add arguments after the player\(aqs input argument or if you don\(aqt want
-any of the player arguments to be logged.
+This option allows the arguments which are used to launch the player process to be customized.
 .sp
-The value can contain formatting variables surrounded by curly braces,
-\fB{\fP and \fB}\fP\&. If you need to include a brace character, it can be escaped
-by doubling, e.g. \fB{{\fP and \fB}}\fP\&.
+The value can contain formatting variables surrounded by curly braces, \fB{\fP and \fB}\fP\&.
+Curly brace characters can be escaped by doubling, e.g. \fB{{\fP and \fB}}\fP\&.
 .sp
-Formatting variables available:
+Available formatting variables:
 .INDENT 7.0
 .TP
-.B {playerinput}
-This is the input that the player will use. For standard input (stdin),
-it is \fB\-\fP (dash), but it can also be a URL, depending on the options used.
+.B \fB{playerinput}\fP
+This is the input argument that the player will receive. For standard input (stdin),
+it is \fB\-\fP (dash), but it can also be a file path or URL, depending on the options used.
+If unset, then the player input argument will be appended to the parsed player arguments list.
 .TP
-.B {filename}
-The old fallback variable name with the same functionality.
+.B \fB{playertitleargs}\fP
+The automatically generated player title arguments, if a supported player was found. See \fI\%\-\-title\fP for more.
+If unset, automatically generated player title arguments will be prepended to the parsed player arguments list.
 .UNINDENT
 .sp
 Example:
 .INDENT 7.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-streamlink \-p vlc \-a \(dq\-\-play\-and\-exit {playerinput}\(dq <url> [stream]
+streamlink \-p vlc \-a \(dq\-\-play\-and\-exit \-\-no\-one\-instance\(dq <url> [stream]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-\fBNOTE:\fP
-.INDENT 7.0
-.INDENT 3.5
-When neither of the variables are found, \fB{playerinput}\fP
-will be appended to the whole parameter value, to ensure that the player
-always receives an input argument.
-.UNINDENT
-.UNINDENT
+Default is: \fB\(dq\(dq\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-v
 .TP
 .B \-\-verbose\-player
 Allow the player to display its console output.
@@ -1133,14 +1081,71 @@
 .TP
 .B \-\-http\-timeout TIMEOUT
 General timeout used by all HTTP requests except the ones covered by
 other options.
 .sp
 Default is: \fB20.0\fP\&.
 .UNINDENT
+.SS Web browser options
+.INDENT 0.0
+.TP
+.B \-\-webbrowser {yes,true,1,on,no,false,0,off}
+Enable or disable support for Streamlink\(aqs webbrowser API.
+.sp
+Streamlink\(aqs webbrowser API allows plugins which implement it to launch a web browser and extract data from websites
+which they otherwise couldn\(aqt do via the regular HTTP session in Python due to specific JavaScript restrictions.
+.sp
+The web browser is run isolated and in a clean environment without access to regular user data.
+.sp
+Streamlink currently only supports Chromium\-based web browsers using the Chrome Devtools Protocol (CDP).
+This includes Chromium itself, Google Chrome, Microsoft Edge, Brave, Vivaldi, and others, but full support for
+third party Chromium forks is not guaranteed. If you encounter any issues, please try Chromium or Google Chrome instead.
+.sp
+Default is: \fBtrue\fP\&.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-webbrowser\-executable PATH
+Path to the web browser\(aqs executable.
+.sp
+By default, it is looked up automatically according to the rules of the used webbrowser API implementation.
+This usually involves a list of known executable names and fallback paths on all supported operating systems.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-webbrowser\-timeout TIME
+The maximum amount of time which the web browser can take to launch and execute.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-webbrowser\-cdp\-host HOST
+Host for the web browser\(aqs inter\-process communication interface (CDP specific).
+.sp
+Default is: \fB127.0.0.1\fP\&.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-webbrowser\-cdp\-port PORT
+Port for the web browser\(aqs inter\-process communication interface (CDP specific).
+.sp
+Tries to find a free port by default.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-webbrowser\-cdp\-timeout TIME
+The maximum amount of time for waiting on a single CDP command response.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-webbrowser\-headless {yes,true,1,on,no,false,0,off}
+Whether to launch the web browser in headless mode or not.
+When enabled, it stays completely hidden and doesn\(aqt require a desktop environment to run.
+.sp
+Default is: \fBtrue\fP\&.
+.UNINDENT
 .SS Plugin options
 .SS Afreeca
 .INDENT 0.0
 .TP
 .B \-\-afreeca\-username USERNAME
 The username used to register with afreecatv.com.
 .UNINDENT
@@ -1345,14 +1350,19 @@
 .INDENT 0.0
 .TP
 .B \-\-twitch\-access\-token\-param KEY=VALUE
 A parameter to add to the API request for acquiring the streaming access token.
 .sp
 Can be repeated to add multiple parameters.
 .UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-twitch\-purge\-client\-integrity
+Purge cached Twitch client\-integrity token and acquire a new one.
+.UNINDENT
 .SS Ustreamtv
 .INDENT 0.0
 .TP
 .B \-\-ustream\-password PASSWORD
 A password to access password protected UStream.tv channels.
 .UNINDENT
 .SS Ustvnow
```

### Comparing `streamlink-5.5.1/docs/_man.rst` & `streamlink-6.0.0/docs/_man.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/apple-touch-icon.png` & `streamlink-6.0.0/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/favicon-16x16.png` & `streamlink-6.0.0/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/favicon-32x32.png` & `streamlink-6.0.0/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/favicon.ico` & `streamlink-6.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/icon-ffmpeg.svg` & `streamlink-6.0.0/docs/_static/icon-ffmpeg.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/icon-python.svg` & `streamlink-6.0.0/docs/_static/icon-python.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/icon.svg` & `streamlink-6.0.0/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/opengraph-image.png` & `streamlink-6.0.0/docs/_static/opengraph-image.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_static/styles/custom.css` & `streamlink-6.0.0/docs/_static/styles/custom.css`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_templates/base.html` & `streamlink-6.0.0/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_templates/sidebar/brand.html` & `streamlink-6.0.0/docs/_templates/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/_templates/sidebar/github-buttons.html` & `streamlink-6.0.0/docs/_templates/sidebar/github-buttons.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/api_guide.rst` & `streamlink-6.0.0/docs/api_guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 If an error occurs while opening a stream, a :py:exc:`StreamError <streamlink.exceptions.StreamError>` will be raised.
 
 
 Inspecting streams
 ------------------
 
 It's also possible to inspect the stream's internal parameters. Go to
-:ref:`Stream subclasses <api:Streams>` to see which attributes are available
+:ref:`Stream subclasses <api/stream:Stream>` to see which attributes are available
 for inspection for each stream type.
 
 For example, this is a :py:class:`HLSStream <streamlink.stream.HLSStream>` object which
 contains a :py:attr:`url <streamlink.stream.HTTPStream.url>` attribute.
 
 .. code-block:: python
 
@@ -71,15 +71,15 @@
 
 
 Session object
 --------------
 
 The session allows you to set various options and is more efficient
 when extracting streams more than once. You start by creating a
-:py:class:`Streamlink <streamlink.Streamlink>` object:
+:py:class:`Streamlink <streamlink.session.Streamlink>` object:
 
 .. code-block:: python
 
     >>> from streamlink import Streamlink
     >>> session = Streamlink()
 
 You can then set options like this:
@@ -91,8 +91,8 @@
 and extract streams like this:
 
 .. code-block:: python
 
     >>> streams = session.streams("URL")
 
 
-See :py:meth:`Streamlink.set_option <streamlink.Streamlink.set_option>` to see which options are available.
+See :py:meth:`Streamlink.set_option() <streamlink.session.Streamlink.set_option>` to see which options are available.
```

### Comparing `streamlink-5.5.1/docs/applications.rst` & `streamlink-6.0.0/docs/applications.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Streamlink Applications
 =======================
 
 
 Streamlink Twitch GUI
 ---------------------
 
-.. image:: https://user-images.githubusercontent.com/467294/151660267-97a8c0a3-62b3-4aa5-b960-c307da1b4fb2.png
+.. image:: https://user-images.githubusercontent.com/467294/199009198-011d23f2-a884-4bf8-94d0-bb304ceecc08.jpg
     :alt: Streamlink Twitch GUI
 
 :Description: A multi platform Twitch.tv browser for Streamlink
 :Type: Graphical User Interface
 :OS: |Windows| |MacOS| |Linux|
 :Author: `Sebastian Meyer <https://github.com/bastimeyer>`_
 :Website: https://streamlink.github.io/streamlink-twitch-gui
```

### Comparing `streamlink-5.5.1/docs/changelog.md` & `streamlink-6.0.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,42 @@
 # Changelog
 
+## streamlink 6.0.0 (2023-07-20)
+
+Breaking changes:
+
+- BREAKING: dropped support for Python 3.7 ([#5302](https://github.com/streamlink/streamlink/pull/5302))
+- BREAKING: [turned `--player` CLI argument into a player-path-only argument](https://streamlink.github.io/migrations.html#player-path-only-player-cli-argument) ([#5305](https://github.com/streamlink/streamlink/issues/5305), [#5310](https://github.com/streamlink/streamlink/pull/5310))  
+  Its value won't be interpreted as a command line string anymore, so paths with whitespace don't require additional quotation. Custom player arguments now always need to be set via `--player-args`.
+- BREAKING: [removed deprecated `{filename}` variable from `--player-args`](https://streamlink.github.io/migrations.html#filename-variable-in-player-args) ([#5310](https://github.com/streamlink/streamlink/pull/5310))
+- BREAKING/API: [removed support for the deprecated `Plugin.can_handle_url()` / `Plugin.priority()` classmethods](https://streamlink.github.io/migrations.html#plugin-can-handle-url-and-plugin-priority) ([#5403](https://github.com/streamlink/streamlink/pull/5403))
+- BREAKING/API: [removed deprecated compatibility wrapper for the `Plugin` constructor](https://streamlink.github.io/migrations.html#plugin-init-self-url-compatibility-wrapper) ([#5402](https://github.com/streamlink/streamlink/pull/5402))
+- BREAKING/API: [removed deprecated global plugin arguments](https://streamlink.github.io/migrations.html#global-plugin-arguments) ([#5033](https://github.com/streamlink/streamlink/pull/5033))
+- BREAKING/API: [removed deprecated `streamlink.plugin.api.validate.text`](https://streamlink.github.io/migrations.html#plugin-api-validate-text) ([#5404](https://github.com/streamlink/streamlink/pull/5404))
+- BREAKING/API: [fixed/changed signatures of `HTTPStream`, `HLSStream` and `HLSStream.parse_variant_playlist()`](https://streamlink.github.io/migrations.html#httpstream-and-hlsstream-signature-changes) ([#5429](https://github.com/streamlink/streamlink/pull/5429))
+- BREAKING/packaging: new signing key [`44448A298D5C3618`](https://keyserver.ubuntu.com/pks/lookup?search=44448A298D5C3618&fingerprint=on&op=index) ([#5449](https://github.com/streamlink/streamlink/pull/5449))
+
+Release highlights:
+
+- Added: experimental `streamlink.webbrowser` API for extracting data from websites using the system's Chromium-based web browser ([#5380](https://github.com/streamlink/streamlink/issues/5380), [#5381](https://github.com/streamlink/streamlink/pull/5381), [#5386](https://github.com/streamlink/streamlink/pull/5386), [#5388](https://github.com/streamlink/streamlink/pull/5388), [#5410](https://github.com/streamlink/streamlink/pull/5410))  
+  See the [`--webbrowser`, `--webbrowser-executable` and related CLI arguments](https://streamlink.github.io/cli.html#web-browser-options) for more
+- Added: client-integrity token support to Twitch plugin using the `streamlink.webbrowser` API (currently only used as a fallback when acquiring the access token fails) ([#5414](https://github.com/streamlink/streamlink/pull/5414))
+- Added: `{playertitleargs}` variable to `--player-args` ([#5310](https://github.com/streamlink/streamlink/pull/5310))
+- Added: `with_{video,audio}_only` parameters to `DASHStream.parse_manifest()` ([#5340](https://github.com/streamlink/streamlink/pull/5340))
+- Changed: HLS streams to stop early on missing `EXT-X-ENDLIST` tag when polling the playlist doesn't yield new segments for twice its targetduration value ([#5330](https://github.com/streamlink/streamlink/pull/5330))
+- Fixed: regex of optional protocol plugin parameters ([#5367](https://github.com/streamlink/streamlink/pull/5367))
+- Fixed plugins: lrt ([#5444](https://github.com/streamlink/streamlink/pull/5444)), mediavitrina ([#5376](https://github.com/streamlink/streamlink/pull/5376)), mitele ([#5436](https://github.com/streamlink/streamlink/pull/5436)), NRK ([#5408](https://github.com/streamlink/streamlink/pull/5408)), pluzz ([#5369](https://github.com/streamlink/streamlink/pull/5369)), rtvs ([#5443](https://github.com/streamlink/streamlink/pull/5443)), showroom ([#5390](https://github.com/streamlink/streamlink/pull/5390)), turkuvaz ([#5374](https://github.com/streamlink/streamlink/pull/5374)), vimeo ([#5335](https://github.com/streamlink/streamlink/pull/5335)), youtube ([#5351](https://github.com/streamlink/streamlink/pull/5351))
+- Docs: added migrations page for further guidance on resolving breaking changes ([#5433](https://github.com/streamlink/streamlink/pull/5433))
+- Docs: split up, updated and improved API docs ([#5398](https://github.com/streamlink/streamlink/pull/5398))
+- Build: moved project metadata to pyproject.toml (PEP621) ([#5438](https://github.com/streamlink/streamlink/pull/5438))
+- Dependencies: added `trio` ([#5386](https://github.com/streamlink/streamlink/pull/5386)), `trio-websocket` and `typing-extensions` ([#5388](https://github.com/streamlink/streamlink/pull/5388)), and removed `importlib_metadata` ([#5302](https://github.com/streamlink/streamlink/pull/5302))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.5.1...6.0.0)
+
+
 ## streamlink 5.5.1 (2023-05-08)
 
 Patch release:
 
 - Fixed: shifting time offset when reloading HLS playlists ([#5321](https://github.com/streamlink/streamlink/pull/5321))
 - Fixed: import of `create_urllib3_context` on `urllib3 <2.0.0` ([#5333](https://github.com/streamlink/streamlink/pull/5333))
 - Fixed: Vimeo plugin ([#5331](https://github.com/streamlink/streamlink/pull/5331))
```

### Comparing `streamlink-5.5.1/docs/cli/config.rst` & `streamlink-6.0.0/docs/cli/config.rst`

 * *Files 13% similar despite different names*

```diff
@@ -8,51 +8,76 @@
 --------
 
 Streamlink will look for config files in different locations depending on
 your platform:
 
 .. rst-class:: table-custom-layout table-custom-layout-platform-locations
 
-================= ====================================================
-Platform          Location
-================= ====================================================
-Linux, BSD        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config``
+.. list-table::
+    :header-rows: 1
+    :width: 100%
 
-                  Deprecated:
+    * - Platform
+      - Location
+    * - Linux, BSD
+      - :bdg-primary:`Path`
 
-                  - ``${HOME}/.streamlinkrc``
-macOS             - ``${HOME}/Library/Application Support/streamlink/config``
+        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config``
 
-                  Deprecated:
+        :bdg-info-line:`Example`
 
-                  - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config``
-                  - ``${HOME}/.streamlinkrc``
-Windows           - ``%APPDATA%\streamlink\config``
+        - ``/home/USERNAME/.config/streamlink/config``
 
-                  Deprecated:
+        :bdg-danger-line:`Deprecated`
 
-                  - ``%APPDATA%\streamlink\streamlinkrc``
-================= ====================================================
+        - ``${HOME}/.streamlinkrc``
+    * - macOS
+      - :bdg-primary:`Path`
+
+        - ``${HOME}/Library/Application Support/streamlink/config``
+
+        :bdg-info-line:`Example`
+
+        - ``/Users/USERNAME/Library/Application Support/streamlink/config``
+
+        :bdg-danger-line:`Deprecated`
+
+        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config``
+        - ``${HOME}/.streamlinkrc``
+    * - Windows
+      - :bdg-primary:`Path`
+
+        - ``%APPDATA%\streamlink\config``
+
+        :bdg-info-line:`Example`
+
+        - ``C:\Users\USERNAME\AppData\Roaming\streamlink\config``
+
+        :bdg-danger-line:`Deprecated`
+
+        - ``%APPDATA%\streamlink\streamlinkrc``
 
 You can also specify the location yourself using the :option:`--config` option.
 
+Loading config files can be suppressed using the :option:`--no-config` option.
+
 .. warning::
 
   Streamlink's Windows installers automatically create a config file if it doesn't exist yet, but on any
   other platform or installation method, you must create the file yourself.
 
 .. note::
 
-   The ``XDG_CONFIG_HOME`` environment variable is part of the `XDG base directory specification`_ (`Arch Wiki <xdg-base-dir-arch-wiki_>`_).
+   The ``XDG_CONFIG_HOME`` environment variable is part of the `XDG base directory specification`_ (`Arch Linux Wiki <xdg-base-dir-arch-wiki_>`_).
 
    The ``${VARIABLENAME:-DEFAULTVALUE}`` syntax is explained `here <Parameter expansion_>`_.
 
 .. _XDG base directory specification: https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html
 .. _xdg-base-dir-arch-wiki: https://wiki.archlinux.org/title/XDG_Base_Directory
-.. _Parameter expansion: https://wiki.bash-hackers.org/syntax/pe
+.. _Parameter expansion: https://www.gnu.org/software/bash/manual/bash.html#Shell-Parameter-Expansion
 
 
 Syntax
 ------
 
 The config file is a simple text file and should contain one
 :ref:`command-line option <cli:Command-line usage>` (omitting the leading dashes) per
@@ -60,64 +85,79 @@
 
   option=value
 
 or for an option without value::
 
   option
 
-.. note::
-    Any quotes used will be part of the value, so only use them when the value needs them,
-    e.g. when specifying a player with a path which contains spaces.
+.. warning::
+
+    Any quotes will be used as part of the argument value.
 
 Example
 ^^^^^^^
 
 .. code-block:: bash
 
     # Player options
-    player=mpv --cache 2048
+    player=mpv
+    player-args=--cache 2048
     player-no-close
 
-.. note::
-    Full player paths are supported via configuration file options such as
-    ``player="C:\mpv-x86_64\mpv"``
-
 
 Plugin specific configuration file
 ----------------------------------
 
-You may want to use specific options for some plugins only. This
-can be accomplished by placing those settings inside a plugin specific
-config file. Options inside these config files will override the main
+You may want to use specific options for some plugins only. This can be accomplished by setting these options
+in plugin-specific config files. Options defined in plugin-specific config files override options of the main
 config file when a URL matching the plugin is used.
 
-Streamlink expects this config to be named like the main config but
-with ``.<plugin name>`` attached to the end.
-
-Examples
-^^^^^^^^
+Streamlink expects these configs to be named like the main config but with ``.<plugin name>`` attached to the end.
 
 .. rst-class:: table-custom-layout table-custom-layout-platform-locations
 
-================= ====================================================
-Platform          Location
-================= ====================================================
-Linux, BSD        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config.pluginname``
+.. list-table::
+    :header-rows: 1
+    :width: 100%
+
+    * - Platform
+      - Location
+    * - Linux, BSD
+      - :bdg-primary:`Path`
+
+        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config.pluginname``
+
+        :bdg-info-line:`Example`
+
+        - ``/home/USERNAME/.config/streamlink/config.twitch``
+
+        :bdg-danger-line:`Deprecated`
+
+        - ``${HOME}/.streamlinkrc.pluginname``
+    * - macOS
+      - :bdg-primary:`Path`
+
+        - ``${HOME}/Library/Application Support/streamlink/config.pluginname``
+
+        :bdg-info-line:`Example`
+
+        - ``/Users/USERNAME/Library/Application Support/streamlink/config.twitch``
+
+        :bdg-danger-line:`Deprecated`
 
-                  Deprecated:
+        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config.pluginname``
+        - ``${HOME}/.streamlinkrc.pluginname``
+    * - Windows
+      - :bdg-primary:`Path`
 
-                  - ``${HOME}/.streamlinkrc.pluginname``
-macOS             - ``${HOME}/Library/Application Support/streamlink/config.pluginname``
+        - ``%APPDATA%\streamlink\config.pluginname``
 
-                  Deprecated:
+        :bdg-info-line:`Example`
 
-                  - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config.pluginname``
-                  - ``${HOME}/.streamlinkrc.pluginname``
-Windows           - ``%APPDATA%\streamlink\config.pluginname``
+        - ``C:\Users\USERNAME\AppData\Roaming\streamlink\config.twitch``
 
-                  Deprecated:
+        :bdg-danger-line:`Deprecated`
 
-                  - ``%APPDATA%\streamlink\streamlinkrc.pluginname``
-================= ====================================================
+        - ``%APPDATA%\streamlink\streamlinkrc.pluginname``
 
 Have a look at the :ref:`list of plugins <plugins:Plugins>`, or
 check the :option:`--plugins` option to see the name of each built-in plugin.
```

### Comparing `streamlink-5.5.1/docs/cli/metadata.rst` & `streamlink-6.0.0/docs/cli/metadata.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/cli/plugin-sideloading.rst` & `streamlink-6.0.0/docs/cli/plugin-sideloading.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,62 @@
 Plugin sideloading
 ==================
 
 Streamlink will attempt to load standalone plugins from these directories:
 
 .. rst-class:: table-custom-layout table-custom-layout-platform-locations
 
-================= ====================================================
-Platform          Location
-================= ====================================================
-Linux, BSD        - ``${XDG_DATA_HOME:-${HOME}/.local/share}/streamlink/plugins``
+.. list-table::
+    :header-rows: 1
+    :width: 100%
 
-                  Deprecated:
+    * - Platform
+      - Location
+    * - Linux, BSD
+      - :bdg-primary:`Path`
 
-                  - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/plugins``
-macOS             - ``${HOME}/Library/Application Support/streamlink/plugins``
+        - ``${XDG_DATA_HOME:-${HOME}/.local/share}/streamlink/plugins``
 
-                  Deprecated:
+        :bdg-info-line:`Example`
 
-                  - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/plugins``
-Windows           - ``%APPDATA%\streamlink\plugins``
-================= ====================================================
+        - ``/home/USERNAME/.local/share/streamlink/plugins``
+
+        :bdg-danger-line:`Deprecated`
+
+        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/plugins``
+    * - macOS
+      - :bdg-primary:`Path`
+
+        - ``${HOME}/Library/Application Support/streamlink/plugins``
+
+        :bdg-info-line:`Example`
+
+        - ``/Users/USERNAME/Library/Application Support/streamlink/plugins``
+
+        :bdg-danger-line:`Deprecated`
+
+        - ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/plugins``
+    * - Windows
+      - :bdg-primary:`Path`
+
+        - ``%APPDATA%\streamlink\plugins``
+
+        :bdg-info-line:`Example`
+
+        - ``C:\Users\USERNAME\AppData\Roaming\streamlink\plugins``
 
 .. note::
 
     If a plugin is added with the same name as a built-in plugin, then
     the added plugin will take precedence. This is useful if you want
     to upgrade plugins independently of the Streamlink version.
 
+    In this case, a log message will be written to log level :option:`debug <--loglevel>`:
+
+        [session][debug] Plugin PLUGINNAME is being overridden by PATH-TO-PLUGIN-FILE
+
 .. warning::
 
-    If one of the sideloaded plugins fails to load, eg. due to a
-    ``SyntaxError`` being raised by the parser, this exception will
-    not get caught by Streamlink and the execution will stop, even if
+    If one of the sideloaded plugins fails to load, e.g. due to a
+    ``SyntaxError`` being raised by the parser, then this exception won't
+    get caught by Streamlink and the execution will stop, even if
     the input stream URL does not match the faulty plugin.
```

### Comparing `streamlink-5.5.1/docs/cli/plugins/crunchyroll.rst` & `streamlink-6.0.0/docs/cli/plugins/crunchyroll.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/cli/plugins/twitch.rst` & `streamlink-6.0.0/docs/cli/plugins/twitch.rst`

 * *Files 16% similar despite different names*

```diff
@@ -81,14 +81,40 @@
 :ref:`Streamlink 1.7.0 in 2020 <changelog:streamlink 1.7.0 (2020-10-18)>`.
 
 **In addition to that**, special API request headers can be set via :option:`--twitch-api-header` or special API request
 parameters can be set via :option:`--twitch-access-token-param` that can prevent ads from being embedded into the stream,
 either :ref:`authentication data <cli/plugins/twitch:Authentication>` or other data discovered by the community.
 
 
+Client-integrity token
+----------------------
+
+In 2022, Twitch added client-integrity tokens to their web player when getting streaming access tokens. These client-integrity
+tokens are calculated using sophisticated JavaScript code which is infeasible to re-implement, as it not only involves
+obfuscated code that's much harder to reverse engineer and to extract data from, but also a custom JavaScript virtual machine
+implementation where bytecode gets interpreted which is encoded prior to that using randomization patterns. The interpreted
+bytecode performs various checks of the user's web browser and its features, and then determines whether the client is legit
+or not. The goal is to prevent bots and third party applications from accessing streams.
+
+Client-integrity tokens were treated as an optional request parameter when getting streaming access tokens.
+This changed on 2023-05-31 when Twitch made them a requirement, and it broke Streamlink's Twitch plugin (#5370).
+
+Since the only sensible solution for Streamlink to calculate client-integrity tokens was using a web browser, a new
+implementation was needed which could automate that. So in ``6.0.0`` the
+:ref:`streamlink.webbrowser <api/webbrowser:Webbrowser>` API was implemented, which requires a Chromium-based web browser being
+installed on the user's system. See the :option:`--webbrowser` and related CLI arguments for more details.
+
+However, a couple of days after Twitch made these changes, they reverted the requirement again, but in order for Streamlink
+to be prepared for such requirements to be turned on again, the webbrowser API was added nevertheless. The decision was made
+to only use the webbrowser API when getting an access token fails, so launching a web browser unnecessarily could be avoided,
+even though it would run invisibly in "headless mode". Should client-integrity tokens be made a requirement again, then
+Streamlink will cache the generated token in the plugin cache after launching the web browser once. This cache can be cleared
+using the :option:`--twitch-purge-client-integrity` option.
+
+
 Low latency streaming
 ---------------------
 
 Low latency streaming on Twitch can be enabled by setting the :option:`--twitch-low-latency` argument and (optionally)
 configuring the :ref:`player <players:Players>` via :option:`--player-args` and reducing its own buffer to a bare minimum.
 
 Setting :option:`--twitch-low-latency` will make Streamlink prefetch future HLS segments that are included in the HLS playlist
```

### Comparing `streamlink-5.5.1/docs/cli/protocols.rst` & `streamlink-6.0.0/docs/cli/protocols.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/cli/proxy.rst` & `streamlink-6.0.0/docs/cli/proxy.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/cli/tutorial.rst` & `streamlink-6.0.0/docs/cli/tutorial.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/cli.rst` & `streamlink-6.0.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/conf.py` & `streamlink-6.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/deprecations.rst` & `streamlink-6.0.0/docs/deprecations.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,109 +1,95 @@
 Deprecations
 ============
 
 streamlink 5.4.0
 ----------------
 
-Deprecation of --force-progress
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+--force-progress
+^^^^^^^^^^^^^^^^
 
 The ``--force-progress`` CLI argument has been deprecated in favor of :option:`--progress=force`.
 
 
 streamlink 5.3.0
 ----------------
 
-Deprecation of global plugin arguments
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Global plugin arguments
+^^^^^^^^^^^^^^^^^^^^^^^
 
 The ``is_global=True`` :py:class:`plugin argument <streamlink.options.Argument>` parameter has been deprecated.
 Instead of defining a global plugin argument to set a key-value pair on the plugin's options, use the respective option on
 the plugin's Streamlink session instance instead.
 
+:bdg-ref-danger:`Removed in 6.0.0 <migrations:Global plugin arguments>`
+
 
 streamlink 5.2.0
 ----------------
 
-Deprecation of plugin.api.validate.text
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+plugin.api.validate.text
+^^^^^^^^^^^^^^^^^^^^^^^^
 
 The ``plugin.api.validate.text`` alias for ``str`` has been marked as deprecated, as it is a remnant of the py2 implementation.
 Simply replace ``validate.text`` with ``str`` in each validation schema.
 
+:bdg-ref-danger:`Removed in 6.0.0 <migrations:plugin.api.validate.text>`
+
 
 streamlink 5.0.0
 ----------------
 
-Deprecation of Plugin.__init__(self, url)
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Plugin.__init__(self, url) compatibility wrapper
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 With the removal of the ``Plugin.bind()`` class method which was used for setting up the
 :py:class:`Streamlink <streamlink.session.Streamlink>` session instance and module name in each plugin class,
 the :py:class:`Plugin <streamlink.plugin.Plugin>` constructor's signature was changed and it now requires
 the ``session`` and ``url`` arguments. Implementors of custom plugins should define variable positional arguments and keyword
 arguments when subclassing and adding a custom constructor (``*args, **kwargs``), and the ``url`` should be accessed via
 ``self.url`` after calling the constructor of the super class.
 
 Compatibility wrappers were added for old custom plugin implementations, and a deprecation message will be shown until
 the compatibility wrappers will get removed in a future release.
 
-
-Session.resolve_url() return type changes
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-Due to the changes of the :py:class:`Plugin <streamlink.plugin.Plugin>` class mentioned above, the return value of
-:py:meth:`Streamlink.resolve_url <streamlink.Streamlink.resolve_url>` and
-:py:meth:`Streamlink.resolve_url_no_redirect <streamlink.Streamlink.resolve_url_no_redirect>` had to be changed
-from ``tuple[type[Plugin], str]`` to ``tuple[str, type[Plugin], str]``, and both methods now return the resolved plugin name
-as the first item, in addition to the plugin class and resolved URL.
+:bdg-ref-danger:`Removed in 6.0.0 <migrations:Plugin.__init__(self, url) compatibility wrapper>`
 
 
 streamlink 4.2.0
 ----------------
 
-Deprecation of url_master in HLSStream
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-The ``url_master`` parameter and attribute of the :py:class:`streamlink.stream.HLSStream`
-and :py:class:`streamlink.stream.MuxedHLSStream` classes have been deprecated in favor of the ``multivariant`` parameter
-and attribute. ``multivariant`` is an :py:class:`M3U8` reference of the parsed HLS multivariant playlist.
+url_master in HLSStream
+^^^^^^^^^^^^^^^^^^^^^^^
 
-
-streamlink 4.0.0
-----------------
-
-Removal of streamlink.plugin.api.utils
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-The ``streamlink.plugin.api.utils`` module including the ``itertags`` function and export aliases for ``streamlink.utils.parse``
-has been removed. Import the parse functions directly and find data in XML/HTML by parsing it via ``parse_{xml,html}`` and
-applying XPath queries to the parsed result via the available methods provided by the ``lxml.etree`` API. The
-``streamlink.plugin.api.validate`` module also has the necessary validation schema functions for this.
+The ``url_master`` parameter and attribute of the :py:class:`HLSStream <streamlink.stream.HLSStream>`
+and :py:class:`MuxedHLSStream <streamlink.stream.MuxedHLSStream>` classes have been deprecated in favor of
+the ``multivariant`` parameter and attribute. ``multivariant`` is an :py:class:`M3U8` reference of the parsed
+HLS multivariant playlist.
 
 
 streamlink 3.0.0
 ----------------
 
-Removal of separate https-proxy option
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+https-proxy option
+^^^^^^^^^^^^^^^^^^
 
-:ref:`HTTPS proxy CLI option <cli:HTTP options>` and the respective :ref:`Session options <api:Session>`
+:ref:`HTTPS proxy CLI option <cli:HTTP options>` and the respective :ref:`Session options <api/session:Session>`
 have been deprecated in favor of a single :option:`--http-proxy` that sets the proxy for all HTTP and
 HTTPS requests, including WebSocket connections.
 
 
 streamlink 2.4.0
 ----------------
 
 Stream-type related CLI arguments
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-:ref:`Stream-type related CLI arguments <cli:Stream transport options>` and the respective :ref:`Session options <api:Session>`
-have been deprecated in favor of existing generic arguments/options, to avoid redundancy and potential confusion.
+:ref:`Stream-type related CLI arguments <cli:Stream transport options>` and the respective
+:ref:`Session options <api/session:Session>` have been deprecated in favor of existing generic arguments/options,
+to avoid redundancy and potential confusion.
 
 - use :option:`--stream-segment-attempts` instead of ``--{dash,hds,hls}-segment-attempts``
 - use :option:`--stream-segment-threads` instead of ``--{dash,hds,hls}-segment-threads``
 - use :option:`--stream-segment-timeout` instead of ``--{dash,hds,hls}-segment-timeout``
 - use :option:`--stream-timeout` instead of ``--{dash,hds,hls,rtmp,http-stream}-timeout``
 
 
@@ -185,14 +171,16 @@
 
 .. note::
 
    Plugins which have more sophisticated logic in their ``can_handle_url()`` classmethod need to be rewritten with
    multiple ``@pluginmatcher`` decorators and/or an improved ``_get_streams()`` method which returns ``None`` or raises a
    ``NoStreamsError`` when there are no streams to be found on that particular URL.
 
+:bdg-ref-danger:`Removed in 6.0.0 <migrations:Plugin.can_handle_url() and Plugin.priority()>`
+
 
 streamlink 2.2.0
 ----------------
 
 Config file paths
 ^^^^^^^^^^^^^^^^^
 
@@ -240,15 +228,14 @@
 Platform  Location
 ========= ========
 Linux/BSD ``${XDG_CONFIG_HOME:-${HOME}/.config}/streamlink/config``
 macOS     ``${HOME}/Library/Application Support/streamlink/config``
 Windows   ``%APPDATA%\streamlink\config``
 ========= ========
 
-
 Custom plugins sideloading paths
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Streamlink's default custom plugins directory path got updated and corrected on Linux/BSD and macOS.
 Old and deprecated paths will be dropped in the future.
 
 **Deprecated paths**
```

### Comparing `streamlink-5.5.1/docs/developing.rst` & `streamlink-6.0.0/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/donate.rst` & `streamlink-6.0.0/docs/donate.rst`

 * *Files 7% similar despite different names*

```diff
@@ -22,48 +22,56 @@
 
 .. grid:: 2 3 5 5
     :padding: 0
     :class-container: team-members
 
     .. grid-item-card::
         :padding: 3
-        :img-top: https://github.com/back-to.png?size=100
-        :link: https://github.com/back-to
-        :link-alt: @back-to
-        :text-align: center
-
-    .. grid-item-card::
-        :padding: 3
         :img-top: https://github.com/bastimeyer.png?size=100
         :link: https://github.com/bastimeyer
         :link-alt: @bastimeyer
         :text-align: center
 
     .. grid-item-card::
         :padding: 3
-        :img-top: https://github.com/beardypig.png?size=100
-        :link: https://github.com/beardypig
-        :link-alt: @beardypig
-        :text-align: center
-
-    .. grid-item-card::
-        :padding: 3
         :img-top: https://github.com/gravyboat.png?size=100
         :link: https://github.com/gravyboat
         :link-alt: @gravyboat
         :text-align: center
 
     .. grid-item-card::
         :padding: 3
         :img-top: https://github.com/mkbloke.png?size=100
         :link: https://github.com/mkbloke
         :link-alt: @mkbloke
         :text-align: center
 
 
+Inactive / former
+^^^^^^^^^^^^^^^^^
+
+.. grid:: 2 3 5 5
+    :padding: 0
+    :class-container: team-members
+
+    .. grid-item-card::
+        :padding: 3
+        :img-top: https://github.com/back-to.png?size=100
+        :link: https://github.com/back-to
+        :link-alt: @back-to
+        :text-align: center
+
+    .. grid-item-card::
+        :padding: 3
+        :img-top: https://github.com/beardypig.png?size=100
+        :link: https://github.com/beardypig
+        :link-alt: @beardypig
+        :text-align: center
+
+
 Useful links
 ============
 
 - Streamlink's GitHub releases with the changelog summary and commit history of each release:
 
   https://github.com/streamlink/streamlink/releases
```

### Comparing `streamlink-5.5.1/docs/ext_argparse.py` & `streamlink-6.0.0/docs/ext_argparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from docutils.parsers.rst.directives import unchanged
 from docutils.statemachine import ViewList
 from sphinx.util.nodes import nested_parse_with_titles
 
 
 _block_re = re.compile(r":\n{2}\s{2}")
 _default_re = re.compile(r"Default is (.+)\.\n")
-_note_re = re.compile(r"Note: (.*)(?:\n\n|\n*$)", re.DOTALL)
+_note_re = re.compile(r"Note: (.*?)(?:\n\n|\n*$)", re.DOTALL)
 _option_line_re = re.compile(r"^(?!\s{2,}%\(prog\)s|\s{2,}--\w[\w-]*\w\b|Example: )(.+)$", re.MULTILINE)
 _option_re = re.compile(r"(?:^|(?<=\s))(?P<arg>--\w[\w-]*\w)(?P<val>=\w+)?\b")
 _prog_re = re.compile(r"%\(prog\)s")
 _percent_re = re.compile(r"%%")
 _cli_metadata_variables_section_cross_link_re = re.compile(r"the \"Metadata variables\" section")
 _inline_code_block_re = re.compile(r"(?<!`)`([^`]+?)`")
 _example_inline_code_block_re = re.compile(r"(?<=^Example: )(.+)$", re.MULTILINE)
```

### Comparing `streamlink-5.5.1/docs/ext_github.py` & `streamlink-6.0.0/docs/ext_github.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/ext_plugins.py` & `streamlink-6.0.0/docs/ext_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/ext_releaseref.py` & `streamlink-6.0.0/docs/ext_releaseref.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/index.rst` & `streamlink-6.0.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     Overview <self>
     install
     cli
     plugins
     players
     issues
     deprecations
+    migrations
     developing
     api_guide
     api
     changelog
     donate
     applications
     thirdparty
```

### Comparing `streamlink-5.5.1/docs/install.rst` & `streamlink-6.0.0/docs/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                                         sudo eopkg install streamlink
 
 `Void`_                              .. code-block:: bash
 
                                         sudo xbps-install streamlink
 ==================================== ===========================================
 
-.. _Arch Linux: https://www.archlinux.org/packages/community/any/streamlink/
+.. _Arch Linux: https://archlinux.org/packages/extra/any/streamlink/
 .. _Arch Linux (aur, git): https://aur.archlinux.org/packages/streamlink-git/
 .. _Debian (sid, testing): https://packages.debian.org/unstable/streamlink
 .. _Debian (stable): https://packages.debian.org/unstable/streamlink
 .. _Fedora: https://src.fedoraproject.org/rpms/python-streamlink
 .. _Gentoo Linux: https://packages.gentoo.org/package/net-misc/streamlink
 .. _NetBSD (pkgsrc): https://pkgsrc.se/multimedia/streamlink
 .. _NixOS: https://github.com/NixOS/nixpkgs/tree/master/pkgs/applications/video/streamlink
@@ -359,28 +359,31 @@
 Streamlink defines a `build system <pyproject.toml_>`__ according to `PEP-517`_ / `PEP-518`_.
 
 .. rst-class:: table-custom-layout table-custom-layout-dependencies
 
 ========= ========================= ===========================================
 Type      Name                       Notes
 ========= ========================= ===========================================
-python    `Python`_                 At least version **3.7**.
+python    `Python`_                 At least version **3.8**.
 
-build     `setuptools`_             At least version **45.0.0**. |br| Used as build backend.
+build     `setuptools`_             At least version **64.0.0**. |br| Used as build backend.
 build     `wheel`_                  Used by the build frontend for creating Python wheels.
 build     `versioningit`_           At least version **2.0.0**. |br| Used for generating the version string from git
                                     when building, or when running in an editable install.
 
 runtime   `certifi`_                Used for loading the CA bundle extracted from the Mozilla Included CA Certificate List
 runtime   `isodate`_                Used for parsing ISO8601 strings
 runtime   `lxml`_                   Used for processing HTML and XML data
 runtime   `pycountry`_              Used for localization settings, provides country and language data
 runtime   `pycryptodome`_           Used for decrypting encrypted streams
 runtime   `PySocks`_                Used for SOCKS Proxies
 runtime   `requests`_               Used for making any kind of HTTP/HTTPS request
+runtime   `trio`_                   Used for async concurrency and I/O in some parts of Streamlink
+runtime   `trio-websocket`_         Used for WebSocket connections on top of the async trio framework
+runtime   `typing-extensions`_      Used for backporting runtime support of certain type hints on older Python versions
 runtime   `urllib3`_                Used internally by `requests`_, defined as direct dependency
 runtime   `websocket-client`_       Used for making websocket connections
 
 optional  `FFmpeg`_                 Required for `muxing`_ multiple video/audio/subtitle streams into a single output stream.
 
                                      - DASH streams with video and audio content always have to get remuxed.
                                      - HLS streams optionally need to get remuxed depending on the stream selection.
@@ -398,14 +401,17 @@
 .. _certifi: https://certifiio.readthedocs.io/en/latest/
 .. _isodate: https://pypi.org/project/isodate/
 .. _lxml: https://lxml.de/
 .. _pycountry: https://pypi.org/project/pycountry/
 .. _pycryptodome: https://pycryptodome.readthedocs.io/en/latest/
 .. _PySocks: https://github.com/Anorov/PySocks
 .. _requests: https://requests.readthedocs.io/en/latest/
+.. _trio: https://trio.readthedocs.io/en/stable/
+.. _trio-websocket: https://trio-websocket.readthedocs.io/en/stable/
+.. _typing-extensions: https://typing-extensions.readthedocs.io/en/stable/
 .. _urllib3: https://urllib3.readthedocs.io/en/stable/
 .. _websocket-client: https://pypi.org/project/websocket-client/
 
 .. _FFmpeg: https://www.ffmpeg.org/
 .. _muxing: https://en.wikipedia.org/wiki/Multiplexing#Video_processing
```

### Comparing `streamlink-5.5.1/docs/issues.rst` & `streamlink-6.0.0/docs/issues.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/players.rst` & `streamlink-6.0.0/docs/players.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/docs/thirdparty.rst` & `streamlink-6.0.0/docs/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/icon.svg` & `streamlink-6.0.0/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/setup.py` & `streamlink-6.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def format_msg(text, *args, **kwargs):
     return dedent(text).strip(" \n").format(*args, **kwargs)
 
 
 CURRENT_PYTHON = version_info[:2]
-REQUIRED_PYTHON = (3, 7)
+REQUIRED_PYTHON = (3, 8)
 
 # This check and everything above must remain compatible with older Python versions
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     exit(format_msg("""
         ========================================================
                        Unsupported Python version
         ========================================================
```

### Comparing `streamlink-5.5.1/src/streamlink/__init__.py` & `streamlink-6.0.0/src/streamlink/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/_version.py` & `streamlink-6.0.0/src/streamlink/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
     return get_version(
         project_dir=Path(streamlink.__file__).parents[2],
     )
 
 
 # The following _get_version() call will get replaced by versioningit with a static version string when building streamlink
 # `pip install .` / `pip wheel .` / `python setup.py build` / `python setup.py bdist_wheel` / etc.
-__version__ = "5.5.1"
+__version__ = "6.0.0"
```

### Comparing `streamlink-5.5.1/src/streamlink/api.py` & `streamlink-6.0.0/src/streamlink/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def streams(url: str, **params):
     """
     Initializes an empty Streamlink session, attempts to find a plugin and extracts streams from the URL if a plugin was found.
 
     :param url: a URL to match against loaded plugins
-    :param params: Additional keyword arguments passed to :meth:`streamlink.Streamlink.streams`
+    :param params: Additional keyword arguments passed to :meth:`Streamlink.streams() <streamlink.session.Streamlink.streams>`
     :raises NoPluginError: on plugin resolve failure
-    :returns: A :class:`dict` of stream names and :class:`streamlink.stream.Stream` instances
+    :returns: A :class:`dict` of stream names and :class:`Stream <streamlink.stream.Stream>` instances
     """
 
     session = Streamlink()
 
     return session.streams(url, **params)
```

### Comparing `streamlink-5.5.1/src/streamlink/buffers.py` & `streamlink-6.0.0/src/streamlink/buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/cache.py` & `streamlink-6.0.0/src/streamlink/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/exceptions.py` & `streamlink-6.0.0/src/streamlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/logger.py` & `streamlink-6.0.0/src/streamlink/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 import warnings
 from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING
 from pathlib import Path
 from sys import version_info
 from threading import Lock
-from typing import IO, TYPE_CHECKING, Iterator, List, Optional, Union
+from typing import IO, TYPE_CHECKING, Iterator, List, Literal, Optional, Union
 
 # noinspection PyProtectedMember
 from warnings import WarningMessage
 
 from streamlink.exceptions import StreamlinkWarning
 from streamlink.utils.times import fromlocaltimestamp
 
@@ -30,15 +30,15 @@
             yield from messages
 
         for message in messages:
             self._log(level, message, args, **kwargs)
             yield message
 
 
-FORMAT_STYLE = "{"
+FORMAT_STYLE: Literal["%", "{", "$"] = "{"
 FORMAT_BASE = "[{name}][{levelname}] {message}"
 FORMAT_DATE = "%H:%M:%S"
 REMOVE_BASE = ["streamlink", "streamlink_cli"]
 
 # Make NONE ("none") the highest possible level that suppresses all log messages:
 #  `logging.NOTSET` (equal to 0) can't be used as the "none" level because of `logging.Logger.getEffectiveLevel()`, which
 #  loops through the logger instance's ancestor chain and checks whether the instance's level is NOTSET. If it is NOTSET,
@@ -181,15 +181,15 @@
 # noinspection PyShadowingBuiltins,PyPep8Naming
 def basicConfig(
     filename: Optional[Union[str, Path]] = None,
     filemode: str = "a",
     stream: Optional[IO] = None,
     level: Optional[str] = None,
     format: str = FORMAT_BASE,  # noqa: A002  # TODO: rename to "fmt" (breaking)
-    style: str = FORMAT_STYLE,  # TODO: py38: Literal["%", "{", "$"]
+    style: Literal["%", "{", "$"] = FORMAT_STYLE,
     datefmt: str = FORMAT_DATE,
     remove_base: Optional[List[str]] = None,
     capture_warnings: bool = False,
 ) -> logging.StreamHandler:
     with _config_lock:
         handler: logging.StreamHandler
         if filename is not None:
```

### Comparing `streamlink-5.5.1/src/streamlink/options.py` & `streamlink-6.0.0/src/streamlink/options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import warnings
 from typing import Any, Callable, ClassVar, Dict, Iterator, Mapping, Optional, Sequence, Union
 
-from streamlink.exceptions import StreamlinkDeprecationWarning
-
 
 class Options:
     """
     For storing options to be used by the Streamlink session and plugins, with default values.
 
     Note: Option names are normalized by replacing "_" with "-".
           This means that the keys ``example_one`` and ``example-one`` are equivalent.
     """
 
     _MAP_GETTERS: ClassVar[Mapping[str, Callable[[Any, str], Any]]] = {}
+    """Optional getter mapping for :class:`Options` subclasses"""
+
     _MAP_SETTERS: ClassVar[Mapping[str, Callable[[Any, str, Any], None]]] = {}
+    """Optional setter mapping for :class:`Options` subclasses"""
 
     def __init__(self, defaults: Optional[Mapping[str, Any]] = None):
         if not defaults:
             defaults = {}
 
         self.defaults = self._normalize_dict(defaults)
         self.options = self.defaults.copy()
@@ -28,42 +28,54 @@
 
     @classmethod
     def _normalize_dict(cls, src: Mapping[str, Any]) -> Dict[str, Any]:
         normalize_key = cls._normalize_key
         return {normalize_key(key): value for key, value in src.items()}
 
     def clear(self) -> None:
+        """Restore default options"""
+
         self.options.clear()
         self.options.update(self.defaults.copy())
 
     def get(self, key: str) -> Any:
+        """Get the stored value of a specific key"""
+
         normalized = self._normalize_key(key)
         method = self._MAP_GETTERS.get(normalized)
         if method is not None:
             return method(self, normalized)
         else:
             return self.options.get(normalized)
 
     def get_explicit(self, key: str) -> Any:
+        """Get the stored value of a specific key and ignore any get-mappings"""
+
         normalized = self._normalize_key(key)
         return self.options.get(normalized)
 
     def set(self, key: str, value: Any) -> None:
+        """Set the value for a specific key"""
+
         normalized = self._normalize_key(key)
         method = self._MAP_SETTERS.get(normalized)
         if method is not None:
             method(self, normalized, value)
         else:
             self.options[normalized] = value
 
     def set_explicit(self, key: str, value: Any) -> None:
+        """Set the value for a specific key and ignore any set-mappings"""
+
         normalized = self._normalize_key(key)
         self.options[normalized] = value
 
     def update(self, options: Mapping[str, Any]) -> None:
+        """Merge options"""
+
         for key, value in options.items():
             self.set(key, value)
 
     def keys(self):
         return self.options.keys()
 
     def values(self):
@@ -86,15 +98,15 @@
 
     def __iter__(self):
         return self.options.__iter__()
 
 
 class Argument:
     """
-    Accepts most of the parameters accepted by :meth:`ArgumentParser.add_argument`,
+    Accepts most of the parameters accepted by :meth:`ArgumentParser.add_argument()`,
     except that ``requires`` is a special case which is only enforced if the plugin is in use.
     In addition, the ``name`` parameter is the name relative to the plugin name, but can be overridden by ``argument_name``.
 
     Should not be called directly, see the :func:`pluginargument <streamlink.plugin.pluginargument>` decorator.
     """
 
     def __init__(
@@ -102,62 +114,51 @@
         name: str,
         required: bool = False,
         requires: Optional[Union[str, Sequence[str]]] = None,
         prompt: Optional[str] = None,
         sensitive: bool = False,
         argument_name: Optional[str] = None,
         dest: Optional[str] = None,
-        is_global: bool = False,
         **options,
     ):
         """
         :param name: Argument name, without leading ``--`` or plugin name prefixes, e.g. ``"username"``, ``"password"``, etc.
         :param required: Whether the argument is required for the plugin
         :param requires: List of arguments which this argument requires, eg ``["password"]``
         :param prompt: If the argument is required and not set, this prompt message will be shown instead
         :param sensitive: Whether the argument is sensitive (passwords, etc.) and should be masked
         :param argument_name: Custom CLI argument name without plugin name prefix
         :param dest: Custom plugin option name
-        :param is_global: Whether this plugin argument refers to a global CLI argument (deprecated)
-        :param options: Arguments passed to :meth:`ArgumentParser.add_argument`, excluding ``requires`` and ``dest``
+        :param options: Arguments passed to :meth:`ArgumentParser.add_argument()`, excluding ``requires`` and ``dest``
         """
 
         self.required = required
         self.name = name
         self.options = options
         self._argument_name = self._normalize_name(argument_name) if argument_name else None
         self._dest = self._normalize_dest(dest) if dest else None
         requires = requires or []
         self.requires = list(requires) if isinstance(requires, (list, tuple)) else [requires]
         self.prompt = prompt
         self.sensitive = sensitive
         self._default = options.get("default")
-        self.is_global = is_global
-        if is_global:
-            warnings.warn(
-                "Defining global plugin arguments is deprecated. Use the session options instead.",
-                StreamlinkDeprecationWarning,
-                # set stacklevel to 3 because of the @pluginargument decorator
-                # which is the public interface for defining plugin arguments
-                stacklevel=3,
-            )
 
     @staticmethod
     def _normalize_name(name: str) -> str:
         return name.replace("_", "-").strip("-")
 
     @staticmethod
     def _normalize_dest(name: str) -> str:
         return name.replace("-", "_")
 
     def _name(self, plugin):
         return self._argument_name or self._normalize_name(f"{plugin}-{self.name}")
 
     def argument_name(self, plugin):
-        return f"--{self.name if self.is_global else self._name(plugin)}"
+        return f"--{self._name(plugin)}"
 
     def namespace_dest(self, plugin):
         return self._normalize_dest(self._name(plugin))
 
     @property
     def dest(self):
         return self._dest or self._normalize_dest(self.name)
@@ -176,16 +177,15 @@
 
     def __init__(self, *args):
         # keep the initial arguments of the constructor in reverse order (see __iter__())
         self.arguments = {arg.name: arg for arg in reversed(args)}
 
     def __iter__(self) -> Iterator[Argument]:
         # iterate in reverse order due to add() being called by multiple pluginargument decorators in reverse order
-        # TODO: Python 3.7 removal: remove list()
-        return reversed(list(self.arguments.values()))
+        return reversed(self.arguments.values())
 
     def add(self, argument: Argument) -> None:
         self.arguments[argument.name] = argument
 
     def get(self, name: str) -> Optional[Argument]:
         return self.arguments.get(name)
```

### Comparing `streamlink-5.5.1/src/streamlink/packages/requests_file.py` & `streamlink-6.0.0/src/streamlink/packages/requests_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugin/__init__.py` & `streamlink-6.0.0/src/streamlink/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugin/api/http_session.py` & `streamlink-6.0.0/src/streamlink/plugin/api/http_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
 import time
+import warnings
 from typing import Any, Dict, Pattern, Tuple
 
 import requests.adapters
 import urllib3
 from requests import PreparedRequest, Request, Session
 from requests.adapters import HTTPAdapter
 
-from streamlink.exceptions import PluginError
+from streamlink.exceptions import PluginError, StreamlinkDeprecationWarning
 from streamlink.packages.requests_file import FileAdapter
 from streamlink.plugin.api import useragents
 from streamlink.utils.parse import parse_json, parse_xml
 
 
 try:
     from urllib3.util import create_urllib3_context  # type: ignore[attr-defined]
@@ -86,42 +87,48 @@
 
         self.headers["User-Agent"] = useragents.FIREFOX
         self.timeout = 20.0
 
         self.mount("file://", FileAdapter())
 
     @classmethod
-    def determine_json_encoding(cls, sample):
+    def determine_json_encoding(cls, sample: bytes):
         """
         Determine which Unicode encoding the JSON text sample is encoded with
 
-        RFC4627 (http://www.ietf.org/rfc/rfc4627.txt) suggests that the encoding of JSON text can be determined
+        RFC4627 suggests that the encoding of JSON text can be determined
         by checking the pattern of NULL bytes in first 4 octets of the text.
+        https://datatracker.ietf.org/doc/html/rfc4627#section-3
+
         :param sample: a sample of at least 4 bytes of the JSON text
         :return: the most likely encoding of the JSON text
         """
-        nulls_at = [i for i, j in enumerate(bytearray(sample[:4])) if j == 0]
-        if nulls_at == [0, 1, 2]:
+        warnings.warn("Deprecated HTTPSession.determine_json_encoding() call", StreamlinkDeprecationWarning, stacklevel=1)
+        data = int.from_bytes(sample[:4], "big")
+
+        if data & 0xffffff00 == 0:
             return "UTF-32BE"
-        elif nulls_at == [0, 2]:
+        elif data & 0xff00ff00 == 0:
             return "UTF-16BE"
-        elif nulls_at == [1, 2, 3]:
+        elif data & 0x00ffffff == 0:
             return "UTF-32LE"
-        elif nulls_at == [1, 3]:
+        elif data & 0x00ff00ff == 0:
             return "UTF-16LE"
         else:
             return "UTF-8"
 
     @classmethod
     def json(cls, res, *args, **kwargs):
         """Parses JSON from a response."""
-        # if an encoding is already set then use the provided encoding
         if res.encoding is None:
-            res.encoding = cls.determine_json_encoding(res.content[:4])
-        return parse_json(res.text, *args, **kwargs)
+            # encoding is unknown: let ``json.loads`` figure it out from the bytes data via ``json.detect_encoding``
+            return parse_json(res.content, *args, **kwargs)
+        else:
+            # encoding is explicitly set: get the decoded string value and let ``json.loads`` parse it
+            return parse_json(res.text, *args, **kwargs)
 
     @classmethod
     def xml(cls, res, *args, **kwargs):
         """Parses XML from a response."""
         return parse_xml(res.text, *args, **kwargs)
 
     def resolve_url(self, url):
```

### Comparing `streamlink-5.5.1/src/streamlink/plugin/api/validate/_exception.py` & `streamlink-6.0.0/src/streamlink/plugin/api/validate/_exception.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugin/api/validate/_schemas.py` & `streamlink-6.0.0/src/streamlink/plugin/api/validate/_schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, FrozenSet, List, Optional, Pattern, Sequence, Set, Tuple, Type, Union
+from typing import Any, Callable, FrozenSet, List, Literal, Optional, Pattern, Sequence, Set, Tuple, Type, Union
 
 
 class SchemaContainer:
     """
     A simple schema container.
     """
 
@@ -67,16 +67,15 @@
     """
     A regex pattern that must match using the provided method.
     """
 
     def __init__(
         self,
         pattern: Pattern,
-        # TODO: change type from str to Literal["search", "match", "fullmatch", "findall", "split", "sub", "subn"]
-        method: str = "search",
+        method: Literal["search", "match", "fullmatch", "findall", "split", "sub", "subn"] = "search",
     ):
         self.pattern = pattern
         self.method = method
 
 
 class TransformSchema:
     """
```

### Comparing `streamlink-5.5.1/src/streamlink/plugin/api/validate/_validate.py` & `streamlink-6.0.0/src/streamlink/plugin/api/validate/_validate.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugin/api/validate/_validators.py` & `streamlink-6.0.0/src/streamlink/plugin/api/validate/_validators.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugin/api/websocket.py` & `streamlink-6.0.0/src/streamlink/plugin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugin/plugin.py` & `streamlink-6.0.0/src/streamlink/plugin/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import ast
-import inspect
 import logging
 import operator
 import re
 import time
-import warnings
+from contextlib import suppress
 from functools import partial
 from http.cookiejar import Cookie
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
@@ -167,19 +166,16 @@
     rval: Dict[str, Any] = {}
     if not params:
         return rval
 
     matches = re.findall(PARAMS_REGEX, params)
 
     for key, value in matches:
-        try:
+        with suppress(Exception):
             value = ast.literal_eval(value)
-        except Exception:
-            pass
-
         rval[key] = value
 
     return rval
 
 
 class Matcher(NamedTuple):
     pattern: Pattern
@@ -216,24 +212,14 @@
         self.extend(match for matcher, match in matches)
         self._names.clear()
         self._names.update((matcher.name, match) for matcher, match in matches if matcher.name)
 
         return next(((matcher.pattern, match) for matcher, match in matches if match is not None), (None, None))
 
 
-# Add front- and back-wrappers to the deprecated plugin's method resolution order (see Plugin.__new__)
-class PluginWrapperMeta(type):
-    def mro(cls):
-        # cls.__base__ is the PluginWrapperFront which is based on the deprecated plugin class
-        mro = list(cls.__base__.__mro__)
-        # cls is the PluginWrapperBack and needs to be inserted after the deprecated plugin class
-        mro.insert(2, cls)
-        return mro
-
-
 class Plugin:
     """
     Plugin base class for retrieving streams and metadata from the URL specified.
     """
 
     matchers: ClassVar[Optional[Matchers]] = None
     """
@@ -258,80 +244,40 @@
 
     matcher: Optional[Pattern] = None
     """A reference to the compiled :class:`re.Pattern` of the first matching matcher"""
 
     match: Optional[Match] = None
     """A reference to the :class:`re.Match` result of the first matching matcher"""
 
+    options: Options
+    """Plugin options, initialized with the user-set values of the plugin's arguments"""
+
     # plugin metadata attributes
     id: Optional[str] = None
     """Metadata 'id' attribute: unique stream ID, etc."""
     title: Optional[str] = None
     """Metadata 'title' attribute: the stream's short descriptive title"""
     author: Optional[str] = None
     """Metadata 'author' attribute: the channel or broadcaster name, etc."""
     category: Optional[str] = None
     """Metadata 'category' attribute: name of a game being played, a music genre, etc."""
 
-    options = Options()
     _url: str = ""
 
-    # deprecated
-    can_handle_url: Callable[[str], bool]
-    # deprecated
-    priority: Callable[[str], int]
-
-    # Handle deprecated plugin constructors which only take the url argument
-    def __new__(cls, *args, **kwargs):
-        # Ignore plugins without custom constructors or wrappers
-        if cls.__init__ is Plugin.__init__ or hasattr(cls, "_IS_DEPRECATED_PLUGIN_WRAPPER"):
-            return super().__new__(cls)
-
-        # Ignore custom constructors which have a formal "session" parameter or a variable positional parameter
-        sig = inspect.signature(cls.__init__).parameters
-        if "session" in sig or any(param.kind == inspect.Parameter.VAR_POSITIONAL for param in sig.values()):
-            return super().__new__(cls)
-
-        # Wrapper class which overrides the very first constructor in the MRO
-        # noinspection PyAbstractClass
-        class PluginWrapperFront(cls):
-            _IS_DEPRECATED_PLUGIN_WRAPPER = True
-
-            # The __module__ value needs to be copied
-            __module__ = cls.__module__
-
-            def __init__(self, session, url):
-                # Take any arguments, but only pass the URL to the custom constructor of the deprecated plugin
-                # noinspection PyArgumentList
-                super().__init__(url)
-                warnings.warn(
-                    f"Initialized {self.module} plugin with deprecated constructor",
-                    FutureWarning,
-                    stacklevel=2,
-                )
-
-        # Wrapper class which comes after the deprecated plugin in the MRO
-        # noinspection PyAbstractClass
-        class PluginWrapperBack(PluginWrapperFront, metaclass=PluginWrapperMeta):
-            def __init__(self, *_, **__):
-                # Take any arguments from the super() call of the constructor of the deprecated plugin,
-                # but pass the right args and keywords to the Plugin constructor
-                super().__init__(*args, **kwargs)
-
-        return cls.__new__(PluginWrapperBack, *args, **kwargs)
-
-    def __init__(self, session: "Streamlink", url: str):
+    def __init__(self, session: "Streamlink", url: str, options: Optional[Options] = None):
         """
         :param session: The Streamlink session instance
         :param url: The input URL used for finding and resolving streams
+        :param options: An optional :class:`Options` instance
         """
 
         modulename = self.__class__.__module__
         self.module = modulename.split(".")[-1]
         self.logger = logging.getLogger(modulename)
+        self.options = Options() if options is None else options
         self.cache = Cache(
             filename="plugin-cache.json",
             key_prefix=self.module,
         )
 
         self.session: "Streamlink" = session
         self.matches = Matches()
@@ -351,21 +297,19 @@
     @url.setter
     def url(self, value: str):
         self._url = value
 
         if self.matchers:
             self.matcher, self.match = self.matches.update(self.matchers, value)
 
-    @classmethod
-    def set_option(cls, key, value):
-        cls.options.set(key, value)
+    def set_option(self, key, value):
+        self.options.set(key, value)
 
-    @classmethod
-    def get_option(cls, key):
-        return cls.options.get(key)
+    def get_option(self, key):
+        return self.options.get(key)
 
     @classmethod
     def get_argument(cls, key):
         return cls.arguments and cls.arguments.get(key)
 
     @classmethod
     def stream_weight(cls, stream):
@@ -385,15 +329,15 @@
 
     def streams(self, stream_types=None, sorting_excludes=None):
         """
         Attempts to extract available streams.
 
         Returns a :class:`dict` containing the streams, where the key is
         the name of the stream (most commonly the quality name), with the value
-        being a :class:`Stream` instance.
+        being a :class:`Stream <streamlink.stream.Stream>` instance.
 
         The result can contain the synonyms **best** and **worst** which
         point to the streams which are likely to be of highest and
         lowest quality respectively.
 
         If multiple streams with the same name are found, the order of
         streams specified in *stream_types* will determine which stream
@@ -411,15 +355,15 @@
 
             - A function that is passed to :meth:`filter` with a list of
               stream names as input.
 
 
         :param stream_types: A list of stream types to return
         :param sorting_excludes: Specify which streams to exclude from the best/worst synonyms
-        :returns: A :class:`dict` of stream names and :class:`streamlink.stream.Stream` instances
+        :returns: A :class:`dict` of stream names and :class:`Stream <streamlink.stream.Stream>` instances
         """
 
         try:
             ostreams = self._get_streams()
             if isinstance(ostreams, dict):
                 ostreams = ostreams.items()
 
@@ -514,16 +458,17 @@
 
         return final_sorted_streams
 
     def _get_streams(self):
         """
         Implement the stream and metadata retrieval here.
 
-        Needs to return either a dict of :class:`streamlink.stream.Stream` instances mapped by stream name, or needs to act
-        as a generator which yields tuples of stream names and :class:`streamlink.stream.Stream` instances.
+        Needs to return either a dict of :class:`Stream <streamlink.stream.Stream>` instances mapped by stream name,
+        or needs to act as a generator which yields tuples of stream names and :class:`Stream <streamlink.stream.Stream>`
+        instances.
         """
 
         raise NotImplementedError
 
     def get_metadata(self) -> Dict[str, Optional[str]]:
         return dict(
             id=self.get_id(),
@@ -604,15 +549,15 @@
             self.logger.debug(f"Restored cookies: {', '.join(restored)}")
 
         return restored
 
     def clear_cookies(self, cookie_filter: Optional[Callable] = None) -> List[str]:
         """
         Removes all saved cookies for this plugin. To filter the cookies that are deleted
-        specify the ``cookie_filter`` argument (see :func:`save_cookies`).
+        specify the ``cookie_filter`` argument (see :meth:`save_cookies`).
 
         :param cookie_filter: a function to filter the cookies
         :type cookie_filter: function
         :return: list of the removed cookie names
         """
 
         cookie_filter = cookie_filter or (lambda c: True)
@@ -654,15 +599,15 @@
 ) -> Callable[[Type[Plugin]], Type[Plugin]]:
     """
     Decorator for plugin URL matchers.
 
     A matcher consists of a compiled regular expression pattern for the plugin's input URL,
     a priority value and an optional name.
     The priority value determines which plugin gets chosen by
-    :meth:`Streamlink.resolve_url <streamlink.Streamlink.resolve_url>` if multiple plugins match the input URL.
+    :meth:`Streamlink.resolve_url() <streamlink.session.Streamlink.resolve_url>` if multiple plugins match the input URL.
     The matcher name can be used for accessing it and its matching result when multiple matchers are defined.
 
     Plugins must at least have one matcher. If multiple matchers are defined, then the first matching one
     according to the order of which they have been defined (top to bottom) will be responsible for setting the
     :attr:`Plugin.matcher` and :attr:`Plugin.match` attributes on the :class:`Plugin` instance.
     The :attr:`Plugin.matchers` and :attr:`Plugin.matches` attributes are affected by all defined matchers,
     and both support referencing matchers and matches by matcher index and name.
@@ -705,19 +650,18 @@
     name: str,
     required: bool = False,
     requires: Optional[Union[str, Sequence[str]]] = None,
     prompt: Optional[str] = None,
     sensitive: bool = False,
     argument_name: Optional[str] = None,
     dest: Optional[str] = None,
-    is_global: bool = False,
     **options,
 ) -> Callable[[Type[Plugin]], Type[Plugin]]:
     """
-    Decorator for plugin arguments. Takes the same arguments as :class:`streamlink.options.Argument`.
+    Decorator for plugin arguments. Takes the same arguments as :class:`Argument <streamlink.options.Argument>`.
 
     .. code-block:: python
 
         from streamlink.plugin import Plugin, pluginargument
 
 
         @pluginargument(
@@ -743,15 +687,14 @@
         name,
         required=required,
         requires=requires,
         prompt=prompt,
         sensitive=sensitive,
         argument_name=argument_name,
         dest=dest,
-        is_global=is_global,
         **options,
     )
 
     def decorator(cls: Type[Plugin]) -> Type[Plugin]:
         if not issubclass(cls, Plugin):
             raise TypeError(f"{repr(cls)} is not a Plugin")
         if cls.arguments is None:
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/abematv.py` & `streamlink-6.0.0/src/streamlink/plugins/abematv.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import re
 import struct
 import time
 import uuid
 from base64 import urlsafe_b64encode
 from binascii import unhexlify
 
-from Crypto.Cipher import AES
 from requests import Response
 from requests.adapters import BaseAdapter
 
 from streamlink.exceptions import NoStreamsError
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import useragents, validate
 from streamlink.stream.hls import HLSStream, HLSStreamReader, HLSStreamWriter
+from streamlink.utils.crypto import AES
 from streamlink.utils.url import update_qsd
 
 
 log = logging.getLogger(__name__)
 
 
 class AbemaTVHLSStreamWriter(HLSStreamWriter):
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/adultswim.py` & `streamlink-6.0.0/src/streamlink/plugins/adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/afreeca.py` & `streamlink-6.0.0/src/streamlink/plugins/afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/albavision.py` & `streamlink-6.0.0/src/streamlink/plugins/albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/aloula.py` & `streamlink-6.0.0/src/streamlink/plugins/aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/app17.py` & `streamlink-6.0.0/src/streamlink/plugins/app17.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ard_live.py` & `streamlink-6.0.0/src/streamlink/plugins/ard_live.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ard_mediathek.py` & `streamlink-6.0.0/src/streamlink/plugins/ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/artetv.py` & `streamlink-6.0.0/src/streamlink/plugins/artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/atpchallenger.py` & `streamlink-6.0.0/src/streamlink/plugins/atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/atresplayer.py` & `streamlink-6.0.0/src/streamlink/plugins/atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/bbciplayer.py` & `streamlink-6.0.0/src/streamlink/plugins/bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/bfmtv.py` & `streamlink-6.0.0/src/streamlink/plugins/bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/bigo.py` & `streamlink-6.0.0/src/streamlink/plugins/bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/bilibili.py` & `streamlink-6.0.0/src/streamlink/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/blazetv.py` & `streamlink-6.0.0/src/streamlink/plugins/blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/bloomberg.py` & `streamlink-6.0.0/src/streamlink/plugins/bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/booyah.py` & `streamlink-6.0.0/src/streamlink/plugins/booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/brightcove.py` & `streamlink-6.0.0/src/streamlink/plugins/brightcove.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/btv.py` & `streamlink-6.0.0/src/streamlink/plugins/btv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/cbsnews.py` & `streamlink-6.0.0/src/streamlink/plugins/cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/cdnbg.py` & `streamlink-6.0.0/src/streamlink/plugins/cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ceskatelevize.py` & `streamlink-6.0.0/src/streamlink/plugins/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/cinergroup.py` & `streamlink-6.0.0/src/streamlink/plugins/cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/clubbingtv.py` & `streamlink-6.0.0/src/streamlink/plugins/clubbingtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/cmmedia.py` & `streamlink-6.0.0/src/streamlink/plugins/cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/cnews.py` & `streamlink-6.0.0/src/streamlink/plugins/cnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/crunchyroll.py` & `streamlink-6.0.0/src/streamlink/plugins/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/dailymotion.py` & `streamlink-6.0.0/src/streamlink/plugins/dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/dash.py` & `streamlink-6.0.0/src/streamlink/plugins/dash.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from streamlink.utils.url import update_scheme
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"dash://(?P<url>\S+)(?:\s(?P<params>.+))?",
+    r"dash://(?P<url>\S+)(?:\s(?P<params>.+))?$",
 ))
 @pluginmatcher(priority=LOW_PRIORITY, pattern=re.compile(
-    r"(?P<url>\S+\.mpd(?:\?\S*)?)(?:\s(?P<params>.+))?",
+    r"(?P<url>\S+\.mpd(?:\?\S*)?)(?:\s(?P<params>.+))?$",
 ))
 class MPEGDASH(Plugin):
     @classmethod
     def stream_weight(cls, stream):
         match = re.match(r"^(?:(.*)\+)?(?:a(\d+)k)$", stream)
         if match and match.group(1) and match.group(2):
             weight, group = stream_weight(match.group(1))
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/delfi.py` & `streamlink-6.0.0/src/streamlink/plugins/delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/deutschewelle.py` & `streamlink-6.0.0/src/streamlink/plugins/deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/dlive.py` & `streamlink-6.0.0/src/streamlink/plugins/dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/dogan.py` & `streamlink-6.0.0/src/streamlink/plugins/dogan.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             validate.xml_xpath_string(".//*[@data-live][contains(@data-url,'.m3u8')]/@data-url"),
         )
 
         return schema.validate(root)
 
     @staticmethod
     def _get_content_id(root):
-        schema=validate.Schema(
+        schema = validate.Schema(
             validate.any(
                 validate.all(
                     validate.xml_xpath_string("""
                         .//div[@data-id][
                             @data-live
                             or @id='video-element'
                             or @id='player-container'
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/dogus.py` & `streamlink-6.0.0/src/streamlink/plugins/dogus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/drdk.py` & `streamlink-6.0.0/src/streamlink/plugins/drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/earthcam.py` & `streamlink-6.0.0/src/streamlink/plugins/earthcam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/euronews.py` & `streamlink-6.0.0/src/streamlink/plugins/euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/facebook.py` & `streamlink-6.0.0/src/streamlink/plugins/facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/filmon.py` & `streamlink-6.0.0/src/streamlink/plugins/filmon.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     __worker__ = FilmOnHLSStreamWorker
 
 
 class FilmOnHLS(HLSStream):
     __shortname__ = "hls-filmon"
     __reader__ = FilmOnHLSStreamReader
 
-    def __init__(self, session_, url: str, api: "FilmOnAPI", channel=None, vod_id=None, quality="high", **args):
+    def __init__(self, session, url: str, api: "FilmOnAPI", channel=None, vod_id=None, quality="high", **args):
         if channel is None and vod_id is None:
             raise PluginError("Channel or vod_id must be set")
 
-        super().__init__(session_, url, **args)
+        super().__init__(session, url, **args)
         self.api = api
         self.channel = channel
         self.vod_id = vod_id
         self.quality = quality
         self._url = url
         self.watch_timeout = 0.0
         self._first_netloc = ""
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/foxtr.py` & `streamlink-6.0.0/src/streamlink/plugins/foxtr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/galatasaraytv.py` & `streamlink-6.0.0/src/streamlink/plugins/galatasaraytv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/goltelevision.py` & `streamlink-6.0.0/src/streamlink/plugins/goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/goodgame.py` & `streamlink-6.0.0/src/streamlink/plugins/goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/googledrive.py` & `streamlink-6.0.0/src/streamlink/plugins/googledrive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/gulli.py` & `streamlink-6.0.0/src/streamlink/plugins/gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/hiplayer.py` & `streamlink-6.0.0/src/streamlink/plugins/hiplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/hls.py` & `streamlink-6.0.0/src/streamlink/plugins/hls.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from streamlink.utils.url import update_scheme
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"hls(?:variant)?://(?P<url>\S+)(?:\s(?P<params>.+))?",
+    r"hls(?:variant)?://(?P<url>\S+)(?:\s(?P<params>.+))?$",
 ))
 @pluginmatcher(priority=LOW_PRIORITY, pattern=re.compile(
-    r"(?P<url>\S+\.m3u8(?:\?\S*)?)(?:\s(?P<params>.+))?",
+    r"(?P<url>\S+\.m3u8(?:\?\S*)?)(?:\s(?P<params>.+))?$",
 ))
 class HLSPlugin(Plugin):
     def _get_streams(self):
         data = self.match.groupdict()
         url = update_scheme("https://", data.get("url"), force=False)
         params = parse_params(data.get("params"))
         log.debug(f"URL={url}; params={params}")
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/http.py` & `streamlink-6.0.0/src/streamlink/plugins/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from streamlink.utils.url import update_scheme
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"httpstream://(?P<url>\S+)(?:\s(?P<params>.+))?",
+    r"httpstream://(?P<url>\S+)(?:\s(?P<params>.+))?$",
 ))
 class HTTPStreamPlugin(Plugin):
     def _get_streams(self):
         data = self.match.groupdict()
         url = update_scheme("https://", data.get("url"), force=False)
         params = parse_params(data.get("params"))
         log.debug(f"URL={url}; params={params}")
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/htv.py` & `streamlink-6.0.0/src/streamlink/plugins/htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/huajiao.py` & `streamlink-6.0.0/src/streamlink/plugins/huajiao.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/huya.py` & `streamlink-6.0.0/src/streamlink/plugins/huya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/idf1.py` & `streamlink-6.0.0/src/streamlink/plugins/idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/indihometv.py` & `streamlink-6.0.0/src/streamlink/plugins/indihometv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/invintus.py` & `streamlink-6.0.0/src/streamlink/plugins/invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/kugou.py` & `streamlink-6.0.0/src/streamlink/plugins/kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/linelive.py` & `streamlink-6.0.0/src/streamlink/plugins/linelive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/livestream.py` & `streamlink-6.0.0/src/streamlink/plugins/livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/lnk.py` & `streamlink-6.0.0/src/streamlink/plugins/lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ltv_lsm_lv.py` & `streamlink-6.0.0/src/streamlink/plugins/ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mdstrm.py` & `streamlink-6.0.0/src/streamlink/plugins/mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mediaklikk.py` & `streamlink-6.0.0/src/streamlink/plugins/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mediavitrina.py` & `streamlink-6.0.0/src/streamlink/plugins/mediavitrina.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     |
     ctc(?:love)?
     |
     domashniy
 )\.ru/(?:live|online)""", re.VERBOSE))
 @pluginmatcher(re.compile(r"https?://player\.mediavitrina\.ru/.+/player\.html"))
 class MediaVitrina(Plugin):
-    _re_url_json = re.compile(r"https://media\.mediavitrina\.ru/(?:proxy)?api/v3/\w+/playlist/[\w-]+_as_array\.json[^\"']+")
+    _re_url_json = re.compile(r"https://media\.mediavitrina\.ru/(?:proxy)?api/v3/[\w-]+/playlist/[\w-]+_as_array\.json[^\"']+")
 
     def _get_streams(self):
         self.session.http.headers.update({"Referer": self.url})
 
         p_netloc = urlparse(self.url).netloc
         if p_netloc == "player.mediavitrina.ru":
             # https://player.mediavitrina.ru/
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mildom.py` & `streamlink-6.0.0/src/streamlink/plugins/mildom.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 log = logging.getLogger(__name__)
 
 
 class MildomHLSStream(HLSStream):
     __shortname__ = "hls-mildom"
     expiry_time = 60 * 120
 
-    def __init__(self, session_, api, server, token, quality, **args):
-        self.session = session_
+    def __init__(self, session, api, server, token, quality, **args):
+        self.session = session
         self.api = api
         self.server = server
         self.token = token
         self.quality = quality
         self._url = self.build_hls_url()
         super().__init__(self.session, self._url, **args)
         self.expiry = time()
@@ -98,15 +98,15 @@
             schema=validate.Schema(
                 validate.parse_json(),
                 {
                     "code": int,
                     validate.optional("message"): str,
                     validate.optional("body"): {
                         "data": [
-                            {"token": str },
+                            {"token": str},
                         ],
                     },
                 },
             ),
         )
         if self._is_api_error(data):
             return
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mitele.py` & `streamlink-6.0.0/src/streamlink/plugins/mitele.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
 
         urls = set()
         for stream in pdata["dls"]:
             if stream["drm"]:
                 log.warning("Stream may be protected by DRM")
                 continue
             cdn_token = tokens.get(stream["lid"], {}).get("cdn", "")
+            if not cdn_token:
+                continue
             qsd = parse_qsd(cdn_token)
             urls.add(update_qsd(stream["stream"], qsd, quote_via=lambda string, *_, **__: string))
 
         for url in urls:
             yield from HLSStream.parse_variant_playlist(
                 self.session,
                 url,
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mixcloud.py` & `streamlink-6.0.0/src/streamlink/plugins/mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mjunoon.py` & `streamlink-6.0.0/src/streamlink/plugins/mjunoon.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 """
 
 import binascii
 import logging
 import re
 from urllib.parse import urljoin
 
-from Crypto.Cipher import AES
-from Crypto.Util.Padding import unpad
-
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.crypto import AES, unpad
 from streamlink.utils.parse import parse_json
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/mrtmk.py` & `streamlink-6.0.0/src/streamlink/plugins/mrtmk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/n13tv.py` & `streamlink-6.0.0/src/streamlink/plugins/n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/nhkworld.py` & `streamlink-6.0.0/src/streamlink/plugins/nhkworld.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/nicolive.py` & `streamlink-6.0.0/src/streamlink/plugins/nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/nimotv.py` & `streamlink-6.0.0/src/streamlink/plugins/nimotv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/nos.py` & `streamlink-6.0.0/src/streamlink/plugins/nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/nownews.py` & `streamlink-6.0.0/src/streamlink/plugins/nownews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/nrk.py` & `streamlink-6.0.0/src/streamlink/plugins/nrk.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,102 +4,103 @@
 $url radio.nrk.no
 $type live, vod
 $region Norway
 """
 
 import logging
 import re
-from urllib.parse import urljoin
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
     r"https?://(?:tv|radio)\.nrk\.no/(program|direkte|serie|podkast)(?:/.+)?/([^/]+)",
 ))
 class NRK(Plugin):
-    _psapi_url = "https://psapi.nrk.no"
-    # Program type to manifest type mapping
-    _program_type_map = {
+    _URL_MANIFEST = "https://psapi.nrk.no/playback/manifest/{manifest_type}/{program_id}"
+    _URL_METADATA = "https://psapi.nrk.no/playback/metadata/{manifest_type}/{program_id}?eea-portability=true"
+
+    _MAP_MANIFEST_TYPE = {
         "direkte": "channel",
         "serie": "program",
         "program": "program",
         "podkast": "podcast",
     }
 
-    _program_id_re = re.compile(r'<meta property="nrk:program-id" content="([^"]+)"')
-
-    _playable_schema = validate.Schema(validate.any(
-        {
-            "playable": {
-                "assets": [{
-                    "url": validate.url(),
-                    "format": str,
-                }],
-            },
-            "statistics": {
-                validate.optional("luna"): validate.any(None, {
-                    "data": {
-                        "title": str,
-                        "category": validate.any(None, str),
+    def _get_metadata(self, manifest_type, program_id):
+        url_metadata = self._URL_METADATA.format(manifest_type=manifest_type, program_id=program_id)
+        non_playable = self.session.http.get(url_metadata, schema=validate.Schema(
+            validate.parse_json(),
+            {
+                validate.optional("nonPlayable"): validate.none_or_all(
+                    {
+                        "reason": str,
+                        "endUserMessage": str,
                     },
-                }),
-            },
-        },
-        {
-            "nonPlayable": {
-                "reason": str,
+                    validate.union_get("reason", "endUserMessage"),
+                ),
             },
-        },
-    ))
+            validate.get("nonPlayable"),
+        ))
+        if non_playable:
+            reason, end_user_message = non_playable
+            log.error(f"Not playable: {reason} - {end_user_message or 'error'}")
+            return False
+
+        return True
+
+    def _update_program_id(self, program_id):
+        new_program_id = self.session.http.get(self.url, schema=validate.Schema(
+            validate.parse_html(),
+            validate.xml_xpath_string(".//meta[@property='nrk:program-id']/@content"),
+        ))
+        return new_program_id or program_id
+
+    def _get_assets(self, manifest_type, program_id):
+        return self.session.http.get(
+            self._URL_MANIFEST.format(manifest_type=manifest_type, program_id=program_id),
+            schema=validate.Schema(
+                validate.parse_json(),
+                {
+                    "playable": {
+                        "assets": [
+                            validate.all(
+                                {
+                                    "url": validate.url(),
+                                    "format": str,
+                                },
+                                validate.union_get("format", "url"),
+                            ),
+                        ],
+                    },
+                },
+                validate.get(("playable", "assets")),
+            ),
+        )
 
     def _get_streams(self):
-        # Construct manifest URL for this program.
         program_type, program_id = self.match.groups()
-        manifest_type = self._program_type_map.get(program_type)
+        manifest_type = self._MAP_MANIFEST_TYPE.get(program_type)
         if manifest_type is None:
             log.error(f"Unknown program type '{program_type}'")
-            return None
+            return
 
-        # Fetch program_id.
-        res = self.session.http.get(self.url)
-        m = self._program_id_re.search(res.text)
-        if m is not None:
-            program_id = m.group(1)
-        elif program_id is None:
-            log.error("Could not extract program ID from URL")
-            return None
-
-        manifest_url = urljoin(self._psapi_url, f"playback/manifest/{manifest_type}/{program_id}")
-
-        # Extract media URL.
-        res = self.session.http.get(manifest_url)
-        manifest = self.session.http.json(res, schema=self._playable_schema)
-        if "nonPlayable" in manifest:
-            reason = manifest["nonPlayable"]["reason"]
-            log.error(f"Not playable ({reason})")
-            return None
-        self._set_metadata(manifest)
-        asset = manifest["playable"]["assets"][0]
-
-        # Some streams such as podcasts are not HLS but plain files.
-        if asset["format"] == "HLS":
-            return HLSStream.parse_variant_playlist(self.session, asset["url"])
-        else:
-            return [("live", HTTPStream(self.session, asset["url"]))]
-
-    def _set_metadata(self, manifest):
-        luna = manifest.get("statistics").get("luna")
-        if not luna:
+        program_id = self._update_program_id(program_id)
+        if self._get_metadata(manifest_type, program_id) is False:
             return
-        data = luna["data"]
-        self.category = data.get("category")
-        self.title = data.get("title")
+
+        assets = self._get_assets(manifest_type, program_id)
+
+        # just return the first item
+        for stream_type, stream_url in assets:
+            if stream_type == "HLS":
+                return HLSStream.parse_variant_playlist(self.session, stream_url)
+            return [("live", HTTPStream(self.session, stream_url))]
 
 
 __plugin__ = NRK
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ntv.py` & `streamlink-6.0.0/src/streamlink/plugins/ntv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/okru.py` & `streamlink-6.0.0/src/streamlink/plugins/okru.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/olympicchannel.py` & `streamlink-6.0.0/src/streamlink/plugins/olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/oneplusone.py` & `streamlink-6.0.0/src/streamlink/plugins/oneplusone.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
 log = logging.getLogger(__name__)
 
 
 class OnePlusOneHLS(HLSStream):
     __shortname__ = "hls-oneplusone"
 
-    def __init__(self, session_, url, self_url=None, **args):
-        super().__init__(session_, url, None, **args)
+    def __init__(self, session, url, self_url=None, **args):
+        super().__init__(session, url, None, **args)
         self._url = url
 
         first_parsed = urlparse(self._url)
         self._first_netloc = first_parsed.netloc
         self._first_path_chunklist = first_parsed.path.split("/")[-1]
         self.watch_timeout = int(first_parsed.path.split("/")[2]) - 15
-        self.api = OnePlusOneAPI(session_, self_url)
+        self.api = OnePlusOneAPI(session, self_url)
 
     def _next_watch_timeout(self):
         _next = fromlocaltimestamp(self.watch_timeout).isoformat(" ")
         log.debug(f"next watch_timeout at {_next}")
 
     def open(self):
         self._next_watch_timeout()
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/onetv.py` & `streamlink-6.0.0/src/streamlink/plugins/onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/openrectv.py` & `streamlink-6.0.0/src/streamlink/plugins/openrectv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/pandalive.py` & `streamlink-6.0.0/src/streamlink/plugins/pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/picarto.py` & `streamlink-6.0.0/src/streamlink/plugins/picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/piczel.py` & `streamlink-6.0.0/src/streamlink/plugins/piczel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/pixiv.py` & `streamlink-6.0.0/src/streamlink/plugins/pixiv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/pluto.py` & `streamlink-6.0.0/src/streamlink/plugins/pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/pluzz.py` & `streamlink-6.0.0/src/streamlink/plugins/pluzz.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                         validate.get("video_id"),
                     ),
                     validate.all(
                         validate.xml_xpath_string(".//*[@id][contains(@class,'francetv-player-wrapper')][1]/@id"),
                         str,
                     ),
                     validate.all(
-                        validate.xml_xpath_string(".//*[@data-id][@class='magneto'][1]/@data-id"),
+                        validate.xml_xpath_string(".//*[@data-id][contains(@class,'magneto')][1]/@data-id"),
                         str,
                     ),
                 ),
             ))
         except PluginError:
             pass
         if not video_id:
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/qq.py` & `streamlink-6.0.0/src/streamlink/plugins/qq.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/radiko.py` & `streamlink-6.0.0/src/streamlink/plugins/radiko.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/radionet.py` & `streamlink-6.0.0/src/streamlink/plugins/radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/raiplay.py` & `streamlink-6.0.0/src/streamlink/plugins/raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/reuters.py` & `streamlink-6.0.0/src/streamlink/plugins/reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/rtbf.py` & `streamlink-6.0.0/src/streamlink/plugins/rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/rtpa.py` & `streamlink-6.0.0/src/streamlink/plugins/rtpa.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/rtpplay.py` & `streamlink-6.0.0/src/streamlink/plugins/rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/rtve.py` & `streamlink-6.0.0/src/streamlink/plugins/rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/rtvs.py` & `streamlink-6.0.0/src/streamlink/plugins/rtvs.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,51 +2,56 @@
 $description Live TV channels from RTVS, a Slovak public, state-owned broadcaster.
 $url rtvs.sk
 $type live
 $region Slovakia
 """
 
 import re
+from urllib.parse import urlparse
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
-from streamlink.utils.parse import parse_json
 
 
 @pluginmatcher(re.compile(
-    r"https?://www\.rtvs\.sk/televizia/live-[\w-]+",
+    r"https?://www\.rtvs\.sk/televizia/(?:live-|sport)",
 ))
 class Rtvs(Plugin):
-    _re_channel_id = re.compile(r"'stream':\s*'live-(\d+)'")
-
     def _get_streams(self):
-        res = self.session.http.get(self.url)
-        m = self._re_channel_id.search(res.text)
-        if not m:
+        channel = self.session.http.get(self.url, schema=validate.Schema(
+            validate.parse_html(),
+            validate.xml_xpath_string(".//iframe[@id='player_live']//@src"),
+            validate.url(path=validate.startswith("/embed/live/")),
+            validate.transform(lambda embed: urlparse(embed).path[len("/embed/live/"):]),
+        ))
+        if not channel:
             return
 
-        res = self.session.http.get(
+        videos = self.session.http.get(
             "https://www.rtvs.sk/json/live5f.json",
             params={
-                "c": m.group(1),
+                "c": channel,
                 "b": "mozilla",
                 "p": "win",
                 "f": "0",
                 "d": "1",
             },
+            schema=validate.Schema(
+                validate.parse_json(),
+                {
+                    "clip": {
+                        "sources": [{
+                            "src": validate.url(),
+                            "type": str,
+                        }],
+                    },
+                },
+                validate.get(("clip", "sources")),
+                validate.filter(lambda n: n["type"] == "application/x-mpegurl"),
+            ),
         )
-        videos = parse_json(res.text, schema=validate.Schema({
-            "clip": {
-                "sources": [{
-                    "src": validate.url(),
-                    "type": str,
-                }],
-            }},
-            validate.get(("clip", "sources")),
-            validate.filter(lambda n: n["type"] == "application/x-mpegurl"),
-        ))
         for video in videos:
-            yield from HLSStream.parse_variant_playlist(self.session, video["src"]).items()
+            return HLSStream.parse_variant_playlist(self.session, video["src"])
 
 
 __plugin__ = Rtvs
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ruv.py` & `streamlink-6.0.0/src/streamlink/plugins/ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/sbscokr.py` & `streamlink-6.0.0/src/streamlink/plugins/sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/showroom.py` & `streamlink-6.0.0/src/streamlink/plugins/showroom.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 $description Japanese live-streaming service used primarily by Japanese idols & voice actors and their fans.
 $url showroom-live.com
 $type live
 """
 
 import logging
 import re
+from urllib.parse import parse_qsl, urlparse
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
 
 
 log = logging.getLogger(__name__)
@@ -26,24 +27,26 @@
         self.session.set_option("hls-playlist-reload-time", "segment")
 
     def _get_streams(self):
         room_id = self.session.http.get(
             self.url,
             schema=validate.Schema(
                 validate.parse_html(),
-                validate.xml_xpath_string(".//script[contains(text(),'share_url:\"https:')][1]/text()"),
+                validate.xml_xpath_string(".//nav//a[contains(@href,'/room/profile?')]/@href"),
                 validate.none_or_all(
-                    re.compile(r"share_url:\"https:[^?]+?\?room_id=(?P<room_id>\d+)\""),
-                    validate.any(None, validate.get("room_id")),
+                    validate.transform(lambda _url_profile: dict(parse_qsl(urlparse(_url_profile).query))),
+                    validate.get("room_id"),
                 ),
             ),
         )
         if not room_id:
             return
 
+        log.debug(f"Room ID: {room_id}")
+
         live_status, self.title = self.session.http.get(
             "https://www.showroom-live.com/api/live/live_info",
             params={
                 "room_id": room_id,
             },
             schema=validate.Schema(
                 validate.parse_json(),
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/sportal.py` & `streamlink-6.0.0/src/streamlink/plugins/sportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/sportschau.py` & `streamlink-6.0.0/src/streamlink/plugins/sportschau.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ssh101.py` & `streamlink-6.0.0/src/streamlink/plugins/ssh101.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/stadium.py` & `streamlink-6.0.0/src/streamlink/plugins/stadium.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/steam.py` & `streamlink-6.0.0/src/streamlink/plugins/steam.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 """
 
 import base64
 import logging
 import re
 import time
 
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-
 from streamlink.exceptions import FatalPluginError
 from streamlink.plugin import Plugin, pluginargument, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.dash import DASHStream
+from streamlink.utils.crypto import RSA, PKCS1_v1_5
 
 
 log = logging.getLogger(__name__)
 
 
 class SteamLoginFailed(Exception):
     pass
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/streamable.py` & `streamlink-6.0.0/src/streamlink/plugins/streamable.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/streann.py` & `streamlink-6.0.0/src/streamlink/plugins/streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/stv.py` & `streamlink-6.0.0/src/streamlink/plugins/stv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/svtplay.py` & `streamlink-6.0.0/src/streamlink/plugins/svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/swisstxt.py` & `streamlink-6.0.0/src/streamlink/plugins/swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/telefe.py` & `streamlink-6.0.0/src/streamlink/plugins/telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/telemadrid.py` & `streamlink-6.0.0/src/streamlink/plugins/telemadrid.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tf1.py` & `streamlink-6.0.0/src/streamlink/plugins/tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/trovo.py` & `streamlink-6.0.0/src/streamlink/plugins/trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tv360.py` & `streamlink-6.0.0/src/streamlink/plugins/tv360.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tv3cat.py` & `streamlink-6.0.0/src/streamlink/plugins/tv3cat.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tv4play.py` & `streamlink-6.0.0/src/streamlink/plugins/tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tv5monde.py` & `streamlink-6.0.0/src/streamlink/plugins/tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tv8.py` & `streamlink-6.0.0/src/streamlink/plugins/tv8.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tv999.py` & `streamlink-6.0.0/src/streamlink/plugins/tv999.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tvibo.py` & `streamlink-6.0.0/src/streamlink/plugins/tvibo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tviplayer.py` & `streamlink-6.0.0/src/streamlink/plugins/tviplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tvp.py` & `streamlink-6.0.0/src/streamlink/plugins/tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tvrby.py` & `streamlink-6.0.0/src/streamlink/plugins/tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tvrplus.py` & `streamlink-6.0.0/src/streamlink/plugins/tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/tvtoya.py` & `streamlink-6.0.0/src/streamlink/plugins/tvtoya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/twitcasting.py` & `streamlink-6.0.0/src/streamlink/plugins/twitcasting.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/twitch.py` & `streamlink-6.0.0/src/streamlink/plugins/twitch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """
 $description Global live-streaming and video hosting social platform owned by Amazon.
 $url twitch.tv
 $type live, vod
 $notes See the :ref:`Authentication <cli/plugins/twitch:Authentication>` docs on how to prevent ads.
 $notes Read more about :ref:`embedded ads <cli/plugins/twitch:Embedded ads>` here.
 $notes :ref:`Low latency streaming <cli/plugins/twitch:Low latency streaming>` is supported.
+$notes Acquires a :ref:`client-integrity token <cli/plugins/twitch:Client-integrity token>` on streaming access token failure.
 """
 
 import argparse
+import base64
 import logging
 import re
 import sys
 from datetime import datetime, timedelta
+from json import dumps as json_dumps
 from random import random
-from typing import List, NamedTuple, Optional
+from typing import List, Mapping, NamedTuple, Optional, Tuple
 from urllib.parse import urlparse
 
 from streamlink.exceptions import NoStreamsError, PluginError
 from streamlink.plugin import Plugin, pluginargument, pluginmatcher
 from streamlink.plugin.api import validate
+from streamlink.session import Streamlink
 from streamlink.stream.hls import HLSStream, HLSStreamReader, HLSStreamWorker, HLSStreamWriter
 from streamlink.stream.hls_playlist import M3U8, ByteRange, DateRange, ExtInf, Key, M3U8Parser, Map, load as load_hls_playlist
 from streamlink.stream.http import HTTPStream
 from streamlink.utils.args import keyvalue
 from streamlink.utils.parse import parse_json, parse_qsd
-from streamlink.utils.times import hours_minutes_seconds
+from streamlink.utils.random import CHOICES_ALPHA_NUM, random_token
+from streamlink.utils.times import fromtimestamp, hours_minutes_seconds
 from streamlink.utils.url import update_qsd
 
 
 log = logging.getLogger(__name__)
 
 LOW_LATENCY_MAX_LIVE_EDGE = 2
 
@@ -198,18 +203,18 @@
             log.info(f"Low latency streaming (HLS live edge: {live_edge})")
         super().__init__(stream)
 
 
 class TwitchHLSStream(HLSStream):
     __reader__ = TwitchHLSStreamReader
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, disable_ads: bool = False, low_latency: bool = False, **kwargs):
         super().__init__(*args, **kwargs)
-        self.disable_ads = self.session.get_plugin_option("twitch", "disable-ads")
-        self.low_latency = self.session.get_plugin_option("twitch", "low-latency")
+        self.disable_ads = disable_ads
+        self.low_latency = low_latency
 
 
 class UsherService:
     def __init__(self, session):
         self.session = session
 
     def _create_url(self, endpoint, **extra_params):
@@ -249,21 +254,21 @@
     def video(self, video_id, **extra_params):
         return self._create_url(f"/vod/{video_id}", **extra_params)
 
 
 class TwitchAPI:
     CLIENT_ID = "kimne78kx3ncx6brgo4mv6wki5h1ko"
 
-    def __init__(self, session):
+    def __init__(self, session, api_header=None, access_token_param=None):
         self.session = session
         self.headers = {
             "Client-ID": self.CLIENT_ID,
         }
-        self.headers.update(**dict(session.get_plugin_option("twitch", "api-header") or []))
-        self.access_token_params = dict(session.get_plugin_option("twitch", "access-token-param") or [])
+        self.headers.update(**dict(api_header or []))
+        self.access_token_params = dict(access_token_param or [])
         self.access_token_params.setdefault("playerType", "embed")
 
     def call(self, data, schema=None, **kwargs):
         res = self.session.http.post(
             "https://gql.twitch.tv/gql",
             json=data,
             headers={**self.headers, **kwargs.pop("headers", {})},
@@ -402,15 +407,15 @@
                 (0, "id"),
                 (0, "broadcaster", "displayName"),
                 (0, "game", "name"),
                 (1, "title"),
             ),
         ))
 
-    def access_token(self, is_live, channel_or_vod):
+    def access_token(self, is_live, channel_or_vod, client_integrity: Optional[Tuple[str, str]] = None):
         query = self._gql_persisted_query(
             "PlaybackAccessToken",
             "0828119ded1c13477966434e15800ff57ddacf13ba1911c129dc2200705b0712",
             isLive=is_live,
             login=channel_or_vod if is_live else "",
             isVod=not is_live,
             vodID=channel_or_vod if not is_live else "",
@@ -420,17 +425,26 @@
             {
                 "value": str,
                 "signature": str,
             },
             validate.union_get("signature", "value"),
         )
 
-        return self.call(query, acceptable_status=(200, 400, 401, 403), schema=validate.Schema(
+        headers = {}
+        if client_integrity:
+            headers["Device-Id"], headers["Client-Integrity"] = client_integrity
+
+        return self.call(query, acceptable_status=(200, 400, 401, 403), headers=headers, schema=validate.Schema(
             validate.any(
                 validate.all(
+                    {"errors": [{"message": str}]},
+                    validate.get(("errors", 0, "message")),
+                    validate.transform(lambda data: ("error", None, data)),
+                ),
+                validate.all(
                     {"error": str, "message": str},
                     validate.union_get("error", "message"),
                     validate.transform(lambda data: ("error", *data)),
                 ),
                 validate.all(
                     {
                         "data": validate.any(
@@ -441,15 +455,15 @@
                             validate.all(
                                 {"videoPlaybackAccessToken": subschema},
                                 validate.get("videoPlaybackAccessToken"),
                             ),
                         ),
                     },
                     validate.get("data"),
-                    validate.transform(lambda data: ("token", *data)),
+                    validate.transform(lambda data: ("token", *data) if data is not None else ("token", None, None)),
                 ),
             ),
         ))
 
     def clips(self, clipname):
         query = self._gql_persisted_query(
             "VideoAccessToken_Clip",
@@ -492,14 +506,125 @@
 
         return self.call(query, schema=validate.Schema(
             {"data": {"user": {"stream": {"type": str}}}},
             validate.get(("data", "user", "stream")),
         ))
 
 
+class TwitchClientIntegrity:
+    URL_P_SCRIPT = "https://k.twitchcdn.net/149e9513-01fa-4fb0-aad4-566afd725d1b/2d206a39-8ed7-437e-a3be-862e0f06eea3/p.js"
+
+    # language=javascript
+    JS_INTEGRITY_TOKEN = """
+    // noinspection JSIgnoredPromiseFromCall
+    new Promise((resolve, reject) => {
+        function configureKPSDK() {
+            // noinspection JSUnresolvedVariable,JSUnresolvedFunction
+            window.KPSDK.configure([{
+                "protocol": "https:",
+                "method": "POST",
+                "domain": "gql.twitch.tv",
+                "path": "/integrity"
+            }]);
+        }
+
+        async function fetchIntegrity() {
+            // noinspection JSUnresolvedReference
+            const headers = Object.assign(HEADERS, {"x-device-id": "DEVICE_ID"});
+            // window.fetch gets overridden and the patched function needs to be used
+            const resp = await window.fetch("https://gql.twitch.tv/integrity", {
+                "headers": headers,
+                "body": null,
+                "method": "POST",
+                "mode": "cors",
+                "credentials": "omit"
+            });
+
+            if (resp.status !== 200) {
+                throw new Error(`Unexpected integrity response status code ${resp.status}`);
+            }
+
+            return JSON.stringify(await resp.json());
+        }
+
+        document.addEventListener("kpsdk-load", configureKPSDK, {once: true});
+        document.addEventListener("kpsdk-ready", () => fetchIntegrity().then(resolve, reject), {once: true});
+
+        const script = document.createElement("script");
+        script.addEventListener("error", reject);
+        script.src = "SCRIPT_SOURCE";
+        document.body.appendChild(script);
+    });
+    """
+
+    @classmethod
+    def acquire(
+        cls,
+        session: Streamlink,
+        channel: str,
+        headers: Mapping[str, str],
+        device_id: str,
+    ) -> Optional[Tuple[str, int]]:
+        from streamlink.webbrowser.cdp import CDPClient, CDPClientSession, devtools
+        from streamlink.webbrowser.exceptions import WebbrowserError
+
+        url = f"https://www.twitch.tv/{channel}"
+        js_get_integrity_token = cls.JS_INTEGRITY_TOKEN \
+            .replace("SCRIPT_SOURCE", cls.URL_P_SCRIPT) \
+            .replace("HEADERS", json_dumps(headers)) \
+            .replace("DEVICE_ID", device_id)
+        eval_timeout = session.get_option("webbrowser-timeout")
+
+        async def on_main(client_session: CDPClientSession, request: devtools.fetch.RequestPaused):
+            async with client_session.alter_request(request) as cm:
+                cm.body = "<!doctype html>"
+
+        async def acquire_client_integrity_token(client: CDPClient):
+            client_session: CDPClientSession
+            async with client.session() as client_session:
+                client_session.add_request_handler(on_main, url_pattern=url, on_request=True)
+                async with client_session.navigate(url) as frame_id:
+                    await client_session.loaded(frame_id)
+                    return await client_session.evaluate(js_get_integrity_token, timeout=eval_timeout)
+
+        try:
+            client_integrity: Optional[str] = CDPClient.launch(session, acquire_client_integrity_token)
+        except WebbrowserError as err:
+            log.error(f"{type(err).__name__}: {err}")
+            return None
+        if not client_integrity:
+            return None
+
+        token, expiration = parse_json(client_integrity, schema=validate.Schema(
+            {"token": str, "expiration": int},
+            validate.union_get("token", "expiration"),
+        ))
+        is_bad_bot = cls.decode_client_integrity_token(token, schema=validate.Schema(
+            {"is_bad_bot": str},
+            validate.get("is_bad_bot"),
+            validate.transform(lambda val: val.lower() != "false"),
+        ))
+        log.info(f"Is bad bot? {is_bad_bot}")
+        if is_bad_bot:
+            return None
+
+        return token, expiration / 1000
+
+    @staticmethod
+    def decode_client_integrity_token(data: str, schema: Optional[validate.Schema] = None):
+        if not data.startswith("v4.public."):
+            raise PluginError("Invalid client-integrity token format")
+        token = data[len("v4.public."):].replace("-", "+").replace("_", "/")
+        token += "=" * ((4 - (len(token) % 4)) % 4)
+        token = base64.b64decode(token.encode())[:-64].decode()
+        log.debug(f"Client-Integrity token: {token}")
+
+        return parse_json(token, exception=PluginError, schema=schema)
+
+
 @pluginmatcher(re.compile(r"""
     https?://(?:(?P<subdomain>[\w-]+)\.)?twitch\.tv/
     (?:
         videos/(?P<videos_id>\d+)
         |
         (?P<channel>[^/?]+)
         (?:
@@ -564,15 +689,22 @@
     action="append",
     help="""
         A parameter to add to the API request for acquiring the streaming access token.
 
         Can be repeated to add multiple parameters.
     """,
 )
+@pluginargument(
+    "purge-client-integrity",
+    action="store_true",
+    help="Purge cached Twitch client-integrity token and acquire a new one.",
+)
 class Twitch(Plugin):
+    _CACHE_KEY_CLIENT_INTEGRITY = "client-integrity"
+
     @classmethod
     def stream_weight(cls, stream):
         if stream == "source":
             return sys.maxsize, stream
         return super().stream_weight(stream)
 
     def __init__(self, *args, **kwargs):
@@ -595,15 +727,19 @@
             # clip share URL
             self.clip_name = match.get("channel")
         else:
             self.channel = match.get("channel") and match.get("channel").lower()
             self.video_id = match.get("video_id") or match.get("videos_id")
             self.clip_name = match.get("clip_name")
 
-        self.api = TwitchAPI(session=self.session)
+        self.api = TwitchAPI(
+            session=self.session,
+            api_header=self.get_option("api-header"),
+            access_token_param=self.get_option("access-token-param"),
+        )
         self.usher = UsherService(session=self.session)
 
         def method_factory(parent_method):
             def inner():
                 if not self._checked_metadata:
                     self._checked_metadata = True
                     self._get_metadata()
@@ -625,25 +761,60 @@
                 data = self.api.metadata_channel(self.channel)
             else:  # pragma: no cover
                 return
             self.id, self.author, self.category, self.title = data
         except (PluginError, TypeError):
             pass
 
+    def _client_integrity_token(self, channel: str) -> Optional[Tuple[str, str]]:
+        if self.options.get("purge-client-integrity"):
+            log.info("Removing cached client-integrity token...")
+            self.cache.set(self._CACHE_KEY_CLIENT_INTEGRITY, None, 0)
+
+        client_integrity = self.cache.get(self._CACHE_KEY_CLIENT_INTEGRITY)
+        if client_integrity and isinstance(client_integrity, list) and len(client_integrity) == 2:
+            log.info("Using cached client-integrity token")
+            device_id, token = client_integrity
+        else:
+            log.info("Acquiring new client-integrity token...")
+            device_id = random_token(32, CHOICES_ALPHA_NUM)
+            client_integrity = TwitchClientIntegrity.acquire(
+                self.session,
+                channel,
+                self.api.headers,
+                device_id,
+            )
+            if not client_integrity:
+                log.warning("No client-integrity token acquired")
+                return None
+
+            token, expiration = client_integrity
+            self.cache.set(self._CACHE_KEY_CLIENT_INTEGRITY, [device_id, token], expires_at=fromtimestamp(expiration))
+
+        return device_id, token
+
     def _access_token(self, is_live, channel_or_vod):
-        try:
-            response, *data = self.api.access_token(is_live, channel_or_vod)
+        # try without a client-integrity token first (the web player did the same on 2023-05-31)
+        response, *data = self.api.access_token(is_live, channel_or_vod)
+
+        # try again with a client-integrity token if the API response was erroneous
+        if response != "token":
+            client_integrity = self._client_integrity_token(channel_or_vod) if is_live else None
+            response, *data = self.api.access_token(is_live, channel_or_vod, client_integrity)
+
+            # unknown API response error: abort
             if response != "token":
                 error, message = data
-                log.error(f"{error or 'Error'}: {message or 'Unknown error'}")
-                raise PluginError
-            sig, token = data
-        except (PluginError, TypeError):
-            raise NoStreamsError  # noqa: B904
+                raise PluginError(f"{error or 'Error'}: {message or 'Unknown error'}")
+
+        # access token response was empty: stream is offline or channel doesn't exist
+        if response == "token" and data[0] is None:
+            raise NoStreamsError
 
+        sig, token = data
         try:
             restricted_bitrates = self.api.parse_token(token)
         except PluginError:
             restricted_bitrates = []
 
         return sig, token, restricted_bitrates
 
@@ -689,15 +860,22 @@
         if time_offset:
             try:
                 time_offset = hours_minutes_seconds(time_offset)
             except ValueError:
                 time_offset = 0
 
         try:
-            streams = TwitchHLSStream.parse_variant_playlist(self.session, url, start_offset=time_offset, **extra_params)
+            streams = TwitchHLSStream.parse_variant_playlist(
+                self.session,
+                url,
+                start_offset=time_offset,
+                disable_ads=self.get_option("disable-ads"),
+                low_latency=self.get_option("low-latency"),
+                **extra_params,
+            )
         except OSError as err:
             err = str(err)
             if "404 Client Error" in err or "Failed to parse playlist" in err:
                 return
             else:
                 raise PluginError(err) from err
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ustreamtv.py` & `streamlink-6.0.0/src/streamlink/plugins/ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/ustvnow.py` & `streamlink-6.0.0/src/streamlink/plugins/ustvnow.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,17 @@
 import base64
 import json
 import logging
 import re
 from urllib.parse import urljoin, urlparse
 from uuid import uuid4
 
-from Crypto.Cipher import AES
-from Crypto.Hash import SHA256
-from Crypto.Util.Padding import pad, unpad
-
 from streamlink.plugin import Plugin, PluginError, pluginargument, pluginmatcher
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.crypto import AES, SHA256, pad, unpad
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
     r"https?://(?:www\.)?ustvnow\.com/live/(?P<scode>\w+)/-(?P<id>\d+)",
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/vidio.py` & `streamlink-6.0.0/src/streamlink/plugins/vidio.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/vimeo.py` & `streamlink-6.0.0/src/streamlink/plugins/vimeo.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,72 +3,123 @@
 $url vimeo.com
 $type live, vod
 $notes Password protected streams are not supported
 """
 
 import logging
 import re
-from html import unescape as html_unescape
 from urllib.parse import urljoin, urlparse
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.ffmpegmux import MuxedStream
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 from streamlink.utils.url import update_scheme
 
 
 log = logging.getLogger(__name__)
 
 
-@pluginmatcher(re.compile(
-    r"https?://(player\.vimeo\.com/video/\d+|(www\.)?vimeo\.com/.+)",
-))
+@pluginmatcher(
+    name="default",
+    pattern=re.compile(r"https?://(?:www\.)?vimeo\.com/.+"),
+)
+@pluginmatcher(
+    name="player",
+    pattern=re.compile(r"https?://player\.vimeo\.com/video/\d+"),
+)
 class Vimeo(Plugin):
     VIEWER_URL = "https://vimeo.com/_next/viewer"
     OEMBED_URL = "https://vimeo.com/api/oembed.json"
-    _config_url_re = re.compile(r'(?:"config_url"|\bdata-config-url)\s*[:=]\s*(".+?")')
-    _config_re = re.compile(r"playerConfig\s*=\s*({.+?})\s*var")
-    _config_url_schema = validate.Schema(
-        validate.transform(_config_url_re.search),
-        validate.any(
-            None,
-            validate.Schema(
-                validate.get(1),
-                validate.parse_json(),
-                validate.transform(html_unescape),
-                validate.url(),
-            ),
-        ),
-    )
-    _config_schema = validate.Schema(
-        validate.parse_json(),
-        {
-            "request": {
-                "files": {
-                    validate.optional("dash"): {"cdns": {str: {"url": validate.url()}}},
-                    validate.optional("hls"): {"cdns": {str: {"url": validate.url()}}},
-                    validate.optional("progressive"): validate.all(
-                        [{"url": validate.url(), "quality": str}],
+
+    @staticmethod
+    def _schema_config(config):
+        schema_cdns = validate.all(
+            {
+                "cdns": {
+                    str: validate.all(
+                        {"url": validate.url()},
+                        validate.get("url"),
                     ),
                 },
-                validate.optional("text_tracks"): validate.all(
-                    [{"url": str, "lang": str}],
+            },
+            validate.get("cdns"),
+        )
+        schema_config = validate.Schema(
+            {
+                "request": {
+                    "files": {
+                        validate.optional("hls"): schema_cdns,
+                        validate.optional("dash"): schema_cdns,
+                        validate.optional("progressive"): [
+                            validate.all(
+                                {
+                                    "url": validate.url(),
+                                    "quality": str,
+                                },
+                                validate.union_get("quality", "url"),
+                            ),
+                        ],
+                    },
+                    validate.optional("text_tracks"): [
+                        validate.all(
+                            {
+                                "url": str,
+                                "lang": str,
+                            },
+                            validate.union_get("lang", "url"),
+                        ),
+                    ],
+                },
+                validate.optional("video"): validate.none_or_all(
+                    {
+                        "id": int,
+                        "title": str,
+                        "owner": {
+                            "name": str,
+                        },
+                    },
+                    validate.union_get(
+                        "id",
+                        ("owner", "name"),
+                        "title",
+                    ),
                 ),
             },
-        },
-    )
-    _player_schema = validate.Schema(
-        validate.transform(_config_re.search),
-        validate.any(None, validate.Schema(validate.get(1), _config_schema)),
-    )
+            validate.union_get(
+                ("request", "files", "hls"),
+                ("request", "files", "dash"),
+                ("request", "files", "progressive"),
+                ("request", "text_tracks"),
+                "video",
+            ),
+        )
+
+        return schema_config.validate(config)
+
+    def _get_dash_url(self, url):
+        return self.session.http.get(url, schema=validate.Schema(
+            validate.parse_json(),
+            {"url": validate.url()},
+            validate.get("url"),
+        ))
+
+    def _query_player(self):
+        return self.session.http.get(self.url, schema=validate.Schema(
+            re.compile(r"playerConfig\s*=\s*({.+?})\s*var"),
+            validate.none_or_all(
+                validate.get(1),
+                validate.parse_json(),
+                validate.transform(self._schema_config),
+            ),
+        ))
 
-    def get_config_url(self) -> str:
+    def _query_api(self):
         jwt, api_url = self.session.http.get(
             self.VIEWER_URL,
             schema=validate.Schema(
                 validate.parse_json(),
                 {
                     "jwt": str,
                     "apiUrl": str,
@@ -82,74 +133,73 @@
             schema=validate.Schema(
                 validate.parse_json(),
                 {"uri": str},
                 validate.get("uri"),
             ),
         )
         player_config_url = urljoin(update_scheme("https://", api_url), uri)
-
-        return self.session.http.get(
+        config_url = self.session.http.get(
             player_config_url,
             params={"fields": "config_url"},
             headers={"Authorization": f"jwt {jwt}"},
             schema=validate.Schema(
                 validate.parse_json(),
                 {"config_url": validate.url()},
                 validate.get("config_url"),
             ),
         )
 
+        return self.session.http.get(config_url, schema=validate.Schema(
+            validate.parse_json(),
+            validate.transform(self._schema_config),
+        ))
+
     def _get_streams(self):
-        if "player.vimeo.com" in self.url:
-            data = self.session.http.get(self.url, schema=self._player_schema)
+        if self.matches["player"]:
+            data = self._query_player()
         else:
-            api_url = self.session.http.get(self.url, schema=self._config_url_schema)
+            data = self._query_api()
 
-            if not api_url:
-                api_url = self.get_config_url()
+        if not data:
+            return
 
-            if not api_url:
-                return
-            data = self.session.http.get(api_url, schema=self._config_schema)
+        hls, dash, progressive, text_tracks, metadata = data
+        if metadata:
+            self.id, self.author, self.title = metadata
 
-        videos = data["request"]["files"]
         streams = []
 
-        for stream_type in ("hls", "dash"):
-            if stream_type not in videos:
+        for url in hls.values():
+            streams.extend(HLSStream.parse_variant_playlist(self.session, url).items())
+            break
+
+        for url in dash.values():
+            p = urlparse(url)
+            if p.path.endswith("dash.mpd"):
+                # LIVE
+                url = self._get_dash_url(url)
+            elif p.path.endswith("master.json"):
+                # VOD
+                url = url.replace("master.json", "master.mpd")
+            else:
+                log.error(f"Unsupported DASH path: {p.path}")
                 continue
-            for _, video_data in videos[stream_type]["cdns"].items():
-                log.trace("{0!r}".format(video_data))
-                url = video_data.get("url")
-                if stream_type == "hls":
-                    streams.extend(HLSStream.parse_variant_playlist(self.session, url).items())
-
-                elif stream_type == "dash":
-                    p = urlparse(url)
-                    if p.path.endswith("dash.mpd"):
-                        # LIVE
-                        url = self.session.http.get(url).json()["url"]
-                    elif p.path.endswith("master.json"):
-                        # VOD
-                        url = url.replace("master.json", "master.mpd")
-                    else:
-                        log.error("Unsupported DASH path: {0}".format(p.path))
-                        continue
 
-                    streams.extend(DASHStream.parse_manifest(self.session, url).items())
+            streams.extend(DASHStream.parse_manifest(self.session, url).items())
+            break
 
         streams.extend(
-            (stream["quality"], HTTPStream(self.session, stream["url"]))
-            for stream in videos.get("progressive", [])
+            (quality, HTTPStream(self.session, url))
+            for quality, url in progressive or []
         )
 
-        if self.session.get_option("mux-subtitles") and data["request"].get("text_tracks"):
+        if text_tracks and self.session.get_option("mux-subtitles"):
             substreams = {
-                s["lang"]: HTTPStream(self.session, "https://vimeo.com" + s["url"])
-                for s in data["request"]["text_tracks"]
+                lang: HTTPStream(self.session, urljoin("https://vimeo.com/", url))
+                for lang, url in text_tracks
             }
             for quality, stream in streams:
                 yield quality, MuxedStream(self.session, stream, subtitles=substreams)
         else:
             yield from streams
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/vinhlongtv.py` & `streamlink-6.0.0/src/streamlink/plugins/vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/vk.py` & `streamlink-6.0.0/src/streamlink/plugins/vk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/vkplay.py` & `streamlink-6.0.0/src/streamlink/plugins/vkplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/vlive.py` & `streamlink-6.0.0/src/streamlink/plugins/vlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/vtvgo.py` & `streamlink-6.0.0/src/streamlink/plugins/vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/wasd.py` & `streamlink-6.0.0/src/streamlink/plugins/wasd.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/webtv.py` & `streamlink-6.0.0/src/streamlink/plugins/webtv.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 """
 
 import base64
 import binascii
 import logging
 import re
 
-from Crypto.Cipher import AES
-
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
-from streamlink.utils.crypto import unpad_pkcs5
+from streamlink.utils.crypto import AES, unpad_pkcs5
 from streamlink.utils.parse import parse_json
 from streamlink.utils.url import update_scheme
 
 
 log = logging.getLogger(__name__)
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/welt.py` & `streamlink-6.0.0/src/streamlink/plugins/welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/wwenetwork.py` & `streamlink-6.0.0/src/streamlink/plugins/wwenetwork.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/youtube.py` & `streamlink-6.0.0/src/streamlink/plugins/youtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         return schema_canonical.validate(data)
 
     @classmethod
     def _schema_playabilitystatus(cls, data):
         schema = validate.Schema(
             {"playabilityStatus": {
                 "status": str,
-                validate.optional("reason"): str,
+                validate.optional("reason"): validate.any(str, None),
             }},
             validate.get("playabilityStatus"),
             validate.union_get("status", "reason"),
         )
         return schema.validate(data)
 
     @classmethod
@@ -337,15 +337,16 @@
                 if videoId is not None:
                     return videoId
 
     def _data_status(self, data, errorlog=False):
         if not data:
             return False
         status, reason = self._schema_playabilitystatus(data)
-        if status != "OK":
+        # assume that there's an error if reason is set (status will still be "OK" for some reason)
+        if status != "OK" or reason:
             if errorlog:
                 log.error(f"Could not get video info - {status}: {reason}")
             return False
         return True
 
     def _get_streams(self):
         res = self._get_res(self.url)
```

### Comparing `streamlink-5.5.1/src/streamlink/plugins/yupptv.py` & `streamlink-6.0.0/src/streamlink/plugins/yupptv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/zattoo.py` & `streamlink-6.0.0/src/streamlink/plugins/zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/zdf_mediathek.py` & `streamlink-6.0.0/src/streamlink/plugins/zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/zeenews.py` & `streamlink-6.0.0/src/streamlink/plugins/zeenews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/zengatv.py` & `streamlink-6.0.0/src/streamlink/plugins/zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/plugins/zhanqi.py` & `streamlink-6.0.0/src/streamlink/plugins/zhanqi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/session.py` & `streamlink-6.0.0/src/streamlink/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from requests.adapters import HTTPAdapter
 
 from streamlink import __version__, plugins
 from streamlink.exceptions import NoPluginError, PluginError, StreamlinkDeprecationWarning
 from streamlink.logger import StreamlinkLogger
 from streamlink.options import Options
 from streamlink.plugin.api.http_session import HTTPSession, TLSNoDHAdapter
-from streamlink.plugin.plugin import NO_PRIORITY, NORMAL_PRIORITY, Matcher, Plugin
+from streamlink.plugin.plugin import NO_PRIORITY, Matcher, Plugin
 from streamlink.utils.l10n import Localization
 from streamlink.utils.module import load_module
 from streamlink.utils.url import update_scheme
 
 
 # Ensure that the Logger class returned is Streamslink's for using the API (for backwards compatibility)
 logging.setLoggerClass(StreamlinkLogger)
@@ -83,15 +83,15 @@
     # ---- setters
 
     def _set_interface(self, key, value):
         for scheme, adapter in self.session.http.adapters.items():
             if scheme not in ("http://", "https://"):
                 continue
             if not value:
-                adapter.poolmanager.connection_pool_kw.pop("source_address")
+                adapter.poolmanager.connection_pool_kw.pop("source_address", None)
             else:
                 # https://docs.python.org/3/library/socket.html#socket.create_connection
                 adapter.poolmanager.connection_pool_kw.update(source_address=(value, 0))
         self.set_explicit(key, None if not value else value)
 
     def _set_ipv4_ipv6(self, key, value):
         self.set_explicit(key, value)
@@ -139,15 +139,15 @@
                 f"`{key}` has been deprecated in favor of the `{name}` option",
                 StreamlinkDeprecationWarning,
                 stacklevel=3 + _get_deprecation_stacklevel_offset(),
             )
 
         return inner
 
-    # bind explicitly with dummy context, to prevent `TypeError: 'staticmethod' object is not callable` on py<310
+    # TODO: py39 support end: remove explicit dummy context binding of static method
     _factory_set_http_attr_key_equals_value = _factory_set_http_attr_key_equals_value.__get__(object)
     _factory_set_deprecated = _factory_set_deprecated.__get__(object)
 
     # ----
 
     _OPTIONS_HTTP_ATTRS = {
         "http-cookies": "cookies",
@@ -204,14 +204,20 @@
 
     http: HTTPSession
     """
     An instance of Streamlink's :class:`requests.Session` subclass.
     Used for any kind of HTTP request made by plugin and stream implementations.
     """
 
+    options: Options
+    """
+    Session options, which is a subclass of :class:`Options <streamlink.options.Options>`
+    with additional getter/setter mappings for special options.
+    """
+
     def __init__(
         self,
         options: Optional[Dict[str, Any]] = None,
     ):
         """
         :param options: Custom options
         """
@@ -245,14 +251,21 @@
             "ffmpeg-verbose": False,
             "ffmpeg-verbose-path": None,
             "ffmpeg-fout": None,
             "ffmpeg-video-transcode": None,
             "ffmpeg-audio-transcode": None,
             "ffmpeg-copyts": False,
             "ffmpeg-start-at-zero": False,
+            "webbrowser": True,
+            "webbrowser-executable": None,
+            "webbrowser-timeout": 20.0,
+            "webbrowser-cdp-host": None,
+            "webbrowser-cdp-port": None,
+            "webbrowser-cdp-timeout": 2.0,
+            "webbrowser-headless": True,
         })
         if options:
             self.options.update(options)
         self.plugins: Dict[str, Type[Plugin]] = {}
         self.load_builtin_plugins()
 
     def set_option(self, key: str, value: Any) -> None:
@@ -484,52 +497,55 @@
               - ``bool``
               - ``False``
               - Don't shift input stream timestamps when muxing streams
             * - ffmpeg-start-at-zero
               - ``bool``
               - ``False``
               - When ``ffmpeg-copyts`` is ``True``, shift timestamps to zero
+            * - webbrowser
+              - ``bool``
+              - ``True``
+              - Enable or disable support for Streamlink's webbrowser API
+            * - webbrowser-executable
+              - ``str | None``
+              - ``None``
+              - Path to the web browser's executable
+            * - webbrowser-timeout
+              - ``float``
+              - ``20.0``
+              - The maximum amount of time which the webbrowser can take to launch and execute
+            * - webbrowser-cdp-host
+              - ``str | None``
+              - ``None``
+              - Custom host for the Chrome Devtools Protocol (CDP) interface
+            * - webbrowser-cdp-port
+              - ``int | None``
+              - ``None``
+              - Custom port for the Chrome Devtools Protocol (CDP) interface
+            * - webbrowser-cdp-timeout
+              - ``float``
+              - ``2.0``
+              - The maximum amount of time for waiting on a single CDP command response
+            * - webbrowser-headless
+              - ``bool``
+              - ``True``
+              - Whether to launch the webbrowser in headless mode or not
         """
 
         self.options.set(key, value)
 
     def get_option(self, key: str) -> Any:
         """
         Returns the current value of the specified option.
 
         :param key: key of the option
         """
 
         return self.options.get(key)
 
-    def set_plugin_option(self, plugin: str, key: str, value: Any) -> None:
-        """
-        Sets plugin specific options used by plugins originating from this session object.
-
-        :param plugin: name of the plugin
-        :param key: key of the option
-        :param value: value to set the option to
-        """
-
-        if plugin in self.plugins:
-            plugincls = self.plugins[plugin]
-            plugincls.set_option(key, value)
-
-    def get_plugin_option(self, plugin: str, key: str) -> Optional[Any]:
-        """
-        Returns the current value of the plugin specific option.
-
-        :param plugin: name of the plugin
-        :param key: key of the option
-        """
-
-        if plugin in self.plugins:
-            plugincls = self.plugins[plugin]
-            return plugincls.get_option(key)
-
     @lru_cache(maxsize=128)  # noqa: B019
     def resolve_url(
         self,
         url: str,
         follow_redirect: bool = True,
     ) -> Tuple[str, Type[Plugin], str]:
         """
@@ -551,25 +567,14 @@
         priority = NO_PRIORITY
         for name, plugin in self.plugins.items():
             if plugin.matchers:
                 for matcher in plugin.matchers:
                     if matcher.priority > priority and matcher.pattern.match(url) is not None:
                         candidate = name, plugin
                         priority = matcher.priority
-            # TODO: remove deprecated plugin resolver
-            elif hasattr(plugin, "can_handle_url") and callable(plugin.can_handle_url) and plugin.can_handle_url(url):
-                prio = plugin.priority(url) if hasattr(plugin, "priority") and callable(plugin.priority) else NORMAL_PRIORITY
-                if prio > priority:
-                    warnings.warn(
-                        f"Resolved plugin {name} with deprecated can_handle_url API",
-                        StreamlinkDeprecationWarning,
-                        stacklevel=1,
-                    )
-                    candidate = name, plugin
-                    priority = prio
 
         if candidate:
             return candidate[0], candidate[1], url
 
         if follow_redirect:
             # Attempt to handle a redirect URL
             try:
@@ -599,17 +604,17 @@
         return self.resolve_url(url, follow_redirect=False)
 
     def streams(self, url: str, **params):
         """
         Attempts to find a plugin and extracts streams from the *url* if a plugin was found.
 
         :param url: a URL to match against loaded plugins
-        :param params: Additional keyword arguments passed to :meth:`streamlink.plugin.Plugin.streams`
+        :param params: Additional keyword arguments passed to :meth:`Plugin.streams() <streamlink.plugin.Plugin.streams>`
         :raises NoPluginError: on plugin resolve failure
-        :return: A :class:`dict` of stream names and :class:`streamlink.stream.Stream` instances
+        :return: A :class:`dict` of stream names and :class:`Stream <streamlink.stream.Stream>` instances
         """
 
         pluginname, pluginclass, resolved_url = self.resolve_url(url)
         plugin = pluginclass(self, resolved_url)
 
         return plugin.streams(**params)
 
@@ -632,16 +637,16 @@
         success = False
         for _loader, name, _ispkg in pkgutil.iter_modules([path]):
             # set the full plugin module name
             # use the "streamlink.plugins." prefix even for sideloaded plugins
             module_name = f"streamlink.plugins.{name}"
             try:
                 mod = load_module(module_name, path)
-            except ImportError:
-                log.exception(f"Failed to load plugin {name} from {path}\n")
+            except ImportError as err:
+                log.exception(f"Failed to load plugin {name} from {path}", exc_info=err)
                 continue
 
             if not hasattr(mod, "__plugin__") or not issubclass(mod.__plugin__, Plugin):
                 continue
             success = True
             plugin = mod.__plugin__
             if name in self.plugins:
```

### Comparing `streamlink-5.5.1/src/streamlink/stream/dash.py` & `streamlink-6.0.0/src/streamlink/stream/dash.py`

 * *Files 6% similar despite different names*

```diff
@@ -193,29 +193,29 @@
 
     def __init__(
         self,
         session: Streamlink,
         mpd: MPD,
         video_representation: Optional[Representation] = None,
         audio_representation: Optional[Representation] = None,
-        **args,
+        **kwargs,
     ):
         """
         :param session: Streamlink session instance
         :param mpd: Parsed MPD manifest
         :param video_representation: Video representation
         :param audio_representation: Audio representation
-        :param args: Additional keyword arguments passed to :meth:`requests.Session.request`
+        :param kwargs: Additional keyword arguments passed to :meth:`requests.Session.request`
         """
 
         super().__init__(session)
         self.mpd = mpd
         self.video_representation = video_representation
         self.audio_representation = audio_representation
-        self.args = args
+        self.args = session.http.valid_request_args(**kwargs)
 
     def __json__(self):
         json = dict(type=self.shortname())
 
         if self.mpd.url:
             args = self.args.copy()
             args.update(url=self.mpd.url)
@@ -260,35 +260,39 @@
 
     @classmethod
     def parse_manifest(
         cls,
         session: Streamlink,
         url_or_manifest: str,
         period: int = 0,
-        **args,
+        with_video_only: bool = False,
+        with_audio_only: bool = False,
+        **kwargs,
     ) -> Dict[str, "DASHStream"]:
         """
         Parse a DASH manifest file and return its streams.
 
         :param session: Streamlink session instance
         :param url_or_manifest: URL of the manifest file or an XML manifest string
         :param period: Which MPD period to use (index number) for finding representations
-        :param args: Additional keyword arguments passed to :meth:`requests.Session.request`
+        :param with_video_only: Also return video-only streams, otherwise only return muxed streams
+        :param with_audio_only: Also return audio-only streams, otherwise only return muxed streams
+        :param kwargs: Additional keyword arguments passed to :meth:`requests.Session.request`
         """
 
-        manifest, mpd_params = cls.fetch_manifest(session, url_or_manifest)
+        manifest, mpd_params = cls.fetch_manifest(session, url_or_manifest, **kwargs)
 
         try:
             mpd = cls.parse_mpd(manifest, mpd_params)
         except Exception as err:
             raise PluginError(f"Failed to parse MPD manifest: {err}") from err
 
         source = mpd_params.get("url", "MPD manifest")
-        video: List[Optional[Representation]] = []
-        audio: List[Optional[Representation]] = []
+        video: List[Optional[Representation]] = [None] if with_audio_only else []
+        audio: List[Optional[Representation]] = [None] if with_video_only else []
 
         # Search for suitable video and audio representations
         for aset in mpd.periods[period].adaptationSets:
             if aset.contentProtections:
                 raise PluginError(f"{source} is protected by DRM")
             for rep in aset.representations:
                 if rep.contentProtections:
@@ -326,15 +330,18 @@
 
         # if the language is given by the stream, filter out other languages that do not match
         if len(available_languages) > 1:
             audio = [a for a in audio if a and (a.lang is None or a.lang == lang)]
 
         ret = []
         for vid, aud in itertools.product(video, audio):
-            stream = DASHStream(session, mpd, vid, aud, **args)
+            if not vid and not aud:
+                continue
+
+            stream = DASHStream(session, mpd, vid, aud, **kwargs)
             stream_name = []
 
             if vid:
                 stream_name.append(f"{vid.height or vid.bandwidth_rounded:0.0f}{'p' if vid.height else 'k'}")
             if aud and len(audio) > 1:
                 stream_name.append(f"a{aud.bandwidth:0.0f}k")
             ret.append(("+".join(stream_name), stream))
```

### Comparing `streamlink-5.5.1/src/streamlink/stream/dash_manifest.py` & `streamlink-6.0.0/src/streamlink/stream/dash_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import re
 from collections import defaultdict
 from contextlib import contextmanager
 from datetime import datetime, timedelta
 from itertools import count, repeat
 from pathlib import Path
 from typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Dict,
     Iterator,
     List,
+    Literal,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
@@ -31,18 +31,14 @@
 
 # noinspection PyProtectedMember
 from lxml.etree import _Attrib, _Element
 
 from streamlink.utils.times import UTC, fromtimestamp, now
 
 
-if TYPE_CHECKING:  # pragma: no cover
-    from typing_extensions import Literal
-
-
 log = logging.getLogger(__name__)
 
 EPOCH_START = fromtimestamp(0)
 ONE_SECOND = timedelta(seconds=1)
 
 SEGMENT_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
@@ -107,15 +103,15 @@
 
 class MPDParsers:
     @staticmethod
     def bool_str(v: str) -> bool:
         return v.lower() == "true"
 
     @staticmethod
-    def type(mpdtype: "Literal['static', 'dynamic']") -> "Literal['static', 'dynamic']":
+    def type(mpdtype: Literal["static", "dynamic"]) -> Literal["static", "dynamic"]:
         if mpdtype not in ("static", "dynamic"):
             raise MPDParsingError("@type must be static or dynamic")
         return mpdtype
 
     @staticmethod
     def duration(duration: str) -> Union[timedelta, Duration]:
         return parse_duration(duration)
```

### Comparing `streamlink-5.5.1/src/streamlink/stream/ffmpegmux.py` & `streamlink-6.0.0/src/streamlink/stream/ffmpegmux.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/stream/file.py` & `streamlink-6.0.0/src/streamlink/stream/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/stream/filtered.py` & `streamlink-6.0.0/src/streamlink/stream/filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/stream/hls.py` & `streamlink-6.0.0/src/streamlink/stream/hls.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,27 @@
 import re
 import struct
 from concurrent.futures import Future
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Union
 from urllib.parse import urlparse
 
-# noinspection PyPackageRequirements
-from Crypto.Cipher import AES
-
-# noinspection PyPackageRequirements
-from Crypto.Util.Padding import unpad
 from requests import Response
 from requests.exceptions import ChunkedEncodingError, ConnectionError, ContentDecodingError, InvalidSchema
 
 from streamlink.buffers import RingBuffer
 from streamlink.exceptions import StreamError
+from streamlink.session import Streamlink
 from streamlink.stream.ffmpegmux import FFMPEGMuxer, MuxedStream
 from streamlink.stream.filtered import FilteredStream
 from streamlink.stream.hls_playlist import M3U8, ByteRange, Key, Map, Media, Segment, load as load_hls_playlist
 from streamlink.stream.http import HTTPStream
 from streamlink.stream.segmented import SegmentedStreamReader, SegmentedStreamWorker, SegmentedStreamWriter
 from streamlink.utils.cache import LRUCache
+from streamlink.utils.crypto import AES, unpad
 from streamlink.utils.formatter import Formatter
 from streamlink.utils.times import now
 
 
 log = logging.getLogger(__name__)
 
 
@@ -288,21 +285,25 @@
 
 
 class HLSStreamWorker(SegmentedStreamWorker):
     reader: "HLSStreamReader"
     writer: "HLSStreamWriter"
     stream: "HLSStream"
 
+    SEGMENT_QUEUE_TIMING_THRESHOLD_FACTOR = 2
+
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.playlist_changed = False
         self.playlist_end: Optional[int] = None
+        self.playlist_targetduration: float = 0
         self.playlist_sequence: int = -1
         self.playlist_sequences: List[Sequence] = []
+        self.playlist_sequences_last: datetime = now()
         self.playlist_reload_last: datetime = now()
         self.playlist_reload_time: float = 6
         self.playlist_reload_time_override = self.session.options.get("hls-playlist-reload-time")
         self.playlist_reload_retries = self.session.options.get("hls-playlist-reload-attempts")
         self.live_edge = self.session.options.get("hls-live-edge")
         self.duration_offset_start = int(self.stream.start_offset + (self.session.options.get("hls-start-offset") or 0))
         self.duration_limit = self.stream.duration or (
@@ -349,28 +350,29 @@
         if playlist.iframes_only:
             raise StreamError("Streams containing I-frames only are not playable")
 
         media_sequence = playlist.media_sequence or 0
         sequences = [Sequence(media_sequence + i, s)
                      for i, s in enumerate(playlist.segments)]
 
+        self.playlist_targetduration = playlist.targetduration or 0
         self.playlist_reload_time = self._playlist_reload_time(playlist, sequences)
 
         if sequences:
             self.process_sequences(playlist, sequences)
 
     def _playlist_reload_time(self, playlist: M3U8, sequences: List[Sequence]) -> float:
         if self.playlist_reload_time_override == "segment" and sequences:
             return sequences[-1].segment.duration
         if self.playlist_reload_time_override == "live-edge" and sequences:
             return sum(s.segment.duration for s in sequences[-max(1, self.live_edge - 1):])
         if type(self.playlist_reload_time_override) is float and self.playlist_reload_time_override > 0:
             return self.playlist_reload_time_override
-        if playlist.target_duration:
-            return playlist.target_duration
+        if playlist.targetduration:
+            return playlist.targetduration
         if sequences:
             return sum(s.segment.duration for s in sequences[-max(1, self.live_edge - 1):])
 
         return self.playlist_reload_time
 
     def process_sequences(self, playlist: M3U8, sequences: List[Sequence]) -> None:
         first_sequence, last_sequence = sequences[0], sequences[-1]
@@ -394,14 +396,22 @@
                 self.playlist_sequence = edge_sequence.num
             else:
                 self.playlist_sequence = first_sequence.num
 
     def valid_sequence(self, sequence: Sequence) -> bool:
         return sequence.num >= self.playlist_sequence
 
+    def _segment_queue_timing_threshold_reached(self) -> bool:
+        threshold = self.playlist_targetduration * self.SEGMENT_QUEUE_TIMING_THRESHOLD_FACTOR
+        if now() <= self.playlist_sequences_last + timedelta(seconds=threshold):
+            return False
+
+        log.warning(f"No new segments in playlist for more than {threshold:.2f}s. Stopping...")
+        return True
+
     @staticmethod
     def duration_to_sequence(duration: float, sequences: List[Sequence]) -> int:
         d = 0.0
         default = -1
 
         sequences_order = sequences if duration >= 0 else reversed(sequences)
 
@@ -411,15 +421,18 @@
             d += sequence.segment.duration
             default = sequence.num
 
         # could not skip far enough, so return the default
         return default
 
     def iter_segments(self):
-        self.playlist_reload_last = now()
+        self.playlist_reload_last \
+            = self.playlist_sequences_last \
+            = now()
+
         try:
             self.reload_playlist()
         except StreamError as err:
             log.error(f"{err}")
             self.reader.close()
             return
 
@@ -442,29 +455,37 @@
                 f"Duration: {self.duration_limit}",
                 f"Start Sequence: {self.playlist_sequence}",
                 f"End Sequence: {self.playlist_end}",
             ]))
 
         total_duration = 0
         while not self.closed:
+            queued = False
             for sequence in filter(self.valid_sequence, self.playlist_sequences):
                 log.debug(f"Adding segment {sequence.num} to queue")
                 yield sequence
+                queued = True
+
                 total_duration += sequence.segment.duration
                 if self.duration_limit and total_duration >= self.duration_limit:
                     log.info(f"Stopping stream early after {self.duration_limit}")
                     return
 
                 # End of stream
                 stream_end = self.playlist_end is not None and sequence.num >= self.playlist_end
                 if self.closed or stream_end:
                     return
 
                 self.playlist_sequence = sequence.num + 1
 
+            if queued:
+                self.playlist_sequences_last = now()
+            elif self._segment_queue_timing_threshold_reached():
+                return
+
             # Exclude playlist fetch+processing time from the overall playlist reload time
             # and reload playlist in a strict time interval
             time_completed = now()
             time_elapsed = max(0.0, (time_completed - self.playlist_reload_last).total_seconds())
             time_wait = max(0.0, self.playlist_reload_time - time_elapsed)
             if self.wait(time_wait):
                 if time_wait > 0:
@@ -506,43 +527,43 @@
     Muxes multiple HLS video and audio streams into one output stream.
     """
 
     __shortname__ = "hls-multi"
 
     def __init__(
         self,
-        session,
+        session: Streamlink,
         video: str,
         audio: Union[str, List[str]],
         url_master: Optional[str] = None,
         multivariant: Optional[M3U8] = None,
         force_restart: bool = False,
         ffmpeg_options: Optional[Dict[str, Any]] = None,
-        **args,
+        **kwargs,
     ):
         """
-        :param streamlink.Streamlink session: Streamlink session instance
+        :param session: Streamlink session instance
         :param video: Video stream URL
         :param audio: Audio stream URL or list of URLs
         :param url_master: The URL of the HLS playlist's multivariant playlist (deprecated)
         :param multivariant: The parsed multivariant playlist
         :param force_restart: Start from the beginning after reaching the playlist's end
         :param ffmpeg_options: Additional keyword arguments passed to :class:`ffmpegmux.FFMPEGMuxer`
-        :param args: Additional keyword arguments passed to :class:`HLSStream`
+        :param kwargs: Additional keyword arguments passed to :class:`HLSStream`
         """
 
         tracks = [video]
         maps = ["0:v?", "0:a?"]
         if audio:
             if isinstance(audio, list):
                 tracks.extend(audio)
             else:
                 tracks.append(audio)
         maps.extend(f"{i}:a" for i in range(1, len(tracks)))
-        substreams = [HLSStream(session, url, force_restart=force_restart, **args) for url in tracks]
+        substreams = [HLSStream(session, url, force_restart=force_restart, **kwargs) for url in tracks]
         ffmpeg_options = ffmpeg_options or {}
 
         super().__init__(session, *substreams, format="mpegts", maps=maps, **ffmpeg_options)
         self._url_master = url_master
         self.multivariant = multivariant if multivariant and multivariant.is_master else None
 
     @property
@@ -565,35 +586,35 @@
     """
 
     __shortname__ = "hls"
     __reader__ = HLSStreamReader
 
     def __init__(
         self,
-        session_,
+        session: Streamlink,
         url: str,
         url_master: Optional[str] = None,
         multivariant: Optional[M3U8] = None,
         force_restart: bool = False,
         start_offset: float = 0,
         duration: Optional[float] = None,
-        **args,
+        **kwargs,
     ):
         """
-        :param streamlink.Streamlink session_: Streamlink session instance
+        :param session: Streamlink session instance
         :param url: The URL of the HLS playlist
         :param url_master: The URL of the HLS playlist's multivariant playlist (deprecated)
         :param multivariant: The parsed multivariant playlist
         :param force_restart: Start from the beginning after reaching the playlist's end
         :param start_offset: Number of seconds to be skipped from the beginning
         :param duration: Number of seconds until ending the stream
-        :param args: Additional keyword arguments passed to :meth:`requests.Session.request`
+        :param kwargs: Additional keyword arguments passed to :meth:`requests.Session.request`
         """
 
-        super().__init__(session_, url, **args)
+        super().__init__(session, url, **kwargs)
         self._url_master = url_master
         self.multivariant = multivariant if multivariant and multivariant.is_master else None
         self.force_restart = force_restart
         self.start_offset = start_offset
         self.duration = duration
 
     def __json__(self):
@@ -628,59 +649,60 @@
     def open(self):
         reader = self.__reader__(self)
         reader.open()
 
         return reader
 
     @classmethod
-    def _fetch_variant_playlist(cls, session, url: str, **request_params) -> Response:
-        res = session.http.get(url, exception=OSError, **request_params)
+    def _fetch_variant_playlist(cls, session, url: str, **request_args) -> Response:
+        res = session.http.get(url, exception=OSError, **request_args)
         res.encoding = "utf-8"
 
         return res
 
     # TODO: rename to _parse_variant_playlist
     @classmethod
     def _get_variant_playlist(cls, *args, **kwargs):
         return load_hls_playlist(*args, **kwargs)
 
     @classmethod
     def parse_variant_playlist(
         cls,
-        session_,
+        session: Streamlink,
         url: str,
         name_key: str = "name",
         name_prefix: str = "",
         check_streams: bool = False,
         force_restart: bool = False,
         name_fmt: Optional[str] = None,
         start_offset: float = 0,
         duration: Optional[float] = None,
-        **request_params,
+        **kwargs,
     ) -> Dict[str, Union["HLSStream", "MuxedHLSStream"]]:
         """
         Parse a variant playlist and return its streams.
 
-        :param streamlink.Streamlink session_: Streamlink session instance
+        :param session: Streamlink session instance
         :param url: The URL of the variant playlist
         :param name_key: Prefer to use this key as stream name, valid keys are: name, pixels, bitrate
         :param name_prefix: Add this prefix to the stream names
         :param check_streams: Only allow streams that are accessible
         :param force_restart: Start at the first segment even for a live stream
         :param name_fmt: A format string for the name, allowed format keys are: name, pixels, bitrate
         :param start_offset: Number of seconds to be skipped from the beginning
         :param duration: Number of second until ending the stream
-        :param request_params: Additional keyword arguments passed to :class:`HLSStream`, :class:`MuxedHLSStream`,
-                               or :py:meth:`requests.Session.request`
+        :param kwargs: Additional keyword arguments passed to :class:`HLSStream`, :class:`MuxedHLSStream`,
+                       or :py:meth:`requests.Session.request`
         """
 
-        locale = session_.localization
-        audio_select = session_.options.get("hls-audio-select")
+        locale = session.localization
+        audio_select = session.options.get("hls-audio-select")
 
-        res = cls._fetch_variant_playlist(session_, url, **request_params)
+        request_args = session.http.valid_request_args(**kwargs)
+        res = cls._fetch_variant_playlist(session, url, **request_args)
 
         try:
             multivariant = cls._get_variant_playlist(res)
         except ValueError as err:
             raise OSError(f"Failed to parse playlist: {err}") from err
 
         stream_name: Optional[str]
@@ -767,46 +789,46 @@
                     continue
                 elif num_alts > 0:
                     stream_name = f"{stream_name}{num_alts + 1}"
 
             if check_streams:
                 # noinspection PyBroadException
                 try:
-                    session_.http.get(playlist.uri, **request_params)
+                    session.http.get(playlist.uri, **request_args)
                 except KeyboardInterrupt:
                     raise
                 except Exception:
                     continue
 
             external_audio = preferred_audio or default_audio or fallback_audio
 
-            if external_audio and FFMPEGMuxer.is_usable(session_):
+            if external_audio and FFMPEGMuxer.is_usable(session):
                 external_audio_msg = ", ".join([
                     f"(language={x.language}, name={x.name or 'N/A'})"
                     for x in external_audio
                 ])
                 log.debug(f"Using external audio tracks for stream {stream_name} {external_audio_msg}")
 
                 stream = MuxedHLSStream(
-                    session_,
+                    session,
                     video=playlist.uri,
                     audio=[x.uri for x in external_audio if x.uri],
                     multivariant=multivariant,
                     force_restart=force_restart,
                     start_offset=start_offset,
                     duration=duration,
-                    **request_params,
+                    **kwargs,
                 )
             else:
                 stream = cls(
-                    session_,
+                    session,
                     playlist.uri,
                     multivariant=multivariant,
                     force_restart=force_restart,
                     start_offset=start_offset,
                     duration=duration,
-                    **request_params,
+                    **kwargs,
                 )
 
             streams[stream_name] = stream
 
         return streams
```

### Comparing `streamlink-5.5.1/src/streamlink/stream/hls_playlist.py` & `streamlink-6.0.0/src/streamlink/stream/hls_playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         self.is_master: bool = False
 
         self.allow_cache: Optional[bool] = None  # version < 7
         self.discontinuity_sequence: Optional[int] = None
         self.iframes_only: Optional[bool] = None  # version >= 4
         self.media_sequence: Optional[int] = None
         self.playlist_type: Optional[str] = None
-        self.target_duration: Optional[int] = None
+        self.targetduration: Optional[float] = None
         self.start: Optional[Start] = None
         self.version: Optional[int] = None
 
         self.media: List[Media] = []
         self.playlists: List[Playlist] = []
         self.dateranges: List[DateRange] = []
         self.segments: List[Segment] = []
@@ -419,15 +419,15 @@
     # 4.3.3: Media Playlist Tags
 
     def parse_tag_ext_x_targetduration(self, value: str) -> None:
         """
         EXT-X-TARGETDURATION
         https://datatracker.ietf.org/doc/html/rfc8216#section-4.3.3.1
         """
-        self.m3u8.target_duration = int(value)
+        self.m3u8.targetduration = float(value)
 
     def parse_tag_ext_x_media_sequence(self, value: str) -> None:
         """
         EXT-X-MEDIA-SEQUENCE
         https://datatracker.ietf.org/doc/html/rfc8216#section-4.3.3.2
         """
         self.m3u8.media_sequence = int(value)
```

### Comparing `streamlink-5.5.1/src/streamlink/stream/http.py` & `streamlink-6.0.0/src/streamlink/stream/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict
 
 from streamlink.exceptions import StreamError
+from streamlink.session import Streamlink
 from streamlink.stream.stream import Stream
 from streamlink.stream.wrappers import StreamIOIterWrapper, StreamIOThreadWrapper
 
 
 class HTTPStream(Stream):
     """
     An HTTP stream using the :mod:`requests` library.
@@ -13,28 +14,29 @@
     __shortname__ = "http"
 
     args: Dict
     """A dict of keyword arguments passed to :meth:`requests.Session.request`, such as method, headers, cookies, etc."""
 
     def __init__(
         self,
-        session_,
+        session: Streamlink,
         url: str,
         buffered: bool = True,
-        **args,
+        **kwargs,
     ):
         """
-        :param streamlink.Streamlink session_: Streamlink session instance
+        :param session: Streamlink session instance
         :param url: The URL of the HTTP stream
         :param buffered: Wrap stream output in an additional reader-thread
-        :param args: Additional keyword arguments passed to :meth:`requests.Session.request`
+        :param kwargs: Additional keyword arguments passed to :meth:`requests.Session.request`
         """
 
-        super().__init__(session_)
-        self.args = dict(url=url, **args)
+        super().__init__(session)
+        self.args = self.session.http.valid_request_args(**kwargs)
+        self.args["url"] = url
         self.buffered = buffered
 
     def __json__(self):
         req = self.session.http.prepare_new_request(**self.args)
 
         return dict(
             type=self.shortname(),
```

### Comparing `streamlink-5.5.1/src/streamlink/stream/segmented.py` & `streamlink-6.0.0/src/streamlink/stream/segmented.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/stream/stream.py` & `streamlink-6.0.0/src/streamlink/stream/stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/stream/wrappers.py` & `streamlink-6.0.0/src/streamlink/stream/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/user_input.py` & `streamlink-6.0.0/src/streamlink/user_input.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/__init__.py` & `streamlink-6.0.0/src/streamlink/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/args.py` & `streamlink-6.0.0/src/streamlink/utils/args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/cache.py` & `streamlink-6.0.0/src/streamlink/utils/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/data.py` & `streamlink-6.0.0/src/streamlink/utils/data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/formatter.py` & `streamlink-6.0.0/src/streamlink/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/l10n.py` & `streamlink-6.0.0/src/streamlink/utils/l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/named_pipe.py` & `streamlink-6.0.0/src/streamlink/utils/named_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import random
 import tempfile
 import threading
 from contextlib import suppress
 from pathlib import Path
+from typing import Type
 
 from streamlink.compat import is_win32
 
 
 try:
     from ctypes import byref, c_ulong, c_void_p, cast, windll  # type: ignore[attr-defined]
 except ImportError:
@@ -129,8 +130,12 @@
                 windll.kernel32.CloseHandle(self.pipe)
         except OSError:
             raise
         finally:
             self.pipe = None
 
 
-NamedPipe = NamedPipePosix if not is_win32 else NamedPipeWindows
+NamedPipe: Type[NamedPipeBase]
+if not is_win32:
+    NamedPipe = NamedPipePosix
+else:
+    NamedPipe = NamedPipeWindows
```

### Comparing `streamlink-5.5.1/src/streamlink/utils/parse.py` & `streamlink-6.0.0/src/streamlink/utils/parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/processoutput.py` & `streamlink-6.0.0/src/streamlink/utils/processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/times.py` & `streamlink-6.0.0/src/streamlink/utils/times.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink/utils/url.py` & `streamlink-6.0.0/src/streamlink/utils/url.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink.egg-info/PKG-INFO` & `streamlink-6.0.0/src/streamlink.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.5.1
+Version: 6.0.0
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
-Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
+Project-URL: Homepage, https://github.com/streamlink/streamlink
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
 Project-URL: Source, https://github.com/streamlink/streamlink
 Project-URL: Funding, https://streamlink.github.io/latest/donate.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Utilities
-Requires-Python: <4,>=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center"><a href="https://streamlink.github.io/">Streamlink<br><img height="150" alt="Streamlink" src="https://raw.githubusercontent.com/streamlink/streamlink/master/icon.svg"></a></h1>
 
 <p align="center">
   <a href="https://streamlink.github.io/install.html"><img alt="Supported Python versions" src="https://img.shields.io/pypi/pyversions/streamlink.svg?style=flat-square&maxAge=86400"></a>
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.5.1 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 6.0.0 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
-into a video player of choice. Home-page: https://github.com/streamlink/
-streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
-Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
-Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
-URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
-https://streamlink.github.io/latest/donate.html Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: BSD License
-Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
-Desktop Classifier: Operating System :: POSIX Classifier: Operating System ::
-MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Internet :: WWW/
-HTTP Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
-Multimedia :: Video Classifier: Topic :: Utilities Requires-Python: <4,>=3.7
-Description-Content-Type: text/markdown License-File: LICENSE
+into a video player of choice. Author: Streamlink Author-email:
+streamlink@protonmail.com License: Simplified BSD Project-URL: Homepage, https:
+//github.com/streamlink/streamlink Project-URL: Documentation, https://
+streamlink.github.io/ Project-URL: Tracker, https://github.com/streamlink/
+streamlink/issues Project-URL: Source, https://github.com/streamlink/streamlink
+Project-URL: Funding, https://streamlink.github.io/latest/donate.html
+Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
+OSI Approved :: BSD License Classifier: Environment :: Console Classifier:
+Intended Audience :: End Users/Desktop Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS Classifier: Operating System :: Microsoft
+:: Windows Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Multimedia :: Sound/Audio Classifier: Topic :: Multimedia :: Video Classifier:
+Topic :: Utilities Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE
                                ****** Streamlink
                               [Streamlink] ******
   [Supported_Python_versions] [Latest_release] [License] [Open_issues] [Build
                         status] [Overall_code_coverage]
  A Python library and command-line interface which pipes streams from various
                          services into a video player.
     Avoid resource-heavy and unoptimized websites, and still enjoy streamed
```

### Comparing `streamlink-5.5.1/src/streamlink.egg-info/SOURCES.txt` & `streamlink-6.0.0/src/streamlink.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 LICENSE
 MANIFEST.in
 README.md
 dev-requirements.txt
 docs-requirements.txt
 icon.svg
 pyproject.toml
-setup.cfg
 setup.py
 completions/bash/streamlink
 completions/zsh/_streamlink
 docs/Makefile
 docs/_applications.rst
 docs/_man.rst
 docs/api.rst
@@ -28,14 +27,15 @@
 docs/ext_github.py
 docs/ext_html_template_vars.py
 docs/ext_plugins.py
 docs/ext_releaseref.py
 docs/index.rst
 docs/install.rst
 docs/issues.rst
+docs/migrations.rst
 docs/players.rst
 docs/plugins.rst
 docs/thirdparty.rst
 docs/_build/man/streamlink.1
 docs/_static/apple-touch-icon.png
 docs/_static/favicon-16x16.png
 docs/_static/favicon-32x32.png
@@ -46,14 +46,21 @@
 docs/_static/opengraph-image.png
 docs/_static/site.webmanifest
 docs/_static/styles/custom.css
 docs/_templates/base.html
 docs/_templates/page.html
 docs/_templates/sidebar/brand.html
 docs/_templates/sidebar/github-buttons.html
+docs/api/exceptions.rst
+docs/api/options.rst
+docs/api/plugin.rst
+docs/api/session.rst
+docs/api/stream.rst
+docs/api/streamlink.rst
+docs/api/webbrowser.rst
 docs/cli/config.rst
 docs/cli/metadata.rst
 docs/cli/plugin-sideloading.rst
 docs/cli/plugins.rst
 docs/cli/protocols.rst
 docs/cli/proxy.rst
 docs/cli/tutorial.rst
@@ -260,17 +267,43 @@
 src/streamlink/utils/crypto.py
 src/streamlink/utils/data.py
 src/streamlink/utils/formatter.py
 src/streamlink/utils/l10n.py
 src/streamlink/utils/module.py
 src/streamlink/utils/named_pipe.py
 src/streamlink/utils/parse.py
+src/streamlink/utils/path.py
 src/streamlink/utils/processoutput.py
+src/streamlink/utils/random.py
+src/streamlink/utils/socket.py
 src/streamlink/utils/times.py
 src/streamlink/utils/url.py
+src/streamlink/webbrowser/__init__.py
+src/streamlink/webbrowser/chromium.py
+src/streamlink/webbrowser/exceptions.py
+src/streamlink/webbrowser/webbrowser.py
+src/streamlink/webbrowser/cdp/__init__.py
+src/streamlink/webbrowser/cdp/client.py
+src/streamlink/webbrowser/cdp/connection.py
+src/streamlink/webbrowser/cdp/exceptions.py
+src/streamlink/webbrowser/cdp/devtools/__init__.py
+src/streamlink/webbrowser/cdp/devtools/browser.py
+src/streamlink/webbrowser/cdp/devtools/debugger.py
+src/streamlink/webbrowser/cdp/devtools/dom.py
+src/streamlink/webbrowser/cdp/devtools/emulation.py
+src/streamlink/webbrowser/cdp/devtools/fetch.py
+src/streamlink/webbrowser/cdp/devtools/input_.py
+src/streamlink/webbrowser/cdp/devtools/inspector.py
+src/streamlink/webbrowser/cdp/devtools/io.py
+src/streamlink/webbrowser/cdp/devtools/network.py
+src/streamlink/webbrowser/cdp/devtools/page.py
+src/streamlink/webbrowser/cdp/devtools/runtime.py
+src/streamlink/webbrowser/cdp/devtools/security.py
+src/streamlink/webbrowser/cdp/devtools/target.py
+src/streamlink/webbrowser/cdp/devtools/util.py
 src/streamlink_cli/__init__.py
 src/streamlink_cli/__main__.py
 src/streamlink_cli/argparser.py
 src/streamlink_cli/compat.py
 src/streamlink_cli/console.py
 src/streamlink_cli/constants.py
 src/streamlink_cli/main.py
@@ -299,27 +332,28 @@
 tests/test_plugin_userinput.py
 tests/test_plugins.py
 tests/test_session.py
 tests/test_streamlink_api.py
 tests/cli/__init__.py
 tests/cli/test_argparser.py
 tests/cli/test_cmdline.py
-tests/cli/test_cmdline_player_fifo.py
 tests/cli/test_cmdline_title.py
 tests/cli/test_console.py
 tests/cli/test_main.py
 tests/cli/test_main_formatter.py
 tests/cli/test_main_setup_config_args.py
+tests/cli/test_plugin_args_and_options.py
 tests/cli/test_streamrunner.py
 tests/cli/output/__init__.py
-tests/cli/output/test_output.py
-tests/cli/output/test_playeroutput.py
+tests/cli/output/test_file.py
+tests/cli/output/test_player.py
 tests/cli/utils/__init__.py
 tests/cli/utils/test_formatter.py
 tests/cli/utils/test_path.py
+tests/cli/utils/test_player.py
 tests/cli/utils/test_progress.py
 tests/cli/utils/test_versioncheck.py
 tests/mixins/__init__.py
 tests/mixins/stream_hls.py
 tests/plugin/__init__.py
 tests/plugin/testplugin.py
 tests/plugin/testplugin_invalid.py
@@ -370,14 +404,16 @@
 tests/plugins/test_foxtr.py
 tests/plugins/test_galatasaraytv.py
 tests/plugins/test_goltelevision.py
 tests/plugins/test_goodgame.py
 tests/plugins/test_googledrive.py
 tests/plugins/test_gulli.py
 tests/plugins/test_hiplayer.py
+tests/plugins/test_hls.py
+tests/plugins/test_http.py
 tests/plugins/test_htv.py
 tests/plugins/test_huajiao.py
 tests/plugins/test_huya.py
 tests/plugins/test_idf1.py
 tests/plugins/test_indihometv.py
 tests/plugins/test_invintus.py
 tests/plugins/test_kugou.py
@@ -427,15 +463,14 @@
 tests/plugins/test_sbscokr.py
 tests/plugins/test_showroom.py
 tests/plugins/test_sportal.py
 tests/plugins/test_sportschau.py
 tests/plugins/test_ssh101.py
 tests/plugins/test_stadium.py
 tests/plugins/test_steam.py
-tests/plugins/test_stream.py
 tests/plugins/test_streamable.py
 tests/plugins/test_streann.py
 tests/plugins/test_stv.py
 tests/plugins/test_svtplay.py
 tests/plugins/test_swisstxt.py
 tests/plugins/test_telefe.py
 tests/plugins/test_telemadrid.py
@@ -523,10 +558,20 @@
 tests/utils/test_crypto.py
 tests/utils/test_data.py
 tests/utils/test_formatter.py
 tests/utils/test_l10n.py
 tests/utils/test_module.py
 tests/utils/test_named_pipe.py
 tests/utils/test_parse.py
+tests/utils/test_path.py
 tests/utils/test_processoutput.py
+tests/utils/test_random.py
 tests/utils/test_times.py
-tests/utils/test_url.py
+tests/utils/test_url.py
+tests/webbrowser/__init__.py
+tests/webbrowser/conftest.py
+tests/webbrowser/test_chromium.py
+tests/webbrowser/test_webbrowser.py
+tests/webbrowser/cdp/__init__.py
+tests/webbrowser/cdp/conftest.py
+tests/webbrowser/cdp/test_client.py
+tests/webbrowser/cdp/test_connection.py
```

### Comparing `streamlink-5.5.1/src/streamlink_cli/argparser.py` & `streamlink-6.0.0/src/streamlink_cli/argparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import argparse
 import numbers
 import re
+from pathlib import Path
 from string import printable
 from textwrap import dedent
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from streamlink import __version__ as streamlink_version, logger
 from streamlink.session import Streamlink
 from streamlink.utils.args import boolean, comma_list, comma_list_filter, filesize, keyvalue, num
 from streamlink.utils.times import hours_minutes_seconds
-from streamlink_cli.constants import (
-    PLAYER_ARGS_INPUT_DEFAULT,
-    PLAYER_ARGS_INPUT_FALLBACK,
-    STREAM_PASSTHROUGH,
-    SUPPORTED_PLAYERS,
-)
+from streamlink_cli.constants import STREAM_PASSTHROUGH
+from streamlink_cli.output.player import PlayerOutput
 from streamlink_cli.utils import find_default_player
 
 
 _printable_re = re.compile(r"[{0}]".format(printable))
 _option_re = re.compile(r"""
     (?P<name>[A-z-]+) # A option name, valid characters are A to z and dash.
     \s*
@@ -371,91 +368,74 @@
         help="""
         Set the network interface.
         """,
     )
     general.add_argument(
         "-4", "--ipv4",
         action="store_true",
+        default=None,
         help="""
         Resolve address names to IPv4 only. This option overrides --ipv6.
         """,
     )
     general.add_argument(
         "-6", "--ipv6",
         action="store_true",
+        default=None,
         help="""
         Resolve address names to IPv6 only. This option overrides --ipv4.
         """,
     )
 
     player = parser.add_argument_group("Player options")
     player.add_argument(
         "-p", "--player",
-        metavar="COMMAND",
+        metavar="PATH",
+        type=Path,
         default=find_default_player(),
         help="""
-        Player to feed stream data to. By default, VLC will be used if it can be
-        found in its default location.
-
-        This is a shell-like syntax to support using a specific player:
-
-          %(prog)s --player=vlc <url> [stream]
+        The player executable that will be launched (unless a different output method was chosen).
 
-        Absolute or relative paths can also be passed via this option in the
-        event the player's executable can not be resolved:
+        Either set an absolute or relative path to the player executable, or just set the executable's name
+        if it can be resolved from the paths of the system's `PATH` environment variable.
 
-          %(prog)s --player=/path/to/vlc <url> [stream]
-          %(prog)s --player=./vlc-player/vlc <url> [stream]
+        In addition to setting the player executable path, custom player arguments can be set via --player-args.
 
-        To use a player that is located in a path with spaces you must quote the
-        parameter or its value:
+        Note: In the past, --player allowed defining additional player arguments, which as a consequence required wrapping
+        player paths that contained spaces in quotation marks. This is unsupported since release `6.0.0`.
 
-          %(prog)s "--player=/path/with spaces/vlc" <url> [stream]
-          %(prog)s --player "C:\\path\\with spaces\\mpc-hc64.exe" <url> [stream]
-
-        Options may also be passed to the player. For example:
-
-          %(prog)s --player "vlc --file-caching=5000" <url> [stream]
-
-        As an alternative to this, see the --player-args parameter, which does
-        not log any custom player arguments.
+        Default is VLC player, if available.
         """,
     )
     player.add_argument(
         "-a", "--player-args",
         metavar="ARGUMENTS",
         default="",
         help=f"""
-        This option allows you to customize the default arguments which are put
-        together with the value of --player to create a command to execute.
-
-        It's usually enough to only use --player instead of this unless you need
-        to add arguments after the player's input argument or if you don't want
-        any of the player arguments to be logged.
+        This option allows the arguments which are used to launch the player process to be customized.
 
-        The value can contain formatting variables surrounded by curly braces,
-        `{{` and `}}`. If you need to include a brace character, it can be escaped
-        by doubling, e.g. `{{{{` and `}}}}`.
+        The value can contain formatting variables surrounded by curly braces, `{{` and `}}`.
+        Curly brace characters can be escaped by doubling, e.g. `{{{{` and `}}}}`.
 
-        Formatting variables available:
+        Available formatting variables:
 
-        {{{PLAYER_ARGS_INPUT_DEFAULT}}}
-            This is the input that the player will use. For standard input (stdin),
-            it is `-` (dash), but it can also be a URL, depending on the options used.
+        `{{{PlayerOutput.PLAYER_ARGS_INPUT}}}`
+            This is the input argument that the player will receive. For standard input (stdin),
+            it is `-` (dash), but it can also be a file path or URL, depending on the options used.
+            If unset, then the player input argument will be appended to the parsed player arguments list.
 
-        {{{PLAYER_ARGS_INPUT_FALLBACK}}}
-            The old fallback variable name with the same functionality.
+        `{{{PlayerOutput.PLAYER_ARGS_TITLE}}}`
+            The automatically generated player title arguments, if a supported player was found. See --title for more.
+            If unset, automatically generated player title arguments will be prepended to the parsed player arguments list.
 
         Example:
 
-          %(prog)s -p vlc -a "--play-and-exit {{{PLAYER_ARGS_INPUT_DEFAULT}}}" <url> [stream]
+          %(prog)s -p vlc -a "--play-and-exit --no-one-instance" <url> [stream]
 
-        Note: When neither of the variables are found, `{{{PLAYER_ARGS_INPUT_DEFAULT}}}`
-        will be appended to the whole parameter value, to ensure that the player
-        always receives an input argument.
+        Default is "".
         """,
     )
     player.add_argument(
         "-v", "--verbose-player",
         action="store_true",
         help="""
         Allow the player to display its console output.
@@ -578,15 +558,15 @@
         "-t", "--title",
         metavar="TITLE",
         help=f"""
         Change the title of the video player's window.
 
         Please see the "Metadata variables" section of Streamlink's CLI documentation for all available metadata variables.
 
-        This option is only supported for the following players: {', '.join(sorted(SUPPORTED_PLAYERS.keys()))}
+        This option is only supported for the following players: {', '.join(sorted(PlayerOutput.PLAYERS.keys()))}
 
         VLC specific information:
             VLC does support special formatting variables on its own:
             https://wiki.videolan.org/Documentation:Format_String/
 
             These variables are accessible in the --title option by adding a backslash
             in front of the dollar sign which VLC uses as its formatting character.
@@ -909,14 +889,15 @@
 
         Default is 60.0.
         """,
     )
     transport.add_argument(
         "--mux-subtitles",
         action="store_true",
+        default=None,
         help="""
         Automatically mux available subtitles into the output stream.
 
         Needs to be supported by the used plugin.
         """,
     )
 
@@ -939,14 +920,15 @@
         this, please refer to the player's own documentation for the required configuration. Player parameters can be set via
         --player-args.
         """,
     )
     transport_hls.add_argument(
         "--hls-segment-stream-data",
         action="store_true",
+        default=None,
         help="""
         Immediately write segment data into output buffer while downloading.
         """,
     )
     transport_hls.add_argument(
         "--hls-playlist-reload-attempts",
         type=num(int, ge=1),
@@ -1050,14 +1032,15 @@
 
         Default is unlimited.
         """,
     )
     transport_hls.add_argument(
         "--hls-live-restart",
         action="store_true",
+        default=None,
         help="""
         Skip to the beginning of a live stream, or as far back as possible.
         """,
     )
 
     transport_dash.add_argument(
         "--dash-manifest-reload-attempts",
@@ -1086,21 +1069,23 @@
 
         Example: --ffmpeg-ffmpeg "/usr/local/bin/ffmpeg"
         """,
     )
     transport_ffmpeg.add_argument(
         "--ffmpeg-no-validation",
         action="store_true",
+        default=None,
         help="""
         Disable FFmpeg validation and version logging.
         """,
     )
     transport_ffmpeg.add_argument(
         "--ffmpeg-verbose",
         action="store_true",
+        default=None,
         help="""
         Write the console output from ffmpeg to the console.
         """,
     )
     transport_ffmpeg.add_argument(
         "--ffmpeg-verbose-path",
         type=str,
@@ -1142,22 +1127,24 @@
 
         Example: --ffmpeg-audio-transcode "aac"
         """,
     )
     transport_ffmpeg.add_argument(
         "--ffmpeg-copyts",
         action="store_true",
+        default=None,
         help="""
         Forces the `-copyts` ffmpeg option and does not remove
         the initial start time offset value.
         """,
     )
     transport_ffmpeg.add_argument(
         "--ffmpeg-start-at-zero",
         action="store_true",
+        default=None,
         help="""
         Enable the `-start_at_zero` ffmpeg option when using --ffmpeg-copyts.
         """,
     )
 
     http = parser.add_argument_group("HTTP options")
     http.add_argument(
@@ -1201,32 +1188,35 @@
         A query parameter to add to each HTTP request.
 
         Can be repeated to add multiple query parameters.
         """,
     )
     http.add_argument(
         "--http-ignore-env",
-        action="store_true",
+        action="store_false",
+        default=None,
         help="""
         Ignore HTTP settings set in the environment such as environment
         variables (`HTTP_PROXY`, etc) or `~/.netrc` authentication.
         """,
     )
     http.add_argument(
         "--http-no-ssl-verify",
-        action="store_true",
+        action="store_false",
+        default=None,
         help="""
         Don't attempt to verify SSL certificates.
 
         Usually a bad idea, only use this if you know what you're doing.
         """,
     )
     http.add_argument(
         "--http-disable-dh",
         action="store_true",
+        default=None,
         help="""
         Disable Diffie Hellman key exchange
 
         Usually a bad idea, only use this if you know what you're doing.
         """,
     )
     http.add_argument(
@@ -1256,21 +1246,98 @@
         General timeout used by all HTTP requests except the ones covered by
         other options.
 
         Default is 20.0.
         """,
     )
 
-    return parser
+    webbrowser = parser.add_argument_group("Web browser options")
+    webbrowser.add_argument(
+        "--webbrowser",
+        type=boolean,
+        metavar="{yes,true,1,on,no,false,0,off}",
+        default=None,
+        help="""
+        Enable or disable support for Streamlink's webbrowser API.
 
+        Streamlink's webbrowser API allows plugins which implement it to launch a web browser and extract data from websites
+        which they otherwise couldn't do via the regular HTTP session in Python due to specific JavaScript restrictions.
 
-def false(_): return False  # noqa: E704
+        The web browser is run isolated and in a clean environment without access to regular user data.
+
+        Streamlink currently only supports Chromium-based web browsers using the Chrome Devtools Protocol (CDP).
+        This includes Chromium itself, Google Chrome, Microsoft Edge, Brave, Vivaldi, and others, but full support for
+        third party Chromium forks is not guaranteed. If you encounter any issues, please try Chromium or Google Chrome instead.
+
+        Default is true.
+        """,
+    )
+    webbrowser.add_argument(
+        "--webbrowser-executable",
+        metavar="PATH",
+        help="""
+        Path to the web browser's executable.
+
+        By default, it is looked up automatically according to the rules of the used webbrowser API implementation.
+        This usually involves a list of known executable names and fallback paths on all supported operating systems.
+        """,
+    )
+    webbrowser.add_argument(
+        "--webbrowser-timeout",
+        metavar="TIME",
+        type=num(float, gt=0),
+        help="""
+        The maximum amount of time which the web browser can take to launch and execute.
+        """,
+    )
+    webbrowser.add_argument(
+        "--webbrowser-cdp-host",
+        metavar="HOST",
+        help="""
+        Host for the web browser's inter-process communication interface (CDP specific).
+
+        Default is 127.0.0.1.
+        """,
+    )
+    webbrowser.add_argument(
+        "--webbrowser-cdp-port",
+        metavar="PORT",
+        type=num(int, ge=0, le=65535),
+        help="""
+        Port for the web browser's inter-process communication interface (CDP specific).
+
+        Tries to find a free port by default.
+        """,
+    )
+    webbrowser.add_argument(
+        "--webbrowser-cdp-timeout",
+        metavar="TIME",
+        type=num(float, gt=0),
+        help="""
+        The maximum amount of time for waiting on a single CDP command response.
+        """,
+    )
+    webbrowser.add_argument(
+        "--webbrowser-headless",
+        type=boolean,
+        metavar="{yes,true,1,on,no,false,0,off}",
+        default=None,
+        help="""
+        Whether to launch the web browser in headless mode or not.
+        When enabled, it stays completely hidden and doesn't require a desktop environment to run.
+
+        Default is true.
+        """,
+    )
+
+    return parser
 
 
 # The order of arguments determines if options get overridden by `Streamlink.set_option()`
+# NOTE: arguments with `action=store_{true,false}` must set `default=None`
 _ARGUMENT_TO_SESSIONOPTION: List[Tuple[str, str, Optional[Callable[[Any], Any]]]] = [
     # generic arguments
     ("locale", "locale", None),
 
     # network arguments
     ("interface", "interface", None),
     ("ipv4", "ipv4", None),
@@ -1278,16 +1345,16 @@
 
     # HTTP session arguments
     ("https_proxy", "https-proxy", None),
     ("http_proxy", "http-proxy", None),
     ("http_cookie", "http-cookies", dict),
     ("http_header", "http-headers", dict),
     ("http_query_param", "http-query-params", dict),
-    ("http_ignore_env", "http-trust-env", false),
-    ("http_no_ssl_verify", "http-ssl-verify", false),
+    ("http_ignore_env", "http-trust-env", None),
+    ("http_no_ssl_verify", "http-ssl-verify", None),
     ("http_disable_dh", "http-disable-dh", None),
     ("http_ssl_cert", "http-ssl-cert", None),
     ("http_ssl_cert_crt_key", "http-ssl-cert", tuple),
     ("http_timeout", "http-timeout", None),
 
     # deprecated stream transport arguments (need to be defined first, so following ones can override values)
     ("hls_segment_attempts", "hls-segment-attempts", None),
@@ -1319,20 +1386,29 @@
     ("ffmpeg_verbose", "ffmpeg-verbose", None),
     ("ffmpeg_verbose_path", "ffmpeg-verbose-path", None),
     ("ffmpeg_fout", "ffmpeg-fout", None),
     ("ffmpeg_video_transcode", "ffmpeg-video-transcode", None),
     ("ffmpeg_audio_transcode", "ffmpeg-audio-transcode", None),
     ("ffmpeg_copyts", "ffmpeg-copyts", None),
     ("ffmpeg_start_at_zero", "ffmpeg-start-at-zero", None),
+
+    # web browser arguments
+    ("webbrowser", "webbrowser", None),
+    ("webbrowser_executable", "webbrowser-executable", None),
+    ("webbrowser_timeout", "webbrowser-timeout", None),
+    ("webbrowser_cdp_host", "webbrowser-cdp-host", None),
+    ("webbrowser_cdp_port", "webbrowser-cdp-port", None),
+    ("webbrowser_cdp_timeout", "webbrowser-cdp-timeout", None),
+    ("webbrowser_headless", "webbrowser-headless", None),
 ]
 
 
 def setup_session_options(session: Streamlink, args: argparse.Namespace):
     for arg, option, mapper in _ARGUMENT_TO_SESSIONOPTION:
         value = getattr(args, arg)
-        if value:
+        if value is not None:
             if mapper is not None:
                 value = mapper(value)
             session.set_option(option, value)
 
 
 __all__ = ["ArgumentParser", "build_parser", "setup_session_options"]
```

### Comparing `streamlink-5.5.1/src/streamlink_cli/console.py` & `streamlink-6.0.0/src/streamlink_cli/console.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/main.py` & `streamlink-6.0.0/src/streamlink_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import importlib.metadata
 import logging
 import os
 import platform
 import re
 import signal
 import sys
 import warnings
@@ -11,20 +12,21 @@
 from pathlib import Path
 from time import sleep
 from typing import Any, Dict, List, Optional, Type, Union
 
 import streamlink.logger as logger
 from streamlink import NoPluginError, PluginError, StreamError, Streamlink, __version__ as streamlink_version
 from streamlink.exceptions import FatalPluginError, StreamlinkDeprecationWarning
-from streamlink.plugin import Plugin, PluginOptions
+from streamlink.options import Options
+from streamlink.plugin import Plugin
 from streamlink.stream.stream import Stream, StreamIO
 from streamlink.utils.named_pipe import NamedPipe
 from streamlink.utils.times import LOCAL as LOCALTIMEZONE
 from streamlink_cli.argparser import ArgumentParser, build_parser, setup_session_options
-from streamlink_cli.compat import DeprecatedPath, importlib_metadata, stdout
+from streamlink_cli.compat import DeprecatedPath, stdout
 from streamlink_cli.console import ConsoleOutput, ConsoleUserInputRequester
 from streamlink_cli.constants import CONFIG_FILES, DEFAULT_STREAM_METADATA, LOG_DIR, PLUGIN_DIRS, STREAM_SYNONYMS
 from streamlink_cli.output import FileOutput, HTTPOutput, PlayerOutput
 from streamlink_cli.streamrunner import StreamRunner
 from streamlink_cli.utils import Formatter, datetime
 from streamlink_cli.utils.versioncheck import check_version
 
@@ -134,15 +136,15 @@
             else:
                 record = check_file_output(formatter.path(args.record, args.fs_safe_rules), args.force)
 
         log.info(f"Starting player: {args.player}")
 
         return PlayerOutput(
             args.player,
-            args=args.player_args,
+            args.player_args,
             quiet=not args.verbose_player,
             kill=not args.player_no_close,
             namedpipe=namedpipe,
             http=http,
             record=record,
             title=formatter.title(args.title, defaults=DEFAULT_STREAM_METADATA) if args.title else args.url,
         )
@@ -181,17 +183,17 @@
                 "The default player (VLC) does not seem to be installed."
                 + " You must specify the path to a player executable with --player.",
             )
 
         server = create_http_server()
         player = output = PlayerOutput(
             args.player,
-            args=args.player_args,
-            filename=server.url,
+            args.player_args,
             quiet=not args.verbose_player,
+            filename=server.url,
             title=formatter.title(args.title, defaults=DEFAULT_STREAM_METADATA) if args.title else args.url,
         )
 
         try:
             log.info(f"Starting player: {args.player}")
             if player:
                 player.open()
@@ -270,18 +272,18 @@
         url = stream.to_url()
     except TypeError:
         console.exit("The stream specified cannot be translated to a URL")
         return False
 
     output = PlayerOutput(
         args.player,
-        args=args.player_args,
-        filename=f'"{url}"',
-        call=True,
+        args.player_args,
         quiet=not args.verbose_player,
+        call=True,
+        filename=url,
         title=formatter.title(args.title, defaults=DEFAULT_STREAM_METADATA) if args.title else args.url,
     )
 
     try:
         log.info(f"Starting player: {args.player}")
         output.open()
     except OSError as err:
@@ -525,16 +527,16 @@
     Proceeds to handle stream if user specified a valid one,
     otherwise output list of valid streams.
 
     """
 
     try:
         pluginname, pluginclass, resolved_url = streamlink.resolve_url(args.url)
-        setup_plugin_options(streamlink, pluginname, pluginclass)
-        plugin = pluginclass(streamlink, resolved_url)
+        options = setup_plugin_options(pluginname, pluginclass)
+        plugin = pluginclass(streamlink, resolved_url, options)
         log.info(f"Found matching plugin {pluginname} for URL {args.url}")
 
         if args.retry_max or args.retry_streams:
             retry_streams = 1
             retry_max = 0
             if args.retry_streams:
                 retry_streams = args.retry_streams
@@ -706,71 +708,64 @@
     """Creates the Streamlink session."""
     global streamlink
 
     streamlink = Streamlink({"user-input-requester": ConsoleUserInputRequester(console)})
 
 
 def setup_plugin_args(session: Streamlink, parser: ArgumentParser):
-    """Sets Streamlink plugin options."""
+    """Adds plugin argument data to the argument parser."""
 
     plugin_args = parser.add_argument_group("Plugin options")
     for pname, plugin in session.plugins.items():
-        defaults = {}
         group = parser.add_argument_group(pname.capitalize(), parent=plugin_args)
 
         for parg in plugin.arguments or []:
-            if not parg.is_global:
-                group.add_argument(parg.argument_name(pname), **parg.options)
-                defaults[parg.dest] = parg.default
-            else:
-                pargdest = parg.dest
-                for action in parser._actions:
-                    # find matching global argument
-                    if pargdest != action.dest:
-                        continue
-                    defaults[pargdest] = action.default
-
-        plugin.options = PluginOptions(defaults)
+            group.add_argument(parg.argument_name(pname), **parg.options)
 
 
-def setup_plugin_options(session: Streamlink, pluginname: str, pluginclass: Type[Plugin]):
-    """Sets Streamlink plugin options."""
-    if pluginclass.arguments is None:
-        return
+def setup_plugin_options(pluginname: str, pluginclass: Type[Plugin]) -> Options:
+    """Initializes plugin options from argument values."""
+
+    if not pluginclass.arguments:
+        return Options()
 
+    defaults = {}
+    values = {}
     required = {}
 
     for parg in pluginclass.arguments:
+        defaults[parg.dest] = parg.default
+
         if parg.options.get("help") == argparse.SUPPRESS:
             continue
 
-        value = getattr(args, parg.dest if parg.is_global else parg.namespace_dest(pluginname))
-        session.set_plugin_option(pluginname, parg.dest, value)
+        value = getattr(args, parg.namespace_dest(pluginname))
+        values[parg.dest] = value
 
-        if not parg.is_global:
-            if parg.required:
-                required[parg.name] = parg
-            # if the value is set, check to see if any of the required arguments are not set
-            if parg.required or value:
-                try:
-                    for rparg in pluginclass.arguments.requires(parg.name):
-                        required[rparg.name] = rparg
-                except RuntimeError:
-                    log.error(f"{pluginname} plugin has a configuration error and the arguments cannot be parsed")
-                    break
-
-    if required:
-        for req in required.values():
-            if not session.get_plugin_option(pluginname, req.dest):
-                prompt = f"{req.prompt or f'Enter {pluginname} {req.name}'}: "
-                session.set_plugin_option(
-                    pluginname,
-                    req.dest,
-                    console.askpass(prompt) if req.sensitive else console.ask(prompt),
-                )
+        if parg.required:
+            required[parg.name] = parg
+        # if the value is set, check to see if any of the required arguments are not set
+        if parg.required or value:
+            try:
+                for rparg in pluginclass.arguments.requires(parg.name):
+                    required[rparg.name] = rparg
+            except RuntimeError:  # pragma: no cover
+                log.error(f"{pluginname} plugin has a configuration error and the arguments cannot be parsed")
+                break
+
+    for req in required.values():
+        if not values.get(req.dest):
+            prompt = f"{req.prompt or f'Enter {pluginname} {req.name}'}: "
+            value = console.askpass(prompt) if req.sensitive else console.ask(prompt)
+            values[req.dest] = value
+
+    options = Options(defaults)
+    options.update(values)
+
+    return options
 
 
 def log_root_warning():
     if hasattr(os, "geteuid"):  # pragma: no branch
         if os.geteuid() == 0:
             log.info("streamlink is running as root! Be careful!")
 
@@ -795,20 +790,20 @@
     log.debug(f"Streamlink: {streamlink_version}")
 
     # https://peps.python.org/pep-0508/#names
     re_name = re.compile(r"[A-Z\d](?:[A-Z\d._-]*[A-Z\d])?", re.IGNORECASE)
     log.debug("Dependencies:")
     for name in [
         match.group(0)
-        for match in map(re_name.match, importlib_metadata.requires("streamlink"))
+        for match in map(re_name.match, importlib.metadata.requires("streamlink"))
         if match is not None
     ]:
         try:
-            version = importlib_metadata.version(name)
-        except importlib_metadata.PackageNotFoundError:
+            version = importlib.metadata.version(name)
+        except importlib.metadata.PackageNotFoundError:
             continue
         log.debug(f" {name}: {version}")
 
 
 def log_current_arguments(session: Streamlink, parser: argparse.ArgumentParser):
     if not logger.root.isEnabledFor(logging.DEBUG):
         return
```

### Comparing `streamlink-5.5.1/src/streamlink_cli/output/abc.py` & `streamlink-6.0.0/src/streamlink_cli/output/abc.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/output/file.py` & `streamlink-6.0.0/src/streamlink_cli/output/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/output/http.py` & `streamlink-6.0.0/src/streamlink_cli/output/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/streamrunner.py` & `streamlink-6.0.0/src/streamlink_cli/streamrunner.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/utils/__init__.py` & `streamlink-6.0.0/src/streamlink_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/utils/formatter.py` & `streamlink-6.0.0/src/streamlink_cli/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/utils/path.py` & `streamlink-6.0.0/src/streamlink_cli/utils/path.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/utils/progress.py` & `streamlink-6.0.0/src/streamlink_cli/utils/progress.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/src/streamlink_cli/utils/versioncheck.py` & `streamlink-6.0.0/src/streamlink_cli/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/__init__.py` & `streamlink-6.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/cli/test_argparser.py` & `streamlink-6.0.0/tests/cli/test_argparser.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,24 +19,30 @@
     pytest.param(
         ["--locale", "xx_XX"],
         "locale",
         "xx_XX",
         id="Arg+value without mapper",
     ),
     pytest.param(
-        ["--http-query-param", "foo=bar", "--http-query-param", "baz=qux"],
-        "http-query-params",
-        {"foo": "bar", "baz": "qux"},
-        id="Arg+value with dict mapper",
+        ["--http-disable-dh"],
+        "http-disable-dh",
+        True,
+        id="Arg with action=store_true",
     ),
     pytest.param(
         ["--http-no-ssl-verify"],
         "http-ssl-verify",
         False,
-        id="Arg with bool mapper",
+        id="Arg with action=store_false",
+    ),
+    pytest.param(
+        ["--http-query-param", "foo=bar", "--http-query-param", "baz=qux"],
+        "http-query-params",
+        {"foo": "bar", "baz": "qux"},
+        id="Arg+value with dict mapper",
     ),
     pytest.param(
         ["--http-ssl-cert-crt-key", "foo.crt", "bar.key"],
         "http-ssl-cert",
         ("foo.crt", "bar.key"),
         id="Arg+value with tuple mapper",
     ),
@@ -55,14 +61,40 @@
 ])
 def test_setup_session_options(parser: ArgumentParser, session: Streamlink, argv: List, option: str, expected: Any):
     args = parser.parse_args(argv)
     setup_session_options(session, args)
     assert session.get_option(option) == expected
 
 
+def test_setup_session_options_default_values(monkeypatch: pytest.MonkeyPatch, parser: ArgumentParser, session: Streamlink):
+    mock_set_option = Mock()
+    monkeypatch.setattr(session, "set_option", mock_set_option)
+    args = parser.parse_args([])
+    setup_session_options(session, args)
+    assert session.options.options == session.options.defaults
+    assert not mock_set_option.called, "Value of unset session-option arg must be None and must not call set_option()"
+
+
+@pytest.mark.parametrize(("default", "new", "expected"), [
+    pytest.param(False, None, False, id="Default False, unset"),
+    pytest.param(True, None, True, id="Default True, unset"),
+    pytest.param(False, False, False, id="Default False, set to False"),
+    pytest.param(False, True, True, id="Default False, set to True"),
+    pytest.param(True, False, False, id="Default True, set to False"),
+    pytest.param(True, True, True, id="Default True, set to True"),
+])
+def test_setup_session_options_override(monkeypatch: pytest.MonkeyPatch, session: Streamlink, default, new, expected):
+    arg = "NON_EXISTING_ARGPARSER_ARGUMENT"
+    key = "NON-EXISTING-SESSION-OPTION-KEY"
+    monkeypatch.setattr("streamlink_cli.argparser._ARGUMENT_TO_SESSIONOPTION", [(arg, key, None)])
+    session.set_option(key, default)
+    setup_session_options(session, Namespace(**{arg: new}))
+    assert session.get_option(key) == expected
+
+
 def test_cli_main_setup_session_options(monkeypatch: pytest.MonkeyPatch, parser: ArgumentParser, session: Streamlink):
     class StopTest(Exception):
         pass
 
     mock_setup_session_options = Mock()
 
     monkeypatch.setattr("sys.argv", [])
```

### Comparing `streamlink-5.5.1/tests/cli/test_cmdline_title.py` & `streamlink-6.0.0/tests/cli/test_cmdline_title.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,79 +2,113 @@
 
 from tests.cli.test_cmdline import CommandLineTestCase
 
 
 @pytest.mark.posix_only()
 class TestCommandLineWithTitlePOSIX(CommandLineTestCase):
     def test_open_player_with_title_vlc(self):
-        self._test_args(["streamlink", "-p", "/usr/bin/vlc",
-                         "--title", "{title} - {author} - {category}", "http://test.se", "test"],
-                        ["/usr/bin/vlc", "--input-title-format", "Test Title - Tѥst Āuƭhǿr - No Category", "-"])
+        self._test_args(
+            [
+                "streamlink",
+                "-p",
+                "/usr/bin/vlc",
+                "--title",
+                "{title} - {author} - {category}",
+                "http://test.se",
+                "test",
+            ],
+            [
+                "/usr/bin/vlc",
+                "--input-title-format",
+                "Test Title - Tѥst Āuƭhǿr - No Category",
+                "-",
+            ],
+        )
 
     def test_open_player_with_default_title_vlc(self):
-        self._test_args(["streamlink", "-p", "/usr/bin/vlc", "http://test.se", "test"],
-                        ["/usr/bin/vlc", "--input-title-format", "http://test.se", "-"])
+        self._test_args(
+            ["streamlink", "-p", "/usr/bin/vlc", "http://test.se", "test"],
+            ["/usr/bin/vlc", "--input-title-format", "http://test.se", "-"],
+        )
 
     def test_open_player_with_default_title_vlc_args(self):
-        self._test_args(["streamlink", "-p", "\"/Applications/VLC/vlc\" --other-option", "http://test.se", "test"],
-                        ["/Applications/VLC/vlc", "--other-option", "--input-title-format", "http://test.se", "-"])
+        self._test_args(
+            ["streamlink", "-p", "/Applications/VLC/vlc", "-a", "--other-option", "http://test.se", "test"],
+            ["/Applications/VLC/vlc", "--input-title-format", "http://test.se", "--other-option", "-"],
+        )
 
     def test_open_player_with_title_mpv(self):
-        self._test_args(["streamlink", "-p", "/usr/bin/mpv", "--title", "{title}", "http://test.se", "test"],
-                        ["/usr/bin/mpv", "--force-media-title=Test Title", "-"])
-
-    def test_unicode_title_2444(self):
-        self._test_args(["streamlink", "-p", "mpv", "-t", "★ ★ ★", "http://test.se", "test"],
-                        ["mpv", "--force-media-title=★ ★ ★", "-"])
+        self._test_args(
+            ["streamlink", "-p", "/usr/bin/mpv", "--title", "{title}", "http://test.se", "test"],
+            ["/usr/bin/mpv", "--force-media-title=Test Title", "-"],
+        )
 
 
 @pytest.mark.windows_only()
 class TestCommandLineWithTitleWindows(CommandLineTestCase):
     def test_open_player_with_title_vlc(self):
         self._test_args(
-            ["streamlink", "-p", "c:\\Program Files\\VideoLAN\\vlc.exe",
-             "--title", "{title} - {author} - {category}", "http://test.se", "test"],
-            "c:\\Program Files\\VideoLAN\\vlc.exe --input-title-format \"Test Title - Tѥst Āuƭhǿr - No Category\" -",
+            [
+                "streamlink",
+                "-p",
+                "c:\\Program Files\\VideoLAN\\vlc.exe",
+                "--title", "{title} - {author} - {category}",
+                "http://test.se",
+                "test",
+            ],
+            [
+                "c:\\Program Files\\VideoLAN\\vlc.exe",
+                "--input-title-format",
+                "Test Title - Tѥst Āuƭhǿr - No Category",
+                "-",
+            ],
         )
 
     def test_open_player_with_default_title_vlc(self):
         self._test_args(
             ["streamlink", "-p", "c:\\Program Files\\VideoLAN\\vlc.exe", "http://test.se", "test"],
-            "c:\\Program Files\\VideoLAN\\vlc.exe --input-title-format http://test.se -",
+            ["c:\\Program Files\\VideoLAN\\vlc.exe", "--input-title-format", "http://test.se", "-"],
         )
 
     def test_open_player_with_default_arg_vlc(self):
         self._test_args(
-            ["streamlink", "-p", "c:\\Program Files\\VideoLAN\\vlc.exe --argh", "http://test.se", "test"],
-            "c:\\Program Files\\VideoLAN\\vlc.exe --argh --input-title-format http://test.se -",
+            ["streamlink", "-p", "c:\\Program Files\\VideoLAN\\vlc.exe", "-a", "--other-option", "http://test.se", "test"],
+            ["c:\\Program Files\\VideoLAN\\vlc.exe", "--input-title-format", "http://test.se", "--other-option", "-"],
         )
 
-    # PotPlayer
     def test_open_player_with_title_pot(self):
         self._test_args(
-            ["streamlink", "-p", "\"c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe\"",
-             "--title", "{title}", "http://test.se/stream", "hls", "--player-passthrough", "hls"],
-            "\"c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe\" \"http://test.se/playlist.m3u8\\Test Title\"",
-            passthrough=True,
-        )
-
-    def test_open_player_with_unicode_author_pot_py3(self):
-        self._test_args(
-            ["streamlink", "-p", "\"c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe\"",
-             "--title", "{author}", "http://test.se/stream", "hls", "--player-passthrough", "hls"],
-            "\"c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe\" "
-            + "\"http://test.se/playlist.m3u8\\Tѥst Āuƭhǿr\"",
+            [
+                "streamlink",
+                "--player-passthrough",
+                "hls",
+                "-p",
+                "c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe",
+                "--title",
+                "{title}",
+                "http://test.se/stream",
+                "hls",
+            ],
+            [
+                "c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe",
+                "http://test.se/playlist.m3u8\\Test Title",
+            ],
             passthrough=True,
         )
 
     def test_open_player_with_default_title_pot(self):
         self._test_args(
-            ["streamlink", "-p", "\"c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe\"",
-             "http://test.se/stream", "hls", "--player-passthrough", "hls"],
-            "\"c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe\" "
-            + "\"http://test.se/playlist.m3u8\\http://test.se/stream\"",
+            [
+                "streamlink",
+                "--player-passthrough",
+                "hls",
+                "-p",
+                "c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe",
+                "http://test.se/stream",
+                "hls",
+            ],
+            [
+                "c:\\Program Files\\DAUM\\PotPlayer\\PotPlayerMini64.exe",
+                "http://test.se/playlist.m3u8\\http://test.se/stream",
+            ],
             passthrough=True,
         )
-
-    def test_unicode_title_2444_py3(self):
-        self._test_args(["streamlink", "-p", "mpv", "-t", "★ ★ ★", "http://test.se", "test"],
-                        "mpv \"--force-media-title=★ ★ ★\" -")
```

### Comparing `streamlink-5.5.1/tests/cli/test_console.py` & `streamlink-6.0.0/tests/cli/test_console.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-import unittest
 from io import StringIO
 from textwrap import dedent
-from unittest.mock import Mock, patch
+from unittest.mock import Mock
+
+import pytest
 
 from streamlink_cli.console import ConsoleOutput
 
 
-class TestConsoleOutput(unittest.TestCase):
+class TestConsoleOutput:
+    @pytest.fixture(autouse=True)
+    def _isatty(self, request: pytest.FixtureRequest, monkeypatch: pytest.MonkeyPatch):
+        isatty = not request.function.__name__.endswith("_no_tty")
+        monkeypatch.setattr("sys.stdin.isatty", lambda: isatty)
+
     def test_msg(self):
         output = StringIO()
         console = ConsoleOutput(output)
         console.msg("foo")
         console.msg_json({"test": 1})
         assert output.getvalue() == "foo\n"
 
@@ -70,74 +76,73 @@
                 "foo": "bar",
                 "baz": "qux"
               }
             ]
         """).lstrip()
         assert test_list1 == ["foo", "bar"]
 
-    @patch("streamlink_cli.console.sys.exit")
-    def test_msg_json_error(self, mock_exit):
+    def test_msg_json_error(self):
         output = StringIO()
         console = ConsoleOutput(output, json=True)
-        console.msg_json({"error": "bad"})
+        with pytest.raises(SystemExit) as cm:
+            console.msg_json({"error": "bad"})
+        assert cm.value.code == 1
         assert output.getvalue() == '{\n  "error": "bad"\n}\n'
-        mock_exit.assert_called_with(1)
 
-    @patch("streamlink_cli.console.sys.exit")
-    def test_exit(self, mock_exit: Mock):
+    def test_exit(self):
         output = StringIO()
         console = ConsoleOutput(output)
-        console.exit("error")
+        with pytest.raises(SystemExit) as cm:
+            console.exit("error")
+        assert cm.value.code == 1
         assert output.getvalue() == "error: error\n"
-        mock_exit.assert_called_with(1)
 
-    @patch("streamlink_cli.console.sys.exit")
-    def test_exit_json(self, mock_exit: Mock):
+    def test_exit_json(self):
         output = StringIO()
         console = ConsoleOutput(output, json=True)
-        console.exit("error")
+        with pytest.raises(SystemExit) as cm:
+            console.exit("error")
+        assert cm.value.code == 1
         assert output.getvalue() == '{\n  "error": "error"\n}\n'
-        mock_exit.assert_called_with(1)
 
-    @patch("streamlink_cli.console.input", Mock(return_value="hello"))
-    @patch("streamlink_cli.console.sys.stdin.isatty", Mock(return_value=True))
-    def test_ask(self):
+    def test_ask(self, monkeypatch: pytest.MonkeyPatch):
+        monkeypatch.setattr("builtins.input", Mock(return_value="hello"))
+
         output = StringIO()
         console = ConsoleOutput(output)
         assert console.ask("test: ") == "hello"
         assert output.getvalue() == "test: "
 
-    @patch("streamlink_cli.console.input")
-    @patch("streamlink_cli.console.sys.stdin.isatty", Mock(return_value=False))
-    def test_ask_no_tty(self, mock_input: Mock):
+    def test_ask_no_tty(self, monkeypatch: pytest.MonkeyPatch):
+        mock_input = Mock()
+        monkeypatch.setattr("builtins.input", mock_input)
+
         output = StringIO()
         console = ConsoleOutput(output)
         assert console.ask("test: ") is None
         assert output.getvalue() == ""
-        mock_input.assert_not_called()
+        assert mock_input.call_args_list == []
+
+    def test_ask_input_exception(self, monkeypatch: pytest.MonkeyPatch):
+        monkeypatch.setattr("builtins.input", Mock(side_effect=ValueError))
 
-    @patch("streamlink_cli.console.input", Mock(side_effect=ValueError))
-    @patch("streamlink_cli.console.sys.stdin.isatty", Mock(return_value=True))
-    def test_ask_input_exception(self):
         output = StringIO()
         console = ConsoleOutput(output)
         assert console.ask("test: ") is None
         assert output.getvalue() == "test: "
 
-    @patch("streamlink_cli.console.getpass")
-    @patch("streamlink_cli.console.sys.stdin.isatty", Mock(return_value=True))
-    def test_askpass(self, mock_getpass: Mock):
+    def test_askpass(self, monkeypatch: pytest.MonkeyPatch):
         def getpass(prompt, stream):
             stream.write(prompt)
             return "hello"
 
+        monkeypatch.setattr("streamlink_cli.console.getpass", getpass)
+
         output = StringIO()
         console = ConsoleOutput(output)
-        mock_getpass.side_effect = getpass
         assert console.askpass("test: ") == "hello"
         assert output.getvalue() == "test: "
 
-    @patch("streamlink_cli.console.sys.stdin.isatty", Mock(return_value=False))
     def test_askpass_no_tty(self):
         output = StringIO()
         console = ConsoleOutput(output)
         assert console.askpass("test: ") is None
```

### Comparing `streamlink-5.5.1/tests/cli/test_main.py` & `streamlink-6.0.0/tests/cli/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,25 +283,25 @@
         args.stdout = None
         args.record = None
         args.record_and_pipe = None
         args.player_fifo = False
         args.player_http = False
         args.title = None
         args.url = "URL"
-        args.player = "mpv"
+        args.player = Path("mpv")
         args.player_args = ""
 
         output = create_output(formatter)
         assert type(output) is PlayerOutput
-        assert output.title == "URL"
+        assert output.playerargs.title == "URL"
 
         args.title = "{author} - {title}"
         output = create_output(formatter)
         assert type(output) is PlayerOutput
-        assert output.title == "foo - bar"
+        assert output.playerargs.title == "foo - bar"
 
     @patch("streamlink_cli.main.args")
     @patch("streamlink_cli.main.check_file_output")
     def test_create_output_file_output(self, mock_check_file_output: Mock, args: Mock):
         formatter = Formatter({})
         mock_check_file_output.side_effect = lambda path, force: FileOutput(path)
         args.output = "foo"
@@ -373,31 +373,31 @@
         args.stdout = None
         args.record = "foo"
         args.record_and_pipe = None
         args.force = False
         args.fs_safe_rules = None
         args.title = None
         args.url = "URL"
-        args.player = "mpv"
+        args.player = Path("mpv")
         args.player_args = ""
         args.player_fifo = None
         args.player_http = None
 
         output = create_output(formatter)
         assert type(output) is PlayerOutput
-        assert output.title == "URL"
+        assert output.playerargs.title == "URL"
         assert type(output.record) is FileOutput
         assert output.record.filename == Path("foo")
         assert output.record.fd is None
         assert output.record.record is None
 
         args.title = "{author} - {title}"
         output = create_output(formatter)
         assert type(output) is PlayerOutput
-        assert output.title == "foo - bar"
+        assert output.playerargs.title == "foo - bar"
         assert type(output.record) is FileOutput
         assert output.record.filename == Path("foo")
         assert output.record.fd is None
         assert output.record.record is None
 
     @patch("streamlink_cli.main.args")
     @patch("streamlink_cli.main.DEFAULT_STREAM_METADATA", {"title": "bar"})
@@ -409,22 +409,22 @@
         args.stdout = None
         args.record = "-"
         args.record_and_pipe = None
         args.force = False
         args.fs_safe_rules = None
         args.title = "{author} - {title}"
         args.url = "URL"
-        args.player = "mpv"
+        args.player = Path("mpv")
         args.player_args = ""
         args.player_fifo = None
         args.player_http = None
 
         output = create_output(formatter)
         assert type(output) is PlayerOutput
-        assert output.title == "foo - bar"
+        assert output.playerargs.title == "foo - bar"
         assert type(output.record) is FileOutput
         assert output.record.filename is None
         assert output.record.fd is stdout
         assert output.record.record is None
 
     @patch("streamlink_cli.main.args")
     @patch("streamlink_cli.main.console")
@@ -546,14 +546,15 @@
         assert [(record.category, str(record.message)) for record in recwarn.list] == ([(
             StreamlinkDeprecationWarning,
             "The --force-progress option has been deprecated in favor of --progress=force",
         )] if deprecation else [])
         assert mock_streamrunner.call_args_list == [call(streamio, output, show_progress=expected)]
 
 
+# TODO: rewrite using pytest (caplog+capsys fixtures) and move to separate test module
 class _TestCLIMainLogging(unittest.TestCase):
     # stop test execution at the setup_signals() call, as we're not interested in what comes afterwards
     class StopTest(Exception):
         pass
 
     @classmethod
     def subject(cls, argv, **kwargs):
@@ -562,31 +563,27 @@
 
         with patch("streamlink_cli.main.os.geteuid", create=True, new=Mock(return_value=kwargs.get("euid", 1000))), \
              patch("streamlink_cli.main.streamlink", session), \
              patch("streamlink_cli.main.setup_signals", side_effect=cls.StopTest), \
              patch("streamlink_cli.main.CONFIG_FILES", []), \
              patch("streamlink_cli.main.setup_streamlink"), \
              patch("streamlink_cli.main.setup_plugins"), \
+             patch("streamlink_cli.argparser.find_default_player"), \
              patch("streamlink.session.Streamlink.load_builtin_plugins"), \
              patch("sys.argv") as mock_argv:
             mock_argv.__getitem__.side_effect = lambda x: argv[x]
             try:
                 streamlink_cli.main.main()
             except cls.StopTest:
                 pass
 
     def tearDown(self):
         streamlink_cli.main.logger.root.handlers.clear()
 
-    # python >=3.7.2: https://bugs.python.org/issue35046
-    _write_call_log_cli_info = (
-        [call("[cli][info] foo\n")]
-        if sys.version_info >= (3, 7, 2) else
-        [call("[cli][info] foo"), call("\n")]
-    )
+    _write_call_log_cli_info = [call("[cli][info] foo\n")]
     _write_call_console_msg = [call("bar\n")]
     _write_call_console_msg_error = [call("error: bar\n")]
     _write_call_console_msg_json = [call("{\n  \"error\": \"bar\"\n}\n")]
 
     _write_calls = _write_call_log_cli_info + _write_call_console_msg
 
     def write_file_and_assert(self, mock_mkdir: Mock, mock_write: Mock, mock_stdout: Mock):
@@ -594,20 +591,15 @@
         streamlink_cli.main.console.msg("bar")
         assert mock_mkdir.mock_calls == [call(parents=True, exist_ok=True)]
         assert mock_write.mock_calls == self._write_calls
         assert not mock_stdout.write.called
 
 
 class TestCLIMainLoggingStreams(_TestCLIMainLogging):
-    # python >=3.7.2: https://bugs.python.org/issue35046
-    _write_call_log_testcli_err = (
-        [call("[test_cli_main][error] baz\n")]
-        if sys.version_info >= (3, 7, 2) else
-        [call("[test_cli_main][error] baz"), call("\n")]
-    )
+    _write_call_log_testcli_err = [call("[test_cli_main][error] baz\n")]
 
     def subject(self, argv, stream=None):
         super().subject(argv)
         childlogger = logging.getLogger("streamlink.test_cli_main")
 
         streamlink_cli.main.log.info("foo")
         childlogger.error("baz")
@@ -690,15 +682,15 @@
     @patch("streamlink_cli.main.log")
     def test_log_root_warning(self, mock_log):
         self.subject(["streamlink"], euid=0)
         assert mock_log.info.mock_calls == [call("streamlink is running as root! Be careful!")]
 
     @patch("streamlink_cli.main.log")
     @patch("streamlink_cli.main.streamlink_version", "streamlink")
-    @patch("streamlink_cli.main.importlib_metadata")
+    @patch("streamlink_cli.main.importlib.metadata")
     @patch("streamlink_cli.main.log_current_arguments", Mock(side_effect=_TestCLIMainLogging.StopTest))
     @patch("platform.python_version", Mock(return_value="python"))
     def test_log_current_versions(self, mock_importlib_metadata: Mock, mock_log: Mock):
         class FakePackageNotFoundError(Exception):
             pass
 
         def version(dist):
```

### Comparing `streamlink-5.5.1/tests/cli/test_main_formatter.py` & `streamlink-6.0.0/tests/cli/test_main_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/cli/test_main_setup_config_args.py` & `streamlink-6.0.0/tests/cli/test_main_setup_config_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/cli/test_streamrunner.py` & `streamlink-6.0.0/tests/cli/test_streamrunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,17 @@
             return self._write(data)
 
     def _write(self, data):
         self.data.append(data)
 
 
 class FakePlayerOutput(FakeOutput, PlayerOutput):
-    pass
+    def open(self):
+        with patch("streamlink_cli.output.player.which", side_effect=lambda path: path):
+            return super().open()
 
 
 class FakeFileOutput(FakeOutput, FileOutput):
     pass
 
 
 class FakeHTTPOutput(FakeOutput, HTTPOutput):
@@ -159,15 +161,15 @@
         return player_process
 
     @pytest.fixture()
     def output(self, player_process: Mock):
         with patch("subprocess.Popen") as mock_popen, \
              patch("streamlink_cli.output.player.sleep"):
             mock_popen.return_value = player_process
-            output = FakePlayerOutput("mocked")
+            output = FakePlayerOutput(Path("mocked"))
             output.open()
             yield output
             output.close()
 
     @pytest.fixture()
     def stream_runner(self, stream: FakeStream, output: FakePlayerOutput):
         with patch("streamlink_cli.streamrunner.PlayerPollThread", EventedPlayerPollThread):
@@ -555,15 +557,15 @@
 
 
 class TestHasProgress:
     @pytest.mark.parametrize(
         "output",
         [
             pytest.param(
-                FakePlayerOutput("mocked"),
+                FakePlayerOutput(Path("mocked")),
                 id="Player output without record",
             ),
             pytest.param(
                 FakeFileOutput(fd=Mock()),
                 id="FileOutput with file descriptor",
             ),
             pytest.param(
@@ -579,15 +581,15 @@
         stream_runner = FakeStreamRunner(StreamIO(), output, show_progress=True)
         assert not stream_runner.progress
 
     @pytest.mark.parametrize(
         ("output", "expected"),
         [
             pytest.param(
-                FakePlayerOutput("mocked", record=FakeFileOutput(Path("record"))),
+                FakePlayerOutput(Path("mocked"), record=FakeFileOutput(Path("record"))),
                 Path("record"),
                 id="PlayerOutput with record",
             ),
             pytest.param(
                 FakeFileOutput(filename=Path("filename")),
                 Path("filename"),
                 id="FileOutput with file name",
```

### Comparing `streamlink-5.5.1/tests/cli/utils/test_formatter.py` & `streamlink-6.0.0/tests/cli/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/cli/utils/test_path.py` & `streamlink-6.0.0/tests/cli/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/cli/utils/test_progress.py` & `streamlink-6.0.0/tests/cli/utils/test_progress.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import sys
 from io import StringIO
-from pathlib import PurePosixPath, PureWindowsPath
+from pathlib import PurePath, PurePosixPath, PureWindowsPath
 from time import time
 from unittest.mock import Mock, call, patch
 
 import freezegun
 import pytest
 
 from streamlink_cli.utils.progress import Progress, ProgressFormatter
@@ -96,63 +97,97 @@
         (86399, "23h59m59s"),
         (86400, "24h00m00s"),
         (172800, "48h00m00s"),
     ])
     def test_format_time(self, elapsed, expected):
         assert ProgressFormatter.format_time(elapsed) == expected
 
-    _path_posix = PurePosixPath("/foobar/baz/some file name")
-    _path_windows_abs = PureWindowsPath("C:\\foobar\\baz\\some file name")
-    _path_windows_rel = PureWindowsPath("foobar\\baz\\some file name")
-    _path_windows_unc = PureWindowsPath("\\\\?\\foobar\\baz\\some file name")
-
-    @pytest.mark.parametrize(("path", "max_width", "expected"), [
-        pytest.param(_path_posix, 26, "/foobar/baz/some file name", id="posix - full path"),
-        pytest.param(_path_posix, 25, "…oobar/baz/some file name", id="posix - truncated by 1"),
-        pytest.param(_path_posix, 24, "…obar/baz/some file name", id="posix - truncated by 2"),
-        pytest.param(_path_posix, 23, "…bar/baz/some file name", id="posix - truncated by 3"),
-        pytest.param(_path_posix, 22, "…ar/baz/some file name", id="posix - truncated by 4"),
-        pytest.param(_path_posix, 21, "…r/baz/some file name", id="posix - truncated by 5"),
-        pytest.param(_path_posix, 20, "…/baz/some file name", id="posix - truncated by 6"),
-        pytest.param(_path_posix, 19, "…baz/some file name", id="posix - truncated by 7 (cuts off separator)"),
-        pytest.param(_path_posix, 16, "…/some file name", id="posix - truncated (all parts except name)"),
-        pytest.param(_path_posix, 15, "…some file name", id="posix - truncated (name without separator)"),
-        pytest.param(_path_posix, 14, "…ome file name", id="posix - truncated name"),
-        pytest.param(_path_windows_abs, 28, "C:\\foobar\\baz\\some file name", id="windows abs - full path"),
-        pytest.param(_path_windows_abs, 27, "C:…oobar\\baz\\some file name", id="windows abs - truncated by 1"),
-        pytest.param(_path_windows_abs, 26, "C:…obar\\baz\\some file name", id="windows abs - truncated by 2"),
-        pytest.param(_path_windows_abs, 25, "C:…bar\\baz\\some file name", id="windows abs - truncated by 3"),
-        pytest.param(_path_windows_abs, 24, "C:…ar\\baz\\some file name", id="windows abs - truncated by 4"),
-        pytest.param(_path_windows_abs, 23, "C:…r\\baz\\some file name", id="windows abs - truncated by 5"),
-        pytest.param(_path_windows_abs, 22, "C:…\\baz\\some file name", id="windows abs - truncated by 6"),
-        pytest.param(_path_windows_abs, 21, "C:…baz\\some file name", id="windows abs - truncated by 7 (cuts off separator)"),
-        pytest.param(_path_windows_abs, 18, "C:…\\some file name", id="windows abs - truncated (all parts except name)"),
-        pytest.param(_path_windows_abs, 17, "C:…some file name", id="windows abs - truncated (name without separator)"),
-        pytest.param(_path_windows_abs, 16, "C:…ome file name", id="windows abs - truncated name"),
-        pytest.param(_path_windows_rel, 25, "foobar\\baz\\some file name", id="windows rel - full path"),
-        pytest.param(_path_windows_rel, 24, "…obar\\baz\\some file name", id="windows rel - truncated by 1"),
-        pytest.param(_path_windows_rel, 23, "…bar\\baz\\some file name", id="windows rel - truncated by 2"),
-        pytest.param(_path_windows_rel, 22, "…ar\\baz\\some file name", id="windows rel - truncated by 3"),
-        pytest.param(_path_windows_rel, 21, "…r\\baz\\some file name", id="windows rel - truncated by 4"),
-        pytest.param(_path_windows_rel, 20, "…\\baz\\some file name", id="windows rel - truncated by 5"),
-        pytest.param(_path_windows_rel, 19, "…baz\\some file name", id="windows rel - truncated by 6 (cuts off separator)"),
-        pytest.param(_path_windows_rel, 16, "…\\some file name", id="windows rel - truncated (all parts except name)"),
-        pytest.param(_path_windows_rel, 15, "…some file name", id="windows rel - truncated (name without separator)"),
-        pytest.param(_path_windows_rel, 14, "…ome file name", id="windows rel - truncated name"),
-        pytest.param(_path_windows_unc, 29, "\\\\?\\foobar\\baz\\some file name", id="windows UNC - full path"),
-        pytest.param(_path_windows_unc, 28, "\\\\?\\…obar\\baz\\some file name", id="windows UNC - truncated by 1"),
-        pytest.param(_path_windows_unc, 20, "\\\\?\\…\\some file name", id="windows UNC - truncated (all parts except name)"),
-        pytest.param(_path_windows_unc, 19, "\\\\?\\…some file name", id="windows UNC - truncated (name without separator)"),
-        pytest.param(_path_windows_unc, 18, "\\\\?\\…ome file name", id="windows UNC - truncated name"),
-    ])
-    def test_format_path(self, path, max_width, expected):
+
+_PATH_POSIX = PurePosixPath("/foobar/baz/some file name")
+_PATH_WIN_ABS = PureWindowsPath("C:\\foobar\\baz\\some file name")
+_PATH_WIN_REL = PureWindowsPath("foobar\\baz\\some file name")
+_PATH_WIN_UNC = PureWindowsPath("\\\\?\\foobar\\baz\\some file name")
+
+
+class _TestFormatPath:
+    # noinspection PyMethodMayBeStatic
+    def test_format_path(self, path: PurePath, max_width: int, expected: str):
         with patch("os.path.sep", "\\" if type(path) is PureWindowsPath else "/"):
             assert ProgressFormatter.format_path(path, max_width) == expected
 
 
+@pytest.mark.parametrize(("path", "max_width", "expected"), [
+    pytest.param(_PATH_POSIX, 26, "/foobar/baz/some file name", id="full path"),
+    pytest.param(_PATH_POSIX, 25, "…oobar/baz/some file name", id="truncated by 1"),
+    pytest.param(_PATH_POSIX, 24, "…obar/baz/some file name", id="truncated by 2"),
+    pytest.param(_PATH_POSIX, 23, "…bar/baz/some file name", id="truncated by 3"),
+    pytest.param(_PATH_POSIX, 22, "…ar/baz/some file name", id="truncated by 4"),
+    pytest.param(_PATH_POSIX, 21, "…r/baz/some file name", id="truncated by 5"),
+    pytest.param(_PATH_POSIX, 20, "…/baz/some file name", id="truncated by 6"),
+    pytest.param(_PATH_POSIX, 19, "…baz/some file name", id="truncated by 7 (cuts off separator)"),
+    pytest.param(_PATH_POSIX, 16, "…/some file name", id="truncated (all parts except name)"),
+    pytest.param(_PATH_POSIX, 15, "…some file name", id="truncated (name without separator)"),
+    pytest.param(_PATH_POSIX, 14, "…ome file name", id="truncated name"),
+])
+class TestFormatPathPOSIX(_TestFormatPath):
+    pass
+
+
+@pytest.mark.parametrize(("path", "max_width", "expected"), [
+    pytest.param(_PATH_WIN_ABS, 28, "C:\\foobar\\baz\\some file name", id="full path"),
+    pytest.param(_PATH_WIN_ABS, 27, "C:…oobar\\baz\\some file name", id="truncated by 1"),
+    pytest.param(_PATH_WIN_ABS, 26, "C:…obar\\baz\\some file name", id="truncated by 2"),
+    pytest.param(_PATH_WIN_ABS, 25, "C:…bar\\baz\\some file name", id="truncated by 3"),
+    pytest.param(_PATH_WIN_ABS, 24, "C:…ar\\baz\\some file name", id="truncated by 4"),
+    pytest.param(_PATH_WIN_ABS, 23, "C:…r\\baz\\some file name", id="truncated by 5"),
+    pytest.param(_PATH_WIN_ABS, 22, "C:…\\baz\\some file name", id="truncated by 6"),
+    pytest.param(_PATH_WIN_ABS, 21, "C:…baz\\some file name", id="truncated by 7 (cuts off separator)"),
+    pytest.param(_PATH_WIN_ABS, 18, "C:…\\some file name", id="truncated (all parts except name)"),
+    pytest.param(_PATH_WIN_ABS, 17, "C:…some file name", id="truncated (name without separator)"),
+    pytest.param(_PATH_WIN_ABS, 16, "C:…ome file name", id="truncated name"),
+])
+class TestFormatPathWindowsAbsolute(_TestFormatPath):
+    pass
+
+
+@pytest.mark.parametrize(("path", "max_width", "expected"), [
+    pytest.param(_PATH_WIN_REL, 25, "foobar\\baz\\some file name", id="full path"),
+    pytest.param(_PATH_WIN_REL, 24, "…obar\\baz\\some file name", id="truncated by 1"),
+    pytest.param(_PATH_WIN_REL, 23, "…bar\\baz\\some file name", id="truncated by 2"),
+    pytest.param(_PATH_WIN_REL, 22, "…ar\\baz\\some file name", id="truncated by 3"),
+    pytest.param(_PATH_WIN_REL, 21, "…r\\baz\\some file name", id="truncated by 4"),
+    pytest.param(_PATH_WIN_REL, 20, "…\\baz\\some file name", id="truncated by 5"),
+    pytest.param(_PATH_WIN_REL, 19, "…baz\\some file name", id="truncated by 6 (cuts off separator)"),
+    pytest.param(_PATH_WIN_REL, 16, "…\\some file name", id="truncated (all parts except name)"),
+    pytest.param(_PATH_WIN_REL, 15, "…some file name", id="truncated (name without separator)"),
+    pytest.param(_PATH_WIN_REL, 14, "…ome file name", id="truncated name"),
+])
+class TestFormatPathWindowsRelative(_TestFormatPath):
+    pass
+
+
+@pytest.mark.parametrize(("path", "max_width", "expected"), [
+    # <py312: server/host name is not part of the path's drive, so it'll get truncated
+    pytest.param(_PATH_WIN_UNC, 29, "\\\\?\\foobar\\baz\\some file name", id="full path"),
+    pytest.param(_PATH_WIN_UNC, 28, "\\\\?\\…obar\\baz\\some file name", id="truncated by 1"),
+    pytest.param(_PATH_WIN_UNC, 20, "\\\\?\\…\\some file name", id="truncated (all parts except name)"),
+    pytest.param(_PATH_WIN_UNC, 19, "\\\\?\\…some file name", id="truncated (name without separator)"),
+    pytest.param(_PATH_WIN_UNC, 18, "\\\\?\\…ome file name", id="truncated name"),
+] if sys.version_info < (3, 12) else [
+    # >=py312: server/host name is part of the path's drive, so it won't get truncated
+    pytest.param(_PATH_WIN_UNC, 29, "\\\\?\\foobar\\baz\\some file name", id="full path"),
+    pytest.param(_PATH_WIN_UNC, 28, "\\\\?\\foobar…az\\some file name", id="truncated by 1"),
+    pytest.param(_PATH_WIN_UNC, 26, "\\\\?\\foobar…\\some file name", id="truncated (all parts except name)"),
+    pytest.param(_PATH_WIN_UNC, 25, "\\\\?\\foobar…some file name", id="truncated (name without separator)"),
+    pytest.param(_PATH_WIN_UNC, 24, "\\\\?\\foobar…ome file name", id="truncated name"),
+])
+class TestFormatPathWindowsUniversalNamingConvention(_TestFormatPath):
+    pass
+
+
 class TestWidth:
     @pytest.mark.parametrize(("chars", "expected"), [
         ("ABCDEFGHIJ", 10),
         ("A你好世界こんにちは안녕하세요B", 30),
         ("·「」『』【】-=！@#￥%……&×（）", 30),
     ])
     def test_width(self, chars, expected):
```

### Comparing `streamlink-5.5.1/tests/cli/utils/test_versioncheck.py` & `streamlink-6.0.0/tests/cli/utils/test_versioncheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 
 def test_logger_name():
     assert log.name == "streamlink.cli"
 
 
 class TestGetLatest:
     @pytest.fixture()
-    def pypi(self, request, requests_mock: rm.Mocker):
-        invalid = requests_mock.register_uri(rm.ANY, rm.ANY, exc=rm.exceptions.InvalidRequest("Invalid request"))
-        response = requests_mock.register_uri("GET", "https://pypi.python.org/pypi/streamlink/json", **(request.param or {}))
+    def pypi(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker):
+        response = requests_mock.register_uri(
+            "GET",
+            "https://pypi.python.org/pypi/streamlink/json",
+            **getattr(request, "param", {}),
+        )
         yield response
-        assert not invalid.called  # type: ignore[attr-defined]
-        assert response.called_once  # type: ignore[attr-defined]
+        assert response.call_count == 1
 
     @pytest.mark.parametrize(("pypi", "error"), [
         (
             {"status_code": 500},
             "Error while retrieving version data from PyPI API: "
             + "500 Server Error: None for url: https://pypi.python.org/pypi/streamlink/json",
         ),
@@ -57,21 +59,21 @@
     @pytest.fixture()
     def latest(self, request, monkeypatch: pytest.MonkeyPatch):
         mock_get_latest = Mock(return_value=getattr(request, "param", "1.2.3"))
         monkeypatch.setattr("streamlink_cli.utils.versioncheck.get_latest", mock_get_latest)
         return mock_get_latest
 
     @pytest.fixture()
-    def cache(self, request, monkeypatch: pytest.MonkeyPatch):
-        Cache = Mock()
-        cache = Cache("cli.json")
-        cache.get.side_effect = request.param.get
-        monkeypatch.setattr("streamlink_cli.utils.versioncheck.Cache", Cache)
-        yield cache
-        assert cache.called_once
+    def cache(self, request: pytest.FixtureRequest, monkeypatch: pytest.MonkeyPatch):
+        mock_cache = Mock()
+        mock_cache.get.side_effect = getattr(request, "param", {}).get
+        MockCache = Mock(return_value=mock_cache)
+        monkeypatch.setattr("streamlink_cli.utils.versioncheck.Cache", MockCache)
+        yield mock_cache
+        assert MockCache.call_args_list == [call(filename="cli.json")]
 
     @pytest.mark.parametrize("cache", [{}], indirect=True)
     def test_auto_uncached_outdated(self, caplog: pytest.LogCaptureFixture, cache: Mock, latest: Mock):
         assert not check_version()
         assert latest.call_args_list == [call()]
         assert cache.set.call_args_list == [
             call("latest_version", "1.2.3", 86400),
```

### Comparing `streamlink-5.5.1/tests/conftest.py` & `streamlink-6.0.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
-from typing import Dict, List, Tuple
+from typing import Dict, Iterator, List, Tuple
 from unittest.mock import patch
 
 import pytest
+import requests_mock as rm
 
 from streamlink.session import Streamlink
 
 
 _TEST_CONDITION_MARKERS: Dict[str, Tuple[bool, str]] = {
     "posix_only": (os.name == "posix", "only applicable on a POSIX OS"),
     "windows_only": (os.name == "nt", "only applicable on Windows"),
@@ -61,13 +62,24 @@
 
 # ========================
 # globally shared fixtures
 # ========================
 
 
 @pytest.fixture()
-def session(request: pytest.FixtureRequest) -> Streamlink:
+def session(request: pytest.FixtureRequest) -> Iterator[Streamlink]:
     with patch.object(Streamlink, "load_builtin_plugins"):
         session = Streamlink()
         for key, value in getattr(request, "param", {}).items():
             session.set_option(key, value)
-        return session
+        yield session
+
+    Streamlink.resolve_url.cache_clear()
+
+
+@pytest.fixture()
+def requests_mock(requests_mock: rm.Mocker) -> rm.Mocker:  # noqa: PT004
+    """
+    Override of the default `requests_mock` fixture, with `InvalidRequest` raised on unknown requests
+    """
+    requests_mock.register_uri(rm.ANY, rm.ANY, exc=rm.exceptions.InvalidRequest)
+    return requests_mock
```

### Comparing `streamlink-5.5.1/tests/mixins/stream_hls.py` & `streamlink-6.0.0/tests/mixins/stream_hls.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         self.mocks[url] = self.mocker.request(method, url, *args, **kwargs)
 
     def get_mock(self, item):
         return self.mocks[self.url(item)]
 
     def called(self, item, once=False):
         mock = self.get_mock(item)
-        return mock.called_once if once else mock.called
+        return mock.call_count == 1 if once else mock.called
 
     def url(self, item):
         return item.url(self.id())
 
     @staticmethod
     def content(segments, prop="content", cond=None):
         if isinstance(segments, dict):
```

### Comparing `streamlink-5.5.1/tests/plugin/testplugin.py` & `streamlink-6.0.0/tests/plugin/testplugin.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/__init__.py` & `streamlink-6.0.0/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/conftest.py` & `streamlink-6.0.0/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_abematv.py` & `streamlink-6.0.0/tests/plugins/test_abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_adultswim.py` & `streamlink-6.0.0/tests/plugins/test_adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_afreeca.py` & `streamlink-6.0.0/tests/plugins/test_afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_albavision.py` & `streamlink-6.0.0/tests/plugins/test_albavision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import unittest
-
 from streamlink.plugins.albavision import Albavision
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlAlbavision(PluginCanHandleUrl):
     __plugin__ = Albavision
 
@@ -51,11 +49,11 @@
         "https://www.antena7.com.do/envivo-canal-abc",
         "https://www.antena7.com.do/envivo-canal-7/extra",
         "https://www.antena7.com.do/envivo-canal-7#extra",
         "https://www.antena7.com.do/something",
     ]
 
 
-class TestPluginAlbavision(unittest.TestCase):
+class TestPluginAlbavision:
     def test_transform(self):
         token = Albavision.transform_token("6b425761cc8a86569b1a05a9bf1870c95fca717dOK", 436171)
         assert token == "6b425761cc8a86569b1a05a9bf1870c95fca717d"
```

### Comparing `streamlink-5.5.1/tests/plugins/test_aloula.py` & `streamlink-6.0.0/tests/plugins/test_aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_ard_mediathek.py` & `streamlink-6.0.0/tests/plugins/test_ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_artetv.py` & `streamlink-6.0.0/tests/plugins/test_artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_atpchallenger.py` & `streamlink-6.0.0/tests/plugins/test_atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_atresplayer.py` & `streamlink-6.0.0/tests/plugins/test_atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_bbciplayer.py` & `streamlink-6.0.0/tests/plugins/test_bbciplayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import unittest
-
 from streamlink.plugins.bbciplayer import BBCiPlayer
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlBBCiPlayer(PluginCanHandleUrl):
     __plugin__ = BBCiPlayer
 
@@ -13,10 +11,10 @@
     ]
 
     should_not_match = [
         "http://www.bbc.co.uk/iplayer/",
     ]
 
 
-class TestPluginBBCiPlayer(unittest.TestCase):
+class TestPluginBBCiPlayer:
     def test_vpid_hash(self):
         assert BBCiPlayer._hash_vpid("1234567890") == "71c345435589c6ddeea70d6f252e2a52281ecbf3"
```

### Comparing `streamlink-5.5.1/tests/plugins/test_bfmtv.py` & `streamlink-6.0.0/tests/plugins/test_bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_bigo.py` & `streamlink-6.0.0/tests/plugins/test_bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_blazetv.py` & `streamlink-6.0.0/tests/plugins/test_blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_bloomberg.py` & `streamlink-6.0.0/tests/plugins/test_bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_booyah.py` & `streamlink-6.0.0/tests/plugins/test_booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_cbsnews.py` & `streamlink-6.0.0/tests/plugins/test_cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_cdnbg.py` & `streamlink-6.0.0/tests/plugins/test_cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_ceskatelevize.py` & `streamlink-6.0.0/tests/plugins/test_ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_cinergroup.py` & `streamlink-6.0.0/tests/plugins/test_cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_cmmedia.py` & `streamlink-6.0.0/tests/plugins/test_cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_crunchyroll.py` & `streamlink-6.0.0/tests/plugins/test_crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_dailymotion.py` & `streamlink-6.0.0/tests/plugins/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_dash.py` & `streamlink-6.0.0/tests/plugins/test_dash.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,48 @@
-import unittest
-from unittest.mock import Mock, patch
+from unittest.mock import Mock, call
 
 import pytest
 
 from streamlink.plugin.plugin import BIT_RATE_WEIGHT_RATIO, LOW_PRIORITY, NO_PRIORITY, NORMAL_PRIORITY
 from streamlink.plugins.dash import MPEGDASH
+from streamlink.session import Streamlink
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlMPEGDASH(PluginCanHandleUrl):
     __plugin__ = MPEGDASH
 
-    should_match = [
-        "example.com/foo.mpd",
-        "http://example.com/foo.mpd",
-        "https://example.com/foo.mpd",
-        "dash://example.com/foo",
-        "dash://http://example.com/foo",
-        "dash://https://example.com/foo",
+    should_match_groups = [
+        # implicit DASH URLs
+        ("example.com/foo.mpd", {"url": "example.com/foo.mpd"}),
+        ("example.com/foo.mpd?bar", {"url": "example.com/foo.mpd?bar"}),
+        ("http://example.com/foo.mpd", {"url": "http://example.com/foo.mpd"}),
+        ("http://example.com/foo.mpd?bar", {"url": "http://example.com/foo.mpd?bar"}),
+        ("https://example.com/foo.mpd", {"url": "https://example.com/foo.mpd"}),
+        ("https://example.com/foo.mpd?bar", {"url": "https://example.com/foo.mpd?bar"}),
+        # explicit DASH URLs with protocol prefix
+        ("dash://example.com/foo?bar", {"url": "example.com/foo?bar"}),
+        ("dash://http://example.com/foo?bar", {"url": "http://example.com/foo?bar"}),
+        ("dash://https://example.com/foo?bar", {"url": "https://example.com/foo?bar"}),
+        # optional parameters
+        ("example.com/foo.mpd?bar abc=def", {"url": "example.com/foo.mpd?bar", "params": "abc=def"}),
+        ("http://example.com/foo.mpd?bar abc=def", {"url": "http://example.com/foo.mpd?bar", "params": "abc=def"}),
+        ("https://example.com/foo.mpd?bar abc=def", {"url": "https://example.com/foo.mpd?bar", "params": "abc=def"}),
+        ("dash://https://example.com/foo?bar abc=def", {"url": "https://example.com/foo?bar", "params": "abc=def"}),
+    ]
+
+    should_not_match = [
+        # implicit DASH URLs must have their path end with ".mpd"
+        "example.com/mpd",
+        "example.com/mpd abc=def",
+        "example.com/foo.mpd,bar",
+        "example.com/foo.mpd,bar abc=def",
+        # missing parameters
+        "example.com/foo.mpd ",
+        "dash://example.com/foo ",
     ]
 
 
 @pytest.mark.parametrize(("url", "priority"), [
     ("http://example.com/foo.mpd", LOW_PRIORITY),
     ("dash://http://example.com/foo.mpd", NORMAL_PRIORITY),
     ("dash://http://example.com/bar", NORMAL_PRIORITY),
@@ -35,22 +56,26 @@
     ("example.com/foo.mpd", "https://example.com/foo.mpd"),
     ("http://example.com/foo.mpd", "http://example.com/foo.mpd"),
     ("https://example.com/foo.mpd", "https://example.com/foo.mpd"),
     ("dash://example.com/foo", "https://example.com/foo"),
     ("dash://http://example.com/foo", "http://example.com/foo"),
     ("dash://https://example.com/foo", "https://example.com/foo"),
 ])
-@patch("streamlink.stream.DASHStream.parse_manifest")
-def test_get_streams(parse_manifest, url, expected):
-    session = Mock()
+def test_get_streams(monkeypatch: pytest.MonkeyPatch, session: Streamlink, url, expected):
+    mock_parse_manifest = Mock(return_value={})
+    monkeypatch.setattr("streamlink.stream.dash.DASHStream.parse_manifest", mock_parse_manifest)
+
     p = MPEGDASH(session, url)
     p.streams()
-    parse_manifest.assert_called_with(session, expected)
 
+    assert mock_parse_manifest.call_args_list == [call(session, expected)]
 
-class TestPluginMPEGDASH(unittest.TestCase):
-    def test_stream_weight(self):
-        assert MPEGDASH.stream_weight("720p") == pytest.approx((720, "pixels"))
-        assert MPEGDASH.stream_weight("1080p") == pytest.approx((1080, "pixels"))
-        assert MPEGDASH.stream_weight("720p+a128k") == pytest.approx((720 + 128, "pixels"))
-        assert MPEGDASH.stream_weight("720p+a0k") == pytest.approx((720, "pixels"))
-        assert MPEGDASH.stream_weight("a128k") == pytest.approx((128 / BIT_RATE_WEIGHT_RATIO, "bitrate"))
+
+@pytest.mark.parametrize(("weight", "expected"), [
+    ("720p", pytest.approx((720, "pixels"))),
+    ("1080p", pytest.approx((1080, "pixels"))),
+    ("720p+a128k", pytest.approx((720 + 128, "pixels"))),
+    ("720p+a0k", pytest.approx((720, "pixels"))),
+    ("a128k", pytest.approx((128 / BIT_RATE_WEIGHT_RATIO, "bitrate"))),
+])
+def test_stream_weight(weight: str, expected):
+    assert MPEGDASH.stream_weight(weight) == expected
```

### Comparing `streamlink-5.5.1/tests/plugins/test_delfi.py` & `streamlink-6.0.0/tests/plugins/test_delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_deutschewelle.py` & `streamlink-6.0.0/tests/plugins/test_deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_dogan.py` & `streamlink-6.0.0/tests/plugins/test_dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_drdk.py` & `streamlink-6.0.0/tests/plugins/test_drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_euronews.py` & `streamlink-6.0.0/tests/plugins/test_euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_facebook.py` & `streamlink-6.0.0/tests/plugins/test_facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_filmon.py` & `streamlink-6.0.0/tests/plugins/test_filmon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_goltelevision.py` & `streamlink-6.0.0/tests/plugins/test_goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_gulli.py` & `streamlink-6.0.0/tests/plugins/test_gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_htv.py` & `streamlink-6.0.0/tests/plugins/test_htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_idf1.py` & `streamlink-6.0.0/tests/plugins/test_idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_invintus.py` & `streamlink-6.0.0/tests/plugins/test_invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_kugou.py` & `streamlink-6.0.0/tests/plugins/test_kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_livestream.py` & `streamlink-6.0.0/tests/plugins/test_livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_lnk.py` & `streamlink-6.0.0/tests/plugins/test_lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_lrt.py` & `streamlink-6.0.0/tests/plugins/test_lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_ltv_lsm_lv.py` & `streamlink-6.0.0/tests/plugins/test_ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_mdstrm.py` & `streamlink-6.0.0/tests/plugins/test_mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_mediaklikk.py` & `streamlink-6.0.0/tests/plugins/test_mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_mediavitrina.py` & `streamlink-6.0.0/tests/plugins/test_mediavitrina.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "https://player.mediavitrina.ru/russia1/moretv_web/player.html",
         "https://player.mediavitrina.ru/russia24/moretv_web/player.html",
         "https://player.mediavitrina.ru/russia24/vesti_ru_web/player.html?id",
         "https://player.mediavitrina.ru/spas/moretv_web/player.html",
         "https://player.mediavitrina.ru/tvc/tvc/moretv_web/player.html",
         "https://player.mediavitrina.ru/tvzvezda/moretv_web/player.html",
         "https://player.mediavitrina.ru/u_ott/u/moretv_web/player.html",
+        "https://player.mediavitrina.ru/gpm_tnt_v2/tnt/vitrinatv_web/player.html",
     ]
 
     should_not_match = [
         "https://1tv.ru/live",
         "https://ren.tv/live",
         "https://www.5-tv.ru/live/",
         "https://www.5-tv.ru/online/",
```

### Comparing `streamlink-5.5.1/tests/plugins/test_mitele.py` & `streamlink-6.0.0/tests/plugins/test_mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_mixcloud.py` & `streamlink-6.0.0/tests/plugins/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_n13tv.py` & `streamlink-6.0.0/tests/plugins/test_n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_nicolive.py` & `streamlink-6.0.0/tests/plugins/test_nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_nos.py` & `streamlink-6.0.0/tests/plugins/test_nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_nrk.py` & `streamlink-6.0.0/tests/plugins/test_nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_olympicchannel.py` & `streamlink-6.0.0/tests/plugins/test_olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_oneplusone.py` & `streamlink-6.0.0/tests/plugins/test_oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_onetv.py` & `streamlink-6.0.0/tests/plugins/test_onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_pandalive.py` & `streamlink-6.0.0/tests/plugins/test_pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_picarto.py` & `streamlink-6.0.0/tests/plugins/test_picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_pluto.py` & `streamlink-6.0.0/tests/plugins/test_pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_pluzz.py` & `streamlink-6.0.0/tests/plugins/test_pluzz.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,15 @@
     should_match = [
         "https://www.france.tv/france-2/direct.html",
         "https://www.france.tv/france-3/direct.html",
         "https://www.france.tv/france-4/direct.html",
         "https://www.france.tv/france-5/direct.html",
         "https://www.france.tv/franceinfo/direct.html",
         "https://www.france.tv/france-2/journal-20h00/141003-edition-du-lundi-8-mai-2017.html",
-        "https://france3-regions.francetvinfo.fr/bourgogne-franche-comte/tv/direct/franche-comte",
+        "https://france3-regions.francetvinfo.fr/bourgogne-franche-comte/direct/franche-comte",
         "https://www.francetvinfo.fr/en-direct/tv.html",
         "https://www.francetvinfo.fr/meteo/orages/inondations-dans-le-gard-plus-de-deux-mois-de-pluie-en-quelques-heures-des"
         + "-degats-mais-pas-de-victime_4771265.html",
+        "https://la1ere.francetvinfo.fr/info-en-continu-24-24",
+        "https://la1ere.francetvinfo.fr/programme-video/france-3_outremer-ledoc/diffusion/"
+        + "2958951-polynesie-les-sages-de-l-ocean.html",
     ]
```

### Comparing `streamlink-5.5.1/tests/plugins/test_radionet.py` & `streamlink-6.0.0/tests/plugins/test_radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_raiplay.py` & `streamlink-6.0.0/tests/plugins/test_raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_reuters.py` & `streamlink-6.0.0/tests/plugins/test_reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_rtbf.py` & `streamlink-6.0.0/tests/plugins/test_rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_rtpplay.py` & `streamlink-6.0.0/tests/plugins/test_rtpplay.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import unittest
-
 import requests_mock
 
 from streamlink import Streamlink
 from streamlink.plugins.rtpplay import RTPPlay
 from streamlink.stream.hls import HLSStream
 from tests.plugins import PluginCanHandleUrl
 from tests.resources import text
@@ -23,15 +21,15 @@
         "https://www.rtp.pt/programa/",
         "http://www.rtp.pt/programa/",
         "https://media.rtp.pt/",
         "http://media.rtp.pt/",
     ]
 
 
-class TestRTPPlay(unittest.TestCase):
+class TestRTPPlay:
     # all invalid HLS URLs at the beginning need to be ignored ("https://invalid")
     _content_pre = """
         /*  var player1 = new RTPPlayer({
                 file: {hls : atob( decodeURIComponent(["aHR0c", "HM6Ly", "9pbnZ", "hbGlk"].join("") ) ), dash : foo() } }); */
         var f = {hls : atob( decodeURIComponent(["aHR0c", "HM6Ly", "9pbnZ", "hbGlk"].join("") ) ), dash: foo() };
     """
     # invalid resources sometimes have an empty string as HLS URL
```

### Comparing `streamlink-5.5.1/tests/plugins/test_rtve.py` & `streamlink-6.0.0/tests/plugins/test_rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_ruv.py` & `streamlink-6.0.0/tests/plugins/test_ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_sbscokr.py` & `streamlink-6.0.0/tests/plugins/test_sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_showroom.py` & `streamlink-6.0.0/tests/plugins/test_showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_steam.py` & `streamlink-6.0.0/tests/plugins/test_steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_streann.py` & `streamlink-6.0.0/tests/plugins/test_streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_svtplay.py` & `streamlink-6.0.0/tests/plugins/test_svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_swisstxt.py` & `streamlink-6.0.0/tests/plugins/test_swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_telefe.py` & `streamlink-6.0.0/tests/plugins/test_telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_tf1.py` & `streamlink-6.0.0/tests/plugins/test_tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_trovo.py` & `streamlink-6.0.0/tests/plugins/test_trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_turkuvaz.py` & `streamlink-6.0.0/tests/plugins/test_turkuvaz.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,39 @@
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlTurkuvaz(PluginCanHandleUrl):
     __plugin__ = Turkuvaz
 
     should_match = [
-        "https://www.ahaber.com.tr/video/canli-yayin",
-        "https://www.ahaber.com.tr/webtv/canli-yayin",
-        "https://www.anews.com.tr/webtv/live-broadcast",
-        "https://www.apara.com.tr/canli-yayin",
-        "https://www.aspor.com.tr/webtv/canli-yayin",
-        "https://www.atv.com.tr/canli-yayin",
-        "https://www.atv.com.tr/a2tv/canli-yayin",
-        "https://www.atv.com.tr/webtv/canli-yayin",
-        "https://www.atvavrupa.tv/webtv/canli-yayin",
-        "https://www.minikacocuk.com.tr/webtv/canli-yayin",
-        "https://www.minikago.com.tr/webtv/canli-yayin",
-        "https://www.vavtv.com.tr/canli-yayin",
+        # canonical live links
+        "https://www.ahaber.com.tr/video/canli-yayin",  # ahbr
+        "https://www.ahaber.com.tr/canli-yayin-aspor.html",  # ahbr: aspor
+        "https://www.ahaber.com.tr/canli-yayin-anews.html",  # ahbr: anews
+        "https://www.ahaber.com.tr/canli-yayin-a2tv.html",  # ahbr: a2tv
+        "https://www.ahaber.com.tr/canli-yayin-minikago.html",  # ahbr: minika go
+        "https://www.ahaber.com.tr/canli-yayin-minikacocuk.html",  # ahbr: minika cocuk
+        "https://www.anews.com.tr/webtv/live-broadcast",  # anews
+        "https://www.apara.com.tr/canli-yayin",  # apara
+        "https://www.aspor.com.tr/webtv/canli-yayin",  # aspor
+        "https://www.atv.com.tr/canli-yayin",  # atv
+        "https://www.atv.com.tr/a2tv/canli-yayin",  # a2tv
+        "https://www.atvavrupa.tv/canli-yayin",  # atvavrupa
+        "https://www.minikacocuk.com.tr/webtv/canli-yayin",  # minika cocuk
+        "https://www.minikago.com.tr/webtv/canli-yayin",  # minika go
+        "https://vavtv.com.tr/canli-yayin",  # vavtv
+
+        # vods
+        "https://www.ahaber.com.tr/video/yasam-videolari/samsunda-sel-sularindan-kacma-ani-kamerada",
+        "https://www.anews.com.tr/webtv/world/pro-ukraine-militia-says-it-has-captured-russian-soldiers",
+        "https://www.apara.com.tr/video/ekonomide-bugun/bist-100de-kar-satislari-derinlesir-mi",
+        "https://www.aspor.com.tr/webtv/galatasaray/galatasaraydan-forma-tanitiminda-fenerbahceye-gonderme",
+        "https://www.atv.com.tr/kurulus-osman/127-bolum/izle",
+        "https://www.atvavrupa.tv/diger-program//ozelvideo/izle",
+        "https://www.minikacocuk.com.tr/webtv/olly/bolum/olly-eylul-tanitim",
+        "https://www.minikago.com.tr/webtv/mondo-yan/bolum/mondo-yan-eylul-tanitim",
+        "https://vavtv.com.tr/vavradyo/video/guncel/munafiklarin-ozellikleri-nelerdir",
+
+        # other links for info/doc
+        "https://www.atv.com.tr/webtv/canli-yayin",  # redirect to atv.com.tr/canli-yayin
+        "https://www.ahaber.com.tr/canli-yayin-atv.html",  # links to atv.com.tr/webtv/canli-yayin
     ]
```

### Comparing `streamlink-5.5.1/tests/plugins/test_tv4play.py` & `streamlink-6.0.0/tests/plugins/test_tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_tv5monde.py` & `streamlink-6.0.0/tests/plugins/test_tv5monde.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_tvp.py` & `streamlink-6.0.0/tests/plugins/test_tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_tvrby.py` & `streamlink-6.0.0/tests/plugins/test_tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_tvrplus.py` & `streamlink-6.0.0/tests/plugins/test_tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_twitch.py` & `streamlink-6.0.0/tests/plugins/test_twitch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import unittest
 from datetime import datetime, timedelta, timezone
-from unittest.mock import MagicMock, call, patch
+from unittest.mock import MagicMock, Mock, call, patch
 
 import pytest
-import requests_mock
+import requests_mock as rm
 
 from streamlink import Streamlink
-from streamlink.exceptions import NoStreamsError
+from streamlink.exceptions import NoStreamsError, PluginError
+from streamlink.options import Options
 from streamlink.plugins.twitch import Twitch, TwitchAPI, TwitchHLSStream, TwitchHLSStreamReader, TwitchHLSStreamWriter
 from tests.mixins.stream_hls import EventedHLSStreamWriter, Playlist, Segment as _Segment, Tag, TestMixinStreamHLS
 from tests.plugins import PluginCanHandleUrl
 from tests.resources import text
 
 
 class TestPluginCanHandleUrlTwitch(PluginCanHandleUrl):
@@ -94,56 +95,55 @@
     __writer__ = _TwitchHLSStreamWriter
 
 
 class _TwitchHLSStream(TwitchHLSStream):
     __reader__ = _TwitchHLSStreamReader
 
 
-def test_stream_weight():
+def test_stream_weight(requests_mock: rm.Mocker):
     session = Streamlink()
     plugin = Twitch(session, "http://twitch.tv/foo")
 
     with text("hls/test_master_twitch_vod.m3u8") as fh:
         playlist = fh.read()
-    with requests_mock.Mocker() as mocker:
-        mocker.register_uri(requests_mock.ANY, requests_mock.ANY, exc=requests_mock.exceptions.InvalidRequest)
-        mocker.request(method="GET", url="http://mocked/master.m3u8", text=playlist)
-        streams = TwitchHLSStream.parse_variant_playlist(session, "http://mocked/master.m3u8")
+
+    requests_mock.request(method="GET", url="http://mocked/master.m3u8", text=playlist)
+    streams = TwitchHLSStream.parse_variant_playlist(session, "http://mocked/master.m3u8")
+
     with patch.object(plugin, "_get_streams", return_value=streams):
         data = plugin.streams()
 
     assert list(data.keys()) == ["audio", "160p30", "360p30", "480p30", "720p30", "720p60", "source", "worst", "best"]
     assert data["best"] is data["source"]
     assert data["worst"] is data["160p30"]
 
 
 @patch("streamlink.stream.hls.HLSStreamWorker.wait", MagicMock(return_value=True))
 class TestTwitchHLSStream(TestMixinStreamHLS, unittest.TestCase):
     __stream__ = _TwitchHLSStream
+    stream: TwitchHLSStream
 
-    def get_session(self, options=None, disable_ads=False, low_latency=False):
-        session = super().get_session(options)
+    def get_session(self, *args, **kwargs):
+        session = super().get_session(*args, **kwargs)
         session.set_option("hls-live-edge", 4)
-        session.set_plugin_option("twitch", "disable-ads", disable_ads)
-        session.set_plugin_option("twitch", "low-latency", low_latency)
 
         return session
 
     def test_hls_disable_ads_daterange_unknown(self):
         daterange = TagDateRangeAd(
             start=DATETIME_BASE,
             duration=1,
             attrid="foo",
             classname="bar",
             custom=None,
         )
 
         thread, segments = self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1)], end=True),
-        ], disable_ads=True, low_latency=False)
+        ], streamoptions={"disable_ads": True, "low_latency": False})
 
         self.await_write(2)
         data = self.await_read(read_all=True)
         assert data == self.content(segments), "Doesn't filter out segments"
         assert all(self.called(s) for s in segments.values()), "Downloads all segments"
 
     def test_hls_disable_ads_daterange_by_class(self):
@@ -153,15 +153,15 @@
             attrid="foo",
             classname="twitch-stitched-ad",
             custom=None,
         )
 
         thread, segments = self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1)], end=True),
-        ], disable_ads=True, low_latency=False)
+        ], streamoptions={"disable_ads": True, "low_latency": False})
 
         self.await_write(2)
         data = self.await_read(read_all=True)
         assert data == segments[1].content, "Filters out ad segments"
         assert all(self.called(s) for s in segments.values()), "Downloads all segments"
 
     def test_hls_disable_ads_daterange_by_id(self):
@@ -171,15 +171,15 @@
             attrid="stitched-ad-1234",
             classname="/",
             custom=None,
         )
 
         thread, segments = self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1)], end=True),
-        ], disable_ads=True, low_latency=False)
+        ], streamoptions={"disable_ads": True, "low_latency": False})
 
         self.await_write(2)
         data = self.await_read(read_all=True)
         assert data == segments[1].content, "Filters out ad segments"
         assert all(self.called(s) for s in segments.values()), "Downloads all segments"
 
     def test_hls_disable_ads_daterange_by_attr(self):
@@ -189,29 +189,29 @@
             attrid="foo",
             classname="/",
             custom={"X-TV-TWITCH-AD-URL": "/"},
         )
 
         thread, segments = self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1)], end=True),
-        ], disable_ads=True, low_latency=False)
+        ], streamoptions={"disable_ads": True, "low_latency": False})
 
         self.await_write(2)
         data = self.await_read(read_all=True)
         assert data == segments[1].content, "Filters out ad segments"
         assert all(self.called(s) for s in segments.values()), "Downloads all segments"
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_disable_ads_has_preroll(self, mock_log):
         daterange = TagDateRangeAd(duration=4)
         thread, segments = self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1)]),
             Playlist(2, [daterange, Segment(2), Segment(3)]),
             Playlist(4, [Segment(4), Segment(5)], end=True),
-        ], disable_ads=True, low_latency=False)
+        ], streamoptions={"disable_ads": True, "low_latency": False})
 
         self.await_write(6)
         data = self.await_read(read_all=True)
         assert data == self.content(segments, cond=lambda s: s.num >= 4), "Filters out preroll ad segments"
         assert all(self.called(s) for s in segments.values()), "Downloads all segments"
         assert mock_log.info.mock_calls == [
             call("Will skip ad segments"),
@@ -221,15 +221,15 @@
     @patch("streamlink.plugins.twitch.log")
     def test_hls_disable_ads_has_midstream(self, mock_log):
         daterange = TagDateRangeAd(start=DATETIME_BASE + timedelta(seconds=2), duration=2)
         thread, segments = self.subject([
             Playlist(0, [Segment(0), Segment(1)]),
             Playlist(2, [daterange, Segment(2), Segment(3)]),
             Playlist(4, [Segment(4), Segment(5)], end=True),
-        ], disable_ads=True, low_latency=False)
+        ], streamoptions={"disable_ads": True, "low_latency": False})
 
         self.await_write(6)
         data = self.await_read(read_all=True)
         assert data == self.content(segments, cond=lambda s: s.num != 2 and s.num != 3), "Filters out mid-stream ad segments"
         assert all(self.called(s) for s in segments.values()), "Downloads all segments"
         assert mock_log.info.mock_calls == [
             call("Will skip ad segments"),
@@ -237,28 +237,28 @@
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_no_disable_ads_has_preroll(self, mock_log):
         daterange = TagDateRangeAd(duration=2)
         thread, segments = self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1)]),
             Playlist(2, [Segment(2), Segment(3)], end=True),
-        ], disable_ads=False, low_latency=False)
+        ], streamoptions={"disable_ads": False, "low_latency": False})
 
         self.await_write(4)
         data = self.await_read(read_all=True)
         assert data == self.content(segments), "Doesn't filter out segments"
         assert all(self.called(s) for s in segments.values()), "Downloads all segments"
         assert mock_log.info.mock_calls == [], "Doesn't log anything"
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_low_latency_has_prefetch(self, mock_log):
         thread, segments = self.subject([
             Playlist(0, [Segment(0), Segment(1), Segment(2), Segment(3), SegmentPrefetch(4), SegmentPrefetch(5)]),
             Playlist(4, [Segment(4), Segment(5), Segment(6), Segment(7), SegmentPrefetch(8), SegmentPrefetch(9)], end=True),
-        ], disable_ads=False, low_latency=True)
+        ], streamoptions={"disable_ads": False, "low_latency": True})
 
         assert self.session.options.get("hls-live-edge") == 2
         assert self.session.options.get("hls-segment-stream-data")
 
         self.await_write(6)
         data = self.await_read(read_all=True)
         assert data == self.content(segments, cond=lambda s: s.num >= 4), "Skips first four segments due to reduced live-edge"
@@ -269,15 +269,15 @@
         ]
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_no_low_latency_has_prefetch(self, mock_log):
         thread, segments = self.subject([
             Playlist(0, [Segment(0), Segment(1), Segment(2), Segment(3), SegmentPrefetch(4), SegmentPrefetch(5)]),
             Playlist(4, [Segment(4), Segment(5), Segment(6), Segment(7), SegmentPrefetch(8), SegmentPrefetch(9)], end=True),
-        ], disable_ads=False, low_latency=False)
+        ], streamoptions={"disable_ads": False, "low_latency": False})
 
         assert self.session.options.get("hls-live-edge") == 4
         assert not self.session.options.get("hls-segment-stream-data")
 
         self.await_write(8)
         data = self.await_read(read_all=True)
         assert data == self.content(segments, cond=lambda s: s.num < 8), "Ignores prefetch segments"
@@ -286,48 +286,48 @@
         assert mock_log.info.mock_calls == [], "Doesn't log anything"
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_low_latency_no_prefetch(self, mock_log):
         self.subject([
             Playlist(0, [Segment(0), Segment(1), Segment(2), Segment(3)]),
             Playlist(4, [Segment(4), Segment(5), Segment(6), Segment(7)], end=True),
-        ], disable_ads=False, low_latency=True)
+        ], streamoptions={"disable_ads": False, "low_latency": True})
 
-        assert self.session.get_plugin_option("twitch", "low-latency")
-        assert not self.session.get_plugin_option("twitch", "disable-ads")
+        assert not self.stream.disable_ads
+        assert self.stream.low_latency
 
         self.await_write(6)
         self.await_read(read_all=True)
         assert mock_log.info.mock_calls == [
             call("Low latency streaming (HLS live edge: 2)"),
             call("This is not a low latency stream"),
         ]
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_low_latency_has_prefetch_has_preroll(self, mock_log):
         daterange = TagDateRangeAd(duration=4)
         thread, segments = self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1), Segment(2), Segment(3)]),
             Playlist(4, [Segment(4), Segment(5), Segment(6), Segment(7), SegmentPrefetch(8), SegmentPrefetch(9)], end=True),
-        ], disable_ads=False, low_latency=True)
+        ], streamoptions={"disable_ads": False, "low_latency": True})
 
         self.await_write(8)
         data = self.await_read(read_all=True)
         assert data == self.content(segments, cond=lambda s: s.num > 1), "Skips first two segments due to reduced live-edge"
         assert not any(self.called(s) for s in segments.values() if s.num < 2), "Skips first two preroll segments"
         assert all(self.called(s) for s in segments.values() if s.num >= 2), "Downloads all remaining segments"
         assert mock_log.info.mock_calls == [call("Low latency streaming (HLS live edge: 2)")]
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_low_latency_has_prefetch_disable_ads_has_preroll(self, mock_log):
         daterange = TagDateRangeAd(duration=4)
         self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1), Segment(2), Segment(3)]),
             Playlist(4, [Segment(4), Segment(5), Segment(6), Segment(7), SegmentPrefetch(8), SegmentPrefetch(9)], end=True),
-        ], disable_ads=True, low_latency=True)
+        ], streamoptions={"disable_ads": True, "low_latency": True})
 
         self.await_write(8)
         self.await_read(read_all=True)
         assert mock_log.info.mock_calls == [
             call("Will skip ad segments"),
             call("Low latency streaming (HLS live edge: 2)"),
             call("Waiting for pre-roll ads to finish, be patient"),
@@ -353,15 +353,15 @@
             # still no prefetch segments while ads are playing
             Playlist(3, ads + [Seg(3), Seg(4), Seg(5), Seg(6)]),
             # new prefetch segments on the first regular segment occurrence
             Playlist(4, ads + [Seg(4), Seg(5), Seg(6), Seg(7), Pre(8), Pre(9)]),
             Playlist(5, ads + [Seg(5), Seg(6), Seg(7), Seg(8), Pre(9), Pre(10)]),
             Playlist(6, ads + [Seg(6), Seg(7), Seg(8), Seg(9), Pre(10), Pre(11)]),
             Playlist(7, [Seg(7), Seg(8), Seg(9), Seg(10), Pre(11), Pre(12)], end=True),
-        ], disable_ads=True, low_latency=True)
+        ], streamoptions={"disable_ads": True, "low_latency": True})
 
         self.await_write(11)
         data = self.await_read(read_all=True)
         assert data == self.content(segments, cond=lambda s: 2 <= s.num <= 3 or 7 <= s.num)
         assert mock_log.info.mock_calls == [
             call("Will skip ad segments"),
             call("Low latency streaming (HLS live edge: 2)"),
@@ -369,80 +369,79 @@
 
     @patch("streamlink.plugins.twitch.log")
     def test_hls_low_latency_no_prefetch_disable_ads_has_preroll(self, mock_log):
         daterange = TagDateRangeAd(duration=4)
         self.subject([
             Playlist(0, [daterange, Segment(0), Segment(1), Segment(2), Segment(3)]),
             Playlist(4, [Segment(4), Segment(5), Segment(6), Segment(7)], end=True),
-        ], disable_ads=True, low_latency=True)
+        ], streamoptions={"disable_ads": True, "low_latency": True})
 
         self.await_write(6)
         self.await_read(read_all=True)
         assert mock_log.info.mock_calls == [
             call("Will skip ad segments"),
             call("Low latency streaming (HLS live edge: 2)"),
             call("Waiting for pre-roll ads to finish, be patient"),
             call("This is not a low latency stream"),
         ]
 
     def test_hls_low_latency_no_ads_reload_time(self):
         Seg, SegPre = Segment, SegmentPrefetch
         self.subject([
             Playlist(0, [Seg(0, duration=5), Seg(1, duration=7), Seg(2, duration=11), SegPre(3)], end=True),
-        ], low_latency=True)
+        ], streamoptions={"low_latency": True})
 
         self.await_write(4)
         self.await_read(read_all=True)
         assert self.thread.reader.worker.playlist_reload_time == pytest.approx(23 / 3)
 
 
 class TestTwitchAPIAccessToken:
+    @pytest.fixture(autouse=True)
+    def _client_integrity_token(self, monkeypatch: pytest.MonkeyPatch):
+        mock_client_integrity_token = Mock(return_value=("device-id", "client-integrity-token"))
+        monkeypatch.setattr(Twitch, "_client_integrity_token", mock_client_integrity_token)
+
     @pytest.fixture()
-    def plugin(self, request):
+    def plugin(self, request: pytest.FixtureRequest):
         session = Streamlink()
+        options = Options()
         for param in getattr(request, "param", {}):
-            session.set_plugin_option("twitch", *param)
-        yield Twitch(session, "https://twitch.tv/channelname")
-        Twitch.options.clear()
+            options.set(*param)
 
-    @pytest.fixture()
-    def mocker(self):
-        # The built-in requests_mock fixture is bad when trying to reference the following constants or classes
-        with requests_mock.Mocker() as mocker:
-            mocker.register_uri(requests_mock.ANY, requests_mock.ANY, exc=requests_mock.exceptions.InvalidRequest)
-            yield mocker
+        return Twitch(session, "https://twitch.tv/channelname", options)
 
     @pytest.fixture()
-    def mock(self, request, mocker: requests_mock.Mocker):
-        mock = mocker.post("https://gql.twitch.tv/gql", **getattr(request, "param", {"json": {}}))
+    def mock(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker):
+        mock = requests_mock.post("https://gql.twitch.tv/gql", **getattr(request, "param", {"json": {}}))
         yield mock
-        assert mock.called_once
+        assert mock.call_count > 0
         payload = mock.last_request.json()  # type: ignore[union-attr]
         assert tuple(sorted(payload.keys())) == ("extensions", "operationName", "variables")
         assert payload.get("operationName") == "PlaybackAccessToken"
         assert payload.get("extensions") == {
             "persistedQuery": {
                 "sha256Hash": "0828119ded1c13477966434e15800ff57ddacf13ba1911c129dc2200705b0712",
                 "version": 1,
             },
         }
 
     @pytest.fixture()
-    def _assert_live(self, mock):
+    def _assert_live(self, mock: rm.Mocker):
         yield
         assert mock.last_request.json().get("variables") == {  # type: ignore[union-attr]
             "isLive": True,
             "isVod": False,
             "login": "channelname",
             "vodID": "",
             "playerType": "embed",
         }
 
     @pytest.fixture()
-    def _assert_vod(self, mock):
+    def _assert_vod(self, mock: rm.Mocker):
         yield
         assert mock.last_request.json().get("variables") == {  # type: ignore[union-attr]
             "isLive": False,
             "isVod": True,
             "login": "",
             "vodID": "vodid",
             "playerType": "embed",
@@ -481,93 +480,128 @@
                 "login": "channelname",
                 "vodID": "",
                 "playerType": "frontpage",
                 "specialVariable": "specialValue",
             },
         ),
     ], indirect=["plugin"])
-    def test_plugin_options(self, plugin: Twitch, mock: requests_mock.Mocker, exp_headers: dict, exp_variables: dict):
-        with pytest.raises(NoStreamsError):
+    def test_plugin_options(self, plugin: Twitch, mock: rm.Mocker, exp_headers: dict, exp_variables: dict):
+        with pytest.raises(PluginError):
             plugin._access_token(True, "channelname")
         requestheaders = dict(mock.last_request._request.headers)  # type: ignore[union-attr]
         for header in plugin.session.http.headers.keys():
             del requestheaders[header]
         del requestheaders["Content-Type"]
         del requestheaders["Content-Length"]
         assert requestheaders == exp_headers
         assert mock.last_request.json().get("variables") == exp_variables  # type: ignore[union-attr]
 
     @pytest.mark.usefixtures("_assert_live")
     @pytest.mark.parametrize("mock", [{
         "json": {"data": {"streamPlaybackAccessToken": {"value": '{"channel":"foo"}', "signature": "sig"}}},
     }], indirect=True)
-    def test_live_success(self, plugin: Twitch, mock: requests_mock.Mocker):
+    def test_live_success(self, plugin: Twitch, mock: rm.Mocker):
         data = plugin._access_token(True, "channelname")
         assert data == ("sig", '{"channel":"foo"}', [])
 
     @pytest.mark.usefixtures("_assert_live")
     @pytest.mark.parametrize("mock", [{
         "json": {"data": {"streamPlaybackAccessToken": None}},
     }], indirect=True)
-    def test_live_failure(self, plugin: Twitch, mock: requests_mock.Mocker):
+    def test_live_failure(self, plugin: Twitch, mock: rm.Mocker):
         with pytest.raises(NoStreamsError):
             plugin._access_token(True, "channelname")
+        assert len(mock.request_history) == 1, "Only gets the access token once when the channel is offline"
 
     @pytest.mark.usefixtures("_assert_vod")
     @pytest.mark.parametrize("mock", [{
         "json": {"data": {"videoPlaybackAccessToken": {"value": '{"channel":"foo"}', "signature": "sig"}}},
     }], indirect=True)
-    def test_vod_success(self, plugin: Twitch, mock: requests_mock.Mocker):
+    def test_vod_success(self, plugin: Twitch, mock: rm.Mocker):
         data = plugin._access_token(False, "vodid")
         assert data == ("sig", '{"channel":"foo"}', [])
 
     @pytest.mark.usefixtures("_assert_vod")
     @pytest.mark.parametrize("mock", [{
         "json": {"data": {"videoPlaybackAccessToken": None}},
     }], indirect=True)
-    def test_vod_failure(self, plugin: Twitch, mock: requests_mock.Mocker):
+    def test_vod_failure(self, plugin: Twitch, mock: rm.Mocker):
         with pytest.raises(NoStreamsError):
             plugin._access_token(False, "vodid")
+        assert len(mock.request_history) == 1, "Only gets the access token once when the VOD doesn't exist"
 
     @pytest.mark.usefixtures("_assert_live")
     @pytest.mark.parametrize(("plugin", "mock"), [
         (
             [("api-header", [("Authorization", "OAuth invalid-token")])],
             {
                 "status_code": 401,
                 "json": {"error": "Unauthorized", "status": 401, "message": "The \"Authorization\" token is invalid."},
             },
         ),
     ], indirect=True)
-    def test_auth_failure(self, caplog: pytest.LogCaptureFixture, plugin: Twitch, mock: requests_mock.Mocker):
-        with pytest.raises(NoStreamsError):
+    def test_auth_failure(self, plugin: Twitch, mock: rm.Mocker):
+        with pytest.raises(PluginError, match="^Unauthorized: The \"Authorization\" token is invalid\\.$"):
             plugin._access_token(True, "channelname")
-        assert mock.last_request._request.headers["Authorization"] == "OAuth invalid-token"  # type: ignore[union-attr]
-        assert [(record.levelname, record.module, record.message) for record in caplog.records] == [
-            ("error", "twitch", "Unauthorized: The \"Authorization\" token is invalid."),
-        ]
+        assert len(mock.request_history) == 2, "Always tries again on error, with integrity-token on second attempt"
 
+        headers: dict = mock.request_history[0]._request.headers
+        assert headers["Authorization"] == "OAuth invalid-token"
+        assert "Device-Id" not in headers
+        assert "Client-Integrity" not in headers
+
+        headers = mock.request_history[1]._request.headers
+        assert headers["Authorization"] == "OAuth invalid-token"
+        assert headers["Device-Id"] == "device-id"
+        assert headers["Client-Integrity"] == "client-integrity-token"
 
-class TestTwitchMetadata(unittest.TestCase):
-    def setUp(self):
-        self.mock = requests_mock.Mocker()
-        self.mock.register_uri(requests_mock.ANY, requests_mock.ANY, exc=requests_mock.exceptions.InvalidRequest)
-        self.mock.start()
+    @pytest.mark.usefixtures("_assert_live")
+    @pytest.mark.parametrize(("plugin", "mock"), [
+        (
+            [("api-header", [("Authorization", "OAuth invalid-token")])],
+            {"response_list": [
+                {
+                    "status_code": 401,
+                    "json": {"errors": [{"message": "failed integrity check"}]},
+                },
+                {
+                    "json": {"data": {"streamPlaybackAccessToken": {"value": '{"channel":"foo"}', "signature": "sig"}}},
+                },
+            ]},
+        ),
+    ], indirect=True)
+    def test_failed_integrity_check(self, plugin: Twitch, mock: rm.Mocker):
+        data = plugin._access_token(True, "channelname")
+        assert data == ("sig", '{"channel":"foo"}', [])
+        assert len(mock.request_history) == 2, "Always tries again on error, with integrity-token on second attempt"
 
-    def tearDown(self):
-        self.mock.stop()
+        headers: dict = mock.request_history[0]._request.headers
+        assert headers["Authorization"] == "OAuth invalid-token"
+        assert "Device-Id" not in headers
+        assert "Client-Integrity" not in headers
 
-    @staticmethod
-    def subject(url):
-        session = Streamlink()
+        headers = mock.request_history[1]._request.headers
+        assert headers["Authorization"] == "OAuth invalid-token"
+        assert headers["Device-Id"] == "device-id"
+        assert headers["Client-Integrity"] == "client-integrity-token"
+
+
+class TestTwitchMetadata:
+    @pytest.fixture()
+    def metadata(self, request: pytest.FixtureRequest, session: Streamlink):
+        url = getattr(request, "param", "")
         plugin = Twitch(session, url)
+
         return plugin.get_id(), plugin.get_author(), plugin.get_category(), plugin.get_title()
 
-    def mock_request_channel(self, data=True):
-        return self.mock.post(
+    @pytest.fixture()
+    def mock_request_channel(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker):
+        data = getattr(request, "param", True)
+
+        return requests_mock.post(
             "https://gql.twitch.tv/gql",
             json=[
                 {"data": {"userOrError": {"userDoesNotExist": "error"} if not data else {
                     "displayName": "channel name",
                 }}},
                 {"data": {"user": None if not data else {
                     "lastBroadcast": {
@@ -579,31 +613,37 @@
                             "name": "channel game",
                         },
                     },
                 }}},
             ],
         )
 
-    def mock_request_video(self, data=True):
-        return self.mock.post(
+    @pytest.fixture()
+    def mock_request_video(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker):
+        data = getattr(request, "param", True)
+
+        return requests_mock.post(
             "https://gql.twitch.tv/gql",
             json={"data": {"video": None if not data else {
                 "id": "video id",
                 "title": "video title",
                 "game": {
                     "displayName": "video game",
                 },
                 "owner": {
                     "displayName": "channel name",
                 },
             }}},
         )
 
-    def mock_request_clip(self, data=True):
-        return self.mock.post(
+    @pytest.fixture()
+    def mock_request_clip(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker):
+        data = getattr(request, "param", True)
+
+        return requests_mock.post(
             "https://gql.twitch.tv/gql",
             json=[
                 {"data": {
                     "clip": None if not data else {
                         "id": "clip id",
                         "broadcaster": {
                             "displayName": "channel name",
@@ -617,23 +657,23 @@
                     "clip": None if not data else {
                         "title": "clip title",
                     },
                 }},
             ],
         )
 
-    def test_metadata_channel(self):
-        mock = self.mock_request_channel()
-        _id, author, category, title = self.subject("https://twitch.tv/foo")
+    @pytest.mark.parametrize(("mock_request_channel", "metadata"), [(True, "https://twitch.tv/foo")], indirect=True)
+    def test_metadata_channel(self, mock_request_channel, metadata):
+        _id, author, category, title = metadata
         assert _id == "stream id"
         assert author == "channel name"
         assert category == "channel game"
         assert title == "channel status"
-        assert mock.call_count == 1
-        assert mock.request_history[0].json() == [
+        assert mock_request_channel.call_count == 1
+        assert mock_request_channel.request_history[0].json() == [
             {
                 "operationName": "ChannelShell",
                 "extensions": {
                     "persistedQuery": {
                         "version": 1,
                         "sha256Hash": "c3ea5a669ec074a58df5c11ce3c27093fa38534c94286dc14b68a25d5adcbf55",
                     },
@@ -653,61 +693,63 @@
                 },
                 "variables": {
                     "channelLogin": "foo",
                 },
             },
         ]
 
-    def test_metadata_channel_no_data(self):
-        self.mock_request_channel(data=False)
-        _id, author, category, title = self.subject("https://twitch.tv/foo")
+    @pytest.mark.parametrize(("mock_request_channel", "metadata"), [(False, "https://twitch.tv/foo")], indirect=True)
+    def test_metadata_channel_no_data(self, mock_request_channel, metadata):
+        _id, author, category, title = metadata
         assert _id is None
         assert author is None
         assert category is None
         assert title is None
+        assert mock_request_channel.call_count == 1
 
-    def test_metadata_video(self):
-        mock = self.mock_request_video()
-        _id, author, category, title = self.subject("https://twitch.tv/videos/1337")
+    @pytest.mark.parametrize(("mock_request_video", "metadata"), [(True, "https://twitch.tv/videos/1337")], indirect=True)
+    def test_metadata_video(self, mock_request_video, metadata):
+        _id, author, category, title = metadata
         assert _id == "video id"
         assert author == "channel name"
         assert category == "video game"
         assert title == "video title"
-        assert mock.call_count == 1
-        assert mock.request_history[0].json() == {
+        assert mock_request_video.call_count == 1
+        assert mock_request_video.request_history[0].json() == {
             "operationName": "VideoMetadata",
             "extensions": {
                 "persistedQuery": {
                     "version": 1,
                     "sha256Hash": "cb3b1eb2f2d2b2f65b8389ba446ec521d76c3aa44f5424a1b1d235fe21eb4806",
                 },
             },
             "variables": {
                 "channelLogin": "",
                 "videoID": "1337",
             },
         }
 
-    def test_metadata_video_no_data(self):
-        self.mock_request_video(data=False)
-        _id, author, category, title = self.subject("https://twitch.tv/videos/1337")
+    @pytest.mark.parametrize(("mock_request_video", "metadata"), [(False, "https://twitch.tv/videos/1337")], indirect=True)
+    def test_metadata_video_no_data(self, mock_request_video, metadata):
+        _id, author, category, title = metadata
         assert _id is None
         assert author is None
         assert category is None
         assert title is None
+        assert mock_request_video.call_count == 1
 
-    def test_metadata_clip(self):
-        mock = self.mock_request_clip()
-        _id, author, category, title = self.subject("https://clips.twitch.tv/foo")
+    @pytest.mark.parametrize(("mock_request_clip", "metadata"), [(True, "https://clips.twitch.tv/foo")], indirect=True)
+    def test_metadata_clip(self, mock_request_clip, metadata):
+        _id, author, category, title = metadata
         assert _id == "clip id"
         assert author == "channel name"
         assert category == "game name"
         assert title == "clip title"
-        assert mock.call_count == 1
-        assert mock.request_history[0].json() == [
+        assert mock_request_clip.call_count == 1
+        assert mock_request_clip.request_history[0].json() == [
             {
                 "operationName": "ClipsView",
                 "extensions": {
                     "persistedQuery": {
                         "version": 1,
                         "sha256Hash": "4480c1dcc2494a17bb6ef64b94a5213a956afb8a45fe314c66b0d04079a93a8f",
                     },
@@ -726,44 +768,74 @@
                 },
                 "variables": {
                     "slug": "foo",
                 },
             },
         ]
 
-    def test_metadata_clip_no_data(self):
-        self.mock_request_clip(data=False)
-        _id, author, category, title = self.subject("https://clips.twitch.tv/foo")
+    @pytest.mark.parametrize(("mock_request_clip", "metadata"), [(False, "https://clips.twitch.tv/foo")], indirect=True)
+    def test_metadata_clip_no_data(self, mock_request_clip, metadata):
+        _id, author, category, title = metadata
         assert _id is None
         assert author is None
         assert category is None
         assert title is None
 
 
-@patch("streamlink.plugins.twitch.log")
-class TestTwitchReruns(unittest.TestCase):
-    log_call = call("Reruns were disabled by command line option")
-
-    def subject(self, **params):
-        with patch("streamlink.plugins.twitch.TwitchAPI.stream_metadata") as mock:
-            mock.return_value = None if params.pop("offline", False) else {"type": params.pop("stream_type", "live")}
-            session = Streamlink()
-            plugin = Twitch(session, "https://www.twitch.tv/foo")
-            plugin.options.set("disable-reruns", params.pop("disable", True))
-
-            return plugin._check_for_rerun()
-
-    def test_disable_reruns_live(self, mock_log):
-        assert not self.subject()
-        assert self.log_call not in mock_log.info.call_args_list
-
-    def test_disable_reruns_not_live(self, mock_log):
-        assert self.subject(stream_type="rerun")
-        assert self.log_call in mock_log.info.call_args_list
-
-    def test_disable_reruns_offline(self, mock_log):
-        assert not self.subject(offline=True)
-        assert self.log_call not in mock_log.info.call_args_list
-
-    def test_enable_reruns(self, mock_log):
-        assert not self.subject(stream_type="rerun", disable=False)
-        assert self.log_call not in mock_log.info.call_args_list
+@pytest.mark.parametrize(("stream_type", "offline", "disable", "expected", "logs"), [
+    pytest.param(
+        "live",
+        False,
+        True,
+        False,
+        [],
+        id="disable live",
+    ),
+    pytest.param(
+        "rerun",
+        False,
+        True,
+        True,
+        [("streamlink.plugins.twitch", "info", "Reruns were disabled by command line option")],
+        id="disable not live",
+    ),
+    pytest.param(
+        "live",
+        True,
+        True,
+        False,
+        [],
+        id="disable offline",
+    ),
+    pytest.param(
+        "rerun",
+        True,
+        False,
+        False,
+        [],
+        id="enable",
+    ),
+])
+def test_reruns(
+    monkeypatch: pytest.MonkeyPatch,
+    caplog: pytest.LogCaptureFixture,
+    session: Streamlink,
+    stream_type: str,
+    offline: bool,
+    disable: bool,
+    expected: bool,
+    logs: list,
+):
+    caplog.set_level(1, "streamlink")
+    mock_stream_metadata = Mock(return_value=None if offline else {"type": stream_type})
+    monkeypatch.setattr("streamlink.plugins.twitch.TwitchAPI.stream_metadata", mock_stream_metadata)
+
+    # noinspection PyTypeChecker
+    plugin: Twitch = Twitch(session, "https://www.twitch.tv/foo")
+    try:
+        plugin.options.set("disable-reruns", disable)
+        result = plugin._check_for_rerun()
+    finally:
+        plugin.options.clear()
+
+    assert result is expected
+    assert [(record.name, record.levelname, record.message) for record in caplog.records] == logs
```

### Comparing `streamlink-5.5.1/tests/plugins/test_ustreamtv.py` & `streamlink-6.0.0/tests/plugins/test_ustreamtv.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import unittest
 from unittest.mock import ANY, MagicMock
 
 from streamlink import Streamlink
 from streamlink.plugins.ustreamtv import UStreamTV
 from tests.plugins import PluginCanHandleUrl
 
 
@@ -49,15 +48,15 @@
         (
             "https://video.ibm.com/recorded/132041157",
             {"video_id": "132041157"},
         ),
     ]
 
 
-class TestPluginUStreamTV(unittest.TestCase):
+class TestPluginUStreamTV:
     def test_arguments(self):
         from streamlink_cli.main import setup_plugin_args
         session = Streamlink()
         parser = MagicMock()
         plugins = parser.add_argument_group("Plugin Options")
         group = parser.add_argument_group("UStreamTV", parent=plugins)
```

### Comparing `streamlink-5.5.1/tests/plugins/test_ustvnow.py` & `streamlink-6.0.0/tests/plugins/test_ustvnow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import unittest
-
 from streamlink.plugins.ustvnow import USTVNow
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlUSTVNow(PluginCanHandleUrl):
     __plugin__ = USTVNow
 
     should_match = [
         "http://www.ustvnow.com/live/foo/-65",
     ]
 
 
-class TestPluginUSTVNow(unittest.TestCase):
+class TestPluginUSTVNow:
     def test_encrypt_data(self):
         key = "80035ad42d7d-bb08-7a14-f726-78403b29"
         iv = "3157b5680927cc4a"
 
         assert USTVNow.encrypt_data(
             b'{"login_id":"test@test.com","login_key":"testtest1234","login_mode":"1","manufacturer":"123"}',
             key,
```

### Comparing `streamlink-5.5.1/tests/plugins/test_vinhlongtv.py` & `streamlink-6.0.0/tests/plugins/test_vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_vk.py` & `streamlink-6.0.0/tests/plugins/test_vk.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,12 +82,11 @@
         pytest.raises(NoStreamsError),
     ),
 ])
 def test_url_redirect(url: str, newurl: str, raises: nullcontext, requests_mock: rm.Mocker):
     session = Streamlink()
     # noinspection PyTypeChecker
     plugin: VK = VK(session, url)
-    requests_mock.register_uri(rm.ANY, rm.ANY, exc=rm.exceptions.InvalidRequest)
     requests_mock.get(url, text=f"""<!DOCTYPE html><html><head><meta property="og:url" content="{newurl}"/></head></html>""")
     with raises:
         plugin.follow_vk_redirect()
         assert plugin.url == newurl
```

### Comparing `streamlink-5.5.1/tests/plugins/test_vtvgo.py` & `streamlink-6.0.0/tests/plugins/test_vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_webtv.py` & `streamlink-6.0.0/tests/plugins/test_webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_welt.py` & `streamlink-6.0.0/tests/plugins/test_welt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import unittest
-
 from streamlink.plugins.welt import Welt
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlWelt(PluginCanHandleUrl):
     __plugin__ = Welt
 
@@ -19,15 +17,15 @@
         "https://welt.de/tv-programm-live-stream/",
         "https://www.welt.de",
         "https://www.welt.de/",
         "https://www.welt.de/tv-programm-live-stream/",
     ]
 
 
-class TestPluginWelt(unittest.TestCase):
+class TestPluginWelt:
     def test_validate_live(self):
         hls_url = Welt._schema.validate("""
             <!DOCTYPE html><html><body>
             <script type="application/json" data-content="VideoPlayer.Config">
                 {
                     "title": "foo",
                     "sources": [
```

### Comparing `streamlink-5.5.1/tests/plugins/test_youtube.py` & `streamlink-6.0.0/tests/plugins/test_youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_zattoo.py` & `streamlink-6.0.0/tests/plugins/test_zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_zdf_mediathek.py` & `streamlink-6.0.0/tests/plugins/test_zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/plugins/test_zengatv.py` & `streamlink-6.0.0/tests/plugins/test_zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/__init__.py` & `streamlink-6.0.0/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_1.mpd` & `streamlink-6.0.0/tests/resources/dash/test_1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_10.mpd` & `streamlink-6.0.0/tests/resources/dash/test_10.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_11_static.mpd` & `streamlink-6.0.0/tests/resources/dash/test_11_static.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_2.mpd` & `streamlink-6.0.0/tests/resources/dash/test_2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_3.mpd` & `streamlink-6.0.0/tests/resources/dash/test_3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_8.mpd` & `streamlink-6.0.0/tests/resources/dash/test_8.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_9.mpd` & `streamlink-6.0.0/tests/resources/dash/test_9.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd` & `streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd` & `streamlink-6.0.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-6.0.0/tests/resources/dash/test_nested_baseurls.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_no_segment_list_or_template.mpd` & `streamlink-6.0.0/tests/resources/dash/test_no_segment_list_or_template.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_segment_list.mpd` & `streamlink-6.0.0/tests/resources/dash/test_segment_list.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_segments_byterange.mpd` & `streamlink-6.0.0/tests/resources/dash/test_segments_byterange.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_segments_dynamic_number.mpd` & `streamlink-6.0.0/tests/resources/dash/test_segments_dynamic_number.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_static_no_publish_time.mpd` & `streamlink-6.0.0/tests/resources/dash/test_static_no_publish_time.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/dash/test_timeline_ids.mpd` & `streamlink-6.0.0/tests/resources/dash/test_timeline_ids.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/hls/test_1.m3u8` & `streamlink-6.0.0/tests/resources/hls/test_1.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/hls/test_2.m3u8` & `streamlink-6.0.0/tests/resources/hls/test_2.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/hls/test_date.m3u8` & `streamlink-6.0.0/tests/resources/hls/test_date.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/hls/test_master.m3u8` & `streamlink-6.0.0/tests/resources/hls/test_master.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/resources/hls/test_master_twitch_vod.m3u8` & `streamlink-6.0.0/tests/resources/hls/test_master_twitch_vod.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/stream/test_dash.py` & `streamlink-6.0.0/tests/stream/test_dash.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,20 +20,18 @@
     with freezegun.freeze_time("2000-01-01T00:00:00Z"):
         yield datetime.now(timezone.utc)
 
 
 class TestDASHStreamParseManifest:
     @pytest.fixture(autouse=True)
     def _response(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker):
-        invalid = requests_mock.register_uri(rm.ANY, rm.ANY, exc=rm.exceptions.InvalidRequest("Invalid request"))
         response = requests_mock.register_uri("GET", "http://test/manifest.mpd", **getattr(request, "param", {}))
         called_once = "nomockedhttprequest" not in request.keywords
         yield
-        assert not invalid.called
-        assert response.called_once is called_once
+        assert (response.call_count == 1) is called_once
 
     @pytest.fixture()
     def parse_xml(self, monkeypatch: pytest.MonkeyPatch):
         parse_xml = Mock(return_value=Mock())
         monkeypatch.setattr("streamlink.stream.dash.parse_xml", parse_xml)
         return parse_xml
 
@@ -79,14 +77,68 @@
         )
         mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
         streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
         assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["a128k", "a256k"])
 
+    @pytest.mark.parametrize(("with_video_only", "with_audio_only", "expected"), [
+        pytest.param(
+            False,
+            False,
+            ["720p+a128k", "720p+a256k", "1080p+a128k", "1080p+a256k"],
+            id="Only muxed streams",
+        ),
+        pytest.param(
+            True,
+            False,
+            ["720p", "720p+a128k", "720p+a256k", "1080p", "1080p+a128k", "1080p+a256k"],
+            id="With video-only streams",
+        ),
+        pytest.param(
+            False,
+            True,
+            ["a128k", "a256k", "720p+a128k", "720p+a256k", "1080p+a128k", "1080p+a256k"],
+            id="With audio-only streams",
+        ),
+        pytest.param(
+            True,
+            True,
+            ["a128k", "a256k", "720p", "720p+a128k", "720p+a256k", "1080p", "1080p+a128k", "1080p+a256k"],
+            id="With video-only and audio-only streams",
+        ),
+    ])
+    def test_with_videoaudio_only(
+        self,
+        session: Streamlink,
+        mpd: Mock,
+        with_video_only: bool,
+        with_audio_only: bool,
+        expected: List[str],
+    ):
+        adaptationset = Mock(
+            contentProtections=None,
+            representations=[
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
+                Mock(id="3", contentProtections=None, mimeType="audio/mp4", bandwidth=128.0, lang="en"),
+                Mock(id="4", contentProtections=None, mimeType="audio/mp4", bandwidth=256.0, lang="en"),
+            ],
+        )
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
+
+        streams = DASHStream.parse_manifest(
+            session,
+            "http://test/manifest.mpd",
+            with_video_only=with_video_only,
+            with_audio_only=with_audio_only,
+        )
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
+        assert list(streams.keys()) == expected
+
     def test_audio_single(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
             contentProtections=None,
             representations=[
                 Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
                 Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
                 Mock(id="3", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
@@ -275,31 +327,33 @@
 
     def test_stream_open_video_only(self, session: Streamlink, timestamp: datetime, muxer: Mock, reader: Mock):
         rep_video = Mock(ident=(None, None, "1"), mimeType="video/mp4")
         stream = DASHStream(session, Mock(), rep_video)
         stream.open()
 
         assert reader.call_args_list == [call(stream, rep_video, timestamp)]
-        reader_video = reader(stream, rep_video, timestamp)
-        assert reader_video.open.called_once
+        assert reader().open.call_count == 1
         assert muxer.call_args_list == []
 
     def test_stream_open_video_audio(self, session: Streamlink, timestamp: datetime, muxer: Mock, reader: Mock):
         rep_video = Mock(ident=(None, None, "1"), mimeType="video/mp4")
         rep_audio = Mock(ident=(None, None, "2"), mimeType="audio/mp3", lang="en")
+
+        mock_reader_video = Mock()
+        mock_reader_audio = Mock()
+        readers = {rep_video: mock_reader_video, rep_audio: mock_reader_audio}
+        reader.side_effect = lambda _stream, _representation, _timestamp: readers[_representation]
+
         stream = DASHStream(session, Mock(), rep_video, rep_audio)
         stream.open()
 
         assert reader.call_args_list == [call(stream, rep_video, timestamp), call(stream, rep_audio, timestamp)]
-        reader_video = reader(stream, rep_video, timestamp)
-        reader_audio = reader(stream, rep_audio, timestamp)
-        assert reader_video.open.called_once
-        assert reader_audio.open.called_once
-        assert muxer.call_args_list == [call(session, reader_video, reader_audio, copyts=True)]
-        assert reader_video.timestamp is reader_audio.timestamp
+        assert mock_reader_video.open.call_count == 1
+        assert mock_reader_audio.open.call_count == 1
+        assert muxer.call_args_list == [call(session, mock_reader_video, mock_reader_audio, copyts=True)]
 
 
 class TestDASHStreamWorker:
     @pytest.fixture()
     def mock_time(self, monkeypatch: pytest.MonkeyPatch) -> Mock:
         mock = Mock(return_value=1)
         monkeypatch.setattr("streamlink.stream.dash.time", mock)
```

### Comparing `streamlink-5.5.1/tests/stream/test_dash_parser.py` & `streamlink-6.0.0/tests/stream/test_dash_parser.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/stream/test_ffmpegmux.py` & `streamlink-6.0.0/tests/stream/test_ffmpegmux.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
         with patch("streamlink.stream.ffmpegmux.sys.stderr") as mock_stderr:
             streamio = FFMPEGMuxer(session)
 
             streamio.open()
             assert popen.call_args_list[0][1]["stderr"] is mock_stderr
 
             streamio.close()
-            assert not mock_stderr.close.called
+            assert mock_stderr.close.call_count == 0
 
     @pytest.mark.parametrize(("options", "side_effect"), [
         pytest.param({"ffmpeg-verbose-path": "foo"}, None, id="verbose-path"),
         pytest.param({"ffmpeg-verbose-path": "foo", "ffmpeg-verbose": True}, None, id="verbose-path priority"),
         pytest.param({"ffmpeg-verbose-path": "foo"}, OSError, id="OSError on close"),
     ])
     def test_stderr_path(self, session: Streamlink, popen: Mock, options: dict, side_effect: Optional[Type[Exception]]):
@@ -437,11 +437,11 @@
         with patch("streamlink.stream.ffmpegmux.Path") as mock_path:
             file: Mock = mock_path("foo").expanduser().open("w")
             file.close.side_effect = side_effect
             streamio = FFMPEGMuxer(session)
 
             streamio.open()
             assert popen.call_args_list[0][1]["stderr"] is file
-            assert not file.close.called
+            assert file.close.call_count == 0
 
             streamio.close()
-            assert file.close.called_once
+            assert file.close.call_count == 1
```

### Comparing `streamlink-5.5.1/tests/stream/test_hls.py` & `streamlink-6.0.0/tests/stream/test_hls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import typing
 import unittest
 from datetime import datetime, timedelta, timezone
 from threading import Event
+from typing import Dict
 from unittest.mock import Mock, call, patch
 
 import freezegun
 import pytest
-import requests_mock
-from Crypto.Cipher import AES
-from Crypto.Util.Padding import pad
+import requests_mock as rm
 from requests.exceptions import InvalidSchema
 
 from streamlink.session import Streamlink
 from streamlink.stream.hls import HLSStream, HLSStreamReader, MuxedHLSStream
 from streamlink.stream.hls_playlist import M3U8Parser
+from streamlink.utils.crypto import AES, pad
 from tests.mixins.stream_hls import EventedHLSStreamWorker, EventedHLSStreamWriter, Playlist, Segment, Tag, TestMixinStreamHLS
 from tests.resources import text
 
 
 EPOCH = datetime(2000, 1, 1, 0, 0, 0, 0, tzinfo=timezone.utc)
 ONE_SECOND = timedelta(seconds=1.0)
 
@@ -70,57 +70,49 @@
         return self.uri.format(namespace=namespace) if self.uri else super().url(namespace)
 
 
 class SegmentEnc(EncryptedBase, Segment):
     pass
 
 
-class TestHLSStreamRepr(unittest.TestCase):
-    def test_repr(self):
-        session = Streamlink()
+def test_repr(session: Streamlink):
+    stream = HLSStream(session, "https://foo.bar/playlist.m3u8")
+    assert repr(stream) == "<HLSStream ['hls', 'https://foo.bar/playlist.m3u8']>"
 
-        stream = HLSStream(session, "https://foo.bar/playlist.m3u8")
-        assert repr(stream) == "<HLSStream ['hls', 'https://foo.bar/playlist.m3u8']>"
+    stream = HLSStream(session, "https://foo.bar/playlist.m3u8", "https://foo.bar/master.m3u8")
+    assert repr(stream) == "<HLSStream ['hls', 'https://foo.bar/playlist.m3u8', 'https://foo.bar/master.m3u8']>"
 
-        stream = HLSStream(session, "https://foo.bar/playlist.m3u8", "https://foo.bar/master.m3u8")
-        assert repr(stream) == "<HLSStream ['hls', 'https://foo.bar/playlist.m3u8', 'https://foo.bar/master.m3u8']>"
 
+class TestHLSVariantPlaylist:
+    @pytest.fixture()
+    def streams(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker, session: Streamlink):
+        url = f"http://mocked/{request.node.originalname}/master.m3u8"
+        playlist = getattr(request, "param", "")
+
+        with text(playlist) as fd:
+            content = fd.read()
+        requests_mock.get(url, text=content)
 
-class TestHLSVariantPlaylist(unittest.TestCase):
-    @classmethod
-    def get_master_playlist(cls, playlist):
-        with text(playlist) as pl:
-            return pl.read()
-
-    def subject(self, playlist, options=None):
-        with requests_mock.Mocker() as mock:
-            url = f"http://mocked/{self.id()}/master.m3u8"
-            content = self.get_master_playlist(playlist)
-            mock.get(url, text=content)
-
-            session = Streamlink(options)
-
-            return HLSStream.parse_variant_playlist(session, url)
+        return HLSStream.parse_variant_playlist(session, url)
 
-    def test_variant_playlist(self):
-        streams = self.subject("hls/test_master.m3u8")
+    @pytest.mark.parametrize("streams", ["hls/test_master.m3u8"], indirect=True)
+    def test_variant_playlist(self, request: pytest.FixtureRequest, streams: Dict[str, HLSStream]):
         assert list(streams.keys()) == ["720p", "720p_alt", "480p", "360p", "160p", "1080p (source)", "90k"]
         assert all(isinstance(stream, HLSStream) for stream in streams.values())
         assert all(stream.multivariant is not None and stream.multivariant.is_master for stream in streams.values())
 
-        base = f"http://mocked/{self.id()}"
+        base = f"http://mocked/{request.node.originalname}"
         stream = next(iter(streams.values()))
         assert repr(stream) == f"<HLSStream ['hls', '{base}/720p.m3u8', '{base}/master.m3u8']>"
 
         assert stream.multivariant is not None
         assert stream.multivariant.uri == f"{base}/master.m3u8"
         assert stream.url_master == f"{base}/master.m3u8"
 
-    def test_url_master(self):
-        session = Streamlink()
+    def test_url_master(self, session: Streamlink):
         stream = HLSStream(session, "http://mocked/foo", url_master="http://mocked/master.m3u8")
 
         assert stream.multivariant is None
         assert stream.url == "http://mocked/foo"
         assert stream.url_master == "http://mocked/master.m3u8"
 
 
@@ -198,14 +190,85 @@
         worker.handshake_wait.go()
         worker.handshake_reload.go()
         return super().tearDown()
 
     def get_session(self, options=None, *args, **kwargs):
         return super().get_session({**self.OPTIONS, **(options or {})}, *args, **kwargs)
 
+    def test_segment_queue_timing_threshold_reached(self) -> None:
+        thread, segments = self.subject(
+            start=False,
+            playlists=[
+                Playlist(0, targetduration=5, segments=[Segment(0)]),
+                # no EXT-X-ENDLIST, last mocked playlist response will be repreated forever
+                Playlist(0, targetduration=5, segments=[Segment(0), Segment(1)]),
+            ],
+        )
+        worker: EventedHLSStreamWorker = thread.reader.worker
+        targetduration = ONE_SECOND * 5
+
+        with freezegun.freeze_time(EPOCH) as frozen_time, \
+             patch("streamlink.stream.hls.log") as mock_log:
+            self.start()
+
+            assert worker.handshake_reload.wait_ready(1), "Loads playlist for the first time"
+            assert worker.playlist_sequence == -1, "Initial sequence number"
+            assert worker.playlist_sequences_last == EPOCH, "Sets the initial last queue time"
+
+            # first playlist reload has taken one second
+            frozen_time.tick(ONE_SECOND)
+            self.await_playlist_reload(1)
+
+            assert worker.handshake_wait.wait_ready(1), "Arrives at first wait() call"
+            assert worker.playlist_sequence == 1, "Updates the sequence number"
+            assert worker.playlist_sequences_last == EPOCH + ONE_SECOND, "Updates the last queue time"
+            assert worker.playlist_targetduration == 5.0
+
+            # trigger next reload when the target duration has passed
+            frozen_time.tick(targetduration)
+            self.await_playlist_wait(1)
+            self.await_playlist_reload(1)
+
+            assert worker.handshake_wait.wait_ready(1), "Arrives at second wait() call"
+            assert worker.playlist_sequence == 2, "Updates the sequence number again"
+            assert worker.playlist_sequences_last == EPOCH + ONE_SECOND + targetduration, "Updates the last queue time again"
+            assert worker.playlist_targetduration == 5.0
+
+            # trigger next reload when the target duration has passed
+            frozen_time.tick(targetduration)
+            self.await_playlist_wait(1)
+            self.await_playlist_reload(1)
+
+            assert worker.handshake_wait.wait_ready(1), "Arrives at third wait() call"
+            assert worker.playlist_sequence == 2, "Sequence number is unchanged"
+            assert worker.playlist_sequences_last == EPOCH + ONE_SECOND + targetduration, "Last queue time is unchanged"
+            assert worker.playlist_targetduration == 5.0
+
+            # trigger next reload when the target duration has passed
+            frozen_time.tick(targetduration)
+            self.await_playlist_wait(1)
+            self.await_playlist_reload(1)
+
+            assert worker.handshake_wait.wait_ready(1), "Arrives at fourth wait() call"
+            assert worker.playlist_sequence == 2, "Sequence number is unchanged"
+            assert worker.playlist_sequences_last == EPOCH + ONE_SECOND + targetduration, "Last queue time is unchanged"
+            assert worker.playlist_targetduration == 5.0
+
+            assert mock_log.warning.call_args_list == []
+
+            # trigger next reload when the target duration has passed
+            frozen_time.tick(targetduration)
+            self.await_playlist_wait(1)
+            self.await_playlist_reload(1)
+
+            self.await_read(read_all=True)
+            self.await_close(1)
+
+            assert mock_log.warning.call_args_list == [call("No new segments in playlist for more than 10.00s. Stopping...")]
+
     def test_playlist_reload_offset(self) -> None:
         thread, segments = self.subject(
             start=False,
             playlists=[
                 Playlist(0, targetduration=5, segments=[Segment(0)]),
                 Playlist(1, targetduration=5, segments=[Segment(1)]),
                 Playlist(2, targetduration=5, segments=[Segment(2)]),
@@ -685,14 +748,15 @@
     def test_hls_playlist_reload_time_no_data(self):
         time = self.subject([Playlist(0, [], end=True, targetduration=0)], reload_time="default")
         assert time == 6, "sets reload time to 6 seconds when no data is available"
 
 
 @patch("streamlink.stream.hls.log")
 @patch("streamlink.stream.hls.HLSStreamWorker.wait", Mock(return_value=True))
+@patch("streamlink.stream.hls.HLSStreamWorker._segment_queue_timing_threshold_reached", Mock(return_value=False))
 class TestHlsPlaylistParseErrors(TestMixinStreamHLS, unittest.TestCase):
     __stream__ = EventedWriterHLSStream
 
     class FakePlaylist(typing.NamedTuple):
         is_master: bool = False
         iframes_only: bool = False
 
@@ -748,18 +812,17 @@
 
 class TestHlsExtAudio:
     @pytest.fixture(autouse=True)
     def _is_usable(self, monkeypatch: pytest.MonkeyPatch):
         monkeypatch.setattr("streamlink.stream.hls.FFMPEGMuxer.is_usable", Mock(return_value=True))
 
     @pytest.fixture(autouse=True)
-    def _playlist(self):
-        with text("hls/test_2.m3u8") as playlist, \
-             requests_mock.Mocker() as mock_requests:
-            mock_requests.get("http://mocked/path/master.m3u8", text=playlist.read())
+    def _playlist(self, requests_mock: rm.Mocker):
+        with text("hls/test_2.m3u8") as playlist:
+            requests_mock.get("http://mocked/path/master.m3u8", text=playlist.read())
             yield
 
     @pytest.fixture()
     def stream(self, session: Streamlink):
         streams = HLSStream.parse_variant_playlist(session, "http://mocked/path/master.m3u8")
         assert "video" in streams
```

### Comparing `streamlink-5.5.1/tests/stream/test_hls_filtered.py` & `streamlink-6.0.0/tests/stream/test_hls_filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/stream/test_hls_playlist.py` & `streamlink-6.0.0/tests/stream/test_hls_playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import unittest
 from datetime import datetime, timedelta, timezone
 from typing import Optional, Tuple, Union
 
 import pytest
 
 from streamlink.stream.hls_playlist import (
     ByteRange,
@@ -196,15 +195,15 @@
     ("invalid", Resolution(0, 0)),
     ("1920x1080", Resolution(1920, 1080)),
 ])
 def test_parse_resolution(string: str, expected: Resolution):
     assert M3U8Parser.parse_resolution(string) == expected
 
 
-class TestHLSPlaylist(unittest.TestCase):
+class TestHLSPlaylist:
     def test_load(self):
         with text("hls/test_1.m3u8") as m3u8_fh:
             playlist = load(m3u8_fh.read(), "http://test.se/")
 
         assert playlist.media == [
             Media(
                 uri="http://test.se/audio/stereo/en/128kbit.m3u8",
@@ -377,15 +376,15 @@
 
         start_date = datetime(year=2000, month=1, day=1, hour=0, minute=0, second=0, microsecond=0, tzinfo=UTC)
         end_date = datetime(year=2000, month=1, day=1, hour=0, minute=1, second=0, microsecond=0, tzinfo=UTC)
         delta_15 = timedelta(seconds=15)
         delta_30 = timedelta(seconds=30, milliseconds=500)
         delta_60 = timedelta(seconds=60)
 
-        assert playlist.target_duration == 120
+        assert playlist.targetduration == 120
 
         assert list(playlist.dateranges) == [
             DateRange(
                 id="start-invalid",
                 start_date=None,
                 classname=None,
                 end_date=None,
```

### Comparing `streamlink-5.5.1/tests/stream/test_stream_json.py` & `streamlink-6.0.0/tests/stream/test_stream_json.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/stream/test_stream_to_url.py` & `streamlink-6.0.0/tests/stream/test_stream_to_url.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/stream/test_stream_wrappers.py` & `streamlink-6.0.0/tests/stream/test_stream_wrappers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import unittest
-
 from streamlink.stream.wrappers import StreamIOIterWrapper
 
 
-class TestPluginStream(unittest.TestCase):
+class TestPluginStream:
     def test_iter(self):
         def generator():
             yield b"1" * 8192
             yield b"2" * 4096
             yield b"3" * 2048
 
         fd = StreamIOIterWrapper(generator())
```

### Comparing `streamlink-5.5.1/tests/test_api_http_session.py` & `streamlink-6.0.0/tests/test_api_http_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import unittest
-from unittest.mock import PropertyMock, call, patch
+from typing import Optional
+from unittest.mock import Mock, PropertyMock, call
 
 import pytest
 import requests
 
-from streamlink.exceptions import PluginError
+from streamlink.exceptions import PluginError, StreamlinkDeprecationWarning
 from streamlink.plugin.api.http_session import HTTPSession
 from streamlink.plugin.api.useragents import FIREFOX
 
 
 class TestUrllib3Overrides:
     @pytest.fixture(scope="class")
     def httpsession(self) -> HTTPSession:
@@ -29,53 +29,66 @@
     ])
     def test_encode_invalid_chars(self, httpsession: HTTPSession, url: str, expected: str, assertion: str):
         req = requests.Request(method="GET", url=url)
         prep = httpsession.prepare_request(req)
         assert prep.url == expected, assertion
 
 
-class TestPluginAPIHTTPSession(unittest.TestCase):
+class TestHTTPSession:
     def test_session_init(self):
         session = HTTPSession()
         assert session.headers.get("User-Agent") == FIREFOX
         assert session.timeout == 20.0
         assert "file://" in session.adapters.keys()
 
-    @patch("streamlink.plugin.api.http_session.time.sleep")
-    @patch("streamlink.plugin.api.http_session.Session.request", side_effect=requests.Timeout)
-    def test_read_timeout(self, mock_request, mock_sleep):
-        session = HTTPSession()
+    def test_read_timeout(self, monkeypatch: pytest.MonkeyPatch):
+        mock_sleep = Mock()
+        mock_request = Mock(side_effect=requests.Timeout)
+        monkeypatch.setattr("streamlink.plugin.api.http_session.time.sleep", mock_sleep)
+        monkeypatch.setattr("streamlink.plugin.api.http_session.Session.request", mock_request)
 
+        session = HTTPSession()
         with pytest.raises(PluginError, match=r"^Unable to open URL: http://localhost/"):
             session.get("http://localhost/", timeout=123, retries=3, retry_backoff=2, retry_max_backoff=5)
-        assert mock_request.mock_calls == [
+
+        assert mock_request.call_args_list == [
             call("GET", "http://localhost/", headers={}, params={}, timeout=123, proxies={}, allow_redirects=True),
             call("GET", "http://localhost/", headers={}, params={}, timeout=123, proxies={}, allow_redirects=True),
             call("GET", "http://localhost/", headers={}, params={}, timeout=123, proxies={}, allow_redirects=True),
             call("GET", "http://localhost/", headers={}, params={}, timeout=123, proxies={}, allow_redirects=True),
         ]
-        assert mock_sleep.mock_calls == [
+        assert mock_sleep.call_args_list == [
             call(2),
             call(4),
             call(5),
         ]
 
-    def test_json_encoding(self):
-        json_str = "{\"test\": \"Α and Ω\"}"
+    @pytest.mark.parametrize("encoding", ["UTF-32BE", "UTF-32LE", "UTF-16BE", "UTF-16LE", "UTF-8"])
+    def test_determine_json_encoding(self, recwarn: pytest.WarningsRecorder, encoding: str):
+        data = "Hello world, Γειά σου Κόσμε, こんにちは世界".encode(encoding)
+        assert HTTPSession.determine_json_encoding(data) == encoding
+        assert [(record.category, str(record.message)) for record in recwarn.list] == [
+            (StreamlinkDeprecationWarning, "Deprecated HTTPSession.determine_json_encoding() call"),
+        ]
+
+    @pytest.mark.parametrize(("encoding", "override"), [
+        ("utf-32-be", None),
+        ("utf-32-le", None),
+        ("utf-16-be", None),
+        ("utf-16-le", None),
+        ("utf-8", None),
+        # With byte order mark (BOM)
+        ("utf-16", None),
+        ("utf-32", None),
+        ("utf-8-sig", None),
+        # Override
+        ("utf-8", "utf-8"),
+        ("cp949", "cp949"),
+    ])
+    def test_json(self, monkeypatch: pytest.MonkeyPatch, encoding: str, override: Optional[str]):
+        mock_content = PropertyMock(return_value="{\"test\": \"Α and Ω\"}".encode(encoding))
+        monkeypatch.setattr("requests.Response.content", mock_content)
 
-        # encode the json string with each encoding and assert that the correct one is detected
-        for encoding in ["UTF-32BE", "UTF-32LE", "UTF-16BE", "UTF-16LE", "UTF-8"]:
-            with patch("requests.Response.content", new_callable=PropertyMock) as mock_content:
-                mock_content.return_value = json_str.encode(encoding)
-                res = requests.Response()
-
-                assert HTTPSession.json(res) == {"test": "Α and Ω"}
-
-    def test_json_encoding_override(self):
-        json_text = "{\"test\": \"Α and Ω\"}".encode("cp949")
-
-        with patch("requests.Response.content", new_callable=PropertyMock) as mock_content:
-            mock_content.return_value = json_text
-            res = requests.Response()
-            res.encoding = "cp949"
+        res = requests.Response()
+        res.encoding = override
 
-            assert HTTPSession.json(res) == {"test": "Α and Ω"}
+        assert HTTPSession.json(res) == {"test": "Α and Ω"}
```

### Comparing `streamlink-5.5.1/tests/test_api_validate.py` & `streamlink-6.0.0/tests/test_api_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,24 @@
 import re
 from textwrap import dedent
 
 import pytest
 from lxml.etree import Element, tostring as etree_tostring
 
-from streamlink.exceptions import PluginError, StreamlinkDeprecationWarning
+from streamlink.exceptions import PluginError
 from streamlink.plugin.api import validate
 
 # noinspection PyProtectedMember
 from streamlink.plugin.api.validate._exception import ValidationError
 
 
 def assert_validationerror(exception, expected):
     assert str(exception) == dedent(expected).strip("\n")
 
 
-def test_text_is_str(recwarn: pytest.WarningsRecorder):
-    assert "text" not in getattr(validate, "__dict__", {})
-    assert "text" in getattr(validate, "__all__", [])
-    assert validate.text is str, "Exports text as str alias for backwards compatiblity"
-    assert [(record.category, str(record.message), record.filename) for record in recwarn.list] == [
-        (
-            StreamlinkDeprecationWarning,
-            "`streamlink.plugin.api.validate.text` is deprecated. Use `str` instead.",
-            __file__,
-        ),
-    ]
-
-
 class TestSchema:
     @pytest.fixture(scope="class")
     def schema(self):
         return validate.Schema(str, "foo")
 
     @pytest.fixture(scope="class")
     def schema_nested(self, schema: validate.Schema):
```

### Comparing `streamlink-5.5.1/tests/test_api_websocket.py` & `streamlink-6.0.0/tests/test_api_websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/test_buffers.py` & `streamlink-6.0.0/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/test_cache.py` & `streamlink-6.0.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/test_logger.py` & `streamlink-6.0.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/test_plugin.py` & `streamlink-6.0.0/tests/test_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import logging
 import re
 import time
+from operator import eq, gt, lt
 from typing import Type
 from unittest.mock import Mock, call, patch
 
 import freezegun
 import pytest
 import requests.cookies
 
+from streamlink.options import Options
 from streamlink.plugin import (
     HIGH_PRIORITY,
     NORMAL_PRIORITY,
     Plugin,
     PluginArgument,
     PluginArguments,
     pluginargument,
     pluginmatcher,
 )
 
 # noinspection PyProtectedMember
-from streamlink.plugin.plugin import _COOKIE_KEYS, Matcher
+from streamlink.plugin.plugin import _COOKIE_KEYS, Matcher, parse_params, stream_weight
 from streamlink.session import Streamlink
 
 
 class FakePlugin(Plugin):
     def _get_streams(self):
         pass  # pragma: no cover
 
@@ -38,20 +40,14 @@
 
 
 class CustomConstructorTwoPlugin(FakePlugin):
     def __init__(self, session, url):
         super().__init__(session, url)
 
 
-class DeprecatedPlugin(FakePlugin):
-    def __init__(self, url):
-        super().__init__(url)  # type: ignore[call-arg]
-        self.custom_attribute = url.upper()
-
-
 class TestPlugin:
     @pytest.mark.parametrize(("pluginclass", "module", "logger"), [
         (Plugin, "plugin", "streamlink.plugin.plugin"),
         (FakePlugin, "test_plugin", "tests.test_plugin"),
         (RenamedPlugin, "baz", "foo.bar.baz"),
         (CustomConstructorOnePlugin, "test_plugin", "tests.test_plugin"),
         (CustomConstructorTwoPlugin, "test_plugin", "tests.test_plugin"),
@@ -73,42 +69,23 @@
         assert plugin.logger.name == logger
 
         assert mock_cache.call_args_list == [call(filename="plugin-cache.json", key_prefix=module)]
         assert plugin.cache == mock_cache()
 
         assert mock_load_cookies.call_args_list == [call()]
 
-    def test_constructor_wrapper(self, recwarn: pytest.WarningsRecorder):
-        session = Mock()
-        with patch("streamlink.plugin.plugin.Cache") as mock_cache, \
-             patch.object(DeprecatedPlugin, "load_cookies") as mock_load_cookies:
-            plugin = DeprecatedPlugin(session, "http://localhost")  # type: ignore[call-arg]
-
-        assert isinstance(plugin, DeprecatedPlugin)
-        assert plugin.custom_attribute == "HTTP://LOCALHOST"
-        assert [(record.category, str(record.message), record.filename) for record in recwarn.list] == [
-            (
-                FutureWarning,
-                "Initialized test_plugin plugin with deprecated constructor",
-                __file__,
-            ),
-        ]
-
-        assert plugin.session is session
-        assert plugin.url == "http://localhost"
-
-        assert plugin.module == "test_plugin"
-
-        assert isinstance(plugin.logger, logging.Logger)
-        assert plugin.logger.name == "tests.test_plugin"
-
-        assert mock_cache.call_args_list == [call(filename="plugin-cache.json", key_prefix="test_plugin")]
-        assert plugin.cache == mock_cache()
-
-        assert mock_load_cookies.call_args_list == [call()]
+    def test_constructor_options(self):
+        one = FakePlugin(Mock(), "https://mocked", Options({"key": "val"}))
+        two = FakePlugin(Mock(), "https://mocked")
+        assert one.get_option("key") == "val"
+        assert two.get_option("key") is None
+
+        one.set_option("key", "other")
+        assert one.get_option("key") == "other"
+        assert two.get_option("key") is None
 
 
 class TestPluginMatcher:
     # noinspection PyUnusedLocal
     def test_decorator(self):
         with pytest.raises(TypeError) as cm:
             @pluginmatcher(re.compile(""))
@@ -269,34 +246,36 @@
         def __str__(self):
             return " baz qux "
 
     setattr(plugin, attr, Foo())
     assert getter() == "baz qux"
 
 
-# TODO: python 3.7 removal: move this as static method to the TestCookies class
-def _create_cookie_dict(name, value, expires=None):
-    return dict(
-        version=0,
-        name=name,
-        value=value,
-        port=None,
-        domain="test.se",
-        path="/",
-        secure=False,
-        expires=expires,
-        discard=True,
-        comment=None,
-        comment_url=None,
-        rest={"HttpOnly": None},
-        rfc2109=False,
-    )
+class TestCookies:
+    @staticmethod
+    def create_cookie_dict(name, value, expires=None):
+        return dict(
+            version=0,
+            name=name,
+            value=value,
+            port=None,
+            domain="test.se",
+            path="/",
+            secure=False,
+            expires=expires,
+            discard=True,
+            comment=None,
+            comment_url=None,
+            rest={"HttpOnly": None},
+            rfc2109=False,
+        )
 
+    # TODO: py39 support end: remove explicit dummy context binding of static method
+    _create_cookie_dict = create_cookie_dict.__get__(object)
 
-class TestCookies:
     @pytest.fixture()
     def pluginclass(self):
         class MyPlugin(FakePlugin):
             __module__ = "myplugin"
 
         return MyPlugin
 
@@ -350,15 +329,15 @@
         cookie2 = requests.cookies.create_cookie("test-name2", "test-value2", domain="test.se")
         session.http.cookies.set_cookie(cookie1)
         session.http.cookies.set_cookie(cookie2)
 
         plugin.save_cookies(lambda cookie: cookie.name == "test-name1", default_expires=3600)
         assert plugincache.set.call_args_list == [call(
             "__cookie:test-name1:test.se:80:/",
-            _create_cookie_dict("test-name1", "test-value1", None),
+            self.create_cookie_dict("test-name1", "test-value1", None),
             3600,
         )]
         assert logger.debug.call_args_list == [call("Saved cookies: test-name1")]
 
     @freezegun.freeze_time("1970-01-01T00:00:00Z")
     @pytest.mark.parametrize("plugincache", [{}], indirect=True)
     def test_save_expires(self, session: Streamlink, plugin: Plugin, plugincache: Mock):
@@ -370,15 +349,15 @@
             rest={"HttpOnly": None},
         )
         session.http.cookies.set_cookie(cookie)
 
         plugin.save_cookies(default_expires=60)
         assert plugincache.set.call_args_list == [call(
             "__cookie:test-name:test.se:80:/",
-            _create_cookie_dict("test-name", "test-value", 3600),
+            self.create_cookie_dict("test-name", "test-value", 3600),
             3600,
         )]
 
     @pytest.mark.parametrize(
         "plugincache",
         [{
             "__cookie:test-name1:test.se:80:/": _create_cookie_dict("test-name1", "test-value1", None),
@@ -407,7 +386,62 @@
     def test_clear_filter(self, session: Streamlink, plugin: Plugin, plugincache: Mock):
         assert tuple(session.http.cookies.keys()) == ("test-name1", "test-name2")
 
         plugin.clear_cookies(lambda cookie: cookie.name == "test-name2")
         assert call("__cookie:test-name1:test.se:80:/", None, 0) not in plugincache.set.call_args_list
         assert call("__cookie:test-name2:test.se:80:/", None, 0) in plugincache.set.call_args_list
         assert tuple(session.http.cookies.keys()) == ("test-name1",)
+
+
+@pytest.mark.parametrize(("params", "expected"), [
+    (
+        None,
+        {},
+    ),
+    (
+        "foo=bar",
+        dict(foo="bar"),
+    ),
+    (
+        "verify=False",
+        dict(verify=False),
+    ),
+    (
+        "timeout=123.45",
+        dict(timeout=123.45),
+    ),
+    (
+        "verify=False params={'key': 'a value'}",
+        dict(verify=False, params=dict(key="a value")),
+    ),
+    (
+        "\"conn=['B:1', 'S:authMe', 'O:1', 'NN:code:1.23', 'NS:flag:ok', 'O:0']",
+        dict(conn=["B:1", "S:authMe", "O:1", "NN:code:1.23", "NS:flag:ok", "O:0"]),
+    ),
+])
+def test_parse_params(params, expected):
+    assert parse_params(params) == expected
+
+
+@pytest.mark.parametrize(("weight", "expected"), [
+    ("720p", (720, "pixels")),
+    ("720p+", (721, "pixels")),
+    ("720p60", (780, "pixels")),
+])
+def test_stream_weight_value(weight, expected):
+    assert stream_weight(weight) == expected
+
+
+@pytest.mark.parametrize(("weight_a", "operator", "weight_b"), [
+    ("720p+", gt, "720p"),
+    ("720p_3000k", gt, "720p_2500k"),
+    ("720p60_3000k", gt, "720p_3000k"),
+    ("3000k", gt, "2500k"),
+    ("720p", eq, "720p"),
+    ("720p_3000k", lt, "720p+_3000k"),
+    # with audio
+    ("720p+a256k", gt, "720p+a128k"),
+    ("720p+a256k", gt, "360p+a256k"),
+    ("720p+a128k", gt, "360p+a256k"),
+])
+def test_stream_weight(weight_a, weight_b, operator):
+    assert operator(stream_weight(weight_a), stream_weight(weight_b))
```

### Comparing `streamlink-5.5.1/tests/test_plugin_userinput.py` & `streamlink-6.0.0/tests/test_plugin_userinput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/test_plugins.py` & `streamlink-6.0.0/tests/test_plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,20 +80,17 @@
 
     def test_plugin_api(self, plugin):
         pluginclass = plugin.__plugin__
         assert not hasattr(pluginclass, "can_handle_url"), "Does not implement deprecated can_handle_url(url)"
         assert not hasattr(pluginclass, "priority"), "Does not implement deprecated priority(url)"
         assert callable(pluginclass._get_streams), "Implements _get_streams()"
 
-    def test_no_global_args(self, plugin):
-        assert not [parg for parg in plugin.__plugin__.arguments or [] if parg.is_global], "Doesn't define global arguments"
-
 
 class TestPluginTests:
-    @pytest.mark.parametrize("plugin", plugins_no_protocols)
+    @pytest.mark.parametrize("plugin", plugins)
     def test_plugin_has_tests(self, plugin):
         assert plugin in plugintests, "Test module exists for plugin"
 
     @pytest.mark.parametrize("plugintest", plugintests)
     def test_test_has_plugin(self, plugintest):
         assert plugintest in plugins, "Plugin exists for test module"
```

### Comparing `streamlink-5.5.1/tests/test_session.py` & `streamlink-6.0.0/tests/test_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
-import unittest
-import warnings
+from contextlib import nullcontext
 from pathlib import Path
 from socket import AF_INET, AF_INET6
-from unittest.mock import Mock, call, patch
+from typing import Dict
+from unittest.mock import Mock
 
 import pytest
-import requests_mock
+import requests_mock as rm
 import urllib3
 from requests.adapters import HTTPAdapter
 
 import tests.plugin
 from streamlink.exceptions import NoPluginError, StreamlinkDeprecationWarning
 from streamlink.plugin import HIGH_PRIORITY, LOW_PRIORITY, NO_PRIORITY, NORMAL_PRIORITY, Plugin, pluginmatcher
 from streamlink.plugin.api.http_session import TLSNoDHAdapter
@@ -21,140 +21,163 @@
 
 PATH_TESTPLUGINS = Path(tests.plugin.__path__[0])
 PATH_TESTPLUGINS_OVERRIDE = PATH_TESTPLUGINS / "override"
 
 _original_allowed_gai_family = urllib3.util.connection.allowed_gai_family  # type: ignore[attr-defined]
 
 
-class EmptyPlugin(Plugin):
-    def _get_streams(self):
-        pass  # pragma: no cover
-
-
-# TODO: rewrite using pytest
-class TestSession(unittest.TestCase):
-    mocker: requests_mock.Mocker
-
-    def setUp(self):
-        self.mocker = requests_mock.Mocker()
-        self.mocker.register_uri(requests_mock.ANY, requests_mock.ANY, text="")
-        self.mocker.start()
-
-    def tearDown(self):
-        self.mocker.stop()
-        Streamlink.resolve_url.cache_clear()
-
-    def subject(self, load_plugins=True):
-        session = Streamlink()
-        if load_plugins:
-            session.load_plugins(str(PATH_TESTPLUGINS))
-            session.load_plugins(str(PATH_TESTPLUGINS_OVERRIDE))
+class TestLoadPlugins:
+    @pytest.fixture(autouse=True)
+    def caplog(self, caplog: pytest.LogCaptureFixture) -> pytest.LogCaptureFixture:
+        caplog.set_level(1, "streamlink")
+        return caplog
 
-        return session
-
-    # ----
+    def test_load_plugins(self, caplog: pytest.LogCaptureFixture, session: Streamlink):
+        session.load_plugins(str(PATH_TESTPLUGINS))
+        plugins = session.get_plugins()
+        assert list(plugins.keys()) == ["testplugin"]
+        assert plugins["testplugin"].__name__ == "TestPlugin"
+        assert plugins["testplugin"].__module__ == "streamlink.plugins.testplugin"
+        assert caplog.records == []
 
-    def test_load_plugins(self):
-        session = self.subject()
+    def test_load_plugins_override(self, caplog: pytest.LogCaptureFixture, session: Streamlink):
+        session.load_plugins(str(PATH_TESTPLUGINS))
+        session.load_plugins(str(PATH_TESTPLUGINS_OVERRIDE))
         plugins = session.get_plugins()
-        assert "testplugin" in plugins
-        assert "testplugin_missing" not in plugins
-        assert "testplugin_invalid" not in plugins
+        assert list(plugins.keys()) == ["testplugin"]
+        assert plugins["testplugin"].__name__ == "TestPluginOverride"
+        assert plugins["testplugin"].__module__ == "streamlink.plugins.testplugin"
+        assert [(record.name, record.levelname, record.message) for record in caplog.records] == [
+            (
+                "streamlink.session",
+                "debug",
+                f"Plugin testplugin is being overridden by {PATH_TESTPLUGINS_OVERRIDE / 'testplugin.py'}",
+            ),
+        ]
 
     def test_load_plugins_builtin(self):
-        session = self.subject()
+        session = Streamlink()
         plugins = session.get_plugins()
         assert "twitch" in plugins
         assert plugins["twitch"].__module__ == "streamlink.plugins.twitch"
 
-    @patch("streamlink.session.log")
-    def test_load_plugins_override(self, mock_log):
-        session = self.subject()
-        plugins = session.get_plugins()
-        assert "testplugin" in plugins
-        assert "testplugin_override" not in plugins
-        assert plugins["testplugin"].__name__ == "TestPluginOverride"
-        assert plugins["testplugin"].__module__ == "streamlink.plugins.testplugin"
-        assert mock_log.debug.call_args_list == [
-            call(f"Plugin testplugin is being overridden by {PATH_TESTPLUGINS_OVERRIDE / 'testplugin.py'}"),
-        ]
+    @pytest.mark.parametrize(("side_effect", "raises", "logs"), [
+        pytest.param(
+            ImportError,
+            nullcontext(),
+            [
+                (
+                    "streamlink.session",
+                    "error",
+                    f"Failed to load plugin testplugin from {PATH_TESTPLUGINS}",
+                    True,
+                ),
+                (
+                    "streamlink.session",
+                    "error",
+                    f"Failed to load plugin testplugin_invalid from {PATH_TESTPLUGINS}",
+                    True,
+                ),
+                (
+                    "streamlink.session",
+                    "error",
+                    f"Failed to load plugin testplugin_missing from {PATH_TESTPLUGINS}",
+                    True,
+                ),
+            ],
+            id="ImportError",
+        ),
+        pytest.param(
+            SyntaxError,
+            pytest.raises(SyntaxError),
+            [],
+            id="SyntaxError",
+        ),
+    ])
+    def test_load_plugins_failure(
+        self,
+        monkeypatch: pytest.MonkeyPatch,
+        caplog: pytest.LogCaptureFixture,
+        side_effect: Exception,
+        raises: nullcontext,
+        logs: list,
+    ):
+        monkeypatch.setattr("streamlink.session.Streamlink.load_builtin_plugins", Mock())
+        monkeypatch.setattr("streamlink.session.load_module", Mock(side_effect=side_effect))
+        session = Streamlink()
+        with raises:
+            session.load_plugins(str(PATH_TESTPLUGINS))
+        assert session.get_plugins() == {}
+        assert [(record.name, record.levelname, record.message, bool(record.exc_info)) for record in caplog.records] == logs
 
-    @patch("streamlink.session.load_module")
-    @patch("streamlink.session.log")
-    def test_load_plugins_importerror(self, mock_log, mock_load_module):
-        mock_load_module.side_effect = ImportError()
-        session = self.subject()
-        assert not session.get_plugins()
-        assert len(mock_log.exception.call_args_list) > 0
-
-    @patch("streamlink.session.load_module")
-    @patch("streamlink.session.log")
-    def test_load_plugins_syntaxerror(self, mock_log, mock_load_module):
-        mock_load_module.side_effect = SyntaxError()
-        with pytest.raises(SyntaxError):
-            self.subject()
 
-    def test_resolve_url(self):
-        session = self.subject()
-        plugins = session.get_plugins()
+class _EmptyPlugin(Plugin):
+    def _get_streams(self):
+        pass  # pragma: no cover
+
 
-        with warnings.catch_warnings(record=True) as record_warnings:
-            pluginname, pluginclass, resolved_url = session.resolve_url("http://test.se/channel")
+class TestResolveURL:
+    @pytest.fixture(autouse=True)
+    def _load_builtins(self, session: Streamlink):
+        session.load_plugins(str(PATH_TESTPLUGINS))
+
+    @pytest.fixture(autouse=True)
+    def requests_mock(self, requests_mock: rm.Mocker):
+        return requests_mock
+
+    def test_resolve_url(self, recwarn: pytest.WarningsRecorder, session: Streamlink):
+        plugins = session.get_plugins()
+        pluginname, pluginclass, resolved_url = session.resolve_url("http://test.se/channel")
 
         assert issubclass(pluginclass, Plugin)
         assert pluginclass is plugins["testplugin"]
         assert resolved_url == "http://test.se/channel"
         assert hasattr(session.resolve_url, "cache_info"), "resolve_url has a lookup cache"
-        assert record_warnings == []
+        assert recwarn.list == []
 
-    def test_resolve_url__noplugin(self):
-        session = self.subject()
-        self.mocker.get("http://invalid2", status_code=301, headers={"Location": "http://invalid3"})
+    def test_resolve_url__noplugin(self, requests_mock: rm.Mocker, session: Streamlink):
+        requests_mock.get("http://invalid2", status_code=301, headers={"Location": "http://invalid3"})
 
         with pytest.raises(NoPluginError):
             session.resolve_url("http://invalid1")
         with pytest.raises(NoPluginError):
             session.resolve_url("http://invalid2")
 
-    def test_resolve_url__redirected(self):
-        session = self.subject()
-        plugins = session.get_plugins()
-        self.mocker.head("http://redirect1", status_code=501)
-        self.mocker.get("http://redirect1", status_code=301, headers={"Location": "http://redirect2"})
-        self.mocker.head("http://redirect2", status_code=301, headers={"Location": "http://test.se/channel"})
+    def test_resolve_url__redirected(self, requests_mock: rm.Mocker, session: Streamlink):
+        requests_mock.request("HEAD", "http://redirect1", status_code=501)
+        requests_mock.request("GET", "http://redirect1", status_code=301, headers={"Location": "http://redirect2"})
+        requests_mock.request("GET", "http://redirect2", status_code=301, headers={"Location": "http://test.se/channel"})
+        requests_mock.request("GET", "http://test.se/channel", content=b"")
 
+        plugins = session.get_plugins()
         pluginname, pluginclass, resolved_url = session.resolve_url("http://redirect1")
         assert issubclass(pluginclass, Plugin)
         assert pluginclass is plugins["testplugin"]
         assert resolved_url == "http://test.se/channel"
 
-    def test_resolve_url_no_redirect(self):
-        session = self.subject()
+    def test_resolve_url_no_redirect(self, session: Streamlink):
         plugins = session.get_plugins()
-
         pluginname, pluginclass, resolved_url = session.resolve_url_no_redirect("http://test.se/channel")
         assert issubclass(pluginclass, Plugin)
         assert pluginclass is plugins["testplugin"]
         assert resolved_url == "http://test.se/channel"
 
-    def test_resolve_url_no_redirect__noplugin(self):
-        session = self.subject()
+    def test_resolve_url_no_redirect__noplugin(self, session: Streamlink):
         with pytest.raises(NoPluginError):
             session.resolve_url_no_redirect("http://invalid")
 
-    def test_resolve_url_scheme(self):
+    def test_resolve_url_scheme(self, session: Streamlink):
         @pluginmatcher(re.compile("http://insecure"))
-        class PluginHttp(EmptyPlugin):
+        class PluginHttp(_EmptyPlugin):
             pass
 
         @pluginmatcher(re.compile("https://secure"))
-        class PluginHttps(EmptyPlugin):
+        class PluginHttps(_EmptyPlugin):
             pass
 
-        session = self.subject(load_plugins=False)
         session.plugins = {
             "insecure": PluginHttp,
             "secure": PluginHttps,
         }
 
         with pytest.raises(NoPluginError):
             session.resolve_url("insecure")
@@ -163,40 +186,39 @@
             session.resolve_url("https://insecure")
 
         assert session.resolve_url("secure")[1] is PluginHttps
         with pytest.raises(NoPluginError):
             session.resolve_url("http://secure")
         assert session.resolve_url("https://secure")[1] is PluginHttps
 
-    def test_resolve_url_priority(self):
+    def test_resolve_url_priority(self, session: Streamlink):
         @pluginmatcher(priority=HIGH_PRIORITY, pattern=re.compile(
             "https://(high|normal|low|no)$",
         ))
-        class HighPriority(EmptyPlugin):
+        class HighPriority(_EmptyPlugin):
             pass
 
         @pluginmatcher(priority=NORMAL_PRIORITY, pattern=re.compile(
             "https://(normal|low|no)$",
         ))
-        class NormalPriority(EmptyPlugin):
+        class NormalPriority(_EmptyPlugin):
             pass
 
         @pluginmatcher(priority=LOW_PRIORITY, pattern=re.compile(
             "https://(low|no)$",
         ))
-        class LowPriority(EmptyPlugin):
+        class LowPriority(_EmptyPlugin):
             pass
 
         @pluginmatcher(priority=NO_PRIORITY, pattern=re.compile(
             "https://(no)$",
         ))
-        class NoPriority(EmptyPlugin):
+        class NoPriority(_EmptyPlugin):
             pass
 
-        session = self.subject(load_plugins=False)
         session.plugins = {
             "high": HighPriority,
             "normal": NormalPriority,
             "low": LowPriority,
             "no": NoPriority,
         }
         no = session.resolve_url_no_redirect("no")[1]
@@ -212,88 +234,40 @@
         session.resolve_url.cache_clear()
         session.plugins = {
             "no": NoPriority,
         }
         with pytest.raises(NoPluginError):
             session.resolve_url_no_redirect("no")
 
-    def test_resolve_deprecated(self):
-        @pluginmatcher(priority=LOW_PRIORITY, pattern=re.compile(
-            "https://low",
-        ))
-        class LowPriority(EmptyPlugin):
-            pass
-
-        class DeprecatedNormalPriority(EmptyPlugin):
-            # noinspection PyUnusedLocal
-            @classmethod
-            def can_handle_url(cls, url):
-                return True
-
-        class DeprecatedHighPriority(DeprecatedNormalPriority):
-            # noinspection PyUnusedLocal
-            @classmethod
-            def priority(cls, url):
-                return HIGH_PRIORITY
-
-        session = self.subject(load_plugins=False)
-        session.plugins = {
-            "empty": EmptyPlugin,
-            "low": LowPriority,
-            "dep-normal-one": DeprecatedNormalPriority,
-            "dep-normal-two": DeprecatedNormalPriority,
-            "dep-high": DeprecatedHighPriority,
-        }
-
-        with pytest.warns() as recwarn:
-            plugin = session.resolve_url_no_redirect("low")[1]
-
-        assert plugin is DeprecatedHighPriority
-        assert [(record.category, str(record.message)) for record in recwarn.list] == [
-            (StreamlinkDeprecationWarning, "Resolved plugin dep-normal-one with deprecated can_handle_url API"),
-            (StreamlinkDeprecationWarning, "Resolved plugin dep-high with deprecated can_handle_url API"),
-        ]
 
-    def test_options(self):
-        session = self.subject()
-        session.set_option("test_option", "option")
-        assert session.get_option("test_option") == "option"
-        assert session.get_option("non_existing") is None
-
-        assert session.get_plugin_option("testplugin", "a_option") == "default"
-        session.set_plugin_option("testplugin", "another_option", "test")
-        assert session.get_plugin_option("testplugin", "another_option") == "test"
-        assert session.get_plugin_option("non_existing", "non_existing") is None
-        assert session.get_plugin_option("testplugin", "non_existing") is None
+class TestStreams:
+    @pytest.fixture(autouse=True)
+    def _load_builtins(self, session: Streamlink):
+        session.load_plugins(str(PATH_TESTPLUGINS))
 
-    def test_streams(self):
-        session = self.subject()
+    def test_streams(self, session: Streamlink):
         streams = session.streams("http://test.se/channel")
 
         assert "best" in streams
         assert "worst" in streams
         assert streams["best"] is streams["1080p"]
         assert streams["worst"] is streams["350k"]
         assert isinstance(streams["http"], HTTPStream)
         assert isinstance(streams["hls"], HLSStream)
 
-    def test_streams_stream_types(self):
-        session = self.subject()
-
+    def test_stream_types(self, session: Streamlink):
         streams = session.streams("http://test.se/channel", stream_types=["http", "hls"])
         assert isinstance(streams["480p"], HTTPStream)
         assert isinstance(streams["480p_hls"], HLSStream)
 
         streams = session.streams("http://test.se/channel", stream_types=["hls", "http"])
         assert isinstance(streams["480p"], HLSStream)
         assert isinstance(streams["480p_http"], HTTPStream)
 
-    def test_streams_stream_sorting_excludes(self):
-        session = self.subject()
-
+    def test_stream_sorting_excludes(self, session: Streamlink):
         streams = session.streams("http://test.se/channel", sorting_excludes=[])
         assert "best" in streams
         assert "worst" in streams
         assert "best-unfiltered" not in streams
         assert "worst-unfiltered" not in streams
         assert streams["worst"] is streams["350k"]
         assert streams["best"] is streams["1080p"]
@@ -325,95 +299,125 @@
         assert "worst" not in streams
         assert "best-unfiltered" not in streams
         assert "worst-unfiltered" not in streams
         assert "vod" in streams
         assert "vod_alt" in streams
         assert "vod_alt2" in streams
 
-    def test_set_and_get_locale(self):
-        session = Streamlink()
-        session.set_option("locale", "en_US")
-        assert session.localization.country.alpha2 == "US"
-        assert session.localization.language.alpha2 == "en"
-        assert session.localization.language_code == "en_US"
-
-    @patch("streamlink.session.HTTPSession")
-    def test_interface(self, mock_httpsession):
-        adapter_http = Mock(poolmanager=Mock(connection_pool_kw={}))
-        adapter_https = Mock(poolmanager=Mock(connection_pool_kw={}))
-        adapter_foo = Mock(poolmanager=Mock(connection_pool_kw={}))
-        mock_httpsession.return_value = Mock(adapters={
-            "http://": adapter_http,
-            "https://": adapter_https,
-            "foo://": adapter_foo,
-        })
-        session = self.subject(load_plugins=False)
+
+def test_options(session: Streamlink):
+    session.set_option("test_option", "option")
+    assert session.get_option("test_option") == "option"
+    assert session.get_option("non_existing") is None
+
+
+def test_options_locale(monkeypatch: pytest.MonkeyPatch, session: Streamlink):
+    monkeypatch.setattr("locale.getlocale", lambda: ("C", None))
+    assert session.get_option("locale") is None
+
+    localization = session.localization
+    assert localization.explicit is False
+    assert localization.language_code == "en_US"
+    assert localization.country.alpha2 == "US"
+    assert localization.country.name == "United States"
+    assert localization.language.alpha2 == "en"
+    assert localization.language.name == "English"
+
+    session.set_option("locale", "de_DE")
+    assert session.get_option("locale") == "de_DE"
+
+    localization = session.localization
+    assert localization.explicit is True
+    assert localization.language_code == "de_DE"
+    assert localization.country.alpha2 == "DE"
+    assert localization.country.name == "Germany"
+    assert localization.language.alpha2 == "de"
+    assert localization.language.name == "German"
+
+
+class TestOptionsInterface:
+    @pytest.fixture()
+    def adapters(self, monkeypatch: pytest.MonkeyPatch):
+        adapters = {
+            scheme: Mock(poolmanager=Mock(connection_pool_kw={}))
+            for scheme in ("http://", "https://", "foo://")
+        }
+        monkeypatch.setattr("streamlink.session.HTTPSession", Mock(return_value=Mock(adapters=adapters)))
+
+        return adapters
+
+    def test_options_interface(self, adapters: Dict[str, Mock], session: Streamlink):
         assert session.get_option("interface") is None
 
         session.set_option("interface", "my-interface")
-        assert adapter_http.poolmanager.connection_pool_kw == {"source_address": ("my-interface", 0)}
-        assert adapter_https.poolmanager.connection_pool_kw == {"source_address": ("my-interface", 0)}
-        assert adapter_foo.poolmanager.connection_pool_kw == {}
+        assert adapters["http://"].poolmanager.connection_pool_kw == {"source_address": ("my-interface", 0)}
+        assert adapters["https://"].poolmanager.connection_pool_kw == {"source_address": ("my-interface", 0)}
+        assert adapters["foo://"].poolmanager.connection_pool_kw == {}
         assert session.get_option("interface") == "my-interface"
 
         session.set_option("interface", None)
-        assert adapter_http.poolmanager.connection_pool_kw == {}
-        assert adapter_https.poolmanager.connection_pool_kw == {}
-        assert adapter_foo.poolmanager.connection_pool_kw == {}
+        assert adapters["http://"].poolmanager.connection_pool_kw == {}
+        assert adapters["https://"].poolmanager.connection_pool_kw == {}
+        assert adapters["foo://"].poolmanager.connection_pool_kw == {}
         assert session.get_option("interface") is None
 
-    @patch("streamlink.session.urllib3_util_connection", allowed_gai_family=_original_allowed_gai_family)
-    def test_ipv4_ipv6(self, mock_urllib3_util_connection):
-        session = self.subject(load_plugins=False)
-        assert session.get_option("ipv4") is False
-        assert session.get_option("ipv6") is False
-        assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
-
-        session.set_option("ipv4", True)
-        assert session.get_option("ipv4") is True
-        assert session.get_option("ipv6") is False
-        assert mock_urllib3_util_connection.allowed_gai_family is not _original_allowed_gai_family
-        assert mock_urllib3_util_connection.allowed_gai_family() is AF_INET
-
-        session.set_option("ipv4", False)
-        assert session.get_option("ipv4") is False
-        assert session.get_option("ipv6") is False
-        assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
-
-        session.set_option("ipv6", True)
-        assert session.get_option("ipv4") is False
-        assert session.get_option("ipv6") is True
-        assert mock_urllib3_util_connection.allowed_gai_family is not _original_allowed_gai_family
-        assert mock_urllib3_util_connection.allowed_gai_family() is AF_INET6
-
-        session.set_option("ipv6", False)
-        assert session.get_option("ipv4") is False
-        assert session.get_option("ipv6") is False
-        assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
-
-        session.set_option("ipv4", True)
-        session.set_option("ipv6", False)
-        assert session.get_option("ipv4") is True
-        assert session.get_option("ipv6") is False
-        assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
-
-    def test_http_disable_dh(self):
-        session = self.subject(load_plugins=False)
-        assert isinstance(session.http.adapters["https://"], HTTPAdapter)
-        assert not isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
-
-        session.set_option("http-disable-dh", True)
-        assert isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
-
-        session.set_option("http-disable-dh", False)
-        assert isinstance(session.http.adapters["https://"], HTTPAdapter)
-        assert not isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
+        # doesn't raise
+        session.set_option("interface", None)
+
+
+def test_options_ipv4_ipv6(monkeypatch: pytest.MonkeyPatch, session: Streamlink):
+    mock_urllib3_util_connection = Mock(allowed_gai_family=_original_allowed_gai_family)
+    monkeypatch.setattr("streamlink.session.urllib3_util_connection", mock_urllib3_util_connection)
+
+    assert session.get_option("ipv4") is False
+    assert session.get_option("ipv6") is False
+    assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
+
+    session.set_option("ipv4", True)
+    assert session.get_option("ipv4") is True
+    assert session.get_option("ipv6") is False
+    assert mock_urllib3_util_connection.allowed_gai_family is not _original_allowed_gai_family
+    assert mock_urllib3_util_connection.allowed_gai_family() is AF_INET
+
+    session.set_option("ipv4", False)
+    assert session.get_option("ipv4") is False
+    assert session.get_option("ipv6") is False
+    assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
+
+    session.set_option("ipv6", True)
+    assert session.get_option("ipv4") is False
+    assert session.get_option("ipv6") is True
+    assert mock_urllib3_util_connection.allowed_gai_family is not _original_allowed_gai_family
+    assert mock_urllib3_util_connection.allowed_gai_family() is AF_INET6
+
+    session.set_option("ipv6", False)
+    assert session.get_option("ipv4") is False
+    assert session.get_option("ipv6") is False
+    assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
+
+    session.set_option("ipv4", True)
+    session.set_option("ipv6", False)
+    assert session.get_option("ipv4") is True
+    assert session.get_option("ipv6") is False
+    assert mock_urllib3_util_connection.allowed_gai_family is _original_allowed_gai_family
+
+
+def test_options_http_disable_dh(session: Streamlink):
+    assert isinstance(session.http.adapters["https://"], HTTPAdapter)
+    assert not isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
+
+    session.set_option("http-disable-dh", True)
+    assert isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
+
+    session.set_option("http-disable-dh", False)
+    assert isinstance(session.http.adapters["https://"], HTTPAdapter)
+    assert not isinstance(session.http.adapters["https://"], TLSNoDHAdapter)
 
 
-class TestSessionOptionHttpProxy:
+class TestOptionsHttpProxy:
     @pytest.fixture()
     def _no_deprecation(self, recwarn: pytest.WarningsRecorder):
         yield
         assert recwarn.list == []
 
     @pytest.fixture()
     def _logs_deprecation(self, recwarn: pytest.WarningsRecorder):
```

### Comparing `streamlink-5.5.1/tests/test_streamlink_api.py` & `streamlink-6.0.0/tests/test_streamlink_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-import os.path
-import unittest
-from unittest.mock import patch
+import pytest
 
+import tests.plugin
 from streamlink import Streamlink
 from streamlink.api import streams
 
 
-PluginPath = os.path.join(os.path.dirname(__file__), "plugin")
+class TestStreamlinkAPI:
+    @pytest.fixture(autouse=True)
+    def _session(self, monkeypatch: pytest.MonkeyPatch, session: Streamlink):
+        monkeypatch.setattr("streamlink.api.Streamlink", lambda: session)
+        session.load_plugins(tests.plugin.__path__[0])
 
-
-def get_session():
-    s = Streamlink()
-    s.load_plugins(PluginPath)
-    return s
-
-
-class TestStreamlinkAPI(unittest.TestCase):
-    @patch("streamlink.api.Streamlink", side_effect=get_session)
-    def test_find_test_plugin(self, session):
+    def test_find_test_plugin(self):
         assert "hls" in streams("test.se")
 
-    @patch("streamlink.api.Streamlink", side_effect=get_session)
-    def test_no_streams_exception(self, session):
+    def test_no_streams_exception(self):
         assert streams("test.se/NoStreamsError") == {}
 
-    @patch("streamlink.api.Streamlink", side_effect=get_session)
-    def test_no_streams(self, session):
+    def test_no_streams(self):
         assert streams("test.se/empty") == {}
 
-    @patch("streamlink.api.Streamlink", side_effect=get_session)
-    def test_stream_type_filter(self, session):
+    def test_stream_type_filter(self):
         stream_types = ["hls"]
         available_streams = streams("test.se", stream_types=stream_types)
         assert "hls" in available_streams
         assert "test" not in available_streams
         assert "http" not in available_streams
 
-    @patch("streamlink.api.Streamlink", side_effect=get_session)
-    def test_stream_type_wildcard(self, session):
+    def test_stream_type_wildcard(self):
         stream_types = ["hls", "*"]
         available_streams = streams("test.se", stream_types=stream_types)
         assert "hls" in available_streams
         assert "test" in available_streams
         assert "http" in available_streams
```

### Comparing `streamlink-5.5.1/tests/testutils/handshake.py` & `streamlink-6.0.0/tests/testutils/handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/testutils/test_handshake.py` & `streamlink-6.0.0/tests/testutils/test_handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/utils/test_args.py` & `streamlink-6.0.0/tests/utils/test_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/utils/test_cache.py` & `streamlink-6.0.0/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/utils/test_crypto.py` & `streamlink-6.0.0/tests/utils/test_crypto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import base64
-import unittest
 
 from streamlink.utils.crypto import decrypt_openssl, evp_bytestokey
 
 
-class TestUtil(unittest.TestCase):
+class TestUtil:
     def test_evp_bytestokey(self):
         assert evp_bytestokey(b"hello", b"", 16, 16) == (
             b"]A@*\xbcK*v\xb9q\x9d\x91\x10\x17\xc5\x92",
             b"(\xb4n\xd3\xc1\x11\xe8Q\x02\x90\x9b\x1c\xfbP\xea\x0f",
         )
 
     def test_decrpyt(self):
```

### Comparing `streamlink-5.5.1/tests/utils/test_data.py` & `streamlink-6.0.0/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/utils/test_formatter.py` & `streamlink-6.0.0/tests/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/utils/test_l10n.py` & `streamlink-6.0.0/tests/utils/test_l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/utils/test_named_pipe.py` & `streamlink-6.0.0/tests/utils/test_named_pipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import threading
-import unittest
-from unittest.mock import Mock, call, patch
+from unittest.mock import Mock, call
 
 import pytest
 
 from streamlink.utils.named_pipe import NamedPipe, NamedPipeBase, NamedPipePosix, NamedPipeWindows
 
 
 try:
@@ -58,49 +57,66 @@
                 self.data += data.value
                 if read.value != len(data.value):
                     break
         finally:
             windll.kernel32.CloseHandle(handle)
 
 
-class TestNamedPipe(unittest.TestCase):
-    @patch("streamlink.utils.named_pipe._id", 0)
-    @patch("streamlink.utils.named_pipe.os.getpid", Mock(return_value=12345))
-    @patch("streamlink.utils.named_pipe.random.randint", Mock(return_value=67890))
-    @patch("streamlink.utils.named_pipe.NamedPipe._create", Mock(return_value=None))
-    @patch("streamlink.utils.named_pipe.log")
-    def test_name(self, mock_log):
+class TestNamedPipe:
+    def test_name(self, monkeypatch: pytest.MonkeyPatch, caplog: pytest.LogCaptureFixture):
+        caplog.set_level(1, "streamlink")
+        monkeypatch.setattr("streamlink.utils.named_pipe._id", 0)
+        monkeypatch.setattr("streamlink.utils.named_pipe.os.getpid", Mock(return_value=12345))
+        monkeypatch.setattr("streamlink.utils.named_pipe.random.randint", Mock(return_value=67890))
+        monkeypatch.setattr("streamlink.utils.named_pipe.NamedPipe._create", Mock(return_value=None))
+
         NamedPipe()
         NamedPipe()
-        assert mock_log.info.mock_calls == [
-            call("Creating pipe streamlinkpipe-12345-1-67890"),
-            call("Creating pipe streamlinkpipe-12345-2-67890"),
+
+        assert [(record.name, record.levelname, record.message) for record in caplog.records] == [
+            ("streamlink.utils.named_pipe", "info", "Creating pipe streamlinkpipe-12345-1-67890"),
+            ("streamlink.utils.named_pipe", "info", "Creating pipe streamlinkpipe-12345-2-67890"),
         ]
 
 
 @pytest.mark.posix_only()
-class TestNamedPipePosix(unittest.TestCase):
+class TestNamedPipePosix:
     def test_export(self):
         assert NamedPipe is NamedPipePosix
 
-    @patch("streamlink.utils.named_pipe.os.mkfifo")
-    def test_create(self, mock_mkfifo):
-        mock_mkfifo.side_effect = OSError
+    def test_create(self, monkeypatch: pytest.MonkeyPatch):
+        mock_mkfifo = Mock(side_effect=OSError)
+        monkeypatch.setattr("streamlink.utils.named_pipe.os.mkfifo", mock_mkfifo)
         with pytest.raises(OSError):  # noqa: PT011
             NamedPipePosix()
         assert mock_mkfifo.call_args[0][1:] == (0o660,)
 
     def test_close_before_open(self):
         pipe = NamedPipePosix()
         assert pipe.path.is_fifo()
         pipe.close()
         assert not pipe.path.is_fifo()
         # closing twice doesn't raise
         pipe.close()
 
+    def test_close_error(self, monkeypatch: pytest.MonkeyPatch):
+        mock_fd_close = Mock(side_effect=OSError)
+        mock_fd = Mock(close=mock_fd_close)
+        monkeypatch.setattr("builtins.open", Mock(return_value=mock_fd))
+
+        pipe = NamedPipePosix()
+        assert pipe.path.is_fifo()
+        pipe.open()
+        assert mock_fd_close.call_args_list == []
+
+        with pytest.raises(OSError):  # noqa: PT011
+            pipe.close()
+        assert mock_fd_close.call_args_list == [call()]
+        assert not pipe.path.is_fifo()
+
     def test_write_before_open(self):
         pipe = NamedPipePosix()
         assert pipe.path.is_fifo()
         with pytest.raises(AttributeError):
             pipe.write(b"foo")
         pipe.close()
 
@@ -117,24 +133,27 @@
         reader.done.wait(4000)
         assert reader.error is None
         assert reader.data == b"foobar"
         assert not reader.is_alive()
 
 
 @pytest.mark.windows_only()
-class TestNamedPipeWindows(unittest.TestCase):
+class TestNamedPipeWindows:
     def test_export(self):
         assert NamedPipe is NamedPipeWindows
 
-    @patch("streamlink.utils.named_pipe.windll.kernel32")
-    def test_create(self, mock_kernel32):
+    def test_create(self, monkeypatch: pytest.MonkeyPatch):
+        mock_kernel32 = Mock()
         mock_kernel32.CreateNamedPipeW.return_value = NamedPipeWindows.INVALID_HANDLE_VALUE
         mock_kernel32.GetLastError.return_value = 12345
+        monkeypatch.setattr("streamlink.utils.named_pipe.windll.kernel32", mock_kernel32)
+
         with pytest.raises(OSError, match=r"^Named pipe error code 0x00003039$"):
             NamedPipeWindows()
+
         assert mock_kernel32.CreateNamedPipeW.call_args[0][1:] == (
             0x00000002,
             0x00000000,
             255,
             8192,
             8192,
             0,
@@ -148,14 +167,31 @@
         windll.kernel32.CloseHandle(handle)
         pipe.close()
         handle = windll.kernel32.CreateFileW(str(pipe.path), GENERIC_READ, 0, None, OPEN_EXISTING, 0, None)
         assert handle == NamedPipeWindows.INVALID_HANDLE_VALUE
         # closing twice doesn't raise
         pipe.close()
 
+    @pytest.mark.parametrize("method", ["DisconnectNamedPipe", "CloseHandle"])
+    def test_close_error(self, monkeypatch: pytest.MonkeyPatch, method: str):
+        mock_method = Mock(side_effect=OSError)
+        mock_kernel32 = Mock(**{method: mock_method})
+        monkeypatch.setattr("streamlink.utils.named_pipe.windll.kernel32", mock_kernel32)
+
+        pipe = NamedPipeWindows()
+        mock_pipe = pipe.pipe
+        assert mock_pipe is not None
+        pipe.open()
+        assert mock_method.call_args_list == []
+
+        with pytest.raises(OSError):  # noqa: PT011
+            pipe.close()
+        assert mock_method.call_args_list == [call(mock_pipe)]
+        assert pipe.pipe is None
+
     def test_named_pipe(self):
         pipe = NamedPipeWindows()
         reader = ReadNamedPipeThreadWindows(pipe)
         reader.start()
         pipe.open()
         assert pipe.write(b"foo") == 3
         assert pipe.write(b"bar") == 3
```

### Comparing `streamlink-5.5.1/tests/utils/test_parse.py` & `streamlink-6.0.0/tests/utils/test_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import unittest
-
 import pytest
 from lxml.etree import Element
 
 from streamlink.exceptions import PluginError
 from streamlink.plugin.api import validate
 from streamlink.plugin.api.validate import xml_element
 from streamlink.utils.parse import parse_html, parse_json, parse_qsd, parse_xml
 
 
-class TestUtilsParse(unittest.TestCase):
+class TestUtilsParse:
     def test_parse_json(self):
         assert parse_json("{}") == {}
         assert parse_json('{"test": 1}') == {"test": 1}
         assert parse_json('{"test": 1}', schema=validate.Schema({"test": 1})) == {"test": 1}
         with pytest.raises(PluginError):
             parse_json("""{"test: 1}""")
         with pytest.raises(SyntaxError):
```

### Comparing `streamlink-5.5.1/tests/utils/test_processoutput.py` & `streamlink-6.0.0/tests/utils/test_processoutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import asyncio
 from collections import deque
 from typing import Iterable, Optional
+from unittest.mock import AsyncMock, Mock, call, patch
 
 import freezegun
 import pytest
 import pytest_asyncio
 
 from streamlink.utils.processoutput import ProcessOutput
 
 
-try:
-    from unittest.mock import AsyncMock, Mock, call, patch  # type: ignore
-except ImportError:
-    # noinspection PyUnresolvedReferences
-    from mock import AsyncMock, Mock, call, patch  # type: ignore
-
-
 class AsyncIterator:
     def __init__(self, event_loop: asyncio.BaseEventLoop, iterable: Optional[Iterable] = None):
         self._loop = event_loop
         self._deque = deque(iterable or ())
         self._newfuture()
 
     def append(self, item):
```

### Comparing `streamlink-5.5.1/tests/utils/test_times.py` & `streamlink-6.0.0/tests/utils/test_times.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.5.1/tests/utils/test_url.py` & `streamlink-6.0.0/tests/utils/test_url.py`

 * *Files identical despite different names*

