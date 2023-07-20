# Comparing `tmp/survey-4.5.2.tar.gz` & `tmp/survey-4.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-4.5.2.tar", last modified: Tue Jul 18 08:45:11 2023, max compression
+gzip compressed data, was "survey-4.5.3.tar", last modified: Thu Jul 20 20:10:26 2023, max compression
```

## Comparing `survey-4.5.2.tar` & `survey-4.5.3.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 08:44:57.000000 survey-4.5.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-18 08:44:57.000000 survey-4.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 08:44:57.000000 survey-4.5.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 08:44:57.000000 survey-4.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-18 08:45:11.228669 survey-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-18 08:44:57.000000 survey-4.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-18 08:44:57.000000 survey-4.5.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.224670 survey-4.5.2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/graphics.lineprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/graphics.spinprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/printers.done-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/printers.fail-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/printers.info-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    92650 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.basket-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    64730 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.basket-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.conceal-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.datetime-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.datetime-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    52677 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.form-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.input-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.input-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.inquire-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.numeric-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.numeric-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    27647 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.select-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    39313 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.select-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)   472099 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/showcase-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)   121555 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/showcase-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-18 08:44:57.000000 survey-4.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-18 08:44:57.000000 survey-4.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 08:44:57.000000 survey-4.5.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 08:44:57.000000 survey-4.5.2/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:45:11.228669 survey-4.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-18 08:44:57.000000 survey-4.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/survey/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-18 08:44:57.000000 survey-4.5.2/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    58184 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.756712 survey-4.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.740712 survey-4.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.744712 survey-4.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 20:10:06.000000 survey-4.5.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-20 20:10:06.000000 survey-4.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 20:10:06.000000 survey-4.5.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-20 20:10:06.000000 survey-4.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-20 20:10:26.752712 survey-4.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-20 20:10:06.000000 survey-4.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.744712 survey-4.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 20:10:06.000000 survey-4.5.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.740712 survey-4.5.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.748712 survey-4.5.3/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/graphics.lineprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/graphics.spinprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/printers.done-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/printers.fail-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/printers.info-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    92650 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.basket-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    64730 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.basket-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.conceal-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.datetime-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.datetime-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    52677 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.form-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.input-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.input-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.inquire-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.numeric-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.numeric-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    27647 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.select-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    39313 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/routines.select-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   472099 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/showcase-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   121555 2023-07-20 20:10:06.000000 survey-4.5.3/docs/_static/images/showcase-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-20 20:10:06.000000 survey-4.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 20:10:06.000000 survey-4.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 20:10:06.000000 survey-4.5.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-20 20:10:06.000000 survey-4.5.3/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 20:10:26.756712 survey-4.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 20:10:06.000000 survey-4.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.752712 survey-4.5.3/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-20 20:10:06.000000 survey-4.5.3/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.752712 survey-4.5.3/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58184 2023-07-20 20:10:06.000000 survey-4.5.3/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:10:26.752712 survey-4.5.3/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 20:10:26.000000 survey-4.5.3/survey.egg-info/top_level.txt
```

### Comparing `survey-4.5.2/.github/workflows/publish.yml` & `survey-4.5.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/.gitignore` & `survey-4.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/LICENSE` & `survey-4.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/PKG-INFO` & `survey-4.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.5.2
+Version: 4.5.3
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.5.2/README.rst` & `survey-4.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/Makefile` & `survey-4.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/graphics.lineprogress-1.gif` & `survey-4.5.3/docs/_static/images/graphics.lineprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/graphics.spinprogress-1.gif` & `survey-4.5.3/docs/_static/images/graphics.spinprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/printers.done-1.png` & `survey-4.5.3/docs/_static/images/printers.done-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/printers.fail-1.png` & `survey-4.5.3/docs/_static/images/printers.fail-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/printers.info-1.png` & `survey-4.5.3/docs/_static/images/printers.info-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.basket-1.gif` & `survey-4.5.3/docs/_static/images/routines.basket-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.basket-2.gif` & `survey-4.5.3/docs/_static/images/routines.basket-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.conceal-1.gif` & `survey-4.5.3/docs/_static/images/routines.conceal-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.datetime-1.gif` & `survey-4.5.3/docs/_static/images/routines.datetime-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.datetime-2.gif` & `survey-4.5.3/docs/_static/images/routines.datetime-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.form-1.gif` & `survey-4.5.3/docs/_static/images/routines.form-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.input-1.gif` & `survey-4.5.3/docs/_static/images/routines.input-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.input-2.gif` & `survey-4.5.3/docs/_static/images/routines.input-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.inquire-1.gif` & `survey-4.5.3/docs/_static/images/routines.inquire-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.numeric-1.gif` & `survey-4.5.3/docs/_static/images/routines.numeric-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.numeric-2.gif` & `survey-4.5.3/docs/_static/images/routines.numeric-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.select-1.gif` & `survey-4.5.3/docs/_static/images/routines.select-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/routines.select-2.gif` & `survey-4.5.3/docs/_static/images/routines.select-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/showcase-1.gif` & `survey-4.5.3/docs/_static/images/showcase-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/_static/images/showcase-2.gif` & `survey-4.5.3/docs/_static/images/showcase-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/conf.py` & `survey-4.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/index.rst` & `survey-4.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/make.bat` & `survey-4.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/docs/reference.rst` & `survey-4.5.3/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/setup.py` & `survey-4.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/__init__.py` & `survey-4.5.3/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_colors.py` & `survey-4.5.3/survey/_colors.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_controls.py` & `survey-4.5.3/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/__init__.py` & `survey-4.5.3/survey/_core/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 from . import _ansi as ansi
 
 from ._io     import IO
+from ._intel  import Intel
 from ._cursor import Cursor, ClearMode, EraseMode
 from ._source import Source, Event
 from ._handle import Handle, Terminate
 from ._render import Render
 from ._screen import Screen
 
 from ._console import Console, SkipDraw
@@ -14,10 +15,10 @@
 from ._render import _type_Render_draw_lines, _type_Render_draw_point
 from ._screen import _type_Screen_draw_sketch
 from ._handle import _type_Handle_start_invoke
 
 
 __all__ = (
     'ansi', 
-    'IO', 'Cursor', 'ClearMode', 'EraseMode', 'Source', 'Event', 'Render', 'Screen', 'Handle', 'Terminate', 
+    'IO', 'Intel', 'Cursor', 'ClearMode', 'EraseMode', 'Source', 'Event', 'Render', 'Screen', 'Handle', 'Terminate', 
     'Console', 'SkipDraw'
 )
```

### Comparing `survey-4.5.2/survey/_core/_ansi.py` & `survey-4.5.3/survey/_core/_ansi.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_console.py` & `survey-4.5.3/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_cursor.py` & `survey-4.5.3/survey/_core/_cursor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 import enum
 import threading
 
 from . import _helpers
 from . import _ansi
-from . import _io
+from . import _intel
 
 
 __all__ = ('ClearMode', 'EraseMode', 'Cursor')
 
 
 class ClearMode(enum.IntEnum):
 
@@ -50,30 +50,31 @@
     Emulates the on-screen cursor.
 
     .. note::
 
         Coordinates here are ``1``-offset indexes, meaning they start from 1. 
         The position of the cursor on the top-left-most of the screen is :code:`(1, 1)`.
         
-    :param io:
-        Used for sending ANSI sequences to output.
+    :parma intel:
+        Used for fetching parsed items from input and sending to output.
 
     .. code-block:: python
     
         io = IO(sys.stdin, sys.stdout)
-        cursor = Cursor(io)
+        intel = Intel(io)
+        cursor = Cursor(intel)
         location = cursor.locate()
     """
 
-    __slots__ = ('_lock', '_hidden', '_io')
+    __slots__ = ('_intel', '_hidden', '_lock')
 
     def __init__(self, 
-                 io: _io.IO):
+                 intel: _intel.Intel):
 
-        self._io = io
+        self._intel = intel
 
         self._hidden = _helpers.Atomic(self.hide, self.show)
 
         self._lock = threading.RLock()
 
     @property
     def hidden(self):
@@ -85,22 +86,21 @@
 
             with cursor.hidden:
                 ...
         """
 
         return self._hidden
 
-    @_helpers.ctxmethod(lambda self: self._io)
     def _send(self, *args, escape = False, **kwargs):
 
         function = _ansi.get_escape if escape else _ansi.get_control
 
         value = function(*args, **kwargs)
 
-        self._io.send(value)
+        self._intel.send(value)
 
     def _up(self, size):
 
         self._send('A', size)
 
     def up(self, size: typing.Union[int, None] = None):
 
@@ -295,25 +295,23 @@
         """
         Become visible.
         """
 
         self._show()
 
     @_helpers.ctxmethod(lambda self: self._lock)
-    @_helpers.ctxmethod(lambda self: self._io)
     def _locate(self):
 
         self._send('n', '6')
-        
-        while True:
-            code = _ansi.parse(self._io.recv)
-            if not isinstance(code, _ansi.Sequence) and code.rune == 'R':
-                continue
-            break
 
+        def check(code):
+            return isinstance(code, _ansi.Sequence) and code.rune == 'R'
+        
+        code = self._intel.read(check = check)
+    
         point = tuple(map(int, code.args))
 
         return point
 
     def locate(self) -> typing.Tuple[int, int]:
 
         """
```

### Comparing `survey-4.5.2/survey/_core/_handle.py` & `survey-4.5.3/survey/_core/_handle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
 from . import _helpers
-from . import _io
+from . import _intel
 from . import _ansi
 from . import _source
 
 
 __all__ = ('Terminate', 'Handle')
 
 
@@ -21,25 +21,24 @@
     
 class Handle:
 
     """
     Encapsulates the invokation loop logic.
     """
 
-    __slots__ = ('_io',)
+    __slots__ = ('_intel',)
 
     def __init__(self, 
-                 io: _io.IO):
+                 intel: _intel.Intel):
 
-        self._io = io
+        self._intel = intel
 
-    @_helpers.ctxmethod(lambda self: self._io)
     def _start(self, invoke):
 
-        source = _source.Source(invoke, self._io)
+        source = _source.Source(invoke, self._intel)
 
         try:
             source.listen()
         except Terminate:
             pass
 
     def start(self,
```

### Comparing `survey-4.5.2/survey/_core/_helpers.py` & `survey-4.5.3/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_io.py` & `survey-4.5.3/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_io_os.py` & `survey-4.5.3/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_io_os_nt.py` & `survey-4.5.3/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_io_os_posix.py` & `survey-4.5.3/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_render.py` & `survey-4.5.3/survey/_core/_render.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import threading
 import weakref
 
 from . import _helpers
 from . import _constants
 from . import _ansi
 from . import _cursor
-from . import _io
+from . import _intel
 
 
 __all__ = ('Render',)
 
 
 def _get_line_wrap_y(limit: int, 
                      size: int):
@@ -99,50 +99,51 @@
     Assists with printing text in a predictible way.
 
     .. note::
         In contrast to how :class:`.Cursor` works, point coordinates here are 0-offset indexes.
     
     :param cursor:
         Used for moving and clearing.
-    :param io:
+    :param intel:
         Used for sending to the output.
 
     .. code-block:: python
     
         io = IO(sys.stdin, sys.stdout)
-        cursor = Cursor(io)
-        render = Render(cursor, io)
+        intel = Intel(io)
+        cursor = Cursor(intel)
+        render = Render(cursor, intel)
         # draw "Hello\\nWorld" and place cursor between "r" and "l".
         render.draw([['H', 'e', 'l', 'l', 'o'], ['W', 'o', 'r', 'l', 'd']], [1, 3])
     """
 
     _history = weakref.WeakSet()
 
     _style_reset = _ansi.get_control('m', 0)
 
-    __slots__ = ('_io', '_cursor', '_memory', '_lock')
+    __slots__ = ('_intel', '_cursor', '_memory', '_lock')
 
     def __init__(self,
                  cursor: _cursor.Cursor, 
-                 io: _io.IO):
+                 intel: _intel.Intel):
 
-        self._io = io
+        self._intel = intel
         self._cursor = cursor
         self._memory = None
         
         self._lock = threading.Lock()
     
     @property
-    def io(self) -> _io.IO:
+    def intel(self) -> _intel.Intel:
 
         """
-        The io used for sending text.
+        The intel used for sending text.
         """
 
-        return self._io
+        return self._intel
     
     @property
     def cursor(self) -> _cursor.Cursor:
 
         """
         The cursor used for positioning the cursor and fetching coordinate information.
         """
@@ -158,17 +159,17 @@
 
         return self._memory
 
     def _send(self, clean, lines):
         
         for index, line in enumerate(lines):
             if index:
-                self._io.send(_constants.linesep)
+                self._intel.send(_constants.linesep)
             text = ''.join(line)
-            self._io.send(text)
+            self._intel.send(text)
             if clean:
                 self._cursor.erase()
 
     def _move(self, sizes, cur_y, cur_x, max_x, point):
 
         usr_y, usr_x = point
 
@@ -177,26 +178,23 @@
         usr_y, usr_x = _get_point_wrap(max_x, sizes, usr_y, usr_x)
 
         usr_y += cur_y
         
         self._cursor.move(usr_y, usr_x)
 
     @_helpers.ctxmethod(lambda self: self._lock)
-    @_helpers.ctxmethod(lambda self: self._io)
     def _draw(self, learn, clean, lines, point):
 
         lines = tuple(map(tuple, lines))
 
         cur_y, cur_x = self._cursor.locate()
         max_y, max_x = self._cursor.measure()
 
-        self._io.send(self._style_reset)
+        self._intel.send(self._style_reset)
 
-        # does not make sense not
-        # to clean each lines end
         self._send(True, lines)
 
         if clean:
             self._cursor.clear()
 
         sizes = list(map(len, lines))
```

### Comparing `survey-4.5.2/survey/_core/_screen.py` & `survey-4.5.3/survey/_core/_screen.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_core/_source.py` & `survey-4.5.3/survey/_core/_source.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing
 import enum
 import threading
 
 from . import _helpers
 from . import _ansi
-from . import _io
+from . import _intel
 
 
 __all__ = ('Source', 'Event')
 
 
 class EventType(enum.Enum):
 
@@ -60,65 +60,29 @@
 class Source:
 
     """
     Translates incoming ANSI sequences to events and calls back with relevant information.
 
     :param callback:
         Called with ``(name, info)`` upon receiving and translating.
-    :param io:
+    :param intel:
         Used for receiving from input.
     """
 
-    __slots__ = ('_callback', '_io', '_lock', '_buffer')
+    __slots__ = ('_callback', '_intel', '_lock')
 
     def __init__(self, 
                  callback: _type_Source_init_callback, 
-                 io: _io.IO):
+                 intel   : _intel.Intel):
 
         self._callback = callback
-        self._io = io
+        self._intel = intel
 
         self._lock = threading.RLock()
 
-        self._buffer = []
-
-    def _read(self):
-
-        if self._buffer:
-            return
-        
-        text = self._io.recv()
-
-        if text == '\x1b':
-            return
-
-        self._buffer.extend(text)
-        
-    def _get(self):
-
-        self._read()
-
-        try:
-            rune = self._buffer.pop(0)
-        except IndexError:
-            raise _EmptyRead()
-
-        return rune
-    
-    _empty = _ansi.Escape('')
-
-    def _next(self):
-
-        try:
-            code = _ansi.parse(self._get)
-        except _EmptyRead:
-            code = self._empty
-
-        return code
-
     _group = {
         EventType.control: {
             '\x7f': Event.delete_left,
             '\x08': Event.delete_right,
             '\x0d': Event.enter,
             '\x09': Event.indent
         },
@@ -166,19 +130,18 @@
                 return
         
         self._callback(name, info)
 
     @_helpers.ctxmethod(lambda self: self._lock)
     def _advance(self):
 
-        info = self._next()
+        info = self._intel.read()
 
         self._process(info)
 
-    _helpers.ctxmethod(lambda self: self._io)
     def _listen(self):
 
         while True:
             self._advance()
 
     def listen(self):
```

### Comparing `survey-4.5.2/survey/_funnels.py` & `survey-4.5.3/survey/_funnels.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_graphics.py` & `survey-4.5.3/survey/_graphics.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_handle.py` & `survey-4.5.3/survey/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_helpers.py` & `survey-4.5.3/survey/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_mutates.py` & `survey-4.5.3/survey/_mutates.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_printers.py` & `survey-4.5.3/survey/_printers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_routines.py` & `survey-4.5.3/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_searches.py` & `survey-4.5.3/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_stage.py` & `survey-4.5.3/survey/_stage.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_theme.py` & `survey-4.5.3/survey/_theme.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_utils.py` & `survey-4.5.3/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_visuals.py` & `survey-4.5.3/survey/_visuals.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey/_widgets.py` & `survey-4.5.3/survey/_widgets.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.2/survey.egg-info/PKG-INFO` & `survey-4.5.3/survey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.5.2
+Version: 4.5.3
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.5.2/survey.egg-info/SOURCES.txt` & `survey-4.5.3/survey.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 survey/_core/__init__.py
 survey/_core/_ansi.py
 survey/_core/_console.py
 survey/_core/_constants.py
 survey/_core/_cursor.py
 survey/_core/_handle.py
 survey/_core/_helpers.py
+survey/_core/_intel.py
 survey/_core/_io.py
 survey/_core/_io_os.py
 survey/_core/_io_os_nt.py
 survey/_core/_io_os_posix.py
 survey/_core/_render.py
 survey/_core/_screen.py
 survey/_core/_source.py
```

