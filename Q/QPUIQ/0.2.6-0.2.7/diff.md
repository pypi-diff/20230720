# Comparing `tmp/QPUIQ-0.2.6.tar.gz` & `tmp/QPUIQ-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.2.6.tar", last modified: Mon Jul  3 05:53:56 2023, max compression
+gzip compressed data, was "QPUIQ-0.2.7.tar", last modified: Thu Jul 20 09:04:02 2023, max compression
```

## Comparing `QPUIQ-0.2.6.tar` & `QPUIQ-0.2.7.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-03 05:53:56.054374 QPUIQ-0.2.6/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.6/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     7847 2023-07-03 05:53:56.054049 QPUIQ-0.2.6/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-03 05:53:56.037642 QPUIQ-0.2.6/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-03 05:53:56.042108 QPUIQ-0.2.6/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      925 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      497 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     5783 2023-07-02 15:30:26.000000 QPUIQ-0.2.6/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      561 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2765 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     2327 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/combobox.py
--rw-r--r--   0 Bug        (504) staff       (20)     2200 2023-07-03 05:53:53.000000 QPUIQ-0.2.6/PUI/PySide6/dialog.py
--rw-r--r--   0 Bug        (504) staff       (20)     1032 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1561 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      801 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/mdi.py
--rw-r--r--   0 Bug        (504) staff       (20)     2802 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/menu.py
--rw-r--r--   0 Bug        (504) staff       (20)     4366 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/modal.py
--rw-r--r--   0 Bug        (504) staff       (20)      479 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      770 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     5566 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)      793 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/splitter.py
--rw-r--r--   0 Bug        (504) staff       (20)     1192 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/PySide6/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)     1706 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/text.py
--rw-r--r--   0 Bug        (504) staff       (20)     1508 2023-07-02 19:31:49.000000 QPUIQ-0.2.6/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     2032 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/PySide6/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      557 2023-07-03 05:53:53.000000 QPUIQ-0.2.6/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.6/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     3984 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-03 05:53:56.045656 QPUIQ-0.2.6/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      421 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      587 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.6/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      540 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2066 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      633 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1201 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      620 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      830 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     2212 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/flet/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1003 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)     1457 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/flet/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      838 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     5653 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)    13523 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/state.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-03 05:53:56.050072 QPUIQ-0.2.6/PUI/textual/
--rw-r--r--   0 Bug        (504) staff       (20)      685 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     2144 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2950 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      436 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      518 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/textual/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1536 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/textual/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      501 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      621 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     2158 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/textual/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     2280 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)      778 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/textual/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      785 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      380 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/textual/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.6/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-03 05:53:56.052795 QPUIQ-0.2.6/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      514 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     2602 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      467 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1127 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      741 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/checkbox.py
--rw-r--r--   0 Bug        (504) staff       (20)      554 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     2698 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      488 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/radiobutton.py
--rw-r--r--   0 Bug        (504) staff       (20)     6659 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/tkinter/scroll.py
--rw-r--r--   0 Bug        (504) staff       (20)     1743 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/tab.py
--rw-r--r--   0 Bug        (504) staff       (20)      493 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/tkinter/text.py
--rw-r--r--   0 Bug        (504) staff       (20)      862 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1548 2023-06-19 04:17:18.000000 QPUIQ-0.2.6/PUI/tkinter/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.6/PUI/utils.py
--rw-r--r--   0 Bug        (504) staff       (20)     3021 2023-06-30 19:44:46.000000 QPUIQ-0.2.6/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-03 05:53:56.053532 QPUIQ-0.2.6/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     7847 2023-07-03 05:53:55.000000 QPUIQ-0.2.6/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1695 2023-07-03 05:53:56.000000 QPUIQ-0.2.6/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-07-03 05:53:55.000000 QPUIQ-0.2.6/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-07-03 05:53:55.000000 QPUIQ-0.2.6/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     7587 2023-07-02 15:30:26.000000 QPUIQ-0.2.6/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-07-03 05:53:56.054474 QPUIQ-0.2.6/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.6/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-20 09:04:02.981771 QPUIQ-0.2.7/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-06-05 21:02:12.000000 QPUIQ-0.2.7/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     7872 2023-07-20 09:04:02.981630 QPUIQ-0.2.7/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-20 09:04:02.962805 QPUIQ-0.2.7/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-20 09:04:02.968299 QPUIQ-0.2.7/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)      946 2023-07-19 09:43:36.000000 QPUIQ-0.2.7/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      497 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5783 2023-07-02 15:30:26.000000 QPUIQ-0.2.7/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      561 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2765 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2327 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/combobox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2200 2023-07-03 05:53:53.000000 QPUIQ-0.2.7/PUI/PySide6/dialog.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1032 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1561 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      801 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/mdi.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2802 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/PySide6/menu.py
+-rw-r--r--   0 Bug        (504) staff       (20)     4366 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/PySide6/modal.py
+-rw-r--r--   0 Bug        (504) staff       (20)      479 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      770 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5723 2023-07-20 09:01:48.000000 QPUIQ-0.2.7/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      793 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/splitter.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1192 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/PySide6/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2012 2023-07-20 09:01:48.000000 QPUIQ-0.2.7/PUI/PySide6/table.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1706 2023-07-20 09:01:48.000000 QPUIQ-0.2.7/PUI/PySide6/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1521 2023-07-19 09:43:36.000000 QPUIQ-0.2.7/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2032 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/PySide6/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      557 2023-07-20 09:03:59.000000 QPUIQ-0.2.7/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      432 2023-06-05 21:02:12.000000 QPUIQ-0.2.7/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3984 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-20 09:04:02.971345 QPUIQ-0.2.7/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      421 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      587 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      848 2023-06-05 21:02:12.000000 QPUIQ-0.2.7/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      540 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2066 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      633 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1201 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      620 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      830 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2212 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/flet/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1003 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1457 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/flet/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      838 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     5661 2023-07-20 09:01:48.000000 QPUIQ-0.2.7/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)    14194 2023-07-20 09:01:48.000000 QPUIQ-0.2.7/PUI/state.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-20 09:04:02.974248 QPUIQ-0.2.7/PUI/textual/
+-rw-r--r--   0 Bug        (504) staff       (20)      685 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2144 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2950 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      436 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      518 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/textual/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1536 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/textual/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      501 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      621 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2158 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/textual/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2280 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)      778 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/textual/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      785 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      380 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/textual/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1005 2023-06-05 21:02:12.000000 QPUIQ-0.2.7/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-20 09:04:02.976445 QPUIQ-0.2.7/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      514 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2602 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      467 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1127 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      741 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/checkbox.py
+-rw-r--r--   0 Bug        (504) staff       (20)      554 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2698 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      750 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/radiobutton.py
+-rw-r--r--   0 Bug        (504) staff       (20)     6659 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1743 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/tab.py
+-rw-r--r--   0 Bug        (504) staff       (20)      493 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/tkinter/text.py
+-rw-r--r--   0 Bug        (504) staff       (20)      862 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1548 2023-06-19 04:17:18.000000 QPUIQ-0.2.7/PUI/tkinter/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      505 2023-06-05 21:02:12.000000 QPUIQ-0.2.7/PUI/utils.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3021 2023-06-30 19:44:46.000000 QPUIQ-0.2.7/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-07-20 09:04:02.981434 QPUIQ-0.2.7/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     7872 2023-07-20 09:04:02.000000 QPUIQ-0.2.7/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1716 2023-07-20 09:04:02.000000 QPUIQ-0.2.7/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-07-20 09:04:02.000000 QPUIQ-0.2.7/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-07-20 09:04:02.000000 QPUIQ-0.2.7/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     7612 2023-07-20 09:01:48.000000 QPUIQ-0.2.7/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-07-20 09:04:02.981812 QPUIQ-0.2.7/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-06-05 21:02:12.000000 QPUIQ-0.2.7/setup.py
```

### Comparing `QPUIQ-0.2.6/LICENSE.txt` & `QPUIQ-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PKG-INFO` & `QPUIQ-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.6
+Version: 0.2.7
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -200,14 +200,15 @@
 |ProgressBar|QProgressBar|ProgressBar|Progressbar|ProgressBar|
 |Scroll|QScrollArea|✓|✓|ScrollableContainer|
 |Text|QLabel|Text|Label|Text|
 |Html|QLabel|⚠ Text|⚠ Label|⚠ Text|
 |MarkDown|QLabel|Markdown|⚠ Label|Markdown|
 |Combobox|QComboBox|-|-|-|
 |ComboboxItem|✓|-|-|-|
+|Table|QTableView|-|-|-|
 |Tabs|QTabWidget|Tabs|Notebook|Tabs|
 |Tab|✓|Tab|✓|✓|
 |MenuBar|QMenuBar|-|-|-|
 |Menu|QMenu|-|-|-|
 |MenuAction|QAction|-|-|-|
 |MdiArea|QMdiArea|-|-|-|
 |MdiSubWindow|QMdiSubWindow|-|-|-|
```

### Comparing `QPUIQ-0.2.6/PUI/PySide6/__init__.py` & `QPUIQ-0.2.7/PUI/PySide6/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .label import *
 from .layout import *
 from .modal import *
 from .progressbar import *
 from .radiobutton import *
 from .scroll import *
 from .splitter import *
+from .table import *
 from .tab import *
 from .text import *
 from .textfield import *
 from .window import *
 from .mdi import *
 
 PUIView = QtPUIView
```

### Comparing `QPUIQ-0.2.6/PUI/PySide6/base.py` & `QPUIQ-0.2.7/PUI/PySide6/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/button.py` & `QPUIQ-0.2.7/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/canvas.py` & `QPUIQ-0.2.7/PUI/PySide6/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/checkbox.py` & `QPUIQ-0.2.7/PUI/PySide6/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/combobox.py` & `QPUIQ-0.2.7/PUI/PySide6/combobox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/dialog.py` & `QPUIQ-0.2.7/PUI/PySide6/dialog.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/label.py` & `QPUIQ-0.2.7/PUI/PySide6/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/layout.py` & `QPUIQ-0.2.7/PUI/PySide6/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/mdi.py` & `QPUIQ-0.2.7/PUI/PySide6/mdi.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/menu.py` & `QPUIQ-0.2.7/PUI/PySide6/menu.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/modal.py` & `QPUIQ-0.2.7/PUI/PySide6/modal.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/radiobutton.py` & `QPUIQ-0.2.7/PUI/PySide6/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/scroll.py` & `QPUIQ-0.2.7/PUI/PySide6/scroll.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .. import *
 from .base import *
+from PySide6.QtWidgets import QSizePolicy
 import math
 
 class Scroll(QtBaseWidget):
     terminal = False
     END = -0.0
 
     def __init__(self, vertical=None, horizontal=False):
@@ -52,14 +53,15 @@
     def addChild(self, idx, child):
         if idx != 0:
             return
         if isinstance(child, QtBaseWidget) or isinstance(child, QtBaseLayout):
             self.ui.setWidget(child.outer)
             if not hasattr(child.outer, "origResizeEvent"):
                 child.outer.origResizeEvent = child.outer.resizeEvent
+                child.outer.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Preferred))
             child.outer.resizeEvent = self.onUiResized
         elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if idx != 0:
             return
```

### Comparing `QPUIQ-0.2.6/PUI/PySide6/splitter.py` & `QPUIQ-0.2.7/PUI/PySide6/splitter.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/tab.py` & `QPUIQ-0.2.7/PUI/PySide6/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/text.py` & `QPUIQ-0.2.7/PUI/PySide6/text.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/PySide6/textfield.py` & `QPUIQ-0.2.7/PUI/PySide6/textfield.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         value = self.model.value
         if prev and prev.ui:
             self.editing = prev.editing
             self.ui = prev.ui
             self.ui.focusOutEvent = self.focusOutEvent
             if prev.last_value != value:
                 self.ui.textChanged.disconnect()
-                if not self.editing:
+                if not self.editing or not value:
                     self.ui.setText(str(value))
                 self.ui.textChanged.connect(self.on_textchanged)
             self.last_value = value
         else:
             self.last_value = value
             self.ui = QtWidgets.QLineEdit()
             self.ui.origFocusOutEvent = self.ui.focusOutEvent
```

### Comparing `QPUIQ-0.2.6/PUI/PySide6/window.py` & `QPUIQ-0.2.7/PUI/PySide6/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/__init__.py` & `QPUIQ-0.2.7/PUI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 from .node import *
 from .view import *
 from .state import *
 from .timeline import *
 from .decorator import *
```

### Comparing `QPUIQ-0.2.6/PUI/dom.py` & `QPUIQ-0.2.7/PUI/dom.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/application.py` & `QPUIQ-0.2.7/PUI/flet/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/base.py` & `QPUIQ-0.2.7/PUI/flet/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/button.py` & `QPUIQ-0.2.7/PUI/flet/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/canvas.py` & `QPUIQ-0.2.7/PUI/flet/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/checkbox.py` & `QPUIQ-0.2.7/PUI/flet/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/label.py` & `QPUIQ-0.2.7/PUI/flet/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/layout.py` & `QPUIQ-0.2.7/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/progressbar.py` & `QPUIQ-0.2.7/PUI/flet/progressbar.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/radiobutton.py` & `QPUIQ-0.2.7/PUI/flet/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/scroll.py` & `QPUIQ-0.2.7/PUI/flet/scroll.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/tab.py` & `QPUIQ-0.2.7/PUI/flet/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/text.py` & `QPUIQ-0.2.7/PUI/flet/text.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/textfield.py` & `QPUIQ-0.2.7/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/flet/window.py` & `QPUIQ-0.2.7/PUI/flet/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/node.py` & `QPUIQ-0.2.7/PUI/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
             self.root = self
 
         self.genKey()
 
         self.children = []
 
         if self.parent is self:
-            self.path = tuple()
+            self._path = tuple()
         else:
-            self.path = self.parent.path + tuple([len(self.parent.children)])
+            self._path = self.parent._path + tuple([len(self.parent.children)])
             self.parent.children.append(self)
 
-        # print(type(self).__name__, self.path, "parent=", self.parent.path)
+        # print(type(self).__name__, self._path, "parent=", self.parent._path)
 
     def genKey(self):
         # key has to be relative to PUIView, so that it can be identical when a sub-PUIView is updated individually
         self.key = "|".join([x.name or type(x).__name__ for x in self.root.frames]+[self.name or type(self).__name__]+[str(id(x)) for x in self.args])
         if self._tag:
             self.key += f"@{self._tag}"
 
@@ -134,40 +134,40 @@
         while node.retired_by:
             node = node.retired_by
         return node
 
     def __repr__(self):
         segs = []
         headline = [
-            "  "*len(self.path),
+            "  "*len(self._path),
             self.name or type(self).__name__,
             # f"@{str(id(self))}", # print view id
             " {",
         ]
 
         # print view key
         headline.append(" # ")
         headline.append(self.key)
 
         headline.append("\n")
         segs.append("".join(headline))
 
         comment = self.comment()
         if comment:
-            segs.append("  "*(len(self.path)+1))
+            segs.append("  "*(len(self._path)+1))
             segs.append("# ")
             segs.append(comment)
             segs.append("\n")
 
         for i,c in enumerate(self.children):
             if i > 0:
                 segs.append(",\n")
             segs.append(c.__repr__())
         segs.append("\n")
-        segs.append("".join(["  "*len(self.path), "}"]))
+        segs.append("".join(["  "*len(self._path), "}"]))
         return "".join(segs)
 
     def layout(self, width=None, height=None, weight=None, padding=None, margin=None):
         if not width is None:
             self.layout_width = width
         if not height is None:
             self.layout_height = height
```

### Comparing `QPUIQ-0.2.6/PUI/state.py` & `QPUIQ-0.2.7/PUI/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         getattr(self.state, "_StateObject__callbacks")[self.key].add(callback)
 
     def bind(self, getter, setter):
         getattr(self.state, "_StateObject__binders")[self.key] = None
         setattr(getattr(self.state, "_StateObject__values"), self.key, getter())
         getattr(self.state, "_StateObject__binders")[self.key] = (getter, setter)
 
+    def emit(self):
+        _notify(getattr(self.state, "_StateObject__listeners"))
+
 class ListBinding():
     def __init__(self, state, key):
         try:
             self.viewroot = find_puiview()
             self.viewparent = self.viewroot.frames[-1]
         except PuiViewNotFoundError:
             pass
@@ -77,14 +80,17 @@
         getattr(self.state, "_StateList__callbacks")[self.key].add(callback)
 
     def bind(self, getter, setter):
         getattr(self.state, "_StateList__binders")[self.key] = None
         self.state[self.key] = getter()
         getattr(self.state, "_StateList__binders")[self.key] = (getter, setter)
 
+    def emit(self):
+        _notify(getattr(self.state, "_StateList__listeners"))
+
 class DictBinding():
     def __init__(self, state, key):
         try:
             self.viewroot = find_puiview()
             self.viewparent = self.viewroot.frames[-1]
         except PuiViewNotFoundError:
             pass
@@ -115,14 +121,17 @@
         getattr(self.state, "_StateDict__callbacks")[self.key].add(callback)
 
     def bind(self, getter, setter):
         getattr(self.state, "_StateDict__binders")[self.key] = None
         self.state[self.key] = getter()
         getattr(self.state, "_StateDict__binders")[self.key] = (getter, setter)
 
+    def emit(self):
+        _notify(getattr(self.state, "_StateDict__listeners"))
+
 def _notify(listeners):
     tbd = []
     for l in listeners:
         if l.retired_by:
             tbd.append(l)
     for l in tbd:
         listeners.remove(l)
@@ -148,14 +157,19 @@
         self.__binders = {}
         if values is None:
             self.__values = BaseState()
         else:
             self.__values = values
 
     def __call__(self, key=None):
+        try:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
+            pass
         return AttrBinding(self, key)
 
     def __getattr__(self, key):
         if not key.startswith("_"):
             try:
                 view = find_puiview()
                 self.__listeners.add(view)
@@ -190,14 +204,19 @@
         self.__binders = {}
         if values is None:
             self.__values = []
         else:
             self.__values = values
 
     def __call__(self, key=None):
+        try:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
+            pass
         return ListBinding(self, key)
 
     def __getitem__(self, key):
         try:
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
@@ -346,14 +365,19 @@
         self.__binders = {}
         if values is None:
             self.__values = {}
         else:
             self.__values = values
 
     def __call__(self, key=None):
+        try:
+            view = find_puiview()
+            self.__listeners.add(view)
+        except PuiViewNotFoundError:
+            pass
         return DictBinding(self, key)
 
     def __delitem__(self, key):
         self.__values.__delitem__(key)
         _notify(self.__listeners)
         for cb in self.__callbacks[None]:
             cb(self.__values)
```

### Comparing `QPUIQ-0.2.6/PUI/textual/__init__.py` & `QPUIQ-0.2.7/PUI/textual/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/application.py` & `QPUIQ-0.2.7/PUI/textual/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/base.py` & `QPUIQ-0.2.7/PUI/textual/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/checkbox.py` & `QPUIQ-0.2.7/PUI/textual/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/label.py` & `QPUIQ-0.2.7/PUI/textual/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/layout.py` & `QPUIQ-0.2.7/PUI/textual/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/radiobutton.py` & `QPUIQ-0.2.7/PUI/textual/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/scroll.py` & `QPUIQ-0.2.7/PUI/textual/scroll.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/tab.py` & `QPUIQ-0.2.7/PUI/textual/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/text.py` & `QPUIQ-0.2.7/PUI/textual/text.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/textual/textfield.py` & `QPUIQ-0.2.7/PUI/textual/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/timeline.py` & `QPUIQ-0.2.7/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/__init__.py` & `QPUIQ-0.2.7/PUI/tkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/application.py` & `QPUIQ-0.2.7/PUI/tkinter/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/base.py` & `QPUIQ-0.2.7/PUI/tkinter/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/canvas.py` & `QPUIQ-0.2.7/PUI/tkinter/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/checkbox.py` & `QPUIQ-0.2.7/PUI/tkinter/checkbox.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/label.py` & `QPUIQ-0.2.7/PUI/tkinter/label.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/layout.py` & `QPUIQ-0.2.7/PUI/tkinter/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/radiobutton.py` & `QPUIQ-0.2.7/PUI/tkinter/radiobutton.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/scroll.py` & `QPUIQ-0.2.7/PUI/tkinter/scroll.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/tab.py` & `QPUIQ-0.2.7/PUI/tkinter/tab.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/textfield.py` & `QPUIQ-0.2.7/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/tkinter/window.py` & `QPUIQ-0.2.7/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/PUI/view.py` & `QPUIQ-0.2.7/PUI/view.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.2.6/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.2.7/QPUIQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.2.6
+Version: 0.2.7
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -200,14 +200,15 @@
 |ProgressBar|QProgressBar|ProgressBar|Progressbar|ProgressBar|
 |Scroll|QScrollArea|✓|✓|ScrollableContainer|
 |Text|QLabel|Text|Label|Text|
 |Html|QLabel|⚠ Text|⚠ Label|⚠ Text|
 |MarkDown|QLabel|Markdown|⚠ Label|Markdown|
 |Combobox|QComboBox|-|-|-|
 |ComboboxItem|✓|-|-|-|
+|Table|QTableView|-|-|-|
 |Tabs|QTabWidget|Tabs|Notebook|Tabs|
 |Tab|✓|Tab|✓|✓|
 |MenuBar|QMenuBar|-|-|-|
 |Menu|QMenu|-|-|-|
 |MenuAction|QAction|-|-|-|
 |MdiArea|QMdiArea|-|-|-|
 |MdiSubWindow|QMdiSubWindow|-|-|-|
```

### Comparing `QPUIQ-0.2.6/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.2.7/QPUIQ.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 PUI/PySide6/menu.py
 PUI/PySide6/modal.py
 PUI/PySide6/progressbar.py
 PUI/PySide6/radiobutton.py
 PUI/PySide6/scroll.py
 PUI/PySide6/splitter.py
 PUI/PySide6/tab.py
+PUI/PySide6/table.py
 PUI/PySide6/text.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
 PUI/flet/__init__.py
 PUI/flet/application.py
 PUI/flet/base.py
 PUI/flet/button.py
```

### Comparing `QPUIQ-0.2.6/README.md` & `QPUIQ-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 |ProgressBar|QProgressBar|ProgressBar|Progressbar|ProgressBar|
 |Scroll|QScrollArea|✓|✓|ScrollableContainer|
 |Text|QLabel|Text|Label|Text|
 |Html|QLabel|⚠ Text|⚠ Label|⚠ Text|
 |MarkDown|QLabel|Markdown|⚠ Label|Markdown|
 |Combobox|QComboBox|-|-|-|
 |ComboboxItem|✓|-|-|-|
+|Table|QTableView|-|-|-|
 |Tabs|QTabWidget|Tabs|Notebook|Tabs|
 |Tab|✓|Tab|✓|✓|
 |MenuBar|QMenuBar|-|-|-|
 |Menu|QMenu|-|-|-|
 |MenuAction|QAction|-|-|-|
 |MdiArea|QMdiArea|-|-|-|
 |MdiSubWindow|QMdiSubWindow|-|-|-|
```

### Comparing `QPUIQ-0.2.6/setup.py` & `QPUIQ-0.2.7/setup.py`

 * *Files identical despite different names*

