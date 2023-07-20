# Comparing `tmp/cubicweb-web-1.2.0.tar.gz` & `tmp/cubicweb-web-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-web-1.2.0.tar", last modified: Tue Jul 11 15:30:14 2023, max compression
+gzip compressed data, was "cubicweb-web-1.2.1.tar", last modified: Thu Jul 20 13:07:04 2023, max compression
```

## Comparing `cubicweb-web-1.2.0.tar` & `cubicweb-web-1.2.1.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.982829 cubicweb-web-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1208 2023-07-11 15:30:14.982829 cubicweb-web-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.754826 cubicweb-web-1.2.0/cubicweb_web/
--rw-rw-rw-   0 root         (0) root         (0)     2821 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/action.py
--rw-rw-rw-   0 root         (0) root         (0)    21197 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/application.py
--rw-rw-rw-   0 root         (0) root         (0)     6976 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/box.py
--rw-rw-rw-   0 root         (0) root         (0)    21362 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/bwcompat.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/captcha.py
--rw-rw-rw-   0 root         (0) root         (0)     4834 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/ccplugin.py
--rw-rw-rw-   0 root         (0) root         (0)    29090 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/component.py
--rw-rw-rw-   0 root         (0) root         (0)     8635 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.826827 cubicweb-web-1.2.0/cubicweb_web/data/
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/accessories-text-editor.png
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/add_button.png
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/asc.gif
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/banner.png
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/bg.gif
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/bg_trame_grise.png
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/black-check.png
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/black-uncheck.png
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/bullet.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/bullet_orange.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/button.png
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/calendar.gif
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cancel.png
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/contextFreeBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/contextualBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/critical.png
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.acl.css
--rw-rw-rw-   0 root         (0) root         (0)     3589 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.ajax.box.js
--rw-rw-rw-   0 root         (0) root         (0)    24133 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.ajax.js
--rw-rw-rw-   0 root         (0) root         (0)     7895 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.calendar.css
--rw-rw-rw-   0 root         (0) root         (0)     9665 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.calendar.js
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.calendar_popup.css
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.compat.js
--rw-rw-rw-   0 root         (0) root         (0)    18494 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.css
--rw-rw-rw-   0 root         (0) root         (0)    18779 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.edition.js
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.facets.css
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.facets.js
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.fckcwconfig-full.js
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.fckcwconfig.js
--rw-rw-rw-   0 root         (0) root         (0)     1505 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.flot.js
--rw-rw-rw-   0 root         (0) root         (0)     3811 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.form.css
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.html_tree.css
--rw-rw-rw-   0 root         (0) root         (0)     4595 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.htmlhelpers.js
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.ie.css
--rw-rw-rw-   0 root         (0) root         (0)     1318 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.image.js
--rw-rw-rw-   0 root         (0) root         (0)    12621 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.js
--rw-rw-rw-   0 root         (0) root         (0)     1975 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.log.css
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.log.js
--rw-rw-rw-   0 root         (0) root         (0)     1756 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.login.css
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.manageview.css
--rw-rw-rw-   0 root         (0) root         (0)    16860 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.pictograms.css
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.preferences.css
--rw-rw-rw-   0 root         (0) root         (0)     4559 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.preferences.js
--rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.print.css
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.python.js
--rw-rw-rw-   0 root         (0) root         (0)     2754 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.reledit.js
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.schema.css
--rw-rw-rw-   0 root         (0) root         (0)      756 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.suggest.css
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.tablesorter.css
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.tableview.css
--rw-rw-rw-   0 root         (0) root         (0)     2901 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.timetable.css
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.treeview.css
--rw-rw-rw-   0 root         (0) root         (0)    19668 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.widgets.js
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/desc.gif
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/download.gif
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/dublincore-button.png
--rw-rw-rw-   0 root         (0) root         (0)     2179 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/dublincore-icon.png
--rw-rw-rw-   0 root         (0) root         (0)    67968 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/entypo.eot
--rw-rw-rw-   0 root         (0) root         (0)    97203 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/entypo.svg
--rw-rw-rw-   0 root         (0) root         (0)    67680 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/entypo.ttf
--rw-rw-rw-   0 root         (0) root         (0)    42064 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/entypo.woff
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/error.png
--rw-rw-rw-   0 root         (0) root         (0)    42086 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/excanvas.js
--rw-rw-rw-   0 root         (0) root         (0)    34494 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     5468 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/feed-icon.png
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/feed-icon16x16.png
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/feed-icon32x32.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/file.gif
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/folder-closed.gif
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/folder.gif
--rw-rw-rw-   0 root         (0) root         (0)    11147 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   151629 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.locale.js
--rw-rw-rw-   0 root         (0) root         (0)    51213 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.min.js
--rw-rw-rw-   0 root         (0) root         (0)      668 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.print.css
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/go.png
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/go_next.png
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/go_prev.png
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/gradient-grey-up.png
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/gradient-grey.gif
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/help.png
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/help_ie.png
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/icon_blank.png
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/icon_bookmark.gif
--rw-rw-rw-   0 root         (0) root         (0)      401 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/icon_emailaddress.gif
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/icon_euser.gif
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/icon_map.png
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/icon_state.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.834827 cubicweb-web-1.2.0/cubicweb_web/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/animated-overlay.gif
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_flat_75_ffffff_40x100.png
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_glass_65_ffffff_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_glass_75_dadada_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-rw-rw-   0 root         (0) root         (0)     3824 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_222222_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_454545_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_888888_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/incontextBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/information.png
--rw-rw-rw-   0 root         (0) root         (0)    16621 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-migrate.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.838827 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/
--rw-rw-rw-   0 root         (0) root         (0)     1772 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/changelog.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.846827 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/file.gif
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/folder-closed.gif
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/folder.gif
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/minus.gif
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/plus.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-black.gif
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-default.gif
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-gray.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-red.gif
--rw-rw-rw-   0 root         (0) root         (0)     2946 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.css
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js
--rw-rw-rw-   0 root         (0) root         (0)     8065 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.js
--rw-rw-rw-   0 root         (0) root         (0)    13015 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js
--rw-rw-rw-   0 root         (0) root         (0)     1563 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/readme.md
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)     1536 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.cookie.js
--rw-rw-rw-   0 root         (0) root         (0)    89666 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.flot.js
--rw-rw-rw-   0 root         (0) root         (0)   273199 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    85184 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.qtip.js
--rw-rw-rw-   0 root         (0) root         (0)    38404 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.qtip.min.js
--rw-rw-rw-   0 root         (0) root         (0)    41257 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.tablesorter.js
--rw-rw-rw-   0 root         (0) root         (0)     8760 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.timePicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.timepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    32456 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.css
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.datepicker-de.js
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.datepicker-es.js
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.datepicker-fr.js
--rw-rw-rw-   0 root         (0) root         (0)   435844 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.js
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/liveclipboard-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     2606 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/loading.gif
--rw-rw-rw-   0 root         (0) root         (0)     9083 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb-gray.svg
--rw-rw-rw-   0 root         (0) root         (0)     3438 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb-icon.svg
--rw-rw-rw-   0 root         (0) root         (0)     7325 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb-text.svg
--rw-rw-rw-   0 root         (0) root         (0)     9202 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)     2775 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/logo-logilab.png
--rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/logo.png
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/microformats-button.png
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/microformats-icon.png
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/minus.gif
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/no-check-no-border.png
--rw-rw-rw-   0 root         (0) root         (0)      537 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/ok.png
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/pen_icon.png
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/plus.gif
--rw-rw-rw-   0 root         (0) root         (0)      443 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/plus.png
--rw-rw-rw-   0 root         (0) root         (0)    79752 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/porkys.ttf
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/puce.png
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/puce_down.png
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/puce_down_black.png
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/puce_up.png
--rw-rw-rw-   0 root         (0) root         (0)     3151 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/pygments.css
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/required.png
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/rss-button.png
--rw-rw-rw-   0 root         (0) root         (0)      288 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/rss.png
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/search.png
--rw-rw-rw-   0 root         (0) root         (0)      959 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/sendcancel.png
--rw-rw-rw-   0 root         (0) root         (0)     1257 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/sendok.png
--rw-rw-rw-   0 root         (0) root         (0)     1279 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/trash_can.png
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/trash_can_small.png
--rw-rw-rw-   0 root         (0) root         (0)    27374 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/ui.all.css
--rw-rw-rw-   0 root         (0) root         (0)     5055 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/up.gif
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/data/upload.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.846827 cubicweb-web-1.2.0/cubicweb_web/devtools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/devtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39352 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/devtools/testlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.846827 cubicweb-web-1.2.0/cubicweb_web/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17396 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/ext/rest.py
--rw-rw-rw-   0 root         (0) root         (0)    69654 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/facet.py
--rw-rw-rw-   0 root         (0) root         (0)    11044 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/form.py
--rw-rw-rw-   0 root         (0) root         (0)    49324 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/formfields.py
--rw-rw-rw-   0 root         (0) root         (0)    42471 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)    11249 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/htmlwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)    55646 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/http_headers.py
--rw-rw-rw-   0 root         (0) root         (0)     6189 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/httpcache.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     4971 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/propertysheet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.850827 cubicweb-web-1.2.0/cubicweb_web/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/pyramid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/pyramid/login.py
--rw-rw-rw-   0 root         (0) root         (0)     1803 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/pyramid/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     5584 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/pyramid/test.py
--rw-rw-rw-   0 root         (0) root         (0)     3915 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/pyramid/url_redirection.py
--rw-rw-rw-   0 root         (0) root         (0)    40224 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/request.py
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/schemaviewer.py
--rw-rw-rw-   0 root         (0) root         (0)     6699 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/uihelper.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19979 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.882828 cubicweb-web-1.2.0/cubicweb_web/views/
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/_vid_by_mimetype.py
--rw-rw-rw-   0 root         (0) root         (0)    14788 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    16562 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/ajaxcontroller.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/ajaxedit.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/apacherewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     6730 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)    46301 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/autoform.py
--rw-rw-rw-   0 root         (0) root         (0)     8971 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/basecomponents.py
--rw-rw-rw-   0 root         (0) root         (0)    11545 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/basecontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)    22595 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     6017 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     9230 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     9783 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     4352 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/csvexport.py
--rw-rw-rw-   0 root         (0) root         (0)    17032 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/cwproperties.py
--rw-rw-rw-   0 root         (0) root         (0)    16247 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/cwsources.py
--rw-rw-rw-   0 root         (0) root         (0)    10516 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/cwuser.py
--rw-rw-rw-   0 root         (0) root         (0)     7008 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     2465 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/dotgraphview.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/edit_attributes.pt
--rw-rw-rw-   0 root         (0) root         (0)    20973 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/editcontroller.py
--rw-rw-rw-   0 root         (0) root         (0)    12498 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/editforms.py
--rw-rw-rw-   0 root         (0) root         (0)     4687 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/editviews.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/emailaddress.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/error.py
--rw-rw-rw-   0 root         (0) root         (0)    16347 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/facets.py
--rw-rw-rw-   0 root         (0) root         (0)    20026 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/formrenderers.py
--rw-rw-rw-   0 root         (0) root         (0)    18194 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     7798 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/ibreadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     8266 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/idownloadable.py
--rw-rw-rw-   0 root         (0) root         (0)     5584 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/json.py
--rw-rw-rw-   0 root         (0) root         (0)    16883 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/magicsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     9042 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/management.py
--rw-rw-rw-   0 root         (0) root         (0)    17293 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     9023 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/owl.py
--rw-rw-rw-   0 root         (0) root         (0)     4632 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/plots.py
--rw-rw-rw-   0 root         (0) root         (0)    18367 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/primary.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/pyviews.py
--rw-rw-rw-   0 root         (0) root         (0)     5345 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/rdf.py
--rw-rw-rw-   0 root         (0) root         (0)    22006 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/reledit.py
--rw-rw-rw-   0 root         (0) root         (0)    29416 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/searchrestriction.py
--rw-rw-rw-   0 root         (0) root         (0)     7050 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)     7293 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/startup.py
--rw-rw-rw-   0 root         (0) root         (0)    11217 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/staticcontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)    48960 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/tableview.py
--rw-rw-rw-   0 root         (0) root         (0)     9630 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     8971 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/timetable.py
--rw-rw-rw-   0 root         (0) root         (0)    12731 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/treeview.py
--rw-rw-rw-   0 root         (0) root         (0)    29932 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/uicfg.py
--rw-rw-rw-   0 root         (0) root         (0)     8479 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/undohistory.py
--rw-rw-rw-   0 root         (0) root         (0)    16430 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/urlpublishing.py
--rw-rw-rw-   0 root         (0) root         (0)     9037 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/urlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/vcard.py
--rw-rw-rw-   0 root         (0) root         (0)     7288 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/wdoc.py
--rw-rw-rw-   0 root         (0) root         (0)    17749 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     2320 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/xbel.py
--rw-rw-rw-   0 root         (0) root         (0)    10739 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/views/xmlrss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.898828 cubicweb-web-1.2.0/cubicweb_web/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/about_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/about_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/add_content_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/add_content_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/advanced_usage_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/advanced_usage_schema_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/advanced_usage_schema_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/bookmarks_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/bookmarks_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_last_update_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_last_update_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_rss_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_rss_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/glossary_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      728 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/glossary_fr.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.898828 cubicweb-web-1.2.0/cubicweb_web/wdoc/images/
--rw-rw-rw-   0 root         (0) root         (0)     5590 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/images/userprefs_en.png
--rw-rw-rw-   0 root         (0) root         (0)     6423 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/images/userprefs_fr.png
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/main_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      312 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/search_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/search_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/search_sample_queries_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/search_sample_queries_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/standard_usage_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/standard_usage_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/toc.xml
--rw-rw-rw-   0 root         (0) root         (0)     6393 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/tut_rql_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     7275 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/tut_rql_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/userprefs_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/wdoc/userprefs_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)    17696 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/cubicweb_web/webconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.758826 cubicweb-web-1.2.0/cubicweb_web.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1208 2023-07-11 15:30:14.000000 cubicweb-web-1.2.0/cubicweb_web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14985 2023-07-11 15:30:14.000000 cubicweb-web-1.2.0/cubicweb_web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:30:14.000000 cubicweb-web-1.2.0/cubicweb_web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-11 15:30:14.000000 cubicweb-web-1.2.0/cubicweb_web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 15:30:14.000000 cubicweb-web-1.2.0/cubicweb_web.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-11 15:30:14.000000 cubicweb-web-1.2.0/cubicweb_web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 15:30:14.000000 cubicweb-web-1.2.0/cubicweb_web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 15:30:14.982829 cubicweb-web-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.934828 cubicweb-web-1.2.0/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.942829 cubicweb-web-1.2.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.942829 cubicweb-web-1.2.0/test/data/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_blog/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_blog/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.946829 cubicweb-web-1.2.0/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.950829 cubicweb-web-1.2.0/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.950829 cubicweb-web-1.2.0/test/data/cubicweb_file/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/data/file.png
--rw-rw-rw-   0 root         (0) root         (0)     2000 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/schema.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.954829 cubicweb-web-1.2.0/test/data/cubicweb_file/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_file/wdoc/toc.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.954829 cubicweb-web-1.2.0/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/cubicweb_tag/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.734826 cubicweb-web-1.2.0/test/data/libpython/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.958829 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.962829 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/excludeme/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.966829 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2261 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.962829 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/INSTALLER
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/METADATA
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/RECORD
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/WHEEL
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/pouet.css
--rw-rw-rw-   0 root         (0) root         (0)     8663 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/sheet1.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/sheet2.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/data/views.py
--rw-rw-rw-   0 root         (0) root         (0)    35939 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_application.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_breadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_bw_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2319 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     4974 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_csrf.py
--rw-rw-rw-   0 root         (0) root         (0)    12888 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_entity.py
--rw-rw-rw-   0 root         (0) root         (0)    24397 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_facet.py
--rw-rw-rw-   0 root         (0) root         (0)    17839 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_form.py
--rw-rw-rw-   0 root         (0) root         (0)     9449 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_formfields.py
--rw-rw-rw-   0 root         (0) root         (0)     3291 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)     9718 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_http.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_http_headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_httptest.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     6668 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_idownloadable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.970829 cubicweb-web-1.2.0/test/test_js_scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.974829 cubicweb-web-1.2.0/test/test_js_scripts/data/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/data/ajax_url0.html
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/data/ajax_url1.html
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/data/ajaxresult.json
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/data/test_htmlhelpers.html
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/data/test_utils.html
--rw-rw-rw-   0 root         (0) root         (0)     6549 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/jest.config.js
--rw-rw-rw-   0 root         (0) root         (0)   122226 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/package.json
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/setup.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.978829 cubicweb-web-1.2.0/test/test_js_scripts/test/
--rw-rw-rw-   0 root         (0) root         (0)     7373 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/test/ajax.test.js
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/test/htmlhelpers.test.js
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/test/utils.js
--rw-rw-rw-   0 root         (0) root         (0)     3723 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_js_scripts/test/utils.test.js
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_login.py
--rw-rw-rw-   0 root         (0) root         (0)    13290 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_magicsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     6986 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_propertysheet.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_pyramid.py
--rw-rw-rw-   0 root         (0) root         (0)     3124 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_pyramid_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     3122 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_pyramid_predicates.py
--rw-rw-rw-   0 root         (0) root         (0)    23077 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_reledit.py
--rw-rw-rw-   0 root         (0) root         (0)     6166 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)    10906 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_rest.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_rset.py
--rw-rw-rw-   0 root         (0) root         (0)     5569 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_testlib.py
--rw-rw-rw-   0 root         (0) root         (0)     9086 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_uicfg.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_url_redirection.py
--rw-rw-rw-   0 root         (0) root         (0)     8483 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_urlpublisher.py
--rw-rw-rw-   0 root         (0) root         (0)     9697 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_urlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     3147 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     2791 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_apacherewrite.py
--rw-rw-rw-   0 root         (0) root         (0)    54787 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_basecontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)    13844 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_csv.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_cwsources.py
--rw-rw-rw-   0 root         (0) root         (0)     1791 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_debug_html.py
--rw-rw-rw-   0 root         (0) root         (0)    19638 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_editforms.py
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_errorform.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_forms.py
--rw-rw-rw-   0 root         (0) root         (0)     4531 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_json.py
--rw-rw-rw-   0 root         (0) root         (0)     6177 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_pyviews.py
--rw-rw-rw-   0 root         (0) root         (0)     4912 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_searchrestriction.py
--rw-rw-rw-   0 root         (0) root         (0)     7239 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_staticcontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_treeview.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_wdoc.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_views_xmlrss.py
--rw-rw-rw-   0 root         (0) root         (0)    29065 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_viewselector.py
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_vregistry.py
--rw-rw-rw-   0 root         (0) root         (0)     6074 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_web.py
--rw-rw-rw-   0 root         (0) root         (0)     2920 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_webconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/test_webtest.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/testutils.js
--rw-rw-rw-   0 root         (0) root         (0)     6438 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test/unittest_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.978829 cubicweb-web-1.2.0/test_auto/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test_auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 15:30:14.982829 cubicweb-web-1.2.0/test_auto/data/
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test_auto/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     3560 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/test_auto/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-07-11 15:29:51.000000 cubicweb-web-1.2.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.934000 cubicweb-web-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-07-20 13:07:04.934000 cubicweb-web-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.289992 cubicweb-web-1.2.1/cubicweb_web/
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/action.py
+-rw-rw-rw-   0 root         (0) root         (0)    21197 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     6976 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/box.py
+-rw-rw-rw-   0 root         (0) root         (0)    21362 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/bwcompat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/captcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     4834 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/ccplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    29090 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     8635 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.773998 cubicweb-web-1.2.1/cubicweb_web/data/
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/accessories-text-editor.png
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/add_button.png
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/asc.gif
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/banner.png
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/bg.gif
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/bg_trame_grise.png
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/black-check.png
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/black-uncheck.png
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/bullet.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/bullet_orange.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/button.png
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/calendar.gif
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cancel.png
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/contextFreeBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/contextualBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/critical.png
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.acl.css
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.ajax.box.js
+-rw-rw-rw-   0 root         (0) root         (0)    24133 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.ajax.js
+-rw-rw-rw-   0 root         (0) root         (0)     7895 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.calendar.css
+-rw-rw-rw-   0 root         (0) root         (0)     9665 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.calendar.js
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.calendar_popup.css
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.compat.js
+-rw-rw-rw-   0 root         (0) root         (0)    18494 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.css
+-rw-rw-rw-   0 root         (0) root         (0)    18779 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.edition.js
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.facets.css
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.facets.js
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.fckcwconfig-full.js
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.fckcwconfig.js
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.flot.js
+-rw-rw-rw-   0 root         (0) root         (0)     3811 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.form.css
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.html_tree.css
+-rw-rw-rw-   0 root         (0) root         (0)     4595 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.htmlhelpers.js
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.ie.css
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.image.js
+-rw-rw-rw-   0 root         (0) root         (0)    12621 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.js
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.log.css
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.log.js
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.login.css
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.manageview.css
+-rw-rw-rw-   0 root         (0) root         (0)    16860 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.pictograms.css
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.preferences.css
+-rw-rw-rw-   0 root         (0) root         (0)     4559 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.preferences.js
+-rw-rw-rw-   0 root         (0) root         (0)      189 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.print.css
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.python.js
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.reledit.js
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.schema.css
+-rw-rw-rw-   0 root         (0) root         (0)      756 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.suggest.css
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.tablesorter.css
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.tableview.css
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.timetable.css
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.treeview.css
+-rw-rw-rw-   0 root         (0) root         (0)    19668 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.widgets.js
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/desc.gif
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/download.gif
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/dublincore-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     2179 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/dublincore-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)    67968 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/entypo.eot
+-rw-rw-rw-   0 root         (0) root         (0)    97203 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/entypo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    67680 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/entypo.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    42064 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/entypo.woff
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/error.png
+-rw-rw-rw-   0 root         (0) root         (0)    42086 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/excanvas.js
+-rw-rw-rw-   0 root         (0) root         (0)    34494 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/feed-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/feed-icon16x16.png
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/feed-icon32x32.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/file.gif
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/folder-closed.gif
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/folder.gif
+-rw-rw-rw-   0 root         (0) root         (0)    11147 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   151629 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.locale.js
+-rw-rw-rw-   0 root         (0) root         (0)    51213 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      668 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.print.css
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/go.png
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/go_next.png
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/go_prev.png
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/gradient-grey-up.png
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/gradient-grey.gif
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/help.png
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/help_ie.png
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/icon_blank.png
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/icon_bookmark.gif
+-rw-rw-rw-   0 root         (0) root         (0)      401 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/icon_emailaddress.gif
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/icon_euser.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/icon_map.png
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/icon_state.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.781998 cubicweb-web-1.2.1/cubicweb_web/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/animated-overlay.gif
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_glass_75_dadada_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_222222_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_454545_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_888888_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/incontextBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/information.png
+-rw-rw-rw-   0 root         (0) root         (0)    16621 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-migrate.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.785998 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/
+-rw-rw-rw-   0 root         (0) root         (0)     1772 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/changelog.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.797999 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/file.gif
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/folder-closed.gif
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/folder.gif
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/minus.gif
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/plus.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-black.gif
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-default.gif
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-gray.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      394 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-red.gif
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js
+-rw-rw-rw-   0 root         (0) root         (0)     8065 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.js
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.cookie.js
+-rw-rw-rw-   0 root         (0) root         (0)    89666 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.flot.js
+-rw-rw-rw-   0 root         (0) root         (0)   273199 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    85184 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.qtip.js
+-rw-rw-rw-   0 root         (0) root         (0)    38404 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.qtip.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    41257 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.tablesorter.js
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.timePicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.timepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    32456 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.css
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.datepicker-de.js
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.datepicker-es.js
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.datepicker-fr.js
+-rw-rw-rw-   0 root         (0) root         (0)   435844 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.js
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/liveclipboard-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/loading.gif
+-rw-rw-rw-   0 root         (0) root         (0)     9083 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb-gray.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb-icon.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/logo-logilab.png
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/microformats-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/microformats-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/minus.gif
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/no-check-no-border.png
+-rw-rw-rw-   0 root         (0) root         (0)      537 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/ok.png
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/pen_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/plus.gif
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/plus.png
+-rw-rw-rw-   0 root         (0) root         (0)    79752 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/porkys.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/puce.png
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/puce_down.png
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/puce_down_black.png
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/puce_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/pygments.css
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/required.png
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/rss-button.png
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/rss.png
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/search.png
+-rw-rw-rw-   0 root         (0) root         (0)      959 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/sendcancel.png
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/data/sendok.png
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/trash_can.png
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/trash_can_small.png
+-rw-rw-rw-   0 root         (0) root         (0)    27374 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/ui.all.css
+-rw-rw-rw-   0 root         (0) root         (0)     5055 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/up.gif
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/data/upload.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.797999 cubicweb-web-1.2.1/cubicweb_web/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/devtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39364 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/devtools/testlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.797999 cubicweb-web-1.2.1/cubicweb_web/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17396 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/ext/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    69654 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/facet.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/form.py
+-rw-rw-rw-   0 root         (0) root         (0)    49324 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)    42471 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    11249 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/htmlwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    55646 2023-07-20 13:05:44.000000 cubicweb-web-1.2.1/cubicweb_web/http_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6189 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/httpcache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/propertysheet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.801999 cubicweb-web-1.2.1/cubicweb_web/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/pyramid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/pyramid/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/pyramid/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     5584 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/pyramid/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/pyramid/url_redirection.py
+-rw-rw-rw-   0 root         (0) root         (0)    40224 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/schemaviewer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6699 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/uihelper.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19979 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.837999 cubicweb-web-1.2.1/cubicweb_web/views/
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/_vid_by_mimetype.py
+-rw-rw-rw-   0 root         (0) root         (0)    14788 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    16562 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/ajaxcontroller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/ajaxedit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/apacherewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)    46301 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/autoform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8971 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/basecomponents.py
+-rw-rw-rw-   0 root         (0) root         (0)    11545 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/basecontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)    20464 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)    22595 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     6017 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     9230 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9783 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4352 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/csvexport.py
+-rw-rw-rw-   0 root         (0) root         (0)    17032 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/cwproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)    16247 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/cwsources.py
+-rw-rw-rw-   0 root         (0) root         (0)    10516 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/cwuser.py
+-rw-rw-rw-   0 root         (0) root         (0)     7008 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     2465 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/dotgraphview.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/edit_attributes.pt
+-rw-rw-rw-   0 root         (0) root         (0)    20973 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/editcontroller.py
+-rw-rw-rw-   0 root         (0) root         (0)    12498 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4687 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/editviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     5183 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/emailaddress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    16347 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)    20026 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/formrenderers.py
+-rw-rw-rw-   0 root         (0) root         (0)    18194 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     7798 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/ibreadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8266 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/idownloadable.py
+-rw-rw-rw-   0 root         (0) root         (0)     5584 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    16883 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/magicsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     9042 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/management.py
+-rw-rw-rw-   0 root         (0) root         (0)    17293 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9023 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/owl.py
+-rw-rw-rw-   0 root         (0) root         (0)     4632 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    18367 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/primary.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/pyviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     5345 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    22006 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)    29416 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/searchrestriction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7050 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7293 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/startup.py
+-rw-rw-rw-   0 root         (0) root         (0)    11217 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/staticcontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)    48960 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/tableview.py
+-rw-rw-rw-   0 root         (0) root         (0)     9630 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8971 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/timetable.py
+-rw-rw-rw-   0 root         (0) root         (0)    12731 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/treeview.py
+-rw-rw-rw-   0 root         (0) root         (0)    29932 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/uicfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     8479 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/undohistory.py
+-rw-rw-rw-   0 root         (0) root         (0)    16377 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/urlpublishing.py
+-rw-rw-rw-   0 root         (0) root         (0)     9037 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/urlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/vcard.py
+-rw-rw-rw-   0 root         (0) root         (0)     7288 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/wdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)    17749 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/xbel.py
+-rw-rw-rw-   0 root         (0) root         (0)    10739 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/views/xmlrss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.853999 cubicweb-web-1.2.1/cubicweb_web/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/about_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/about_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/add_content_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/add_content_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/advanced_usage_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/advanced_usage_schema_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/advanced_usage_schema_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/bookmarks_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/bookmarks_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_last_update_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_last_update_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_rss_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_rss_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/glossary_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      728 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/glossary_fr.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.853999 cubicweb-web-1.2.1/cubicweb_web/wdoc/images/
+-rw-rw-rw-   0 root         (0) root         (0)     5590 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/images/userprefs_en.png
+-rw-rw-rw-   0 root         (0) root         (0)     6423 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/images/userprefs_fr.png
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/main_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      312 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/search_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/search_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/search_sample_queries_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/search_sample_queries_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/standard_usage_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/standard_usage_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/toc.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6393 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/tut_rql_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7275 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/tut_rql_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/userprefs_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/wdoc/userprefs_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17696 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/cubicweb_web/webconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.293992 cubicweb-web-1.2.1/cubicweb_web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-07-20 13:07:03.000000 cubicweb-web-1.2.1/cubicweb_web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14985 2023-07-20 13:07:04.000000 cubicweb-web-1.2.1/cubicweb_web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 13:07:03.000000 cubicweb-web-1.2.1/cubicweb_web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-20 13:07:03.000000 cubicweb-web-1.2.1/cubicweb_web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 13:07:03.000000 cubicweb-web-1.2.1/cubicweb_web.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-20 13:07:03.000000 cubicweb-web-1.2.1/cubicweb_web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-20 13:07:03.000000 cubicweb-web-1.2.1/cubicweb_web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 13:07:04.934000 cubicweb-web-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.890000 cubicweb-web-1.2.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.894000 cubicweb-web-1.2.1/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.898000 cubicweb-web-1.2.1/test/data/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_blog/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_blog/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.902000 cubicweb-web-1.2.1/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.906000 cubicweb-web-1.2.1/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.906000 cubicweb-web-1.2.1/test/data/cubicweb_file/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/data/file.png
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.910000 cubicweb-web-1.2.1/test/data/cubicweb_file/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_file/wdoc/toc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.914000 cubicweb-web-1.2.1/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/cubicweb_tag/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.117990 cubicweb-web-1.2.1/test/data/libpython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.914000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.918000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.918000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.918000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/INSTALLER
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/METADATA
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/RECORD
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/WHEEL
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/pouet.css
+-rw-rw-rw-   0 root         (0) root         (0)     8663 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/sheet1.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/sheet2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/data/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    35939 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_breadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_bw_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2319 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     4974 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_csrf.py
+-rw-rw-rw-   0 root         (0) root         (0)    12888 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)    24397 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_facet.py
+-rw-rw-rw-   0 root         (0) root         (0)    17839 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     9449 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3291 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     9718 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_http.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_http_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_httptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     6668 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_idownloadable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.922000 cubicweb-web-1.2.1/test/test_js_scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.926000 cubicweb-web-1.2.1/test/test_js_scripts/data/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/data/ajax_url0.html
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/data/ajax_url1.html
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/data/ajaxresult.json
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/data/test_htmlhelpers.html
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/data/test_utils.html
+-rw-rw-rw-   0 root         (0) root         (0)     6549 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/jest.config.js
+-rw-rw-rw-   0 root         (0) root         (0)   122226 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/package.json
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/setup.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.930000 cubicweb-web-1.2.1/test/test_js_scripts/test/
+-rw-rw-rw-   0 root         (0) root         (0)     7373 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/test/ajax.test.js
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/test/htmlhelpers.test.js
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/test/utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_js_scripts/test/utils.test.js
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_login.py
+-rw-rw-rw-   0 root         (0) root         (0)    13290 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_magicsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6986 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_propertysheet.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_pyramid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_pyramid_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3122 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_pyramid_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)    23077 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6166 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_rset.py
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     9086 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_uicfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_url_redirection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8483 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_urlpublisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     9697 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_urlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     3147 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_apacherewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)    54787 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_basecontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)    13844 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_cwsources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_debug_html.py
+-rw-rw-rw-   0 root         (0) root         (0)    19638 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_errorform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4531 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     6177 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_pyviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     4912 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_searchrestriction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7239 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_staticcontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_treeview.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_wdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_views_xmlrss.py
+-rw-rw-rw-   0 root         (0) root         (0)    29065 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_viewselector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_vregistry.py
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_web.py
+-rw-rw-rw-   0 root         (0) root         (0)     2920 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_webconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/test_webtest.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/testutils.js
+-rw-rw-rw-   0 root         (0) root         (0)     6438 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test/unittest_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.930000 cubicweb-web-1.2.1/test_auto/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test_auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 13:07:04.930000 cubicweb-web-1.2.1/test_auto/data/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test_auto/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/test_auto/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-07-20 13:05:45.000000 cubicweb-web-1.2.1/tox.ini
```

### Comparing `cubicweb-web-1.2.0/MANIFEST.in` & `cubicweb-web-1.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/PKG-INFO` & `cubicweb-web-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-web
-Version: 1.2.0
+Version: 1.2.1
 Summary: Legacy component for web application
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/web
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-web-1.2.0/README.rst` & `cubicweb-web-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/__init__.py` & `cubicweb-web-1.2.1/cubicweb_web/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/__pkginfo__.py` & `cubicweb-web-1.2.1/cubicweb_web/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=W0622
 """cubicweb_web application packaging information"""
 
 
 modname = "web"
 distname = "cubicweb-web"
 
-numversion = (1, 2, 0)
+numversion = (1, 2, 1)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Legacy component for web application"
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/web"
```

### Comparing `cubicweb-web-1.2.0/cubicweb_web/_exceptions.py` & `cubicweb-web-1.2.1/cubicweb_web/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/action.py` & `cubicweb-web-1.2.1/cubicweb_web/action.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/application.py` & `cubicweb-web-1.2.1/cubicweb_web/application.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/box.py` & `cubicweb-web-1.2.1/cubicweb_web/box.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/bwcompat.py` & `cubicweb-web-1.2.1/cubicweb_web/bwcompat.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/captcha.py` & `cubicweb-web-1.2.1/cubicweb_web/captcha.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/ccplugin.py` & `cubicweb-web-1.2.1/cubicweb_web/ccplugin.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/component.py` & `cubicweb-web-1.2.1/cubicweb_web/component.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/controller.py` & `cubicweb-web-1.2.1/cubicweb_web/controller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/banner.png` & `cubicweb-web-1.2.1/cubicweb_web/data/banner.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/black-check.png` & `cubicweb-web-1.2.1/cubicweb_web/data/black-check.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/black-uncheck.png` & `cubicweb-web-1.2.1/cubicweb_web/data/black-uncheck.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cancel.png` & `cubicweb-web-1.2.1/cubicweb_web/data/cancel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.acl.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.acl.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.ajax.box.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.ajax.box.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.ajax.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.ajax.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.calendar.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.calendar.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.calendar.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.calendar.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.calendar_popup.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.calendar_popup.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.compat.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.compat.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.edition.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.edition.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.facets.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.facets.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.facets.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.facets.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.fckcwconfig-full.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.fckcwconfig-full.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.fckcwconfig.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.fckcwconfig.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.flot.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.flot.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.form.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.form.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.html_tree.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.html_tree.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.htmlhelpers.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.htmlhelpers.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.ie.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.ie.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.image.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.image.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.log.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.log.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.login.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.login.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.pictograms.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.pictograms.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.preferences.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.preferences.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.preferences.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.preferences.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.python.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.python.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.reledit.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.reledit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.schema.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.schema.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.suggest.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.suggest.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.tableview.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.tableview.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.timetable.css` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.timetable.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/cubicweb.widgets.js` & `cubicweb-web-1.2.1/cubicweb_web/data/cubicweb.widgets.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/download.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/download.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/dublincore-button.png` & `cubicweb-web-1.2.1/cubicweb_web/data/dublincore-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/dublincore-icon.png` & `cubicweb-web-1.2.1/cubicweb_web/data/dublincore-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/entypo.eot` & `cubicweb-web-1.2.1/cubicweb_web/data/entypo.eot`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/entypo.svg` & `cubicweb-web-1.2.1/cubicweb_web/data/entypo.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/entypo.ttf` & `cubicweb-web-1.2.1/cubicweb_web/data/entypo.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/entypo.woff` & `cubicweb-web-1.2.1/cubicweb_web/data/entypo.woff`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/error.png` & `cubicweb-web-1.2.1/cubicweb_web/data/error.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/excanvas.js` & `cubicweb-web-1.2.1/cubicweb_web/data/excanvas.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/favicon.ico` & `cubicweb-web-1.2.1/cubicweb_web/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/feed-icon.png` & `cubicweb-web-1.2.1/cubicweb_web/data/feed-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/feed-icon16x16.png` & `cubicweb-web-1.2.1/cubicweb_web/data/feed-icon16x16.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/feed-icon32x32.png` & `cubicweb-web-1.2.1/cubicweb_web/data/feed-icon32x32.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.css` & `cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.js` & `cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.locale.js` & `cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.locale.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.min.js` & `cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/fullcalendar.print.css` & `cubicweb-web-1.2.1/cubicweb_web/data/fullcalendar.print.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/go_next.png` & `cubicweb-web-1.2.1/cubicweb_web/data/go_next.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/go_prev.png` & `cubicweb-web-1.2.1/cubicweb_web/data/go_prev.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/gradient-grey.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/gradient-grey.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/help.png` & `cubicweb-web-1.2.1/cubicweb_web/data/help.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/help_ie.png` & `cubicweb-web-1.2.1/cubicweb_web/data/help_ie.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/icon_map.png` & `cubicweb-web-1.2.1/cubicweb_web/data/icon_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/images/animated-overlay.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_222222_256x240.png` & `cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png` & `cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_454545_256x240.png` & `cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_888888_256x240.png` & `cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png` & `cubicweb-web-1.2.1/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-migrate.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-migrate.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/changelog.md` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/changelog.md`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.css` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/readme.md` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/readme.md`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery-treeview/screenshot.png` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery-treeview/screenshot.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.cookie.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.flot.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.qtip.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.qtip.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.qtip.min.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.qtip.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.tablesorter.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.timePicker.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.timePicker.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.timepicker.css` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.timepicker.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.css` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.datepicker-de.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.datepicker-de.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.datepicker-es.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.datepicker-es.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.datepicker-fr.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.datepicker-fr.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/jquery.ui.js` & `cubicweb-web-1.2.1/cubicweb_web/data/jquery.ui.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/liveclipboard-icon.png` & `cubicweb-web-1.2.1/cubicweb_web/data/liveclipboard-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/loading.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/loading.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb-gray.svg` & `cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb-gray.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb-icon.svg` & `cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb-icon.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb-text.svg` & `cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb-text.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/logo-cubicweb.svg` & `cubicweb-web-1.2.1/cubicweb_web/data/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/logo-logilab.png` & `cubicweb-web-1.2.1/cubicweb_web/data/logo-logilab.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/logo.png` & `cubicweb-web-1.2.1/cubicweb_web/data/logo.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/microformats-button.png` & `cubicweb-web-1.2.1/cubicweb_web/data/microformats-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/microformats-icon.png` & `cubicweb-web-1.2.1/cubicweb_web/data/microformats-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/minus.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/minus.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/ok.png` & `cubicweb-web-1.2.1/cubicweb_web/data/ok.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/plus.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/plus.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/porkys.ttf` & `cubicweb-web-1.2.1/cubicweb_web/data/porkys.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/pygments.css` & `cubicweb-web-1.2.1/cubicweb_web/data/pygments.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/rss-button.png` & `cubicweb-web-1.2.1/cubicweb_web/data/rss-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/sendcancel.png` & `cubicweb-web-1.2.1/cubicweb_web/data/sendcancel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/sendok.png` & `cubicweb-web-1.2.1/cubicweb_web/data/sendok.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/trash_can.png` & `cubicweb-web-1.2.1/cubicweb_web/data/trash_can.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/trash_can_small.png` & `cubicweb-web-1.2.1/cubicweb_web/data/trash_can_small.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/ui.all.css` & `cubicweb-web-1.2.1/cubicweb_web/data/ui.all.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/uiprops.py` & `cubicweb-web-1.2.1/cubicweb_web/data/uiprops.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/data/upload.gif` & `cubicweb-web-1.2.1/cubicweb_web/data/upload.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/devtools/testlib.py` & `cubicweb-web-1.2.1/cubicweb_web/devtools/testlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,25 +31,25 @@
     not_selected,
     JsonValidator,
     line_context_filter,
     real_error_handling,
     unprotected_entities,
     CubicWebDebugger,
 )
-from cubicweb.pyramid.test import PyramidCWTest, ACCEPTED_ORIGINS
+from cubicweb.pyramid.test import PyramidCWTest, ACCEPTED_ORIGINS, CustomTestApp
 from cubicweb.sobjects.notification import NotificationView
 from cubicweb.uilib import eid_param
 from logilab.common.decorators import cachedproperty
 from logilab.common.deprecation import class_deprecated
 from logilab.common.registry import NoSelectableObject
 from logilab.common.testlib import Tags, nocoverage
 from pyramid.csrf import LegacySessionCSRFStoragePolicy
 from pyramid.interfaces import ICSRFStoragePolicy
 from pyramid.testing import DummyRequest
-from webtest import TestApp, AppError
+from webtest import AppError
 from yams import ValidationError
 
 from cubicweb_web._exceptions import Redirect
 from cubicweb_web.application import CubicWebPublisher
 from cubicweb_web.request import CubicWebRequestBase
 from cubicweb_web.webconfig import WebAllInOneConfiguration
 
@@ -614,15 +614,15 @@
         # doctest returns tuple (failure_count, test_count)
         with self.admin_access.shell() as mih:
             result = mih.process_script(testfile)
         if result[0] and result[1]:
             raise self.failureException("doctest file '%s' failed" % testfile)
 
 
-class PyramidWebTestApp(TestApp):
+class PyramidWebTestApp(CustomTestApp):
     def __init__(self, *args, admin_login, admin_password, **kwargs):
         super().__init__(*args, **kwargs)
         self.admin_login = admin_login
         self.admin_password = admin_password
         self._ident_cookie = None
         self._csrf_token = None
```

### Comparing `cubicweb-web-1.2.0/cubicweb_web/ext/rest.py` & `cubicweb-web-1.2.1/cubicweb_web/ext/rest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/facet.py` & `cubicweb-web-1.2.1/cubicweb_web/facet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/form.py` & `cubicweb-web-1.2.1/cubicweb_web/form.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/formfields.py` & `cubicweb-web-1.2.1/cubicweb_web/formfields.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/formwidgets.py` & `cubicweb-web-1.2.1/cubicweb_web/formwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/htmlwidgets.py` & `cubicweb-web-1.2.1/cubicweb_web/htmlwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/http_headers.py` & `cubicweb-web-1.2.1/cubicweb_web/http_headers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/httpcache.py` & `cubicweb-web-1.2.1/cubicweb_web/httpcache.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/i18n.py` & `cubicweb-web-1.2.1/cubicweb_web/i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/predicates.py` & `cubicweb-web-1.2.1/cubicweb_web/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/propertysheet.py` & `cubicweb-web-1.2.1/cubicweb_web/propertysheet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/pyramid/__init__.py` & `cubicweb-web-1.2.1/cubicweb_web/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/pyramid/login.py` & `cubicweb-web-1.2.1/cubicweb_web/pyramid/login.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/pyramid/predicates.py` & `cubicweb-web-1.2.1/cubicweb_web/pyramid/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/pyramid/test.py` & `cubicweb-web-1.2.1/cubicweb_web/pyramid/test.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/pyramid/url_redirection.py` & `cubicweb-web-1.2.1/cubicweb_web/pyramid/url_redirection.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/request.py` & `cubicweb-web-1.2.1/cubicweb_web/request.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/schemaviewer.py` & `cubicweb-web-1.2.1/cubicweb_web/schemaviewer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/uihelper.py` & `cubicweb-web-1.2.1/cubicweb_web/uihelper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/utils.py` & `cubicweb-web-1.2.1/cubicweb_web/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/view.py` & `cubicweb-web-1.2.1/cubicweb_web/view.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/__init__.py` & `cubicweb-web-1.2.1/cubicweb_web/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/_vid_by_mimetype.py` & `cubicweb-web-1.2.1/cubicweb_web/views/_vid_by_mimetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/actions.py` & `cubicweb-web-1.2.1/cubicweb_web/views/actions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/ajaxcontroller.py` & `cubicweb-web-1.2.1/cubicweb_web/views/ajaxcontroller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/ajaxedit.py` & `cubicweb-web-1.2.1/cubicweb_web/views/ajaxedit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/apacherewrite.py` & `cubicweb-web-1.2.1/cubicweb_web/views/apacherewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/authentication.py` & `cubicweb-web-1.2.1/cubicweb_web/views/authentication.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/autoform.py` & `cubicweb-web-1.2.1/cubicweb_web/views/autoform.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/basecomponents.py` & `cubicweb-web-1.2.1/cubicweb_web/views/basecomponents.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/basecontrollers.py` & `cubicweb-web-1.2.1/cubicweb_web/views/basecontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/basetemplates.py` & `cubicweb-web-1.2.1/cubicweb_web/views/basetemplates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/baseviews.py` & `cubicweb-web-1.2.1/cubicweb_web/views/baseviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/bookmark.py` & `cubicweb-web-1.2.1/cubicweb_web/views/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/boxes.py` & `cubicweb-web-1.2.1/cubicweb_web/views/boxes.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/calendar.py` & `cubicweb-web-1.2.1/cubicweb_web/views/calendar.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/csvexport.py` & `cubicweb-web-1.2.1/cubicweb_web/views/csvexport.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/cwproperties.py` & `cubicweb-web-1.2.1/cubicweb_web/views/cwproperties.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/cwsources.py` & `cubicweb-web-1.2.1/cubicweb_web/views/cwsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/cwuser.py` & `cubicweb-web-1.2.1/cubicweb_web/views/cwuser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/debug.py` & `cubicweb-web-1.2.1/cubicweb_web/views/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/dotgraphview.py` & `cubicweb-web-1.2.1/cubicweb_web/views/dotgraphview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/edit_attributes.pt` & `cubicweb-web-1.2.1/cubicweb_web/views/edit_attributes.pt`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/editcontroller.py` & `cubicweb-web-1.2.1/cubicweb_web/views/editcontroller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/editforms.py` & `cubicweb-web-1.2.1/cubicweb_web/views/editforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/editviews.py` & `cubicweb-web-1.2.1/cubicweb_web/views/editviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/emailaddress.py` & `cubicweb-web-1.2.1/cubicweb_web/views/emailaddress.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/error.py` & `cubicweb-web-1.2.1/cubicweb_web/views/error.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/facets.py` & `cubicweb-web-1.2.1/cubicweb_web/views/facets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/formrenderers.py` & `cubicweb-web-1.2.1/cubicweb_web/views/formrenderers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/forms.py` & `cubicweb-web-1.2.1/cubicweb_web/views/forms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/ibreadcrumbs.py` & `cubicweb-web-1.2.1/cubicweb_web/views/ibreadcrumbs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/idownloadable.py` & `cubicweb-web-1.2.1/cubicweb_web/views/idownloadable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/json.py` & `cubicweb-web-1.2.1/cubicweb_web/views/json.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/magicsearch.py` & `cubicweb-web-1.2.1/cubicweb_web/views/magicsearch.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/management.py` & `cubicweb-web-1.2.1/cubicweb_web/views/management.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/navigation.py` & `cubicweb-web-1.2.1/cubicweb_web/views/navigation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/owl.py` & `cubicweb-web-1.2.1/cubicweb_web/views/owl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/plots.py` & `cubicweb-web-1.2.1/cubicweb_web/views/plots.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/primary.py` & `cubicweb-web-1.2.1/cubicweb_web/views/primary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/pyviews.py` & `cubicweb-web-1.2.1/cubicweb_web/views/pyviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/rdf.py` & `cubicweb-web-1.2.1/cubicweb_web/views/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/reledit.py` & `cubicweb-web-1.2.1/cubicweb_web/views/reledit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/schema.py` & `cubicweb-web-1.2.1/cubicweb_web/views/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/searchrestriction.py` & `cubicweb-web-1.2.1/cubicweb_web/views/searchrestriction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/sessions.py` & `cubicweb-web-1.2.1/cubicweb_web/views/sessions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/startup.py` & `cubicweb-web-1.2.1/cubicweb_web/views/startup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/staticcontrollers.py` & `cubicweb-web-1.2.1/cubicweb_web/views/staticcontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/tableview.py` & `cubicweb-web-1.2.1/cubicweb_web/views/tableview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/tabs.py` & `cubicweb-web-1.2.1/cubicweb_web/views/tabs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/timetable.py` & `cubicweb-web-1.2.1/cubicweb_web/views/timetable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/treeview.py` & `cubicweb-web-1.2.1/cubicweb_web/views/treeview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/uicfg.py` & `cubicweb-web-1.2.1/cubicweb_web/views/uicfg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/undohistory.py` & `cubicweb-web-1.2.1/cubicweb_web/views/undohistory.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/urlpublishing.py` & `cubicweb-web-1.2.1/cubicweb_web/views/urlpublishing.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,14 @@
 """
 
 import logging
 import warnings
 
 from urllib.parse import urlparse
 
-from pyramid.httpexceptions import HTTPNotFound
-
 from rql import TypeResolverException
 
 from cubicweb import RegistryException
 from cubicweb_web import NotFound, Redirect, component, views
 from cubicweb_web.utils import url_path_starts_with_prefix, remove_prefix_from_url_path
 
 logger = logging.getLogger(__name__)
@@ -141,15 +139,15 @@
                 datadir_url and url_path_starts_with_prefix(path, datadir_route_prefix)
             ):
                 if not url_path_starts_with_prefix(path, route_prefix):
                     logger.warning(
                         f"Error 404: instance has recieved the request '{req}' with path '{path}' but "
                         f"it doesn't start with the route_prefix '{route_prefix}'"
                     )
-                    raise HTTPNotFound()
+                    raise NotFound()
 
                 path = remove_prefix_from_url_path(path, route_prefix)
 
         elif route_prefix:
             warnings.warn(
                 "in your configuration your base url "
                 f"'{self.vreg.config['base-url']}' has a route prefix: "
```

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/urlrewrite.py` & `cubicweb-web-1.2.1/cubicweb_web/views/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/vcard.py` & `cubicweb-web-1.2.1/cubicweb_web/views/vcard.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/wdoc.py` & `cubicweb-web-1.2.1/cubicweb_web/views/wdoc.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/workflow.py` & `cubicweb-web-1.2.1/cubicweb_web/views/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/xbel.py` & `cubicweb-web-1.2.1/cubicweb_web/views/xbel.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/views/xmlrss.py` & `cubicweb-web-1.2.1/cubicweb_web/views/xmlrss.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/about_en.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/about_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/about_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/about_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/advanced_usage_schema_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/advanced_usage_schema_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/bookmarks_en.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/bookmarks_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/bookmarks_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/bookmarks_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_en.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/custom_view_rss_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/custom_view_rss_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/glossary_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/glossary_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/images/userprefs_en.png` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/images/userprefs_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/images/userprefs_fr.png` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/images/userprefs_fr.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/standard_usage_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/standard_usage_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/toc.xml` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/toc.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/tut_rql_en.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/tut_rql_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/tut_rql_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/tut_rql_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/wdoc/userprefs_fr.rst` & `cubicweb-web-1.2.1/cubicweb_web/wdoc/userprefs_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web/webconfig.py` & `cubicweb-web-1.2.1/cubicweb_web/webconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/cubicweb_web.egg-info/PKG-INFO` & `cubicweb-web-1.2.1/cubicweb_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-web
-Version: 1.2.0
+Version: 1.2.1
 Summary: Legacy component for web application
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/web
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-web-1.2.0/cubicweb_web.egg-info/SOURCES.txt` & `cubicweb-web-1.2.1/cubicweb_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/setup.py` & `cubicweb-web-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/cubicweb_blog/schema.py` & `cubicweb-web-1.2.1/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/cubicweb_card/schema.py` & `cubicweb-web-1.2.1/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/cubicweb_file/entities.py` & `cubicweb-web-1.2.1/test/data/cubicweb_file/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/cubicweb_file/hooks.py` & `cubicweb-web-1.2.1/test/data/cubicweb_file/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/cubicweb_file/schema.py` & `cubicweb-web-1.2.1/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/cubicweb_tag/schema.py` & `cubicweb-web-1.2.1/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/cubicweb_tag/views.py` & `cubicweb-web-1.2.1/test/data/cubicweb_tag/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/entities.py` & `cubicweb-web-1.2.1/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref` & `cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/schema.py` & `cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/libpython/cubicweb_i18ntestcube/views.py` & `cubicweb-web-1.2.1/test/data/libpython/cubicweb_i18ntestcube/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/schema.py` & `cubicweb-web-1.2.1/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/data/views.py` & `cubicweb-web-1.2.1/test/data/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_application.py` & `cubicweb-web-1.2.1/test/test_application.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_breadcrumbs.py` & `cubicweb-web-1.2.1/test/test_breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_bw_request.py` & `cubicweb-web-1.2.1/test/test_bw_request.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_controller.py` & `cubicweb-web-1.2.1/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_csrf.py` & `cubicweb-web-1.2.1/test/test_csrf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_entity.py` & `cubicweb-web-1.2.1/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_facet.py` & `cubicweb-web-1.2.1/test/test_facet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_form.py` & `cubicweb-web-1.2.1/test/test_form.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_formfields.py` & `cubicweb-web-1.2.1/test/test_formfields.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_formwidgets.py` & `cubicweb-web-1.2.1/test/test_formwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_http.py` & `cubicweb-web-1.2.1/test/test_http.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_http_headers.py` & `cubicweb-web-1.2.1/test/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_httptest.py` & `cubicweb-web-1.2.1/test/test_httptest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_i18n.py` & `cubicweb-web-1.2.1/test/test_i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_idownloadable.py` & `cubicweb-web-1.2.1/test/test_idownloadable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/data/test_htmlhelpers.html` & `cubicweb-web-1.2.1/test/test_js_scripts/data/test_htmlhelpers.html`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/data/test_utils.html` & `cubicweb-web-1.2.1/test/test_js_scripts/data/test_utils.html`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/jest.config.js` & `cubicweb-web-1.2.1/test/test_js_scripts/jest.config.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/package-lock.json` & `cubicweb-web-1.2.1/test/test_js_scripts/package-lock.json`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/test/ajax.test.js` & `cubicweb-web-1.2.1/test/test_js_scripts/test/ajax.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/test/htmlhelpers.test.js` & `cubicweb-web-1.2.1/test/test_js_scripts/test/htmlhelpers.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/test/utils.js` & `cubicweb-web-1.2.1/test/test_js_scripts/test/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_js_scripts/test/utils.test.js` & `cubicweb-web-1.2.1/test/test_js_scripts/test/utils.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_login.py` & `cubicweb-web-1.2.1/test/test_login.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_magicsearch.py` & `cubicweb-web-1.2.1/test/test_magicsearch.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_predicates.py` & `cubicweb-web-1.2.1/test/test_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_propertysheet.py` & `cubicweb-web-1.2.1/test/test_propertysheet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_pyramid.py` & `cubicweb-web-1.2.1/test/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_pyramid_hooks.py` & `cubicweb-web-1.2.1/test/test_pyramid_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_pyramid_predicates.py` & `cubicweb-web-1.2.1/test/test_pyramid_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_reledit.py` & `cubicweb-web-1.2.1/test/test_reledit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_request.py` & `cubicweb-web-1.2.1/test/test_request.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_rest.py` & `cubicweb-web-1.2.1/test/test_rest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_rset.py` & `cubicweb-web-1.2.1/test/test_rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_testlib.py` & `cubicweb-web-1.2.1/test/test_testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_uicfg.py` & `cubicweb-web-1.2.1/test/test_uicfg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_url_redirection.py` & `cubicweb-web-1.2.1/test/test_url_redirection.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_urlpublisher.py` & `cubicweb-web-1.2.1/test/test_urlpublisher.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_urlrewrite.py` & `cubicweb-web-1.2.1/test/test_urlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_actions.py` & `cubicweb-web-1.2.1/test/test_views_actions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_apacherewrite.py` & `cubicweb-web-1.2.1/test/test_views_apacherewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_basecontrollers.py` & `cubicweb-web-1.2.1/test/test_views_basecontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_basetemplates.py` & `cubicweb-web-1.2.1/test/test_views_basetemplates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_baseviews.py` & `cubicweb-web-1.2.1/test/test_views_baseviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_csv.py` & `cubicweb-web-1.2.1/test/test_views_csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_cwsources.py` & `cubicweb-web-1.2.1/test/test_views_cwsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_debug_html.py` & `cubicweb-web-1.2.1/test/test_views_debug_html.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_editforms.py` & `cubicweb-web-1.2.1/test/test_views_editforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_errorform.py` & `cubicweb-web-1.2.1/test/test_views_errorform.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_forms.py` & `cubicweb-web-1.2.1/test/test_views_forms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_json.py` & `cubicweb-web-1.2.1/test/test_views_json.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_navigation.py` & `cubicweb-web-1.2.1/test/test_views_navigation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_pyviews.py` & `cubicweb-web-1.2.1/test/test_views_pyviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_searchrestriction.py` & `cubicweb-web-1.2.1/test/test_views_searchrestriction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_staticcontrollers.py` & `cubicweb-web-1.2.1/test/test_views_staticcontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_treeview.py` & `cubicweb-web-1.2.1/test/test_views_treeview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_wdoc.py` & `cubicweb-web-1.2.1/test/test_views_wdoc.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_views_xmlrss.py` & `cubicweb-web-1.2.1/test/test_views_xmlrss.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_viewselector.py` & `cubicweb-web-1.2.1/test/test_viewselector.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_vregistry.py` & `cubicweb-web-1.2.1/test/test_vregistry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_web.py` & `cubicweb-web-1.2.1/test/test_web.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_webconfig.py` & `cubicweb-web-1.2.1/test/test_webconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/test_webtest.py` & `cubicweb-web-1.2.1/test/test_webtest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/testutils.js` & `cubicweb-web-1.2.1/test/testutils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test/unittest_utils.py` & `cubicweb-web-1.2.1/test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/test_auto/test_views.py` & `cubicweb-web-1.2.1/test_auto/test_views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.0/tox.ini` & `cubicweb-web-1.2.1/tox.ini`

 * *Files identical despite different names*

