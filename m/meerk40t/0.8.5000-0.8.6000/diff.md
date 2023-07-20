# Comparing `tmp/meerk40t-0.8.5000.tar.gz` & `tmp/meerk40t-0.8.6000.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerk40t-0.8.5000.tar", last modified: Tue Jun 13 22:02:15 2023, max compression
+gzip compressed data, was "meerk40t-0.8.6000.tar", last modified: Thu Jul 20 13:53:49 2023, max compression
```

## Comparing `meerk40t-0.8.5000.tar` & `meerk40t-0.8.6000.tar`

### file list

```diff
@@ -1,467 +1,467 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.269945 meerk40t-0.8.5000/
--rw-rw-rw-   0        0        0     1086 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/LICENSE
--rw-rw-rw-   0        0        0     5619 2023-06-13 22:02:15.269945 meerk40t-0.8.5000/PKG-INFO
--rw-rw-rw-   0        0        0     3981 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.637909 meerk40t-0.8.5000/meerk40t/
--rw-rw-rw-   0        0        0       19 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.656911 meerk40t-0.8.5000/meerk40t/balormk/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/__init__.py
--rw-rw-rw-   0        0        0     5556 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/balor_params.py
--rw-rw-rw-   0        0        0    46666 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/controller.py
--rw-rw-rw-   0        0        0    69469 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/device.py
--rw-rw-rw-   0        0        0    20843 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/driver.py
--rw-rw-rw-   0        0        0     5304 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/elementlightjob.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.664911 meerk40t-0.8.5000/meerk40t/balormk/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/gui/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/gui/balorconfig.py
--rw-rw-rw-   0        0        0     5987 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/gui/balorcontroller.py
--rw-rw-rw-   0        0        0     5858 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/gui/baloroperationproperties.py
--rw-rw-rw-   0        0        0     5311 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/gui/gui.py
--rw-rw-rw-   0        0        0     7755 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/livefulllightjob.py
--rw-rw-rw-   0        0        0     5981 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/liveselectionlightjob.py
--rw-rw-rw-   0        0        0     3646 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/mock_connection.py
--rw-rw-rw-   0        0        0     4991 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/plugin.py
--rw-rw-rw-   0        0        0    11181 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/balormk/usb_connection.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.667911 meerk40t-0.8.5000/meerk40t/camera/
--rw-rw-rw-   0        0        0       17 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/camera/__init__.py
--rw-rw-rw-   0        0        0    13273 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/camera/camera.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.672911 meerk40t-0.8.5000/meerk40t/camera/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/camera/gui/__init__.py
--rw-rw-rw-   0        0        0    40400 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/camera/gui/camerapanel.py
--rw-rw-rw-   0        0        0     2341 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/camera/gui/gui.py
--rw-rw-rw-   0        0        0    10112 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/camera/plugin.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.677912 meerk40t-0.8.5000/meerk40t/ch341/
--rw-rw-rw-   0        0        0      739 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/ch341/__init__.py
--rw-rw-rw-   0        0        0    21369 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/ch341/libusb.py
--rw-rw-rw-   0        0        0     5656 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/ch341/mock.py
--rw-rw-rw-   0        0        0     6729 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/ch341/windll.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.710914 meerk40t-0.8.5000/meerk40t/core/
--rw-rw-rw-   0        0        0       15 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/__init__.py
--rw-rw-rw-   0        0        0    17576 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/bindalias.py
--rw-rw-rw-   0        0        0      912 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/core.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.731915 meerk40t-0.8.5000/meerk40t/core/cutcode/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/__init__.py
--rw-rw-rw-   0        0        0     2074 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/cubiccut.py
--rw-rw-rw-   0        0        0    12473 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/cutcode.py
--rw-rw-rw-   0        0        0     5392 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/cutgroup.py
--rw-rw-rw-   0        0        0     5129 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/cutobject.py
--rw-rw-rw-   0        0        0      847 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/dwellcut.py
--rw-rw-rw-   0        0        0      727 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/gotocut.py
--rw-rw-rw-   0        0        0      693 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/homecut.py
--rw-rw-rw-   0        0        0      776 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/inputcut.py
--rw-rw-rw-   0        0        0      952 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/linecut.py
--rw-rw-rw-   0        0        0      786 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/outputcut.py
--rw-rw-rw-   0        0        0    10566 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/plotcut.py
--rw-rw-rw-   0        0        0     1653 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/quadcut.py
--rw-rw-rw-   0        0        0     4189 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/rastercut.py
--rw-rw-rw-   0        0        0      900 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutcode/waitcut.py
--rw-rw-rw-   0        0        0    46028 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/cutplan.py
--rw-rw-rw-   0        0        0     9898 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/drivers.py
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/element_commands.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.757916 meerk40t-0.8.5000/meerk40t/core/elements/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/__init__.py
--rw-rw-rw-   0        0        0    24050 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/align.py
--rw-rw-rw-   0        0        0    50696 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/branches.py
--rw-rw-rw-   0        0        0     7178 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/clipboard.py
--rw-rw-rw-   0        0        0    95595 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/element_treeops.py
--rw-rw-rw-   0        0        0     2667 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/element_types.py
--rw-rw-rw-   0        0        0   150831 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/elements.py
--rw-rw-rw-   0        0        0    19837 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/grid.py
--rw-rw-rw-   0        0        0     3214 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/materials.py
--rw-rw-rw-   0        0        0     1152 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/notes.py
--rw-rw-rw-   0        0        0    27078 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/offset.py
--rw-rw-rw-   0        0        0    10838 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/penbox.py
--rw-rw-rw-   0        0        0     2345 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/placements.py
--rw-rw-rw-   0        0        0    23836 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/render.py
--rw-rw-rw-   0        0        0    76714 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/shapes.py
--rw-rw-rw-   0        0        0    16569 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/trace.py
--rw-rw-rw-   0        0        0    14470 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/tree_commands.py
--rw-rw-rw-   0        0        0     1571 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/undo_redo.py
--rw-rw-rw-   0        0        0     8274 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/elements/wordlist.py
--rw-rw-rw-   0        0        0      269 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/exceptions.py
--rw-rw-rw-   0        0        0     6790 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/laserjob.py
--rw-rw-rw-   0        0        0     2136 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/logging.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.809919 meerk40t-0.8.5000/meerk40t/core/node/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/blobnode.py
--rw-rw-rw-   0        0        0     4020 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/bootstrap.py
--rw-rw-rw-   0        0        0      894 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/branch_elems.py
--rw-rw-rw-   0        0        0     1188 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/branch_ops.py
--rw-rw-rw-   0        0        0     1236 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/branch_regmark.py
--rw-rw-rw-   0        0        0      937 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/cutnode.py
--rw-rw-rw-   0        0        0     6801 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_ellipse.py
--rw-rw-rw-   0        0        0     3187 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_geomstr.py
--rw-rw-rw-   0        0        0    30142 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_image.py
--rw-rw-rw-   0        0        0     6789 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_line.py
--rw-rw-rw-   0        0        0     6597 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_path.py
--rw-rw-rw-   0        0        0     2654 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_point.py
--rw-rw-rw-   0        0        0     7041 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_polyline.py
--rw-rw-rw-   0        0        0     6805 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_rect.py
--rw-rw-rw-   0        0        0    15489 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/elem_text.py
--rw-rw-rw-   0        0        0     1088 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/filenode.py
--rw-rw-rw-   0        0        0     2139 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/groupnode.py
--rw-rw-rw-   0        0        0     1881 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/lasercodenode.py
--rw-rw-rw-   0        0        0      928 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/layernode.py
--rw-rw-rw-   0        0        0     2172 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/mixins.py
--rw-rw-rw-   0        0        0    37366 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/node.py
--rw-rw-rw-   0        0        0     4015 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/nutils.py
--rw-rw-rw-   0        0        0    12948 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/op_cut.py
--rw-rw-rw-   0        0        0    10483 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/op_dots.py
--rw-rw-rw-   0        0        0    12341 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/op_engrave.py
--rw-rw-rw-   0        0        0    15348 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/op_hatch.py
--rw-rw-rw-   0        0        0    14692 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/op_image.py
--rw-rw-rw-   0        0        0    20806 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/op_raster.py
--rw-rw-rw-   0        0        0     1567 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/place_current.py
--rw-rw-rw-   0        0        0     4869 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/place_point.py
--rw-rw-rw-   0        0        0     1580 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/refnode.py
--rw-rw-rw-   0        0        0     7504 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/rootnode.py
--rw-rw-rw-   0        0        0     1511 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/util_console.py
--rw-rw-rw-   0        0        0     2216 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/util_goto.py
--rw-rw-rw-   0        0        0     1955 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/util_home.py
--rw-rw-rw-   0        0        0     3411 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/util_input.py
--rw-rw-rw-   0        0        0     3451 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/util_output.py
--rw-rw-rw-   0        0        0     2220 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/node/util_wait.py
--rw-rw-rw-   0        0        0    16615 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/parameters.py
--rw-rw-rw-   0        0        0    30751 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/planner.py
--rw-rw-rw-   0        0        0    22754 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/plotplanner.py
--rw-rw-rw-   0        0        0     3972 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/space.py
--rw-rw-rw-   0        0        0    25069 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/spoolers.py
--rw-rw-rw-   0        0        0    48106 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/svg_io.py
--rw-rw-rw-   0        0        0     6158 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/treeop.py
--rw-rw-rw-   0        0        0     2858 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/undos.py
--rw-rw-rw-   0        0        0    31404 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/units.py
--rw-rw-rw-   0        0        0     7764 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/view.py
--rw-rw-rw-   0        0        0     2866 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/webhelp.py
--rw-rw-rw-   0        0        0    18364 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/core/wordlist.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.813919 meerk40t-0.8.5000/meerk40t/device/
--rw-rw-rw-   0        0        0       17 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/__init__.py
--rw-rw-rw-   0        0        0     4253 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/basedevice.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.821920 meerk40t-0.8.5000/meerk40t/device/ch341/
--rw-rw-rw-   0        0        0       16 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/ch341/__init__.py
--rw-rw-rw-   0        0        0     7197 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/ch341/ch341.py
--rw-rw-rw-   0        0        0    16050 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/ch341/ch341libusbdriver.py
--rw-rw-rw-   0        0        0     5505 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/ch341/libusb.py
--rw-rw-rw-   0        0        0     5948 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/ch341/mock.py
--rw-rw-rw-   0        0        0     6759 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/ch341/windll.py
--rw-rw-rw-   0        0        0     4504 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/dummydevice.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.826920 meerk40t-0.8.5000/meerk40t/device/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/gui/__init__.py
--rw-rw-rw-   0        0        0    23684 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/gui/defaultactions.py
--rw-rw-rw-   0        0        0     9860 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/gui/formatterpanel.py
--rw-rw-rw-   0        0        0     9284 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/device/gui/warningpanel.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.830920 meerk40t-0.8.5000/meerk40t/dxf/
--rw-rw-rw-   0        0        0       14 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/dxf/__init__.py
--rw-rw-rw-   0        0        0    23432 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/dxf/dxf_io.py
--rw-rw-rw-   0        0        0     1318 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/dxf/plugin.py
--rw-rw-rw-   0        0        0     1245 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/external_plugins.py
--rw-rw-rw-   0        0        0      885 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/external_plugins_build.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.844921 meerk40t-0.8.5000/meerk40t/extra/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/__init__.py
--rw-rw-rw-   0        0        0     4516 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/cag.py
--rw-rw-rw-   0        0        0     2027 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/embroider.py
--rw-rw-rw-   0        0        0    34734 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/ezd.py
--rw-rw-rw-   0        0        0    12009 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/hershey.py
--rw-rw-rw-   0        0        0    13066 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/imageactions.py
--rw-rw-rw-   0        0        0    23446 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/inkscape.py
--rw-rw-rw-   0        0        0     8348 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/pathoptimize.py
--rw-rw-rw-   0        0        0     9470 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/potrace.py
--rw-rw-rw-   0        0        0    14647 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/updater.py
--rw-rw-rw-   0        0        0     5120 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/vectrace.py
--rw-rw-rw-   0        0        0     2769 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/extra/winsleep.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.848921 meerk40t-0.8.5000/meerk40t/fill/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/fill/__init__.py
--rw-rw-rw-   0        0        0    10357 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/fill/fills.py
--rw-rw-rw-   0        0        0    38279 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/fill/patternfill.py
--rw-rw-rw-   0        0        0    16519 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/fill/patterns.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.862922 meerk40t-0.8.5000/meerk40t/grbl/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/__init__.py
--rw-rw-rw-   0        0        0     2702 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/control.py
--rw-rw-rw-   0        0        0    27956 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/controller.py
--rw-rw-rw-   0        0        0    27885 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/device.py
--rw-rw-rw-   0        0        0    22885 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/driver.py
--rw-rw-rw-   0        0        0    18636 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/emulator.py
--rw-rw-rw-   0        0        0    28028 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/gcodejob.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.867922 meerk40t-0.8.5000/meerk40t/grbl/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/gui/__init__.py
--rw-rw-rw-   0        0        0    11439 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/gui/grblconfiguration.py
--rw-rw-rw-   0        0        0     9172 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/gui/grblcontroller.py
--rw-rw-rw-   0        0        0     3861 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/gui/gui.py
--rw-rw-rw-   0        0        0     1615 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/interpreter.py
--rw-rw-rw-   0        0        0      617 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/loader.py
--rw-rw-rw-   0        0        0     2219 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/mock_connection.py
--rw-rw-rw-   0        0        0     8447 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/plugin.py
--rw-rw-rw-   0        0        0     2663 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/serial_connection.py
--rw-rw-rw-   0        0        0     2572 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/grbl/tcp_connection.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.920925 meerk40t-0.8.5000/meerk40t/gui/
--rw-rw-rw-   0        0        0       14 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/__init__.py
--rw-rw-rw-   0        0        0    11627 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/about.py
--rw-rw-rw-   0        0        0    64922 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/alignment.py
--rw-rw-rw-   0        0        0     2314 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/bufferview.py
--rw-rw-rw-   0        0        0     4325 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/busy.py
--rw-rw-rw-   0        0        0    62799 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/choicepropertypanel.py
--rw-rw-rw-   0        0        0    18111 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/consolepanel.py
--rw-rw-rw-   0        0        0    20551 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/devicepanel.py
--rw-rw-rw-   0        0        0     3866 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/dialogoptions.py
--rw-rw-rw-   0        0        0    12237 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/executejob.py
--rw-rw-rw-   0        0        0     2800 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/fonts.py
--rw-rw-rw-   0        0        0     4810 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/guicolors.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.922926 meerk40t-0.8.5000/meerk40t/gui/help_assets/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/help_assets/__init__.py
--rw-rw-rw-   0        0        0     9381 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/help_assets/help_assets.py
--rw-rw-rw-   0        0        0    31290 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/hersheymanager.py
--rw-rw-rw-   0        0        0   246387 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/icons.py
--rw-rw-rw-   0        0        0    19129 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/imagesplitter.py
--rw-rw-rw-   0        0        0    11758 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/keymap.py
--rw-rw-rw-   0        0        0    28136 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/laserpanel.py
--rw-rw-rw-   0        0        0    45142 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/laserrender.py
--rw-rw-rw-   0        0        0    30777 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/lasertoolpanel.py
--rw-rw-rw-   0        0        0    59131 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/materialtest.py
--rw-rw-rw-   0        0        0     3623 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/mkdebug.py
--rw-rw-rw-   0        0        0     4640 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/mwindow.py
--rw-rw-rw-   0        0        0    87911 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/navigationpanels.py
--rw-rw-rw-   0        0        0     4715 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/notes.py
--rw-rw-rw-   0        0        0    14969 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/opassignment.py
--rw-rw-rw-   0        0        0    10919 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/operation_info.py
--rw-rw-rw-   0        0        0    11787 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/plugin.py
--rw-rw-rw-   0        0        0    21548 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/position.py
--rw-rw-rw-   0        0        0    21902 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/preferences.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.943927 meerk40t-0.8.5000/meerk40t/gui/propertypanels/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/__init__.py
--rw-rw-rw-   0        0        0    38837 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/attributes.py
--rw-rw-rw-   0        0        0     5561 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/blobproperty.py
--rw-rw-rw-   0        0        0     2837 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/consoleproperty.py
--rw-rw-rw-   0        0        0     7360 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/groupproperties.py
--rw-rw-rw-   0        0        0    53880 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/imageproperty.py
--rw-rw-rw-   0        0        0     1781 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/inputproperty.py
--rw-rw-rw-   0        0        0     2612 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/opbranchproperties.py
--rw-rw-rw-   0        0        0    71934 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/operationpropertymain.py
--rw-rw-rw-   0        0        0     1789 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/outputproperty.py
--rw-rw-rw-   0        0        0    13370 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/pathproperty.py
--rw-rw-rw-   0        0        0    13701 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/placementproperty.py
--rw-rw-rw-   0        0        0     4398 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/pointproperty.py
--rw-rw-rw-   0        0        0     5748 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/propertywindow.py
--rw-rw-rw-   0        0        0    36709 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/rasterwizardpanels.py
--rw-rw-rw-   0        0        0    28059 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/textproperty.py
--rw-rw-rw-   0        0        0     1771 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/propertypanels/waitproperty.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.950927 meerk40t-0.8.5000/meerk40t/gui/scene/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scene/__init__.py
--rw-rw-rw-   0        0        0    33636 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scene/scene.py
--rw-rw-rw-   0        0        0      675 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scene/sceneconst.py
--rw-rw-rw-   0        0        0    11805 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scene/scenepanel.py
--rw-rw-rw-   0        0        0    13224 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scene/scenespacewidget.py
--rw-rw-rw-   0        0        0    16262 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scene/widget.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.966928 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/__init__.py
--rw-rw-rw-   0        0        0     7657 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/affinemover.py
--rw-rw-rw-   0        0        0    15658 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/attractionwidget.py
--rw-rw-rw-   0        0        0     3033 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/bedwidget.py
--rw-rw-rw-   0        0        0     3431 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/elementswidget.py
--rw-rw-rw-   0        0        0    28244 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/gridwidget.py
--rw-rw-rw-   0        0        0    29128 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/guidewidget.py
--rw-rw-rw-   0        0        0     1876 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/laserpathwidget.py
--rw-rw-rw-   0        0        0     2323 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/machineoriginwidget.py
--rw-rw-rw-   0        0        0    12777 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/rectselectwidget.py
--rw-rw-rw-   0        0        0     1196 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/relocatewidget.py
--rw-rw-rw-   0        0        0     2403 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/reticlewidget.py
--rw-rw-rw-   0        0        0   103410 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/scenewidgets/selectionwidget.py
--rw-rw-rw-   0        0        0    86262 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/simulation.py
--rw-rw-rw-   0        0        0     8323 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/snapoptions.py
--rw-rw-rw-   0        0        0    38968 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/spoolerpanel.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.976929 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/__init__.py
--rw-rw-rw-   0        0        0    17561 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/infowidget.py
--rw-rw-rw-   0        0        0    13740 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/opassignwidget.py
--rw-rw-rw-   0        0        0     3844 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/selectionwidget.py
--rw-rw-rw-   0        0        0     8335 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/shapepropwidget.py
--rw-rw-rw-   0        0        0     9756 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/statusbar.py
--rw-rw-rw-   0        0        0     9050 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/statusbarwidget.py
--rw-rw-rw-   0        0        0     9357 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/strokewidget.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:14.999930 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/__init__.py
--rw-rw-rw-   0        0        0      983 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/circlebrush.py
--rw-rw-rw-   0        0        0     8750 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolcircle.py
--rw-rw-rw-   0        0        0     1476 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolcontainer.py
--rw-rw-rw-   0        0        0     3313 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/tooldraw.py
--rw-rw-rw-   0        0        0     8603 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolellipse.py
--rw-rw-rw-   0        0        0     9358 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toollinetext.py
--rw-rw-rw-   0        0        0     7926 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolmeasure.py
--rw-rw-rw-   0        0        0    94628 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolnodeedit.py
--rw-rw-rw-   0        0        0     3425 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolplacement.py
--rw-rw-rw-   0        0        0     1791 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolpoint.py
--rw-rw-rw-   0        0        0     7078 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolpolygon.py
--rw-rw-rw-   0        0        0     7173 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolpolyline.py
--rw-rw-rw-   0        0        0     8146 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolrect.py
--rw-rw-rw-   0        0        0     2229 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolrelocate.py
--rw-rw-rw-   0        0        0     4234 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolribbon.py
--rw-rw-rw-   0        0        0     3061 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/tooltext.py
--rw-rw-rw-   0        0        0     7516 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolvector.py
--rw-rw-rw-   0        0        0     1194 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolwidget.py
--rw-rw-rw-   0        0        0     2844 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/usbconnect.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.013931 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/__init__.py
--rw-rw-rw-   0        0        0      737 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/buttonwidget.py
--rw-rw-rw-   0        0        0     2812 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/checkboxwidget.py
--rw-rw-rw-   0        0        0      385 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/controlwidget.py
--rw-rw-rw-   0        0        0    11773 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/cyclocycloidwidget.py
--rw-rw-rw-   0        0        0      926 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/handlewidget.py
--rw-rw-rw-   0        0        0    13518 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/harmonograph.py
--rw-rw-rw-   0        0        0     1073 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/openclosewidget.py
--rw-rw-rw-   0        0        0     1914 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/rotationwidget.py
--rw-rw-rw-   0        0        0     2776 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/scalewidget.py
--rw-rw-rw-   0        0        0     5697 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/seekbarwidget.py
--rw-rw-rw-   0        0        0     5167 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/togglewidget.py
--rw-rw-rw-   0        0        0      344 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/toolbarwidget.py
--rw-rw-rw-   0        0        0    35380 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/wordlisteditor.py
--rw-rw-rw-   0        0        0    38532 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/wxmeerk40t.py
--rw-rw-rw-   0        0        0   143768 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/wxmmain.py
--rw-rw-rw-   0        0        0    54351 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/wxmribbon.py
--rw-rw-rw-   0        0        0    54685 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/wxmscene.py
--rw-rw-rw-   0        0        0    70720 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/wxmtree.py
--rw-rw-rw-   0        0        0    32739 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/wxutils.py
--rw-rw-rw-   0        0        0     2807 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/gui/zmatrix.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.015931 meerk40t-0.8.5000/meerk40t/image/
--rw-rw-rw-   0        0        0       16 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/image/__init__.py
--rw-rw-rw-   0        0        0    65324 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/image/imagetools.py
--rw-rw-rw-   0        0        0     3073 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/internal_plugins.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.032932 meerk40t-0.8.5000/meerk40t/kernel/
--rw-rw-rw-   0        0        0      321 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/__init__.py
--rw-rw-rw-   0        0        0     6819 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/channel.py
--rw-rw-rw-   0        0        0    18178 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/context.py
--rw-rw-rw-   0        0        0     1187 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/exceptions.py
--rw-rw-rw-   0        0        0    14995 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/functions.py
--rw-rw-rw-   0        0        0     2815 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/jobs.py
--rw-rw-rw-   0        0        0   132435 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/kernel.py
--rw-rw-rw-   0        0        0     2263 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/lifecycles.py
--rw-rw-rw-   0        0        0     1941 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/module.py
--rw-rw-rw-   0        0        0     5212 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/service.py
--rw-rw-rw-   0        0        0    11606 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/settings.py
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/kernel/states.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.043933 meerk40t-0.8.5000/meerk40t/lihuiyu/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/__init__.py
--rw-rw-rw-   0        0        0    31573 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/controller.py
--rw-rw-rw-   0        0        0    40110 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/device.py
--rw-rw-rw-   0        0        0    45813 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/driver.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.051933 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/gui.py
--rw-rw-rw-   0        0        0    16374 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhyaccelgui.py
--rw-rw-rw-   0        0        0    25348 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhycontrollergui.py
--rw-rw-rw-   0        0        0    17367 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhydrivergui.py
--rw-rw-rw-   0        0        0     9731 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhyoperationproperties.py
--rw-rw-rw-   0        0        0     7407 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/gui/tcpcontroller.py
--rw-rw-rw-   0        0        0     1692 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/interpreter.py
--rw-rw-rw-   0        0        0    16341 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/laserspeed.py
--rw-rw-rw-   0        0        0     2622 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/loader.py
--rw-rw-rw-   0        0        0    13937 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/parser.py
--rw-rw-rw-   0        0        0     3815 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/plugin.py
--rw-rw-rw-   0        0        0     3474 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/lihuiyu/tcp_connection.py
--rw-rw-rw-   0        0        0     4043 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/main.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.057933 meerk40t-0.8.5000/meerk40t/moshi/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/__init__.py
--rw-rw-rw-   0        0        0    13904 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/builder.py
--rw-rw-rw-   0        0        0    17471 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/controller.py
--rw-rw-rw-   0        0        0    15227 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/device.py
--rw-rw-rw-   0        0        0    22753 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/driver.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.062934 meerk40t-0.8.5000/meerk40t/moshi/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/gui/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/gui/gui.py
--rw-rw-rw-   0        0        0    21985 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/gui/moshicontrollergui.py
--rw-rw-rw-   0        0        0     3661 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/gui/moshidrivergui.py
--rw-rw-rw-   0        0        0     1462 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/moshi/plugin.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.068934 meerk40t-0.8.5000/meerk40t/network/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/network/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/network/console_server.py
--rw-rw-rw-   0        0        0      326 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/network/kernelserver.py
--rw-rw-rw-   0        0        0     4958 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/network/tcp_server.py
--rw-rw-rw-   0        0        0     2680 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/network/udp_server.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.077935 meerk40t-0.8.5000/meerk40t/newly/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/__init__.py
--rw-rw-rw-   0        0        0    35613 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/controller.py
--rw-rw-rw-   0        0        0    25047 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/device.py
--rw-rw-rw-   0        0        0    12304 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/driver.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.083935 meerk40t-0.8.5000/meerk40t/newly/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/gui/__init__.py
--rw-rw-rw-   0        0        0     7263 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/gui/gui.py
--rw-rw-rw-   0        0        0     3586 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/gui/newlyconfig.py
--rw-rw-rw-   0        0        0     6105 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/gui/newlycontroller.py
--rw-rw-rw-   0        0        0     1504 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/gui/operationproperties.py
--rw-rw-rw-   0        0        0     2646 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/mock_connection.py
--rw-rw-rw-   0        0        0     1642 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/newly_params.py
--rw-rw-rw-   0        0        0    44191 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/plugin.py
--rw-rw-rw-   0        0        0    12062 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/newly/usb_connection.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.085935 meerk40t-0.8.5000/meerk40t/rotary/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/rotary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.089935 meerk40t-0.8.5000/meerk40t/rotary/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/rotary/gui/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/rotary/gui/gui.py
--rw-rw-rw-   0        0        0     9599 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/rotary/gui/rotarysettings.py
--rw-rw-rw-   0        0        0     3187 2023-06-13 22:01:37.000000 meerk40t-0.8.5000/meerk40t/rotary/rotary.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.102936 meerk40t-0.8.5000/meerk40t/ruida/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/__init__.py
--rw-rw-rw-   0        0        0     3256 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/control.py
--rw-rw-rw-   0        0        0    31762 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/controller.py
--rw-rw-rw-   0        0        0     6918 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/device.py
--rw-rw-rw-   0        0        0    15187 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/driver.py
--rw-rw-rw-   0        0        0    53030 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/emulator.py
--rw-rw-rw-   0        0        0      120 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.108936 meerk40t-0.8.5000/meerk40t/ruida/gui/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/gui/__init__.py
--rw-rw-rw-   0        0        0     2840 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/gui/gui.py
--rw-rw-rw-   0        0        0     2505 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/gui/ruidaconfig.py
--rw-rw-rw-   0        0        0     5987 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/gui/ruidacontroller.py
--rw-rw-rw-   0        0        0     1274 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/gui/ruidaoperationproperties.py
--rw-rw-rw-   0        0        0      657 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/loader.py
--rw-rw-rw-   0        0        0     3654 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/mock_connection.py
--rw-rw-rw-   0        0        0     3157 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/plugin.py
--rw-rw-rw-   0        0        0    44885 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/ruida/rdjob.py
--rw-rw-rw-   0        0        0   342603 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/svgelements.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.124937 meerk40t-0.8.5000/meerk40t/tools/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/__init__.py
--rw-rw-rw-   0        0        0    21288 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/driver_to_path.py
--rw-rw-rw-   0        0        0    95497 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/geomstr.py
--rw-rw-rw-   0        0        0    12007 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/jhfparser.py
--rw-rw-rw-   0        0        0    33970 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/kerftest.py
--rw-rw-rw-   0        0        0    42419 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/livinghinges.py
--rw-rw-rw-   0        0        0    31344 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/pathtools.py
--rw-rw-rw-   0        0        0    35800 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/pointfinder.py
--rw-rw-rw-   0        0        0    28108 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/polybool.py
--rw-rw-rw-   0        0        0    20221 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/rasterplotter.py
--rw-rw-rw-   0        0        0    30973 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/shxparser.py
--rw-rw-rw-   0        0        0    16287 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/ttfparser.py
--rw-rw-rw-   0        0        0    20709 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/meerk40t/tools/zinglplotter.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.167940 meerk40t-0.8.5000/meerk40t.egg-info/
--rw-rw-rw-   0        0        0     5619 2023-06-13 22:02:14.000000 meerk40t-0.8.5000/meerk40t.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    27065 2023-06-13 22:02:14.000000 meerk40t-0.8.5000/meerk40t.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 22:02:14.000000 meerk40t-0.8.5000/meerk40t.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-13 22:02:14.000000 meerk40t-0.8.5000/meerk40t.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      290 2023-06-13 22:02:14.000000 meerk40t-0.8.5000/meerk40t.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 22:02:14.000000 meerk40t-0.8.5000/meerk40t.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2021-01-18 14:07:22.000000 meerk40t-0.8.5000/meerk40t.egg-info/zip-safe
--rw-rw-rw-   0        0        0    20222 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/pyproject.toml
--rw-rw-rw-   0        0        0     1128 2023-06-13 22:02:15.270945 meerk40t-0.8.5000/setup.cfg
--rw-rw-rw-   0        0        0      599 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 22:02:15.152939 meerk40t-0.8.5000/test/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/__init__.py
--rw-rw-rw-   0        0        0     1493 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/bootstrap.py
--rw-rw-rw-   0        0        0      232 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_cli.py
--rw-rw-rw-   0        0        0    17155 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_core_cutcode.py
--rw-rw-rw-   0        0        0     4323 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_core_elements.py
--rw-rw-rw-   0        0        0    14608 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_core_plotplanner.py
--rw-rw-rw-   0        0        0    13401 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_core_viewports.py
--rw-rw-rw-   0        0        0     2393 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_drivers_grbl.py
--rw-rw-rw-   0        0        0    16583 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_drivers_lihuiyu.py
--rw-rw-rw-   0        0        0     2343 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_element_degenerate_points.py
--rw-rw-rw-   0        0        0     3341 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_elements_classify.py
--rw-rw-rw-   0        0        0      632 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_elements_penbox.py
--rw-rw-rw-   0        0        0     5392 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_fill.py
--rw-rw-rw-   0        0        0    32697 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_geomstr.py
--rw-rw-rw-   0        0        0    12913 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_imagetools_actualize.py
--rw-rw-rw-   0        0        0    11767 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_imagetools_wizard.py
--rw-rw-rw-   0        0        0     4701 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_kernel.py
--rw-rw-rw-   0        0        0   107060 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_laser_speeds.py
--rw-rw-rw-   0        0        0     2138 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_length.py
--rw-rw-rw-   0        0        0     2281 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_lifecycle.py
--rw-rw-rw-   0        0        0     1119 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_operations_hatch.py
--rw-rw-rw-   0        0        0      591 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_spooler.py
--rw-rw-rw-   0        0        0     4624 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_wobble.py
--rw-rw-rw-   0        0        0     4190 2023-06-13 22:01:38.000000 meerk40t-0.8.5000/test/test_zingl.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.223701 meerk40t-0.8.6000/
+-rw-rw-rw-   0        0        0     1086 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/LICENSE
+-rw-rw-rw-   0        0        0     5018 2023-07-20 13:53:49.224701 meerk40t-0.8.6000/PKG-INFO
+-rw-rw-rw-   0        0        0     3981 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.460657 meerk40t-0.8.6000/meerk40t/
+-rw-rw-rw-   0        0        0       19 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.480658 meerk40t-0.8.6000/meerk40t/balormk/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/balormk/__init__.py
+-rw-rw-rw-   0        0        0     5556 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/balormk/balor_params.py
+-rw-rw-rw-   0        0        0    46666 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/controller.py
+-rw-rw-rw-   0        0        0    69640 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/device.py
+-rw-rw-rw-   0        0        0    20843 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/driver.py
+-rw-rw-rw-   0        0        0     5304 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/elementlightjob.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.487659 meerk40t-0.8.6000/meerk40t/balormk/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/balormk/gui/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/gui/balorconfig.py
+-rw-rw-rw-   0        0        0     5987 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/gui/balorcontroller.py
+-rw-rw-rw-   0        0        0     5858 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/balormk/gui/baloroperationproperties.py
+-rw-rw-rw-   0        0        0     5311 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/gui/gui.py
+-rw-rw-rw-   0        0        0     7755 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/livefulllightjob.py
+-rw-rw-rw-   0        0        0     5981 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/balormk/liveselectionlightjob.py
+-rw-rw-rw-   0        0        0     3646 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/balormk/mock_connection.py
+-rw-rw-rw-   0        0        0     4991 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/balormk/plugin.py
+-rw-rw-rw-   0        0        0    11181 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/balormk/usb_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.491659 meerk40t-0.8.6000/meerk40t/camera/
+-rw-rw-rw-   0        0        0       17 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/camera/__init__.py
+-rw-rw-rw-   0        0        0    13273 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/camera/camera.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.496659 meerk40t-0.8.6000/meerk40t/camera/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/camera/gui/__init__.py
+-rw-rw-rw-   0        0        0    40400 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/camera/gui/camerapanel.py
+-rw-rw-rw-   0        0        0     2341 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/camera/gui/gui.py
+-rw-rw-rw-   0        0        0    10112 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/camera/plugin.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.506660 meerk40t-0.8.6000/meerk40t/ch341/
+-rw-rw-rw-   0        0        0      739 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/ch341/__init__.py
+-rw-rw-rw-   0        0        0    21369 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/ch341/libusb.py
+-rw-rw-rw-   0        0        0     5656 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/ch341/mock.py
+-rw-rw-rw-   0        0        0     6718 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/ch341/windll.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.540662 meerk40t-0.8.6000/meerk40t/core/
+-rw-rw-rw-   0        0        0       15 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/core/__init__.py
+-rw-rw-rw-   0        0        0    17576 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/bindalias.py
+-rw-rw-rw-   0        0        0      912 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/core.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.563663 meerk40t-0.8.6000/meerk40t/core/cutcode/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/__init__.py
+-rw-rw-rw-   0        0        0     2074 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/cubiccut.py
+-rw-rw-rw-   0        0        0    12473 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/cutcode.py
+-rw-rw-rw-   0        0        0     5392 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/cutgroup.py
+-rw-rw-rw-   0        0        0     5129 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/cutobject.py
+-rw-rw-rw-   0        0        0      847 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/dwellcut.py
+-rw-rw-rw-   0        0        0      727 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/gotocut.py
+-rw-rw-rw-   0        0        0      693 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/homecut.py
+-rw-rw-rw-   0        0        0      776 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/inputcut.py
+-rw-rw-rw-   0        0        0      952 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/linecut.py
+-rw-rw-rw-   0        0        0      786 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/outputcut.py
+-rw-rw-rw-   0        0        0    10566 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/plotcut.py
+-rw-rw-rw-   0        0        0     1653 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/quadcut.py
+-rw-rw-rw-   0        0        0     4189 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/rastercut.py
+-rw-rw-rw-   0        0        0      900 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/cutcode/waitcut.py
+-rw-rw-rw-   0        0        0    46028 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/cutplan.py
+-rw-rw-rw-   0        0        0     9898 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/drivers.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/element_commands.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.594665 meerk40t-0.8.6000/meerk40t/core/elements/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/elements/__init__.py
+-rw-rw-rw-   0        0        0    24050 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/align.py
+-rw-rw-rw-   0        0        0    50696 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/branches.py
+-rw-rw-rw-   0        0        0     7178 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/clipboard.py
+-rw-rw-rw-   0        0        0    96045 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/element_treeops.py
+-rw-rw-rw-   0        0        0     2667 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/element_types.py
+-rw-rw-rw-   0        0        0   150879 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/elements.py
+-rw-rw-rw-   0        0        0    19837 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/grid.py
+-rw-rw-rw-   0        0        0     3214 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/elements/materials.py
+-rw-rw-rw-   0        0        0     1152 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/elements/notes.py
+-rw-rw-rw-   0        0        0    27454 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/offset.py
+-rw-rw-rw-   0        0        0    10838 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/penbox.py
+-rw-rw-rw-   0        0        0     2345 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/elements/placements.py
+-rw-rw-rw-   0        0        0    23836 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/render.py
+-rw-rw-rw-   0        0        0    76714 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/shapes.py
+-rw-rw-rw-   0        0        0    16641 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/trace.py
+-rw-rw-rw-   0        0        0    14470 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/tree_commands.py
+-rw-rw-rw-   0        0        0     1571 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/elements/undo_redo.py
+-rw-rw-rw-   0        0        0     8274 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/elements/wordlist.py
+-rw-rw-rw-   0        0        0      269 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/exceptions.py
+-rw-rw-rw-   0        0        0     6790 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/laserjob.py
+-rw-rw-rw-   0        0        0     2136 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/logging.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.657669 meerk40t-0.8.6000/meerk40t/core/node/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/blobnode.py
+-rw-rw-rw-   0        0        0     4020 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/bootstrap.py
+-rw-rw-rw-   0        0        0      894 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/branch_elems.py
+-rw-rw-rw-   0        0        0     1188 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/branch_ops.py
+-rw-rw-rw-   0        0        0     1236 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/branch_regmark.py
+-rw-rw-rw-   0        0        0      937 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/cutnode.py
+-rw-rw-rw-   0        0        0     6801 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_ellipse.py
+-rw-rw-rw-   0        0        0     3187 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_geomstr.py
+-rw-rw-rw-   0        0        0    30142 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_image.py
+-rw-rw-rw-   0        0        0     6789 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_line.py
+-rw-rw-rw-   0        0        0     6597 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_path.py
+-rw-rw-rw-   0        0        0     2654 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_point.py
+-rw-rw-rw-   0        0        0     7041 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_polyline.py
+-rw-rw-rw-   0        0        0     6805 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_rect.py
+-rw-rw-rw-   0        0        0    15489 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/elem_text.py
+-rw-rw-rw-   0        0        0     1088 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/filenode.py
+-rw-rw-rw-   0        0        0     2139 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/groupnode.py
+-rw-rw-rw-   0        0        0     1881 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/lasercodenode.py
+-rw-rw-rw-   0        0        0      928 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/layernode.py
+-rw-rw-rw-   0        0        0     2172 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/node/mixins.py
+-rw-rw-rw-   0        0        0    37366 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/node.py
+-rw-rw-rw-   0        0        0     4015 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/nutils.py
+-rw-rw-rw-   0        0        0    12948 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/op_cut.py
+-rw-rw-rw-   0        0        0    10483 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/op_dots.py
+-rw-rw-rw-   0        0        0    12341 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/op_engrave.py
+-rw-rw-rw-   0        0        0    15348 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/op_hatch.py
+-rw-rw-rw-   0        0        0    14692 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/op_image.py
+-rw-rw-rw-   0        0        0    20806 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/op_raster.py
+-rw-rw-rw-   0        0        0     1567 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/place_current.py
+-rw-rw-rw-   0        0        0     4869 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/place_point.py
+-rw-rw-rw-   0        0        0     1580 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/refnode.py
+-rw-rw-rw-   0        0        0     7504 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/rootnode.py
+-rw-rw-rw-   0        0        0     1511 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/util_console.py
+-rw-rw-rw-   0        0        0     2216 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/node/util_goto.py
+-rw-rw-rw-   0        0        0     1955 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/util_home.py
+-rw-rw-rw-   0        0        0     3411 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/util_input.py
+-rw-rw-rw-   0        0        0     3451 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/core/node/util_output.py
+-rw-rw-rw-   0        0        0     2220 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/node/util_wait.py
+-rw-rw-rw-   0        0        0    16615 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/core/parameters.py
+-rw-rw-rw-   0        0        0    30751 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/planner.py
+-rw-rw-rw-   0        0        0    22754 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/plotplanner.py
+-rw-rw-rw-   0        0        0     3972 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/space.py
+-rw-rw-rw-   0        0        0    25069 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/spoolers.py
+-rw-rw-rw-   0        0        0    48106 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/svg_io.py
+-rw-rw-rw-   0        0        0     6158 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/treeop.py
+-rw-rw-rw-   0        0        0     3159 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/undos.py
+-rw-rw-rw-   0        0        0    31404 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/units.py
+-rw-rw-rw-   0        0        0     7764 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/view.py
+-rw-rw-rw-   0        0        0     2866 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/webhelp.py
+-rw-rw-rw-   0        0        0    18364 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/core/wordlist.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.660669 meerk40t-0.8.6000/meerk40t/device/
+-rw-rw-rw-   0        0        0       17 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/device/__init__.py
+-rw-rw-rw-   0        0        0     4253 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/basedevice.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.671669 meerk40t-0.8.6000/meerk40t/device/ch341/
+-rw-rw-rw-   0        0        0       16 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/ch341/__init__.py
+-rw-rw-rw-   0        0        0     7197 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/ch341/ch341.py
+-rw-rw-rw-   0        0        0    16050 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/ch341/ch341libusbdriver.py
+-rw-rw-rw-   0        0        0     5505 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/ch341/libusb.py
+-rw-rw-rw-   0        0        0     5948 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/ch341/mock.py
+-rw-rw-rw-   0        0        0     6759 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/ch341/windll.py
+-rw-rw-rw-   0        0        0     4504 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/device/dummydevice.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.677670 meerk40t-0.8.6000/meerk40t/device/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/device/gui/__init__.py
+-rw-rw-rw-   0        0        0    23684 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/gui/defaultactions.py
+-rw-rw-rw-   0        0        0     9860 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/device/gui/formatterpanel.py
+-rw-rw-rw-   0        0        0     9284 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/device/gui/warningpanel.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.681670 meerk40t-0.8.6000/meerk40t/dxf/
+-rw-rw-rw-   0        0        0       14 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/dxf/__init__.py
+-rw-rw-rw-   0        0        0    23432 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/dxf/dxf_io.py
+-rw-rw-rw-   0        0        0     1318 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/dxf/plugin.py
+-rw-rw-rw-   0        0        0     1245 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/external_plugins.py
+-rw-rw-rw-   0        0        0      885 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/external_plugins_build.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.699671 meerk40t-0.8.6000/meerk40t/extra/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/extra/__init__.py
+-rw-rw-rw-   0        0        0     4516 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/extra/cag.py
+-rw-rw-rw-   0        0        0     2027 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/extra/embroider.py
+-rw-rw-rw-   0        0        0    36959 2023-07-20 13:26:33.000000 meerk40t-0.8.6000/meerk40t/extra/ezd.py
+-rw-rw-rw-   0        0        0    12009 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/extra/hershey.py
+-rw-rw-rw-   0        0        0    13066 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/extra/imageactions.py
+-rw-rw-rw-   0        0        0    23455 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/extra/inkscape.py
+-rw-rw-rw-   0        0        0     8348 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/extra/pathoptimize.py
+-rw-rw-rw-   0        0        0     9470 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/extra/potrace.py
+-rw-rw-rw-   0        0        0    14647 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/extra/updater.py
+-rw-rw-rw-   0        0        0     5120 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/extra/vectrace.py
+-rw-rw-rw-   0        0        0     2769 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/extra/winsleep.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.704671 meerk40t-0.8.6000/meerk40t/fill/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/fill/__init__.py
+-rw-rw-rw-   0        0        0    10399 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/fill/fills.py
+-rw-rw-rw-   0        0        0    38279 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/fill/patternfill.py
+-rw-rw-rw-   0        0        0    16519 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/fill/patterns.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.720672 meerk40t-0.8.6000/meerk40t/grbl/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/grbl/__init__.py
+-rw-rw-rw-   0        0        0     2702 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/grbl/control.py
+-rw-rw-rw-   0        0        0    27956 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/grbl/controller.py
+-rw-rw-rw-   0        0        0    27885 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/grbl/device.py
+-rw-rw-rw-   0        0        0    22840 2023-07-20 12:20:35.000000 meerk40t-0.8.6000/meerk40t/grbl/driver.py
+-rw-rw-rw-   0        0        0    18636 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/grbl/emulator.py
+-rw-rw-rw-   0        0        0    28028 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/grbl/gcodejob.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.725672 meerk40t-0.8.6000/meerk40t/grbl/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/grbl/gui/__init__.py
+-rw-rw-rw-   0        0        0    11439 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/grbl/gui/grblconfiguration.py
+-rw-rw-rw-   0        0        0     9172 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/grbl/gui/grblcontroller.py
+-rw-rw-rw-   0        0        0     3861 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/grbl/gui/gui.py
+-rw-rw-rw-   0        0        0     1615 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/grbl/interpreter.py
+-rw-rw-rw-   0        0        0      617 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/grbl/loader.py
+-rw-rw-rw-   0        0        0     2219 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/grbl/mock_connection.py
+-rw-rw-rw-   0        0        0     8447 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/grbl/plugin.py
+-rw-rw-rw-   0        0        0     2663 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/grbl/serial_connection.py
+-rw-rw-rw-   0        0        0     2572 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/grbl/tcp_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.790676 meerk40t-0.8.6000/meerk40t/gui/
+-rw-rw-rw-   0        0        0       14 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/gui/__init__.py
+-rw-rw-rw-   0        0        0    11627 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/about.py
+-rw-rw-rw-   0        0        0    64922 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/alignment.py
+-rw-rw-rw-   0        0        0     2314 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/bufferview.py
+-rw-rw-rw-   0        0        0     4325 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/busy.py
+-rw-rw-rw-   0        0        0    62799 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/choicepropertypanel.py
+-rw-rw-rw-   0        0        0    18111 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/consolepanel.py
+-rw-rw-rw-   0        0        0    20551 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/devicepanel.py
+-rw-rw-rw-   0        0        0     3866 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/dialogoptions.py
+-rw-rw-rw-   0        0        0    12237 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/executejob.py
+-rw-rw-rw-   0        0        0     2800 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/fonts.py
+-rw-rw-rw-   0        0        0     4810 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/guicolors.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.792676 meerk40t-0.8.6000/meerk40t/gui/help_assets/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/help_assets/__init__.py
+-rw-rw-rw-   0        0        0     9381 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/help_assets/help_assets.py
+-rw-rw-rw-   0        0        0    31290 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/hersheymanager.py
+-rw-rw-rw-   0        0        0   246387 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/icons.py
+-rw-rw-rw-   0        0        0    19129 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/imagesplitter.py
+-rw-rw-rw-   0        0        0    11758 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/keymap.py
+-rw-rw-rw-   0        0        0    28136 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/laserpanel.py
+-rw-rw-rw-   0        0        0    45142 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/laserrender.py
+-rw-rw-rw-   0        0        0    30777 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/lasertoolpanel.py
+-rw-rw-rw-   0        0        0    59131 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/materialtest.py
+-rw-rw-rw-   0        0        0     3623 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/mkdebug.py
+-rw-rw-rw-   0        0        0     4640 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/mwindow.py
+-rw-rw-rw-   0        0        0    88317 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/navigationpanels.py
+-rw-rw-rw-   0        0        0     4715 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/notes.py
+-rw-rw-rw-   0        0        0    14969 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/opassignment.py
+-rw-rw-rw-   0        0        0    10919 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/operation_info.py
+-rw-rw-rw-   0        0        0    11787 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/plugin.py
+-rw-rw-rw-   0        0        0    21970 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/position.py
+-rw-rw-rw-   0        0        0    21902 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/preferences.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.821678 meerk40t-0.8.6000/meerk40t/gui/propertypanels/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/__init__.py
+-rw-rw-rw-   0        0        0    39302 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/attributes.py
+-rw-rw-rw-   0        0        0     5561 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/blobproperty.py
+-rw-rw-rw-   0        0        0     2837 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/consoleproperty.py
+-rw-rw-rw-   0        0        0     7360 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/groupproperties.py
+-rw-rw-rw-   0        0        0    53880 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/imageproperty.py
+-rw-rw-rw-   0        0        0     1781 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/inputproperty.py
+-rw-rw-rw-   0        0        0     2612 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/opbranchproperties.py
+-rw-rw-rw-   0        0        0    71934 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/operationpropertymain.py
+-rw-rw-rw-   0        0        0     1789 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/outputproperty.py
+-rw-rw-rw-   0        0        0    13540 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/pathproperty.py
+-rw-rw-rw-   0        0        0    13701 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/placementproperty.py
+-rw-rw-rw-   0        0        0     4398 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/pointproperty.py
+-rw-rw-rw-   0        0        0     6300 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/propertywindow.py
+-rw-rw-rw-   0        0        0    36709 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/rasterwizardpanels.py
+-rw-rw-rw-   0        0        0    28059 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/textproperty.py
+-rw-rw-rw-   0        0        0     1771 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/propertypanels/waitproperty.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.830679 meerk40t-0.8.6000/meerk40t/gui/scene/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/gui/scene/__init__.py
+-rw-rw-rw-   0        0        0    33636 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/scene/scene.py
+-rw-rw-rw-   0        0        0      675 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/scene/sceneconst.py
+-rw-rw-rw-   0        0        0    11805 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/scene/scenepanel.py
+-rw-rw-rw-   0        0        0    13224 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scene/scenespacewidget.py
+-rw-rw-rw-   0        0        0    16262 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/scene/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.849680 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/__init__.py
+-rw-rw-rw-   0        0        0     7657 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/affinemover.py
+-rw-rw-rw-   0        0        0    15658 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/attractionwidget.py
+-rw-rw-rw-   0        0        0     3033 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/bedwidget.py
+-rw-rw-rw-   0        0        0     3431 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/elementswidget.py
+-rw-rw-rw-   0        0        0    28379 2023-07-20 12:20:35.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/gridwidget.py
+-rw-rw-rw-   0        0        0    29128 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/guidewidget.py
+-rw-rw-rw-   0        0        0     1876 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/laserpathwidget.py
+-rw-rw-rw-   0        0        0     2323 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/machineoriginwidget.py
+-rw-rw-rw-   0        0        0    12777 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/rectselectwidget.py
+-rw-rw-rw-   0        0        0     1196 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/relocatewidget.py
+-rw-rw-rw-   0        0        0     2403 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/reticlewidget.py
+-rw-rw-rw-   0        0        0   103428 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/scenewidgets/selectionwidget.py
+-rw-rw-rw-   0        0        0    86262 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/simulation.py
+-rw-rw-rw-   0        0        0     8323 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/snapoptions.py
+-rw-rw-rw-   0        0        0    38968 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/spoolerpanel.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.860680 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/__init__.py
+-rw-rw-rw-   0        0        0    17561 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/infowidget.py
+-rw-rw-rw-   0        0        0    13740 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/opassignwidget.py
+-rw-rw-rw-   0        0        0     3844 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/selectionwidget.py
+-rw-rw-rw-   0        0        0     8335 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/shapepropwidget.py
+-rw-rw-rw-   0        0        0     9756 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/statusbar.py
+-rw-rw-rw-   0        0        0     9050 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/statusbarwidget.py
+-rw-rw-rw-   0        0        0     9357 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/strokewidget.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.888682 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/circlebrush.py
+-rw-rw-rw-   0        0        0     8750 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolcircle.py
+-rw-rw-rw-   0        0        0     1476 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolcontainer.py
+-rw-rw-rw-   0        0        0     3313 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/tooldraw.py
+-rw-rw-rw-   0        0        0     8603 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolellipse.py
+-rw-rw-rw-   0        0        0     9358 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toollinetext.py
+-rw-rw-rw-   0        0        0     7926 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolmeasure.py
+-rw-rw-rw-   0        0        0    94628 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolnodeedit.py
+-rw-rw-rw-   0        0        0     3425 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolplacement.py
+-rw-rw-rw-   0        0        0     1791 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolpoint.py
+-rw-rw-rw-   0        0        0     7078 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolpolygon.py
+-rw-rw-rw-   0        0        0     7173 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolpolyline.py
+-rw-rw-rw-   0        0        0     8146 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolrect.py
+-rw-rw-rw-   0        0        0     2229 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolrelocate.py
+-rw-rw-rw-   0        0        0     4234 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolribbon.py
+-rw-rw-rw-   0        0        0     3061 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/tooltext.py
+-rw-rw-rw-   0        0        0     7516 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolvector.py
+-rw-rw-rw-   0        0        0     1194 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolwidget.py
+-rw-rw-rw-   0        0        0     2844 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/usbconnect.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.908683 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/buttonwidget.py
+-rw-rw-rw-   0        0        0     2812 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/checkboxwidget.py
+-rw-rw-rw-   0        0        0      385 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/controlwidget.py
+-rw-rw-rw-   0        0        0    11773 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/cyclocycloidwidget.py
+-rw-rw-rw-   0        0        0      926 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/handlewidget.py
+-rw-rw-rw-   0        0        0    13518 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/harmonograph.py
+-rw-rw-rw-   0        0        0     1073 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/openclosewidget.py
+-rw-rw-rw-   0        0        0     1914 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/rotationwidget.py
+-rw-rw-rw-   0        0        0     2776 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/scalewidget.py
+-rw-rw-rw-   0        0        0     5697 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/seekbarwidget.py
+-rw-rw-rw-   0        0        0     5167 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/togglewidget.py
+-rw-rw-rw-   0        0        0      344 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/toolbarwidget.py
+-rw-rw-rw-   0        0        0    35380 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/wordlisteditor.py
+-rw-rw-rw-   0        0        0    38532 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/wxmeerk40t.py
+-rw-rw-rw-   0        0        0   143787 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/wxmmain.py
+-rw-rw-rw-   0        0        0    54351 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/wxmribbon.py
+-rw-rw-rw-   0        0        0    54685 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/wxmscene.py
+-rw-rw-rw-   0        0        0    70720 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/wxmtree.py
+-rw-rw-rw-   0        0        0    32739 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/gui/wxutils.py
+-rw-rw-rw-   0        0        0     2807 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/gui/zmatrix.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.911683 meerk40t-0.8.6000/meerk40t/image/
+-rw-rw-rw-   0        0        0       16 2023-06-13 22:01:37.000000 meerk40t-0.8.6000/meerk40t/image/__init__.py
+-rw-rw-rw-   0        0        0    65324 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/image/imagetools.py
+-rw-rw-rw-   0        0        0     3073 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/internal_plugins.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.929684 meerk40t-0.8.6000/meerk40t/kernel/
+-rw-rw-rw-   0        0        0      321 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/__init__.py
+-rw-rw-rw-   0        0        0     6819 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/channel.py
+-rw-rw-rw-   0        0        0    18178 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/kernel/context.py
+-rw-rw-rw-   0        0        0     1187 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/exceptions.py
+-rw-rw-rw-   0        0        0    14995 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/functions.py
+-rw-rw-rw-   0        0        0     2815 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/jobs.py
+-rw-rw-rw-   0        0        0   132709 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/kernel/kernel.py
+-rw-rw-rw-   0        0        0     2263 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/lifecycles.py
+-rw-rw-rw-   0        0        0     1941 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/module.py
+-rw-rw-rw-   0        0        0     5212 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/service.py
+-rw-rw-rw-   0        0        0    11606 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/kernel/settings.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/kernel/states.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.942685 meerk40t-0.8.6000/meerk40t/lihuiyu/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/__init__.py
+-rw-rw-rw-   0        0        0    31624 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/controller.py
+-rw-rw-rw-   0        0        0    40110 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/device.py
+-rw-rw-rw-   0        0        0    45811 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/driver.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.954686 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/__init__.py
+-rw-rw-rw-   0        0        0     4089 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/gui.py
+-rw-rw-rw-   0        0        0    16374 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhyaccelgui.py
+-rw-rw-rw-   0        0        0    25333 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhycontrollergui.py
+-rw-rw-rw-   0        0        0    17367 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhydrivergui.py
+-rw-rw-rw-   0        0        0     9731 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhyoperationproperties.py
+-rw-rw-rw-   0        0        0     7407 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/gui/tcpcontroller.py
+-rw-rw-rw-   0        0        0     1692 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/interpreter.py
+-rw-rw-rw-   0        0        0    16341 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/laserspeed.py
+-rw-rw-rw-   0        0        0     2622 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/loader.py
+-rw-rw-rw-   0        0        0    13937 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/parser.py
+-rw-rw-rw-   0        0        0     3815 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/plugin.py
+-rw-rw-rw-   0        0        0     3474 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/lihuiyu/tcp_connection.py
+-rw-rw-rw-   0        0        0     4043 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/main.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.962686 meerk40t-0.8.6000/meerk40t/moshi/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/moshi/__init__.py
+-rw-rw-rw-   0        0        0    13904 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/moshi/builder.py
+-rw-rw-rw-   0        0        0    17471 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/moshi/controller.py
+-rw-rw-rw-   0        0        0    15227 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/moshi/device.py
+-rw-rw-rw-   0        0        0    22753 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/moshi/driver.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.968686 meerk40t-0.8.6000/meerk40t/moshi/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/moshi/gui/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/moshi/gui/gui.py
+-rw-rw-rw-   0        0        0    21985 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/moshi/gui/moshicontrollergui.py
+-rw-rw-rw-   0        0        0     3661 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/moshi/gui/moshidrivergui.py
+-rw-rw-rw-   0        0        0     1462 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/moshi/plugin.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.975687 meerk40t-0.8.6000/meerk40t/network/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/network/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/network/console_server.py
+-rw-rw-rw-   0        0        0      326 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/network/kernelserver.py
+-rw-rw-rw-   0        0        0     4958 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/network/tcp_server.py
+-rw-rw-rw-   0        0        0     2680 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/network/udp_server.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.988688 meerk40t-0.8.6000/meerk40t/newly/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/newly/__init__.py
+-rw-rw-rw-   0        0        0    35613 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/newly/controller.py
+-rw-rw-rw-   0        0        0    25848 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/newly/device.py
+-rw-rw-rw-   0        0        0    12304 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/newly/driver.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:48.997688 meerk40t-0.8.6000/meerk40t/newly/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/newly/gui/__init__.py
+-rw-rw-rw-   0        0        0     7263 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/newly/gui/gui.py
+-rw-rw-rw-   0        0        0     3586 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/newly/gui/newlyconfig.py
+-rw-rw-rw-   0        0        0     6105 2023-07-20 12:59:46.000000 meerk40t-0.8.6000/meerk40t/newly/gui/newlycontroller.py
+-rw-rw-rw-   0        0        0     1504 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/newly/gui/operationproperties.py
+-rw-rw-rw-   0        0        0     2646 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/newly/mock_connection.py
+-rw-rw-rw-   0        0        0     1642 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/newly/newly_params.py
+-rw-rw-rw-   0        0        0    44191 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/newly/plugin.py
+-rw-rw-rw-   0        0        0    12062 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/newly/usb_connection.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.000688 meerk40t-0.8.6000/meerk40t/rotary/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/rotary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.004688 meerk40t-0.8.6000/meerk40t/rotary/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/rotary/gui/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/rotary/gui/gui.py
+-rw-rw-rw-   0        0        0     9599 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/rotary/gui/rotarysettings.py
+-rw-rw-rw-   0        0        0     3187 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/rotary/rotary.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.020689 meerk40t-0.8.6000/meerk40t/ruida/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/__init__.py
+-rw-rw-rw-   0        0        0     3256 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/control.py
+-rw-rw-rw-   0        0        0    31762 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/controller.py
+-rw-rw-rw-   0        0        0     7618 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/ruida/device.py
+-rw-rw-rw-   0        0        0    15187 2023-07-20 11:53:01.000000 meerk40t-0.8.6000/meerk40t/ruida/driver.py
+-rw-rw-rw-   0        0        0    53030 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/ruida/emulator.py
+-rw-rw-rw-   0        0        0      120 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.029690 meerk40t-0.8.6000/meerk40t/ruida/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/gui/__init__.py
+-rw-rw-rw-   0        0        0     2840 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/gui/gui.py
+-rw-rw-rw-   0        0        0     2505 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/ruida/gui/ruidaconfig.py
+-rw-rw-rw-   0        0        0     5987 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/ruida/gui/ruidacontroller.py
+-rw-rw-rw-   0        0        0     1274 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/gui/ruidaoperationproperties.py
+-rw-rw-rw-   0        0        0      657 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/ruida/loader.py
+-rw-rw-rw-   0        0        0     3654 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/ruida/mock_connection.py
+-rw-rw-rw-   0        0        0     3209 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/ruida/plugin.py
+-rw-rw-rw-   0        0        0    44885 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/ruida/rdjob.py
+-rw-rw-rw-   0        0        0   342603 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/svgelements.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.049691 meerk40t-0.8.6000/meerk40t/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:01:38.000000 meerk40t-0.8.6000/meerk40t/tools/__init__.py
+-rw-rw-rw-   0        0        0    21288 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/tools/driver_to_path.py
+-rw-rw-rw-   0        0        0    95497 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/tools/geomstr.py
+-rw-rw-rw-   0        0        0    12007 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/tools/jhfparser.py
+-rw-rw-rw-   0        0        0    33970 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/tools/kerftest.py
+-rw-rw-rw-   0        0        0    42419 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/tools/livinghinges.py
+-rw-rw-rw-   0        0        0    31411 2023-07-20 12:20:35.000000 meerk40t-0.8.6000/meerk40t/tools/pathtools.py
+-rw-rw-rw-   0        0        0    35800 2023-06-13 22:01:38.000000 meerk40t-0.8.6000/meerk40t/tools/pointfinder.py
+-rw-rw-rw-   0        0        0    28108 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/tools/polybool.py
+-rw-rw-rw-   0        0        0    20221 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/tools/rasterplotter.py
+-rw-rw-rw-   0        0        0    30973 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/meerk40t/tools/shxparser.py
+-rw-rw-rw-   0        0        0    16287 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/tools/ttfparser.py
+-rw-rw-rw-   0        0        0    20709 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/meerk40t/tools/zinglplotter.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.095694 meerk40t-0.8.6000/meerk40t.egg-info/
+-rw-rw-rw-   0        0        0     5018 2023-07-20 13:53:48.000000 meerk40t-0.8.6000/meerk40t.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    27406 2023-07-20 13:53:48.000000 meerk40t-0.8.6000/meerk40t.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 13:53:48.000000 meerk40t-0.8.6000/meerk40t.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-20 13:53:48.000000 meerk40t-0.8.6000/meerk40t.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      290 2023-07-20 13:53:48.000000 meerk40t-0.8.6000/meerk40t.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 13:53:48.000000 meerk40t-0.8.6000/meerk40t.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2021-01-18 14:07:22.000000 meerk40t-0.8.6000/meerk40t.egg-info/zip-safe
+-rw-rw-rw-   0        0        0    20222 2023-06-13 22:01:38.000000 meerk40t-0.8.6000/pyproject.toml
+-rw-rw-rw-   0        0        0     1128 2023-07-20 13:53:49.226701 meerk40t-0.8.6000/setup.cfg
+-rw-rw-rw-   0        0        0      599 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:53:49.083693 meerk40t-0.8.6000/test/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:01:38.000000 meerk40t-0.8.6000/test/__init__.py
+-rw-rw-rw-   0        0        0     1493 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/test/bootstrap.py
+-rw-rw-rw-   0        0        0      232 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_cli.py
+-rw-rw-rw-   0        0        0    17155 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_core_cutcode.py
+-rw-rw-rw-   0        0        0     4323 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/test/test_core_elements.py
+-rw-rw-rw-   0        0        0    14608 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_core_plotplanner.py
+-rw-rw-rw-   0        0        0    13401 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_core_viewports.py
+-rw-rw-rw-   0        0        0     2393 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_drivers_grbl.py
+-rw-rw-rw-   0        0        0    16583 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_drivers_lihuiyu.py
+-rw-rw-rw-   0        0        0     2343 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_element_degenerate_points.py
+-rw-rw-rw-   0        0        0     3341 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_elements_classify.py
+-rw-rw-rw-   0        0        0      632 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_elements_penbox.py
+-rw-rw-rw-   0        0        0     5392 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/test/test_fill.py
+-rw-rw-rw-   0        0        0    32697 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/test/test_geomstr.py
+-rw-rw-rw-   0        0        0    12913 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_imagetools_actualize.py
+-rw-rw-rw-   0        0        0    11767 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_imagetools_wizard.py
+-rw-rw-rw-   0        0        0     4701 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_kernel.py
+-rw-rw-rw-   0        0        0   107060 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_laser_speeds.py
+-rw-rw-rw-   0        0        0     2138 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_length.py
+-rw-rw-rw-   0        0        0     2281 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_lifecycle.py
+-rw-rw-rw-   0        0        0     1119 2023-07-20 12:59:47.000000 meerk40t-0.8.6000/test/test_operations_hatch.py
+-rw-rw-rw-   0        0        0      591 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_spooler.py
+-rw-rw-rw-   0        0        0     4624 2023-06-15 05:25:58.000000 meerk40t-0.8.6000/test/test_wobble.py
+-rw-rw-rw-   0        0        0     4190 2023-06-13 22:01:38.000000 meerk40t-0.8.6000/test/test_zingl.py
```

### Comparing `meerk40t-0.8.5000/LICENSE` & `meerk40t-0.8.6000/LICENSE`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/PKG-INFO` & `meerk40t-0.8.6000/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,16 @@
 Metadata-Version: 2.1
 Name: meerk40t
-Version: 0.8.5000
+Version: 0.8.6000
 Summary: MeerK40t LaserCutter Software
 Home-page: https://github.com/meerk40t/meerk40t
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
-Description: # MeerK40t
-        MeerK40t (pronounced MeerKat) is a built-from-the-ground-up MIT licensed open-source laser cutting software.
-        
-        ## Primary Goals
-        * Provide users with high quality laser control software.
-        * Provide developers with a highly extensible platform to help further their own ideas, and provide novel work to the laser community at large.
-        
-        ## Running
-        MeerK40t is written in Python and precompiled versions are [available for download](https://github.com/meerk40t/meerk40t/releases) for Windows, Mac OSX, Linux and Raspberry Pi. Due note this sometimes will give false postitives for various viruses (especially since Meerk40t isn't signed).
-        
-        Alternatively you can run MeerK40t directly from Python. `pip install meerk40t[all]` with python installed will usually be sufficient. Then merely run `meerk40t` at the command line.
-        
-        ### GUI
-        ![meerk40t8](https://user-images.githubusercontent.com/3302478/196283699-745d0616-5e74-49b3-ba95-f4902061584b.png)
-        
-        The wxMeerK40t is the GUI and is written in wxPython. We use AUI to allow to have a very highly configurable UI. We can easily add panes and tools and there are quite a few available already.
-        
-        ### Command Line Interface
-        
-        Meerk40t has an advanced internal console system allowing access to most parts of the code with various commands. It also provides a command line interface which should allow you to automate any processes.
-        
-        ## Drivers
-        
-        Meerk40t provides a variety of drivers with an extensible framework to provide support for other new laser devices. The code was written with the myriad of possibilities for different software in mind. For example, it may be essential that GRBL be able to reset an alarm or notify the user of particular error codes. The configuration for GRBL is not the same for the configuration of other laser control drivers. With this in mind, Meerk40t can radically change how and when it works
-        
-        
-        ### Supported devices
-        *   M2-Nano
-        *   Moshiboard
-        *   GRBL
-        *   Fibre Lasers based on the JCZ controllers (still experimental)
-        *   Ruida-Emulation (Middleman between Lightburn and K40)
-        
-        ### Lihuiyu M2-Nano
-        For the Lihuiyu (stock driver), Meerk40t supports both the windows and libusb connection methods, making it compatible with Whisperer and with the original Chinese software. So MeerK40t can usually run alongside these other pieces of software interchangeably.
-        
-        ### Galvo LMC
-        
-        Meerk40t supports controlling galvo as well as gantry lasers with open source support.
-        
-        ### Moshiboard
-        
-        The support for old moshiboards makes meerk40t the only known software opensource software that controls moshiboards.
-        
-        ### GRBL
-        
-        GRBL is itself open source and the various interfaces with the board should be quite well understood.
-        
-        ## Support
-        The primary source for help and documentation is the [MeerK40t Wiki - please click here](https://github.com/meerk40t/meerk40t/wiki).
-        
-        If you have a bug, feature request, or other issue raise it here. These are likely to be resolved. Squeaky wheels get the grease.
-        https://github.com/meerk40t/meerk40t/issues
-        
-        If you need additional support, please research/ask on:
-        
-        *   [Facebook](https://www.facebook.com/groups/716000085655097/)
-        *   [Maker Forums](https://forum.makerforums.info/t/about-the-meerk40t-category/79660)
-        *   [YouTube - David Olsen's channel](https://www.youtube.com/channel/UCsAUV23O2FyKxC0HN7nkAQQ)
-        *   [YouTube - Some instruction videos](https://www.youtube.com/channel/UCMN9gGvpacxZINPZCSOecaQ)
-        *   [Discord](https://discord.gg/vkDD3HdQq6)
-        
-        ## Assisting the Project
-        
-        Open source projects live and die with their support. There are a lots of ways to help the project. There are also a lot of ways the project should help you.
-        *   Code
-        *   Provide Translations in other languages.
-        *   Design ( Good design instincts, smooth out the rough edges)
-        *   Compile/Testers
-        *   Beta testers
-        *   Make helpful support content
-        *   Make guides ("How to setup cameras?", etc)
-        *   Bounce ideas around
-        
-        
 Keywords: lasercutter,laser,vector,parser
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -97,7 +21,83 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: gui
 Provides-Extra: cam
 Provides-Extra: dxf
 Provides-Extra: camhead
+License-File: LICENSE
+
+# MeerK40t
+MeerK40t (pronounced MeerKat) is a built-from-the-ground-up MIT licensed open-source laser cutting software.
+
+## Primary Goals
+* Provide users with high quality laser control software.
+* Provide developers with a highly extensible platform to help further their own ideas, and provide novel work to the laser community at large.
+
+## Running
+MeerK40t is written in Python and precompiled versions are [available for download](https://github.com/meerk40t/meerk40t/releases) for Windows, Mac OSX, Linux and Raspberry Pi. Due note this sometimes will give false postitives for various viruses (especially since Meerk40t isn't signed).
+
+Alternatively you can run MeerK40t directly from Python. `pip install meerk40t[all]` with python installed will usually be sufficient. Then merely run `meerk40t` at the command line.
+
+### GUI
+![meerk40t8](https://user-images.githubusercontent.com/3302478/196283699-745d0616-5e74-49b3-ba95-f4902061584b.png)
+
+The wxMeerK40t is the GUI and is written in wxPython. We use AUI to allow to have a very highly configurable UI. We can easily add panes and tools and there are quite a few available already.
+
+### Command Line Interface
+
+Meerk40t has an advanced internal console system allowing access to most parts of the code with various commands. It also provides a command line interface which should allow you to automate any processes.
+
+## Drivers
+
+Meerk40t provides a variety of drivers with an extensible framework to provide support for other new laser devices. The code was written with the myriad of possibilities for different software in mind. For example, it may be essential that GRBL be able to reset an alarm or notify the user of particular error codes. The configuration for GRBL is not the same for the configuration of other laser control drivers. With this in mind, Meerk40t can radically change how and when it works
+
+
+### Supported devices
+*   M2-Nano
+*   Moshiboard
+*   GRBL
+*   Fibre Lasers based on the JCZ controllers (still experimental)
+*   Ruida-Emulation (Middleman between Lightburn and K40)
+
+### Lihuiyu M2-Nano
+For the Lihuiyu (stock driver), Meerk40t supports both the windows and libusb connection methods, making it compatible with Whisperer and with the original Chinese software. So MeerK40t can usually run alongside these other pieces of software interchangeably.
+
+### Galvo LMC
+
+Meerk40t supports controlling galvo as well as gantry lasers with open source support.
+
+### Moshiboard
+
+The support for old moshiboards makes meerk40t the only known software opensource software that controls moshiboards.
+
+### GRBL
+
+GRBL is itself open source and the various interfaces with the board should be quite well understood.
+
+## Support
+The primary source for help and documentation is the [MeerK40t Wiki - please click here](https://github.com/meerk40t/meerk40t/wiki).
+
+If you have a bug, feature request, or other issue raise it here. These are likely to be resolved. Squeaky wheels get the grease.
+https://github.com/meerk40t/meerk40t/issues
+
+If you need additional support, please research/ask on:
+
+*   [Facebook](https://www.facebook.com/groups/716000085655097/)
+*   [Maker Forums](https://forum.makerforums.info/t/about-the-meerk40t-category/79660)
+*   [YouTube - David Olsen's channel](https://www.youtube.com/channel/UCsAUV23O2FyKxC0HN7nkAQQ)
+*   [YouTube - Some instruction videos](https://www.youtube.com/channel/UCMN9gGvpacxZINPZCSOecaQ)
+*   [Discord](https://discord.gg/vkDD3HdQq6)
+
+## Assisting the Project
+
+Open source projects live and die with their support. There are a lots of ways to help the project. There are also a lot of ways the project should help you.
+*   Code
+*   Provide Translations in other languages.
+*   Design ( Good design instincts, smooth out the rough edges)
+*   Compile/Testers
+*   Beta testers
+*   Make helpful support content
+*   Make guides ("How to setup cameras?", etc)
+*   Bounce ideas around
+
```

### Comparing `meerk40t-0.8.5000/README.md` & `meerk40t-0.8.6000/README.md`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/balor_params.py` & `meerk40t-0.8.6000/meerk40t/balormk/balor_params.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/controller.py` & `meerk40t-0.8.6000/meerk40t/balormk/controller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/device.py` & `meerk40t-0.8.6000/meerk40t/balormk/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,14 +866,19 @@
         )
         def estop(command, channel, _, data=None, remainder=None, **kwgs):
             channel("Stopping Job")
             if self.job is not None:
                 self.job.stop()
             self.spooler.clear_queue()
             self.driver.set_abort()
+            try:
+                channel("Resetting controller.")
+                self.driver.reset()
+            except ConnectionRefusedError:
+                pass
 
         @self.console_command(
             "pause",
             help=_("Pauses the currently running job"),
         )
         def pause(command, channel, _, data=None, remainder=None, **kwgs):
             if self.driver.paused:
```

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/driver.py` & `meerk40t-0.8.6000/meerk40t/balormk/driver.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/elementlightjob.py` & `meerk40t-0.8.6000/meerk40t/balormk/elementlightjob.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/gui/balorconfig.py` & `meerk40t-0.8.6000/meerk40t/balormk/gui/balorconfig.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/gui/balorcontroller.py` & `meerk40t-0.8.6000/meerk40t/balormk/gui/balorcontroller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/gui/baloroperationproperties.py` & `meerk40t-0.8.6000/meerk40t/balormk/gui/baloroperationproperties.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/balormk/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/livefulllightjob.py` & `meerk40t-0.8.6000/meerk40t/balormk/livefulllightjob.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/liveselectionlightjob.py` & `meerk40t-0.8.6000/meerk40t/balormk/liveselectionlightjob.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/mock_connection.py` & `meerk40t-0.8.6000/meerk40t/balormk/mock_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/plugin.py` & `meerk40t-0.8.6000/meerk40t/balormk/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/balormk/usb_connection.py` & `meerk40t-0.8.6000/meerk40t/balormk/usb_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/camera/camera.py` & `meerk40t-0.8.6000/meerk40t/camera/camera.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/camera/gui/camerapanel.py` & `meerk40t-0.8.6000/meerk40t/camera/gui/camerapanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/camera/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/camera/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/camera/plugin.py` & `meerk40t-0.8.6000/meerk40t/camera/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ch341/__init__.py` & `meerk40t-0.8.6000/meerk40t/ch341/__init__.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ch341/libusb.py` & `meerk40t-0.8.6000/meerk40t/ch341/libusb.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ch341/mock.py` & `meerk40t-0.8.6000/meerk40t/ch341/mock.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ch341/windll.py` & `meerk40t-0.8.6000/meerk40t/ch341/windll.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         except FileNotFoundError as e:
             self.channel(f"{str(type(e))}: {str(e)}")
             raise ImportError(
                 "FileNotFoundError for misconfigured CH341DLL.dll. See Issue #459"
             )
         except (NameError, OSError) as e:
             self.channel(str(e))
-            raise ConnectionRefusedError
+            raise ImportError
 
     def is_connected(self):
         return self.driver_value != -1 and self.driver_index is not None
 
     @property
     def driver_name(self):
         return "WinDll"
```

### Comparing `meerk40t-0.8.5000/meerk40t/core/bindalias.py` & `meerk40t-0.8.6000/meerk40t/core/bindalias.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/core.py` & `meerk40t-0.8.6000/meerk40t/core/core.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/cubiccut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/cubiccut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/cutcode.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/cutcode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/cutgroup.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/cutgroup.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/cutobject.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/cutobject.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/dwellcut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/dwellcut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/gotocut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/gotocut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/homecut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/homecut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/inputcut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/inputcut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/linecut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/linecut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/outputcut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/outputcut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/plotcut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/plotcut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/quadcut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/quadcut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/rastercut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/rastercut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutcode/waitcut.py` & `meerk40t-0.8.6000/meerk40t/core/cutcode/waitcut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/cutplan.py` & `meerk40t-0.8.6000/meerk40t/core/cutplan.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/drivers.py` & `meerk40t-0.8.6000/meerk40t/core/drivers.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/align.py` & `meerk40t-0.8.6000/meerk40t/core/elements/align.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/branches.py` & `meerk40t-0.8.6000/meerk40t/core/elements/branches.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/clipboard.py` & `meerk40t-0.8.6000/meerk40t/core/elements/clipboard.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/element_treeops.py` & `meerk40t-0.8.6000/meerk40t/core/elements/element_treeops.py`

 * *Files 0% similar despite different names*

```diff
@@ -2201,18 +2201,18 @@
 00008980: 7267 7329 3a0d 0a20 2020 2020 2020 2069  rgs):..        i
 00008990: 6620 6861 7361 7474 7228 6e6f 6465 2c20  f hasattr(node, 
 000089a0: 2263 616e 5f72 656d 6f76 6522 2920 616e  "can_remove") an
 000089b0: 6420 6e6f 7420 6e6f 6465 2e63 616e 5f72  d not node.can_r
 000089c0: 656d 6f76 653a 0d0a 2020 2020 2020 2020  emove:..        
 000089d0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
 000089e0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000089f0: 2020 2020 206e 6f64 652e 7265 6d6f 7665       node.remove
-00008a00: 5f6e 6f64 6528 290d 0a20 2020 2020 2020  _node()..       
-00008a10: 2020 2020 2073 656c 662e 7365 745f 656d       self.set_em
-00008a20: 7068 6173 6973 284e 6f6e 6529 0d0a 0d0a  phasis(None)....
+000089f0: 2020 2020 2073 656c 662e 7365 745f 656d       self.set_em
+00008a00: 7068 6173 6973 284e 6f6e 6529 0d0a 2020  phasis(None)..  
+00008a10: 2020 2020 2020 2020 2020 6e6f 6465 2e72            node.r
+00008a20: 656d 6f76 655f 6e6f 6465 2829 0d0a 0d0a  emove_node()....
 00008a30: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
 00008a40: 696f 6e61 6c28 0d0a 2020 2020 2020 2020  ional(..        
 00008a50: 6c61 6d62 6461 2063 6f6e 643a 206c 656e  lambda cond: len
 00008a60: 286c 6973 7428 7365 6c66 2e66 6c61 7428  (list(self.flat(
 00008a70: 7365 6c65 6374 6564 3d54 7275 652c 2063  selected=True, c
 00008a80: 6173 6361 6465 3d46 616c 7365 2c20 7479  ascade=False, ty
 00008a90: 7065 733d 6f70 5f6e 6f64 6573 2929 290d  pes=op_nodes))).
@@ -2223,3753 +2223,3781 @@
 00008ae0: 6572 6174 696f 6e20 277b 6e61 6d65 7d27  eration '{name}'
 00008af0: 2066 756c 6c79 2229 2c0d 0a20 2020 2020   fully"),..     
 00008b00: 2020 206e 6f64 655f 7479 7065 3d6f 705f     node_type=op_
 00008b10: 6e6f 6465 732c 0d0a 2020 2020 2020 2020  nodes,..        
 00008b20: 6865 6c70 3d22 222c 0d0a 2020 2020 290d  help="",..    ).
 00008b30: 0a20 2020 2064 6566 2072 656d 6f76 655f  .    def remove_
 00008b40: 7479 7065 5f6f 7028 6e6f 6465 2c20 2a2a  type_op(node, **
-00008b50: 6b77 6172 6773 293a 0d0a 0d0a 2020 2020  kwargs):....    
-00008b60: 2020 2020 6e6f 6465 2e72 656d 6f76 655f      node.remove_
-00008b70: 6e6f 6465 2829 0d0a 2020 2020 2020 2020  node()..        
-00008b80: 7365 6c66 2e73 6574 5f65 6d70 6861 7369  self.set_emphasi
-00008b90: 7328 4e6f 6e65 290d 0a20 2020 2020 2020  s(None)..       
-00008ba0: 2073 656c 662e 7369 676e 616c 2822 6f70   self.signal("op
-00008bb0: 6572 6174 696f 6e5f 7265 6d6f 7665 6422  eration_removed"
-00008bc0: 290d 0a0d 0a20 2020 2040 7472 6565 5f63  )....    @tree_c
-00008bd0: 6f6e 6469 7469 6f6e 616c 280d 0a20 2020  onditional(..   
-00008be0: 2020 2020 206c 616d 6264 6120 636f 6e64       lambda cond
-00008bf0: 3a20 6c65 6e28 6c69 7374 2873 656c 662e  : len(list(self.
-00008c00: 666c 6174 2873 656c 6563 7465 643d 5472  flat(selected=Tr
-00008c10: 7565 2c20 6361 7363 6164 653d 4661 6c73  ue, cascade=Fals
-00008c20: 652c 2074 7970 6573 3d22 626c 6f62 2229  e, types="blob")
-00008c30: 2929 0d0a 2020 2020 2020 2020 3d3d 2031  ))..        == 1
-00008c40: 0d0a 2020 2020 290d 0a20 2020 2040 7472  ..    )..    @tr
-00008c50: 6565 5f6f 7065 7261 7469 6f6e 280d 0a20  ee_operation(.. 
-00008c60: 2020 2020 2020 205f 2822 4465 6c65 7465         _("Delete
-00008c70: 2062 6c6f 6220 277b 6e61 6d65 7d27 2066   blob '{name}' f
-00008c80: 756c 6c79 2229 2c0d 0a20 2020 2020 2020  ully"),..       
-00008c90: 206e 6f64 655f 7479 7065 3d22 626c 6f62   node_type="blob
-00008ca0: 222c 0d0a 2020 2020 2020 2020 6865 6c70  ",..        help
-00008cb0: 3d22 222c 0d0a 2020 2020 290d 0a20 2020  ="",..    )..   
-00008cc0: 2064 6566 2072 656d 6f76 655f 7479 7065   def remove_type
-00008cd0: 5f62 6c6f 6228 6e6f 6465 2c20 2a2a 6b77  _blob(node, **kw
-00008ce0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00008cf0: 6e6f 6465 2e72 656d 6f76 655f 6e6f 6465  node.remove_node
-00008d00: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00008d10: 2e73 6574 5f65 6d70 6861 7369 7328 4e6f  .set_emphasis(No
-00008d20: 6e65 290d 0a20 2020 2020 2020 2073 656c  ne)..        sel
-00008d30: 662e 7369 676e 616c 2822 6f70 6572 6174  f.signal("operat
-00008d40: 696f 6e5f 7265 6d6f 7665 6422 290d 0a0d  ion_removed")...
-00008d50: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
-00008d60: 7469 6f6e 616c 280d 0a20 2020 2020 2020  tional(..       
-00008d70: 206c 616d 6264 6120 636f 6e64 3a20 6c65   lambda cond: le
-00008d80: 6e28 6c69 7374 2873 656c 662e 666c 6174  n(list(self.flat
-00008d90: 2873 656c 6563 7465 643d 5472 7565 2c20  (selected=True, 
-00008da0: 6361 7363 6164 653d 4661 6c73 652c 2074  cascade=False, t
-00008db0: 7970 6573 3d6f 705f 6e6f 6465 7329 2929  ypes=op_nodes)))
-00008dc0: 0d0a 2020 2020 2020 2020 3e20 310d 0a20  ..        > 1.. 
-00008dd0: 2020 2029 0d0a 2020 2020 4074 7265 655f     )..    @tree_
-00008de0: 6361 6c63 280d 0a20 2020 2020 2020 2022  calc(..        "
-00008df0: 6563 6f75 6e74 222c 0d0a 2020 2020 2020  ecount",..      
-00008e00: 2020 6c61 6d62 6461 2069 3a20 6c65 6e28    lambda i: len(
-00008e10: 6c69 7374 2873 656c 662e 666c 6174 2873  list(self.flat(s
-00008e20: 656c 6563 7465 643d 5472 7565 2c20 6361  elected=True, ca
-00008e30: 7363 6164 653d 4661 6c73 652c 2074 7970  scade=False, typ
-00008e40: 6573 3d6f 705f 6e6f 6465 7329 2929 2c0d  es=op_nodes))),.
-00008e50: 0a20 2020 2029 0d0a 2020 2020 4074 7265  .    )..    @tre
-00008e60: 655f 6f70 6572 6174 696f 6e28 0d0a 2020  e_operation(..  
-00008e70: 2020 2020 2020 5f28 2244 656c 6574 6520        _("Delete 
-00008e80: 7b65 636f 756e 747d 206f 7065 7261 7469  {ecount} operati
-00008e90: 6f6e 7320 6675 6c6c 7922 292c 0d0a 2020  ons fully"),..  
-00008ea0: 2020 2020 2020 6e6f 6465 5f74 7970 653d        node_type=
-00008eb0: 6f70 5f6e 6f64 6573 2c0d 0a20 2020 2020  op_nodes,..     
-00008ec0: 2020 2068 656c 703d 2222 2c0d 0a20 2020     help="",..   
-00008ed0: 2029 0d0a 2020 2020 6465 6620 7265 6d6f   )..    def remo
-00008ee0: 7665 5f74 7970 655f 6f70 5f6d 756c 7469  ve_type_op_multi
-00008ef0: 706c 6528 6e6f 6465 2c20 2a2a 6b77 6172  ple(node, **kwar
-00008f00: 6773 293a 0d0a 2020 2020 2020 2020 666f  gs):..        fo
-00008f10: 7220 6f70 2069 6e20 6c69 7374 2873 656c  r op in list(sel
-00008f20: 662e 666c 6174 2873 656c 6563 7465 643d  f.flat(selected=
-00008f30: 5472 7565 2c20 6361 7363 6164 653d 4661  True, cascade=Fa
-00008f40: 6c73 652c 2074 7970 6573 3d6f 705f 6e6f  lse, types=op_no
-00008f50: 6465 7329 293a 0d0a 2020 2020 2020 2020  des)):..        
-00008f60: 2020 2020 6f70 2e72 656d 6f76 655f 6e6f      op.remove_no
-00008f70: 6465 2829 0d0a 2020 2020 2020 2020 7365  de()..        se
-00008f80: 6c66 2e73 6574 5f65 6d70 6861 7369 7328  lf.set_emphasis(
-00008f90: 4e6f 6e65 290d 0a20 2020 2020 2020 2073  None)..        s
-00008fa0: 656c 662e 7369 676e 616c 2822 6f70 6572  elf.signal("oper
-00008fb0: 6174 696f 6e5f 7265 6d6f 7665 6422 290d  ation_removed").
-00008fc0: 0a0d 0a20 2020 2064 6566 2063 6f6e 7461  ...    def conta
-00008fd0: 696e 735f 6e6f 5f75 6e72 656d 6f76 6162  ins_no_unremovab
-00008fe0: 6c65 5f69 7465 6d73 2829 3a0d 0a20 2020  le_items():..   
-00008ff0: 2020 2020 206e 6f6c 6f63 6b20 3d20 5472       nolock = Tr
-00009000: 7565 0d0a 2020 2020 2020 2020 666f 7220  ue..        for 
-00009010: 6520 696e 206c 6973 7428 7365 6c66 2e66  e in list(self.f
-00009020: 6c61 7428 7365 6c65 6374 6564 3d54 7275  lat(selected=Tru
-00009030: 652c 2063 6173 6361 6465 3d54 7275 6529  e, cascade=True)
-00009040: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00009050: 6966 2068 6173 6174 7472 2865 2c20 2263  if hasattr(e, "c
-00009060: 616e 5f72 656d 6f76 6522 2920 616e 6420  an_remove") and 
-00009070: 6e6f 7420 652e 6361 6e5f 7265 6d6f 7665  not e.can_remove
-00009080: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00009090: 2020 206e 6f6c 6f63 6b20 3d20 4661 6c73     nolock = Fals
-000090a0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000090b0: 2020 2062 7265 616b 0d0a 2020 2020 2020     break..      
-000090c0: 2020 7265 7475 726e 206e 6f6c 6f63 6b0d    return nolock.
-000090d0: 0a0d 0a20 2020 2040 7472 6565 5f63 6f6e  ...    @tree_con
-000090e0: 6469 7469 6f6e 616c 286c 616d 6264 6120  ditional(lambda 
-000090f0: 636f 6e64 3a20 636f 6e74 6169 6e73 5f6e  cond: contains_n
-00009100: 6f5f 756e 7265 6d6f 7661 626c 655f 6974  o_unremovable_it
-00009110: 656d 7328 2929 0d0a 2020 2020 4074 7265  ems())..    @tre
-00009120: 655f 636f 6e64 6974 696f 6e61 6c28 0d0a  e_conditional(..
-00009130: 2020 2020 2020 2020 6c61 6d62 6461 2063          lambda c
-00009140: 6f6e 643a 206c 656e 280d 0a20 2020 2020  ond: len(..     
-00009150: 2020 2020 2020 206c 6973 7428 7365 6c66         list(self
-00009160: 2e66 6c61 7428 7365 6c65 6374 6564 3d54  .flat(selected=T
-00009170: 7275 652c 2063 6173 6361 6465 3d46 616c  rue, cascade=Fal
-00009180: 7365 2c20 7479 7065 733d 2822 6669 6c65  se, types=("file
-00009190: 222c 2022 6772 6f75 7022 2929 290d 0a20  ", "group"))).. 
-000091a0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000091b0: 2020 3d3d 2031 0d0a 2020 2020 290d 0a20    == 1..    ).. 
-000091c0: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-000091d0: 6f6e 280d 0a20 2020 2020 2020 205f 2822  on(..        _("
-000091e0: 4465 6c65 7465 2067 726f 7570 2027 7b6e  Delete group '{n
-000091f0: 616d 657d 2720 616e 6420 616c 6c20 6974  ame}' and all it
-00009200: 7320 6368 696c 642d 656c 656d 656e 7473  s child-elements
-00009210: 2066 756c 6c79 2229 2c0d 0a20 2020 2020   fully"),..     
-00009220: 2020 206e 6f64 655f 7479 7065 3d22 6772     node_type="gr
-00009230: 6f75 7022 2c0d 0a20 2020 2020 2020 2068  oup",..        h
-00009240: 656c 703d 2222 2c0d 0a20 2020 2029 0d0a  elp="",..    )..
-00009250: 2020 2020 6465 6620 7265 6d6f 7665 5f74      def remove_t
-00009260: 7970 655f 6772 7028 6e6f 6465 2c20 2a2a  ype_grp(node, **
-00009270: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00009280: 2020 6e6f 6465 2e72 656d 6f76 655f 6e6f    node.remove_no
-00009290: 6465 2829 0d0a 2020 2020 2020 2020 7365  de()..        se
-000092a0: 6c66 2e73 6574 5f65 6d70 6861 7369 7328  lf.set_emphasis(
-000092b0: 4e6f 6e65 290d 0a0d 0a20 2020 2040 7472  None)....    @tr
-000092c0: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
-000092d0: 616d 6264 6120 636f 6e64 3a20 636f 6e74  ambda cond: cont
-000092e0: 6169 6e73 5f6e 6f5f 756e 7265 6d6f 7661  ains_no_unremova
-000092f0: 626c 655f 6974 656d 7328 2929 0d0a 2020  ble_items())..  
-00009300: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
-00009310: 6e61 6c28 0d0a 2020 2020 2020 2020 6c61  nal(..        la
-00009320: 6d62 6461 2063 6f6e 643a 206c 656e 280d  mbda cond: len(.
-00009330: 0a20 2020 2020 2020 2020 2020 206c 6973  .            lis
-00009340: 7428 7365 6c66 2e66 6c61 7428 7365 6c65  t(self.flat(sele
-00009350: 6374 6564 3d54 7275 652c 2063 6173 6361  cted=True, casca
-00009360: 6465 3d46 616c 7365 2c20 7479 7065 733d  de=False, types=
-00009370: 2822 6669 6c65 222c 2022 6772 6f75 7022  ("file", "group"
-00009380: 2929 290d 0a20 2020 2020 2020 2029 0d0a  )))..        )..
-00009390: 2020 2020 2020 2020 3d3d 2031 0d0a 2020          == 1..  
-000093a0: 2020 290d 0a20 2020 2040 7472 6565 5f6f    )..    @tree_o
-000093b0: 7065 7261 7469 6f6e 280d 0a20 2020 2020  peration(..     
-000093c0: 2020 205f 2822 5265 6d6f 7665 206c 6f61     _("Remove loa
-000093d0: 6465 6420 6669 6c65 2027 7b6e 616d 657d  ded file '{name}
-000093e0: 2720 616e 6420 616c 6c20 6974 7320 6368  ' and all its ch
-000093f0: 696c 642d 656c 656d 656e 7473 2066 756c  ild-elements ful
-00009400: 6c79 2229 2c0d 0a20 2020 2020 2020 206e  ly"),..        n
-00009410: 6f64 655f 7479 7065 3d22 6669 6c65 222c  ode_type="file",
-00009420: 0d0a 2020 2020 2020 2020 6865 6c70 3d22  ..        help="
-00009430: 222c 0d0a 2020 2020 290d 0a20 2020 2064  ",..    )..    d
-00009440: 6566 2072 656d 6f76 655f 7479 7065 5f66  ef remove_type_f
-00009450: 696c 6528 6e6f 6465 2c20 2a2a 6b77 6172  ile(node, **kwar
-00009460: 6773 293a 0d0a 2020 2020 2020 2020 6e6f  gs):..        no
-00009470: 6465 2e72 656d 6f76 655f 6e6f 6465 2829  de.remove_node()
-00009480: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00009490: 6574 5f65 6d70 6861 7369 7328 4e6f 6e65  et_emphasis(None
-000094a0: 290d 0a0d 0a20 2020 2040 7472 6565 5f63  )....    @tree_c
-000094b0: 6f6e 6469 7469 6f6e 616c 286c 616d 6264  onditional(lambd
-000094c0: 6120 6e6f 6465 3a20 6e6f 7420 6973 5f72  a node: not is_r
-000094d0: 6567 6d61 726b 286e 6f64 6529 290d 0a20  egmark(node)).. 
-000094e0: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-000094f0: 6f6e 280d 0a20 2020 2020 2020 205f 2822  on(..        _("
-00009500: 5265 6d6f 7665 2074 7261 6e73 7061 7265  Remove transpare
-00009510: 6e74 206f 626a 6563 7473 2229 2c0d 0a20  nt objects"),.. 
-00009520: 2020 2020 2020 206e 6f64 655f 7479 7065         node_type
-00009530: 3d28 2267 726f 7570 222c 2022 6669 6c65  =("group", "file
-00009540: 2229 2c0d 0a20 2020 2020 2020 2068 656c  "),..        hel
-00009550: 703d 5f28 2252 656d 6f76 6520 616c 6c20  p=_("Remove all 
-00009560: 656c 656d 656e 7473 2074 6861 7420 6e65  elements that ne
-00009570: 6974 6865 7220 6861 7665 2061 2062 6f72  ither have a bor
-00009580: 6465 7220 6e6f 7220 6120 6669 6c6c 2063  der nor a fill c
-00009590: 6f6c 6f72 2229 2c0d 0a20 2020 2029 0d0a  olor"),..    )..
-000095a0: 2020 2020 6465 6620 7265 6d6f 7665 5f74      def remove_t
-000095b0: 7261 6e73 7061 7265 6e74 286e 6f64 652c  ransparent(node,
-000095c0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-000095d0: 2020 2020 2072 6573 203d 2030 0d0a 2020       res = 0..  
-000095e0: 2020 2020 2020 746f 5f72 656d 6f76 6520        to_remove 
-000095f0: 3d20 5b5d 0d0a 2020 2020 2020 2020 666f  = []..        fo
-00009600: 7220 656e 6f64 6520 696e 2073 656c 662e  r enode in self.
-00009610: 666c 6174 280d 0a20 2020 2020 2020 2020  flat(..         
-00009620: 2020 2073 656c 6563 7465 643d 5472 7565     selected=True
-00009630: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
-00009640: 6173 6361 6465 3d54 7275 652c 0d0a 2020  ascade=True,..  
-00009650: 2020 2020 2020 2020 2020 7479 7065 733d            types=
-00009660: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00009670: 2020 2022 656c 656d 2072 6563 7422 2c0d     "elem rect",.
-00009680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009690: 2022 656c 656d 2065 6c6c 6970 7365 222c   "elem ellipse",
-000096a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000096b0: 2020 2265 6c65 6d20 7061 7468 222c 0d0a    "elem path",..
-000096c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096d0: 2265 6c65 6d20 6c69 6e65 222c 0d0a 2020  "elem line",..  
-000096e0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-000096f0: 6c65 6d20 706f 6c79 6c69 6e65 222c 0d0a  lem polyline",..
-00009700: 2020 2020 2020 2020 2020 2020 292c 0d0a              ),..
-00009710: 2020 2020 2020 2020 293a 0d0a 2020 2020          ):..    
-00009720: 2020 2020 2020 2020 636f 6c6f 7265 6420          colored 
-00009730: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
-00009740: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-00009750: 2020 2020 2020 2020 2020 2068 6173 6174             hasat
-00009760: 7472 2865 6e6f 6465 2c20 2266 696c 6c22  tr(enode, "fill"
-00009770: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00009780: 2020 2061 6e64 2065 6e6f 6465 2e66 696c     and enode.fil
-00009790: 6c20 6973 206e 6f74 204e 6f6e 650d 0a20  l is not None.. 
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000097b0: 6e64 2065 6e6f 6465 2e66 696c 6c2e 6172  nd enode.fill.ar
-000097c0: 6762 2069 7320 6e6f 7420 4e6f 6e65 0d0a  gb is not None..
-000097d0: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
-000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097f0: 636f 6c6f 7265 6420 3d20 5472 7565 0d0a  colored = True..
-00009800: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00009810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009820: 2020 6861 7361 7474 7228 656e 6f64 652c    hasattr(enode,
-00009830: 2022 7374 726f 6b65 2229 0d0a 2020 2020   "stroke")..    
-00009840: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00009850: 656e 6f64 652e 7374 726f 6b65 2069 7320  enode.stroke is 
-00009860: 6e6f 7420 4e6f 6e65 0d0a 2020 2020 2020  not None..      
-00009870: 2020 2020 2020 2020 2020 616e 6420 656e            and en
-00009880: 6f64 652e 7374 726f 6b65 2e61 7267 6220  ode.stroke.argb 
-00009890: 6973 206e 6f74 204e 6f6e 650d 0a20 2020  is not None..   
-000098a0: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
-000098b0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-000098c0: 6f72 6564 203d 2054 7275 650d 0a20 2020  ored = True..   
-000098d0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-000098e0: 636f 6c6f 7265 643a 0d0a 2020 2020 2020  colored:..      
-000098f0: 2020 2020 2020 2020 2020 7265 7320 2b3d            res +=
-00009900: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00009910: 2020 2020 656e 6f64 652e 7265 6d6f 7665      enode.remove
-00009920: 5f6e 6f64 6528 290d 0a0d 0a20 2020 2020  _node()....     
-00009930: 2020 2069 6620 7265 7320 3e20 303a 0d0a     if res > 0:..
-00009940: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00009950: 2e73 6967 6e61 6c28 2272 6562 7569 6c64  .signal("rebuild
-00009960: 5f74 7265 6522 290d 0a0d 0a20 2020 2023  _tree")....    #
-00009970: 203d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20 2020   ==========..   
-00009980: 2023 2052 656d 6f76 6520 4f70 6572 6174   # Remove Operat
-00009990: 696f 6e73 2028 4966 204e 6f20 5472 6565  ions (If No Tree
-000099a0: 2053 656c 6563 7465 6429 0d0a 2020 2020   Selected)..    
-000099b0: 2320 4e6f 7465 3a20 5468 6973 2063 6f64  # Note: This cod
-000099c0: 6520 776f 756c 6420 7261 7265 6c79 206d  e would rarely m
-000099d0: 6174 6368 2061 6e79 7468 696e 6720 7369  atch anything si
-000099e0: 6e63 6520 7468 6520 7472 6565 2073 656c  nce the tree sel
-000099f0: 6563 7465 6420 7769 6c6c 2061 6c6d 6f73  ected will almos
-00009a00: 7420 616c 7761 7973 2062 6520 7472 7565  t always be true
-00009a10: 2069 6620 7765 2068 6176 650d 0a20 2020   if we have..   
-00009a20: 2023 206d 6174 6368 2074 6869 7320 636f   # match this co
-00009a30: 6e64 6974 696f 6e61 6c2e 2054 6865 2074  nditional. The t
-00009a40: 7265 652d 7365 6c65 6374 6564 2064 656c  ree-selected del
-00009a50: 6574 6520 6675 6e63 7469 6f6e 7320 6172  ete functions ar
-00009a60: 6520 7375 7065 7269 6f72 2e0d 0a20 2020  e superior...   
-00009a70: 2023 203d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20   # ==========.. 
-00009a80: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
-00009a90: 6f6e 616c 280d 0a20 2020 2020 2020 206c  onal(..        l
-00009aa0: 616d 6264 6120 636f 6e64 3a20 6c65 6e28  ambda cond: len(
-00009ab0: 0d0a 2020 2020 2020 2020 2020 2020 6c69  ..            li
-00009ac0: 7374 2873 656c 662e 666c 6174 2873 656c  st(self.flat(sel
-00009ad0: 6563 7465 643d 5472 7565 2c20 6361 7363  ected=True, casc
-00009ae0: 6164 653d 4661 6c73 652c 2074 7970 6573  ade=False, types
-00009af0: 3d6e 6f6e 5f73 7472 7563 7475 7261 6c5f  =non_structural_
-00009b00: 6e6f 6465 7329 290d 0a20 2020 2020 2020  nodes))..       
-00009b10: 2029 0d0a 2020 2020 2020 2020 3d3d 2030   )..        == 0
-00009b20: 0d0a 2020 2020 290d 0a20 2020 2040 7472  ..    )..    @tr
-00009b30: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
-00009b40: 616d 6264 6120 6e6f 6465 3a20 6c65 6e28  ambda node: len(
-00009b50: 6c69 7374 2873 656c 662e 6f70 7328 7365  list(self.ops(se
-00009b60: 6c65 6374 6564 3d54 7275 6529 2929 203e  lected=True))) >
-00009b70: 2031 290d 0a20 2020 2040 7472 6565 5f63   1)..    @tree_c
-00009b80: 616c 6328 2265 636f 756e 7422 2c20 6c61  alc("ecount", la
-00009b90: 6d62 6461 2069 3a20 6c65 6e28 6c69 7374  mbda i: len(list
-00009ba0: 2873 656c 662e 6f70 7328 7365 6c65 6374  (self.ops(select
-00009bb0: 6564 3d54 7275 6529 2929 290d 0a20 2020  ed=True))))..   
-00009bc0: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
-00009bd0: 280d 0a20 2020 2020 2020 205f 2822 4465  (..        _("De
-00009be0: 6c65 7465 207b 6563 6f75 6e74 7d20 6f70  lete {ecount} op
-00009bf0: 6572 6174 696f 6e73 2229 2c0d 0a20 2020  erations"),..   
-00009c00: 2020 2020 206e 6f64 655f 7479 7065 3d28       node_type=(
-00009c10: 0d0a 2020 2020 2020 2020 2020 2020 226f  ..            "o
-00009c20: 7020 6375 7422 2c0d 0a20 2020 2020 2020  p cut",..       
-00009c30: 2020 2020 2022 6f70 2072 6173 7465 7222       "op raster"
-00009c40: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00009c50: 6f70 2069 6d61 6765 222c 0d0a 2020 2020  op image",..    
-00009c60: 2020 2020 2020 2020 226f 7020 656e 6772          "op engr
-00009c70: 6176 6522 2c0d 0a20 2020 2020 2020 2020  ave",..         
-00009c80: 2020 2022 6f70 2064 6f74 7322 2c0d 0a20     "op dots",.. 
-00009c90: 2020 2020 2020 2020 2020 2022 6f70 2068             "op h
-00009ca0: 6174 6368 222c 0d0a 2020 2020 2020 2020  atch",..        
-00009cb0: 2020 2020 2275 7469 6c20 636f 6e73 6f6c      "util consol
-00009cc0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-00009cd0: 2022 7574 696c 2077 6169 7422 2c0d 0a20   "util wait",.. 
-00009ce0: 2020 2020 2020 2020 2020 2022 7574 696c             "util
-00009cf0: 2068 6f6d 6522 2c0d 0a20 2020 2020 2020   home",..       
-00009d00: 2020 2020 2022 7574 696c 2067 6f74 6f22       "util goto"
-00009d10: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00009d20: 7574 696c 206f 7574 7075 7422 2c0d 0a20  util output",.. 
-00009d30: 2020 2020 2020 2020 2020 2022 7574 696c             "util
-00009d40: 2069 6e70 7574 222c 0d0a 2020 2020 2020   input",..      
-00009d50: 2020 2020 2020 226c 6173 6572 636f 6465        "lasercode
-00009d60: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00009d70: 2263 7574 636f 6465 222c 0d0a 2020 2020  "cutcode",..    
-00009d80: 2020 2020 2020 2020 2262 6c6f 6222 2c0d          "blob",.
-00009d90: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
-00009da0: 2020 2020 2068 656c 703d 2222 2c0d 0a20       help="",.. 
-00009db0: 2020 2029 0d0a 2020 2020 6465 6620 7265     )..    def re
-00009dc0: 6d6f 7665 5f6e 5f6f 7073 286e 6f64 652c  move_n_ops(node,
-00009dd0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00009de0: 2020 2020 2073 656c 6628 226f 7065 7261       self("opera
-00009df0: 7469 6f6e 2064 656c 6574 655c 6e22 290d  tion delete\n").
-00009e00: 0a0d 0a20 2020 2040 7472 6565 5f6f 7065  ...    @tree_ope
-00009e10: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
-00009e20: 205f 2822 5365 6c65 6374 2061 6c6c 2065   _("Select all e
-00009e30: 6c65 6d65 6e74 7320 6f66 2073 616d 6520  lements of same 
-00009e40: 7479 7065 2229 2c0d 0a20 2020 2020 2020  type"),..       
-00009e50: 206e 6f64 655f 7479 7065 3d65 6c65 6d5f   node_type=elem_
-00009e60: 6e6f 6465 732c 0d0a 2020 2020 2020 2020  nodes,..        
-00009e70: 6865 6c70 3d5f 2822 5365 6c65 6374 2061  help=_("Select a
-00009e80: 6c6c 2065 6c65 6d65 6e74 7320 696e 2073  ll elements in s
-00009e90: 6365 6e65 2c20 7468 6174 2068 6176 6520  cene, that have 
-00009ea0: 7468 6520 7361 6d65 2074 7970 6520 6173  the same type as
-00009eb0: 2074 6869 7320 6e6f 6465 2229 2c0d 0a20   this node"),.. 
-00009ec0: 2020 2029 0d0a 2020 2020 6465 6620 7365     )..    def se
-00009ed0: 6c65 6374 5f73 696d 696c 6172 286e 6f64  lect_similar(nod
-00009ee0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-00009ef0: 2020 2020 2020 206e 7479 7065 203d 206e         ntype = n
-00009f00: 6f64 652e 7479 7065 0d0a 2020 2020 2020  ode.type..      
-00009f10: 2020 6368 616e 6765 7320 3d20 4661 6c73    changes = Fals
-00009f20: 650d 0a20 2020 2020 2020 2066 6f72 2065  e..        for e
-00009f30: 2069 6e20 7365 6c66 2e65 6c65 6d73 2829   in self.elems()
-00009f40: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00009f50: 6620 652e 7479 7065 203d 3d20 6e74 7970  f e.type == ntyp
-00009f60: 6520 616e 6420 6e6f 7420 652e 656d 7068  e and not e.emph
-00009f70: 6173 697a 6564 2061 6e64 2065 2e63 616e  asized and e.can
-00009f80: 5f65 6d70 6861 7369 7a65 3a0d 0a20 2020  _emphasize:..   
-00009f90: 2020 2020 2020 2020 2020 2020 2065 2e65               e.e
-00009fa0: 6d70 6861 7369 7a65 6420 3d20 5472 7565  mphasized = True
-00009fb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009fc0: 2020 652e 7365 6c65 6374 6564 203d 2054    e.selected = T
-00009fd0: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
-00009fe0: 2020 2020 2063 6861 6e67 6573 203d 2054       changes = T
-00009ff0: 7275 650d 0a20 2020 2020 2020 2069 6620  rue..        if 
-0000a000: 6368 616e 6765 733a 0d0a 2020 2020 2020  changes:..      
-0000a010: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0000a020: 6174 655f 7365 6c65 6374 6564 5f61 7265  ate_selected_are
-0000a030: 6128 290d 0a20 2020 2020 2020 2020 2020  a()..           
-0000a040: 2073 656c 662e 7369 676e 616c 2822 7265   self.signal("re
-0000a050: 6672 6573 685f 7363 656e 6522 2c20 2253  fresh_scene", "S
-0000a060: 6365 6e65 2229 0d0a 0d0a 2020 2020 2320  cene")....    # 
-0000a070: 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020  ==========..    
-0000a080: 2320 5245 4d4f 5645 2045 4c45 4d45 4e54  # REMOVE ELEMENT
-0000a090: 530d 0a20 2020 2023 203d 3d3d 3d3d 3d3d  S..    # =======
-0000a0a0: 3d3d 3d0d 0a20 2020 2023 204d 6f72 6520  ===..    # More 
-0000a0b0: 7468 616e 206f 6e65 2c20 7370 6563 6961  than one, specia
-0000a0c0: 6c20 6361 7365 203d 3d20 3120 616c 7265  l case == 1 alre
-0000a0d0: 6164 7920 6465 616c 7420 7769 7468 0d0a  ady dealt with..
-0000a0e0: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
-0000a0f0: 696f 6e61 6c28 6c61 6d62 6461 206e 6f64  ional(lambda nod
-0000a100: 653a 206c 656e 286c 6973 7428 7365 6c66  e: len(list(self
-0000a110: 2e65 6c65 6d73 2865 6d70 6861 7369 7a65  .elems(emphasize
-0000a120: 643d 5472 7565 2929 2920 3e20 3129 0d0a  d=True))) > 1)..
-0000a130: 2020 2020 4074 7265 655f 6361 6c63 2822      @tree_calc("
-0000a140: 6563 6f75 6e74 222c 206c 616d 6264 6120  ecount", lambda 
-0000a150: 693a 206c 656e 286c 6973 7428 7365 6c66  i: len(list(self
-0000a160: 2e65 6c65 6d73 2865 6d70 6861 7369 7a65  .elems(emphasize
-0000a170: 643d 5472 7565 2929 2929 0d0a 2020 2020  d=True))))..    
-0000a180: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
-0000a190: 0d0a 2020 2020 2020 2020 5f28 2244 656c  ..        _("Del
-0000a1a0: 6574 6520 7b65 636f 756e 747d 2065 6c65  ete {ecount} ele
-0000a1b0: 6d65 6e74 732c 2061 7320 7365 6c65 6374  ments, as select
-0000a1c0: 6564 2069 6e20 7363 656e 6522 292c 0d0a  ed in scene"),..
-0000a1d0: 2020 2020 2020 2020 6e6f 6465 5f74 7970          node_typ
-0000a1e0: 653d 656c 656d 5f67 726f 7570 5f6e 6f64  e=elem_group_nod
-0000a1f0: 6573 2c0d 0a20 2020 2020 2020 2068 656c  es,..        hel
-0000a200: 703d 2222 2c0d 0a20 2020 2029 0d0a 2020  p="",..    )..  
-0000a210: 2020 6465 6620 7265 6d6f 7665 5f6e 5f65    def remove_n_e
-0000a220: 6c65 6d65 6e74 7328 6e6f 6465 2c20 2a2a  lements(node, **
-0000a230: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-0000a240: 2020 7365 6c66 2822 656c 656d 656e 7420    self("element 
-0000a250: 6465 6c65 7465 5c6e 2229 0d0a 0d0a 2020  delete\n")....  
-0000a260: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-0000a270: 6e28 0d0a 2020 2020 2020 2020 5f28 2242  n(..        _("B
-0000a280: 6563 6f6d 6520 7265 6665 7265 6e63 6520  ecome reference 
-0000a290: 6f62 6a65 6374 2229 2c0d 0a20 2020 2020  object"),..     
-0000a2a0: 2020 206e 6f64 655f 7479 7065 3d65 6c65     node_type=ele
-0000a2b0: 6d5f 6e6f 6465 732c 0d0a 2020 2020 2020  m_nodes,..      
-0000a2c0: 2020 6865 6c70 3d22 222c 0d0a 2020 2020    help="",..    
-0000a2d0: 290d 0a20 2020 2064 6566 206d 616b 655f  )..    def make_
-0000a2e0: 6e6f 6465 5f72 6566 6572 656e 6365 286e  node_reference(n
-0000a2f0: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
-0000a300: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-0000a310: 676e 616c 2822 6d61 6b65 5f72 6566 6572  gnal("make_refer
-0000a320: 656e 6365 222c 206e 6f64 6529 0d0a 0d0a  ence", node)....
-0000a330: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
-0000a340: 696f 6e61 6c28 0d0a 2020 2020 2020 2020  ional(..        
-0000a350: 6c61 6d62 6461 206e 6f64 653a 2069 7369  lambda node: isi
-0000a360: 6e73 7461 6e63 6528 6e6f 6465 2e73 6861  nstance(node.sha
-0000a370: 7065 2c20 506f 6c79 676f 6e29 2061 6e64  pe, Polygon) and
-0000a380: 206c 656e 286e 6f64 652e 7368 6170 652e   len(node.shape.
-0000a390: 706f 696e 7473 2920 3e3d 2033 0d0a 2020  points) >= 3..  
-0000a3a0: 2020 290d 0a20 2020 2040 7472 6565 5f6f    )..    @tree_o
-0000a3b0: 7065 7261 7469 6f6e 280d 0a20 2020 2020  peration(..     
-0000a3c0: 2020 205f 2822 4d61 6b65 2050 6f6c 7967     _("Make Polyg
-0000a3d0: 6f6e 2072 6567 756c 6172 2229 2c0d 0a20  on regular"),.. 
-0000a3e0: 2020 2020 2020 206e 6f64 655f 7479 7065         node_type
-0000a3f0: 3d22 656c 656d 2070 6f6c 796c 696e 6522  ="elem polyline"
-0000a400: 2c0d 0a20 2020 2020 2020 2068 656c 703d  ,..        help=
-0000a410: 2222 2c0d 0a20 2020 2029 0d0a 2020 2020  "",..    )..    
-0000a420: 6465 6620 6d61 6b65 5f70 6f6c 7967 6f6e  def make_polygon
-0000a430: 5f72 6567 756c 6172 286e 6f64 652c 202a  _regular(node, *
-0000a440: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-0000a450: 2020 2023 2066 726f 6d20 2e75 6e69 7473     # from .units
-0000a460: 2069 6d70 6f72 7420 4c65 6e67 7468 0d0a   import Length..
-0000a470: 2020 2020 2020 2020 2320 6672 6f6d 202e          # from .
-0000a480: 2e73 7667 656c 656d 656e 7473 2069 6d70  .svgelements imp
-0000a490: 6f72 7420 436f 6c6f 720d 0a0d 0a20 2020  ort Color....   
-0000a4a0: 2020 2020 2023 2064 6566 206d 6b5f 6465       # def mk_de
-0000a4b0: 6275 675f 706f 696e 7428 782c 2079 2c20  bug_point(x, y, 
-0000a4c0: 636f 6c29 3a0d 0a20 2020 2020 2020 2023  col):..        #
-0000a4d0: 2020 2020 2063 6972 6320 3d20 456c 6c69       circ = Elli
-0000a4e0: 7073 6528 6378 3d78 2c20 6379 3d79 2c20  pse(cx=x, cy=y, 
-0000a4f0: 723d 666c 6f61 7428 4c65 6e67 7468 2822  r=float(Length("
-0000a500: 316d 6d22 2929 290d 0a20 2020 2020 2020  1mm")))..       
-0000a510: 2023 2020 2020 2063 6972 632e 7472 616e   #     circ.tran
-0000a520: 7366 6f72 6d20 3d20 636f 7079 286e 6f64  sform = copy(nod
-0000a530: 652e 7368 6170 652e 7472 616e 7366 6f72  e.shape.transfor
-0000a540: 6d29 0d0a 2020 2020 2020 2020 2320 2020  m)..        #   
-0000a550: 2020 7365 6c66 2e65 6c65 6d5f 6272 616e    self.elem_bran
-0000a560: 6368 2e61 6464 280d 0a20 2020 2020 2020  ch.add(..       
-0000a570: 2023 2020 2020 2020 2020 2073 6861 7065   #         shape
-0000a580: 3d63 6972 632c 0d0a 2020 2020 2020 2020  =circ,..        
-0000a590: 2320 2020 2020 2020 2020 7479 7065 3d22  #         type="
-0000a5a0: 656c 656d 2065 6c6c 6970 7365 222c 0d0a  elem ellipse",..
-0000a5b0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0000a5c0: 2020 7374 726f 6b65 3d43 6f6c 6f72 2863    stroke=Color(c
-0000a5d0: 6f6c 292c 0d0a 2020 2020 2020 2020 2320  ol),..        # 
-0000a5e0: 2020 2020 2020 2020 6669 6c6c 3d43 6f6c          fill=Col
-0000a5f0: 6f72 2863 6f6c 292c 0d0a 2020 2020 2020  or(col),..      
-0000a600: 2020 2320 2020 2020 2020 2020 6d61 7472    #         matr
-0000a610: 6978 3d63 6f70 7928 6e6f 6465 2e6d 6174  ix=copy(node.mat
-0000a620: 7269 7829 2c0d 0a20 2020 2020 2020 2023  rix),..        #
-0000a630: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-0000a640: 2020 6966 206e 6f64 6520 6973 204e 6f6e    if node is Non
-0000a650: 6520 6f72 206e 6f64 652e 7479 7065 2021  e or node.type !
-0000a660: 3d20 2265 6c65 6d20 706f 6c79 6c69 6e65  = "elem polyline
-0000a670: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-0000a680: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
-0000a690: 6e75 6d62 6572 5f70 6f69 6e74 7320 3d20  number_points = 
-0000a6a0: 6c65 6e28 6e6f 6465 2e73 6861 7065 2e70  len(node.shape.p
-0000a6b0: 6f69 6e74 7329 0d0a 2020 2020 2020 2020  oints)..        
-0000a6c0: 2320 7072 696e 7420 2866 224e 756d 6265  # print (f"Numbe
-0000a6d0: 7220 6f66 2070 6f69 6e74 733a 207b 6e75  r of points: {nu
-0000a6e0: 6d62 6572 5f70 6f69 6e74 737d 2229 0d0a  mber_points}")..
-0000a6f0: 2020 2020 2020 2020 2320 666f 7220 7072          # for pr
-0000a700: 6f70 2069 6e20 6469 7228 6e6f 6465 293a  op in dir(node):
-0000a710: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
-0000a720: 7072 696e 7420 2866 227b 7072 6f70 7d20  print (f"{prop} 
-0000a730: 2d20 7b67 6574 6174 7472 286e 6f64 652c  - {getattr(node,
-0000a740: 2027 7072 6f70 272c 2027 2729 7d22 290d   'prop', '')}").
-0000a750: 0a20 2020 2020 2020 2023 2066 6f72 2069  .        # for i
-0000a760: 6478 2c20 7074 2069 6e20 656e 756d 6572  dx, pt in enumer
-0000a770: 6174 6528 6e6f 6465 2e73 6861 7065 2e70  ate(node.shape.p
-0000a780: 6f69 6e74 7329 3a0d 0a20 2020 2020 2020  oints):..       
-0000a790: 2023 2020 2020 2070 7269 6e74 2028 6622   #     print (f"
-0000a7a0: 7b69 6478 7d3a 207b 7074 2e78 3a2e 3166  {idx}: {pt.x:.1f
-0000a7b0: 7d2c 207b 7074 2e79 3a2e 3166 7d22 290d  }, {pt.y:.1f}").
-0000a7c0: 0a20 2020 2020 2020 2069 6620 6e75 6d62  .        if numb
-0000a7d0: 6572 5f70 6f69 6e74 7320 3c20 3320 6f72  er_points < 3 or
-0000a7e0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0000a7f0: 6e6f 6465 2e73 6861 7065 2c20 506f 6c79  node.shape, Poly
-0000a800: 676f 6e29 3a0d 0a20 2020 2020 2020 2020  gon):..         
-0000a810: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-0000a820: 2020 2070 7473 203d 206e 6f64 652e 7368     pts = node.sh
-0000a830: 6170 652e 706f 696e 7473 0d0a 2020 2020  ape.points..    
-0000a840: 2020 2020 6478 203d 2070 7473 5b31 5d2e      dx = pts[1].
-0000a850: 7820 2d20 7074 735b 305d 2e78 0d0a 2020  x - pts[0].x..  
-0000a860: 2020 2020 2020 6479 203d 2070 7473 5b31        dy = pts[1
-0000a870: 5d2e 7920 2d20 7074 735b 305d 2e79 0d0a  ].y - pts[0].y..
-0000a880: 2020 2020 2020 2020 6261 7365 6c69 6e65          baseline
-0000a890: 203d 206d 6174 682e 7371 7274 2864 7820   = math.sqrt(dx 
-0000a8a0: 2a20 6478 202b 2064 7920 2a20 6479 290d  * dx + dy * dy).
-0000a8b0: 0a20 2020 2020 2020 2061 706f 7468 656d  .        apothem
-0000a8c0: 203d 2062 6173 656c 696e 6520 2f20 2832   = baseline / (2
-0000a8d0: 202a 206d 6174 682e 7461 6e28 6d61 7468   * math.tan(math
-0000a8e0: 2e74 6175 202f 2028 3220 2a20 6e75 6d62  .tau / (2 * numb
-0000a8f0: 6572 5f70 6f69 6e74 7329 2929 0d0a 2020  er_points)))..  
-0000a900: 2020 2020 2020 6369 7263 756d 7261 6469        circumradi
-0000a910: 7573 203d 2062 6173 656c 696e 6520 2f20  us = baseline / 
-0000a920: 2832 202a 206d 6174 682e 7369 6e28 6d61  (2 * math.sin(ma
-0000a930: 7468 2e74 6175 202f 2028 3220 2a20 6e75  th.tau / (2 * nu
-0000a940: 6d62 6572 5f70 6f69 6e74 7329 2929 0d0a  mber_points)))..
-0000a950: 2020 2020 2020 2020 6d69 6470 6f69 6e74          midpoint
-0000a960: 203d 2050 6f69 6e74 2870 7473 5b30 5d2e   = Point(pts[0].
-0000a970: 7820 2b20 302e 3520 2a20 6478 2c20 7074  x + 0.5 * dx, pt
-0000a980: 735b 305d 2e79 202b 2030 2e35 202a 2064  s[0].y + 0.5 * d
-0000a990: 7929 0d0a 2020 2020 2020 2020 2320 206d  y)..        #  m
-0000a9a0: 6b5f 6465 6275 675f 706f 696e 7428 6d69  k_debug_point(mi
-0000a9b0: 6470 6f69 6e74 2e78 2c20 6d69 6470 6f69  dpoint.x, midpoi
-0000a9c0: 6e74 2e79 2c20 2262 6c61 636b 2229 0d0a  nt.y, "black")..
-0000a9d0: 2020 2020 2020 2020 6178 203d 2030 0d0a          ax = 0..
-0000a9e0: 2020 2020 2020 2020 6179 203d 2030 0d0a          ay = 0..
-0000a9f0: 2020 2020 2020 2020 666f 7220 6964 782c          for idx,
-0000aa00: 2070 7420 696e 2065 6e75 6d65 7261 7465   pt in enumerate
-0000aa10: 2870 7473 293a 0d0a 2020 2020 2020 2020  (pts):..        
-0000aa20: 2020 2020 6178 202b 3d20 7074 2e78 0d0a      ax += pt.x..
-0000aa30: 2020 2020 2020 2020 2020 2020 6179 202b              ay +
-0000aa40: 3d20 7074 2e79 0d0a 2020 2020 2020 2020  = pt.y..        
-0000aa50: 6178 202f 3d20 6e75 6d62 6572 5f70 6f69  ax /= number_poi
-0000aa60: 6e74 730d 0a20 2020 2020 2020 2061 7920  nts..        ay 
-0000aa70: 2f3d 206e 756d 6265 725f 706f 696e 7473  /= number_points
-0000aa80: 0d0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
-0000aa90: 6172 6974 686d 6574 6963 2063 656e 7465  arithmetic cente
-0000aaa0: 7220 2861 782c 2061 7929 2069 6e64 6963  r (ax, ay) indic
-0000aab0: 6174 6573 2074 6f20 7768 6963 680d 0a20  ates to which.. 
-0000aac0: 2020 2020 2020 2023 2027 7369 6465 2720         # 'side' 
-0000aad0: 6f66 2074 6865 2062 6173 656c 696e 6520  of the baseline 
-0000aae0: 7468 6520 706f 6c79 676f 6e20 6e65 6564  the polygon need
-0000aaf0: 7320 746f 2062 6520 636f 6e73 7472 7563  s to be construc
-0000ab00: 7465 640d 0a20 2020 2020 2020 2061 7269  ted..        ari
-0000ab10: 7468 6d65 7469 635f 6365 6e74 6572 203d  thmetic_center =
-0000ab20: 2050 6f69 6e74 2861 782c 2061 7929 0d0a   Point(ax, ay)..
-0000ab30: 2020 2020 2020 2020 2320 6d6b 5f64 6562          # mk_deb
-0000ab40: 7567 5f70 6f69 6e74 2861 782c 2061 792c  ug_point(ax, ay,
-0000ab50: 2022 6772 6565 6e22 290d 0a20 2020 2020   "green")..     
-0000ab60: 2020 2061 6e67 6c65 203d 2070 7473 5b30     angle = pts[0
-0000ab70: 5d2e 616e 676c 655f 746f 2870 7473 5b31  ].angle_to(pts[1
-0000ab80: 5d29 0d0a 2020 2020 2020 2020 6d69 6461  ])..        mida
-0000ab90: 6e67 6c65 203d 206d 6964 706f 696e 742e  ngle = midpoint.
-0000aba0: 616e 676c 655f 746f 2861 7269 7468 6d65  angle_to(arithme
-0000abb0: 7469 635f 6365 6e74 6572 290d 0a20 2020  tic_center)..   
-0000abc0: 2020 2020 2061 6e67 6c65 202b 3d20 6d61       angle += ma
-0000abd0: 7468 2e74 6175 202f 2034 0d0a 2020 2020  th.tau / 4..    
-0000abe0: 2020 2020 6669 7273 745f 706f 696e 7420      first_point 
-0000abf0: 3d20 506f 696e 742e 706f 6c61 7228 6d69  = Point.polar(mi
-0000ac00: 6470 6f69 6e74 2c20 616e 676c 652c 2061  dpoint, angle, a
-0000ac10: 706f 7468 656d 290d 0a20 2020 2020 2020  pothem)..       
-0000ac20: 2073 6563 6f6e 645f 706f 696e 7420 3d20   second_point = 
-0000ac30: 506f 696e 742e 706f 6c61 7228 6d69 6470  Point.polar(midp
-0000ac40: 6f69 6e74 2c20 616e 676c 6520 2b20 6d61  oint, angle + ma
-0000ac50: 7468 2e74 6175 202f 2032 2c20 6170 6f74  th.tau / 2, apot
-0000ac60: 6865 6d29 0d0a 2020 2020 2020 2020 2320  hem)..        # 
-0000ac70: 6d6b 5f64 6562 7567 5f70 6f69 6e74 2866  mk_debug_point(f
-0000ac80: 6972 7374 5f70 6f69 6e74 2e78 2c20 6669  irst_point.x, fi
-0000ac90: 7273 745f 706f 696e 742e 792c 2022 7965  rst_point.y, "ye
-0000aca0: 6c6c 6f77 2229 0d0a 2020 2020 2020 2020  llow")..        
-0000acb0: 2320 6d6b 5f64 6562 7567 5f70 6f69 6e74  # mk_debug_point
-0000acc0: 2873 6563 6f6e 645f 706f 696e 742e 782c  (second_point.x,
-0000acd0: 2073 6563 6f6e 645f 706f 696e 742e 792c   second_point.y,
-0000ace0: 2022 6379 616e 2229 0d0a 2020 2020 2020   "cyan")..      
-0000acf0: 2020 6465 6c74 6161 6e67 6c65 203d 206d    deltaangle = m
-0000ad00: 6174 682e 7461 7520 2f20 6e75 6d62 6572  ath.tau / number
-0000ad10: 5f70 6f69 6e74 730d 0a20 2020 2020 2020  _points..       
-0000ad20: 2064 3120 3d20 6172 6974 686d 6574 6963   d1 = arithmetic
-0000ad30: 5f63 656e 7465 722e 6469 7374 616e 6365  _center.distance
-0000ad40: 5f74 6f28 6669 7273 745f 706f 696e 7429  _to(first_point)
-0000ad50: 0d0a 2020 2020 2020 2020 6432 203d 2061  ..        d2 = a
-0000ad60: 7269 7468 6d65 7469 635f 6365 6e74 6572  rithmetic_center
-0000ad70: 2e64 6973 7461 6e63 655f 746f 2873 6563  .distance_to(sec
-0000ad80: 6f6e 645f 706f 696e 7429 0d0a 2020 2020  ond_point)..    
-0000ad90: 2020 2020 6966 2064 3120 3c20 6432 3a0d      if d1 < d2:.
-0000ada0: 0a20 2020 2020 2020 2020 2020 2063 656e  .            cen
-0000adb0: 7465 725f 706f 696e 7420 3d20 636f 7079  ter_point = copy
-0000adc0: 2866 6972 7374 5f70 6f69 6e74 290d 0a20  (first_point).. 
-0000add0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000ade0: 2020 2020 2020 2020 2020 6365 6e74 6572            center
-0000adf0: 5f70 6f69 6e74 203d 2063 6f70 7928 7365  _point = copy(se
-0000ae00: 636f 6e64 5f70 6f69 6e74 290d 0a20 2020  cond_point)..   
-0000ae10: 2020 2020 2023 206d 6b5f 6465 6275 675f       # mk_debug_
-0000ae20: 706f 696e 7428 6365 6e74 6572 5f70 6f69  point(center_poi
-0000ae30: 6e74 2e78 2c20 6365 6e74 6572 5f70 6f69  nt.x, center_poi
-0000ae40: 6e74 2e79 2c20 2272 6564 2229 0d0a 0d0a  nt.y, "red")....
-0000ae50: 2020 2020 2020 2020 6966 2063 656e 7465          if cente
-0000ae60: 725f 706f 696e 742e 616e 676c 655f 746f  r_point.angle_to
-0000ae70: 2870 7473 5b30 5d29 203e 2063 656e 7465  (pts[0]) > cente
-0000ae80: 725f 706f 696e 742e 616e 676c 655f 746f  r_point.angle_to
-0000ae90: 2870 7473 5b31 5d29 3a0d 0a20 2020 2020  (pts[1]):..     
-0000aea0: 2020 2020 2020 2064 656c 7461 616e 676c         deltaangl
-0000aeb0: 6520 2a3d 202d 310d 0a20 2020 2020 2020  e *= -1..       
-0000aec0: 2061 6e67 6c65 203d 2063 656e 7465 725f   angle = center_
-0000aed0: 706f 696e 742e 616e 676c 655f 746f 2870  point.angle_to(p
-0000aee0: 7473 5b30 5d29 0d0a 2020 2020 2020 2020  ts[0])..        
-0000aef0: 666f 7220 6964 7820 696e 2072 616e 6765  for idx in range
-0000af00: 286e 756d 6265 725f 706f 696e 7473 293a  (number_points):
-0000af10: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000af20: 6966 2069 6478 203e 2031 3a0d 0a20 2020  if idx > 1:..   
-0000af30: 2020 2020 2020 2020 2070 7420 3d20 506f           pt = Po
-0000af40: 696e 742e 706f 6c61 7228 6365 6e74 6572  int.polar(center
-0000af50: 5f70 6f69 6e74 2c20 616e 676c 652c 2063  _point, angle, c
-0000af60: 6972 6375 6d72 6164 6975 7329 0d0a 2020  ircumradius)..  
-0000af70: 2020 2020 2020 2020 2020 7074 735b 6964            pts[id
-0000af80: 785d 2e78 203d 2070 742e 780d 0a20 2020  x].x = pt.x..   
-0000af90: 2020 2020 2020 2020 2070 7473 5b69 6478           pts[idx
-0000afa0: 5d2e 7920 3d20 7074 2e79 0d0a 2020 2020  ].y = pt.y..    
-0000afb0: 2020 2020 2020 2020 616e 676c 6520 2b3d          angle +=
-0000afc0: 2064 656c 7461 616e 676c 650d 0a20 2020   deltaangle..   
-0000afd0: 2020 2020 206e 6f64 652e 616c 7465 7265       node.altere
-0000afe0: 6428 290d 0a20 2020 2020 2020 2073 656c  d()..        sel
-0000aff0: 662e 7369 676e 616c 2822 7265 6672 6573  f.signal("refres
-0000b000: 685f 7363 656e 6522 2c20 2253 6365 6e65  h_scene", "Scene
-0000b010: 2229 0d0a 0d0a 2020 2020 2320 3d3d 3d3d  ")....    # ====
-0000b020: 3d3d 3d3d 3d3d 0d0a 2020 2020 2320 434f  ======..    # CO
-0000b030: 4e56 4552 5420 5452 4545 204f 5045 5241  NVERT TREE OPERA
-0000b040: 5449 4f4e 530d 0a20 2020 2023 203d 3d3d  TIONS..    # ===
-0000b050: 3d3d 3d3d 3d3d 3d0d 0a20 2020 2040 7472  =======..    @tr
-0000b060: 6565 5f6f 7065 7261 7469 6f6e 280d 0a20  ee_operation(.. 
-0000b070: 2020 2020 2020 205f 2822 436f 6e76 6572         _("Conver
-0000b080: 7420 746f 2043 7574 636f 6465 2229 2c0d  t to Cutcode"),.
-0000b090: 0a20 2020 2020 2020 206e 6f64 655f 7479  .        node_ty
-0000b0a0: 7065 3d22 6c61 7365 7263 6f64 6522 2c0d  pe="lasercode",.
-0000b0b0: 0a20 2020 2020 2020 2068 656c 703d 2222  .        help=""
-0000b0c0: 2c0d 0a20 2020 2029 0d0a 2020 2020 6465  ,..    )..    de
-0000b0d0: 6620 6c61 7365 7263 6f64 6532 6375 7428  f lasercode2cut(
-0000b0e0: 6e6f 6465 2c20 2a2a 6b77 6172 6773 293a  node, **kwargs):
-0000b0f0: 0d0a 2020 2020 2020 2020 6e6f 6465 2e72  ..        node.r
-0000b100: 6570 6c61 6365 5f6e 6f64 6528 4375 7443  eplace_node(CutC
-0000b110: 6f64 652e 6672 6f6d 5f6c 6173 6572 636f  ode.from_laserco
-0000b120: 6465 286e 6f64 652e 636f 6d6d 616e 6473  de(node.commands
-0000b130: 292c 2074 7970 653d 2263 7574 636f 6465  ), type="cutcode
-0000b140: 2229 0d0a 0d0a 2020 2020 4074 7265 655f  ")....    @tree_
-0000b150: 636f 6e64 6974 696f 6e61 6c5f 7472 7928  conditional_try(
-0000b160: 0d0a 2020 2020 2020 2020 6c61 6d62 6461  ..        lambda
-0000b170: 206e 6f64 653a 206b 6572 6e65 6c2e 6c6f   node: kernel.lo
-0000b180: 6f6b 7570 2866 2273 706f 6f6c 6572 6a6f  okup(f"spoolerjo
-0000b190: 622f 7b6e 6f64 652e 6461 7461 5f74 7970  b/{node.data_typ
-0000b1a0: 657d 2229 2069 7320 6e6f 7420 4e6f 6e65  e}") is not None
-0000b1b0: 0d0a 2020 2020 290d 0a20 2020 2040 7472  ..    )..    @tr
-0000b1c0: 6565 5f6f 7065 7261 7469 6f6e 280d 0a20  ee_operation(.. 
-0000b1d0: 2020 2020 2020 205f 2822 436f 6e76 6572         _("Conver
-0000b1e0: 7420 746f 2045 6c65 6d65 6e74 7322 292c  t to Elements"),
-0000b1f0: 0d0a 2020 2020 2020 2020 6e6f 6465 5f74  ..        node_t
-0000b200: 7970 653d 2262 6c6f 6222 2c0d 0a20 2020  ype="blob",..   
-0000b210: 2020 2020 2068 656c 703d 5f28 2243 6f6e       help=_("Con
-0000b220: 7665 7274 2061 7474 6163 6865 6420 6269  vert attached bi
-0000b230: 6e61 7279 206f 626a 6563 7420 746f 2065  nary object to e
-0000b240: 6c65 6d65 6e74 7322 292c 0d0a 2020 2020  lements"),..    
-0000b250: 290d 0a20 2020 2064 6566 2062 6c6f 6232  )..    def blob2
-0000b260: 7061 7468 286e 6f64 652c 202a 2a6b 7761  path(node, **kwa
-0000b270: 7267 7329 3a0d 0a20 2020 2020 2020 2063  rgs):..        c
-0000b280: 616e 6365 6c6c 6564 203d 2046 616c 7365  ancelled = False
-0000b290: 0d0a 2020 2020 2020 2020 6672 6f6d 206d  ..        from m
-0000b2a0: 6565 726b 3430 742e 746f 6f6c 732e 6472  eerk40t.tools.dr
-0000b2b0: 6976 6572 5f74 6f5f 7061 7468 2069 6d70  iver_to_path imp
-0000b2c0: 6f72 7420 4472 6976 6572 546f 5061 7468  ort DriverToPath
-0000b2d0: 0d0a 0d0a 2020 2020 2020 2020 6432 7020  ....        d2p 
-0000b2e0: 3d20 4472 6976 6572 546f 5061 7468 2829  = DriverToPath()
-0000b2f0: 0d0a 2020 2020 2020 2020 6469 616c 6f67  ..        dialog
-0000b300: 5f63 6c61 7373 203d 206b 6572 6e65 6c2e  _class = kernel.
-0000b310: 6c6f 6f6b 7570 2822 6469 616c 6f67 2f6f  lookup("dialog/o
-0000b320: 7074 696f 6e73 2229 0d0a 2020 2020 2020  ptions")..      
-0000b330: 2020 6966 2064 6961 6c6f 675f 636c 6173    if dialog_clas
-0000b340: 7320 616e 6420 6861 7361 7474 7228 6432  s and hasattr(d2
-0000b350: 702c 2022 6f70 7469 6f6e 7322 293a 0d0a  p, "options"):..
-0000b360: 2020 2020 2020 2020 2020 2020 6368 6f69              choi
-0000b370: 6365 7320 3d20 6765 7461 7474 7228 6432  ces = getattr(d2
-0000b380: 702c 2022 6f70 7469 6f6e 7322 2c20 4e6f  p, "options", No
-0000b390: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
-0000b3a0: 2069 6620 6368 6f69 6365 7320 6973 206e   if choices is n
-0000b3b0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-0000b3c0: 2020 2020 2020 2020 2020 666f 7220 656e            for en
-0000b3d0: 7472 7920 696e 2063 686f 6963 6573 3a0d  try in choices:.
-0000b3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b3f0: 2020 2020 2069 6620 226c 6162 656c 2220       if "label" 
-0000b400: 696e 2065 6e74 7279 3a0d 0a20 2020 2020  in entry:..     
+00008b50: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+00008b60: 2020 7365 6c66 2e73 6574 5f65 6d70 6861    self.set_empha
+00008b70: 7369 7328 4e6f 6e65 290d 0a20 2020 2020  sis(None)..     
+00008b80: 2020 206e 6f64 652e 7265 6d6f 7665 5f6e     node.remove_n
+00008b90: 6f64 6528 290d 0a20 2020 2020 2020 2073  ode()..        s
+00008ba0: 656c 662e 7369 676e 616c 2822 6f70 6572  elf.signal("oper
+00008bb0: 6174 696f 6e5f 7265 6d6f 7665 6422 290d  ation_removed").
+00008bc0: 0a0d 0a20 2020 2040 7472 6565 5f63 6f6e  ...    @tree_con
+00008bd0: 6469 7469 6f6e 616c 280d 0a20 2020 2020  ditional(..     
+00008be0: 2020 206c 616d 6264 6120 636f 6e64 3a20     lambda cond: 
+00008bf0: 6c65 6e28 6c69 7374 2873 656c 662e 666c  len(list(self.fl
+00008c00: 6174 2873 656c 6563 7465 643d 5472 7565  at(selected=True
+00008c10: 2c20 6361 7363 6164 653d 4661 6c73 652c  , cascade=False,
+00008c20: 2074 7970 6573 3d22 626c 6f62 2229 2929   types="blob")))
+00008c30: 0d0a 2020 2020 2020 2020 3d3d 2031 0d0a  ..        == 1..
+00008c40: 2020 2020 290d 0a20 2020 2040 7472 6565      )..    @tree
+00008c50: 5f6f 7065 7261 7469 6f6e 280d 0a20 2020  _operation(..   
+00008c60: 2020 2020 205f 2822 4465 6c65 7465 2062       _("Delete b
+00008c70: 6c6f 6220 277b 6e61 6d65 7d27 2066 756c  lob '{name}' ful
+00008c80: 6c79 2229 2c0d 0a20 2020 2020 2020 206e  ly"),..        n
+00008c90: 6f64 655f 7479 7065 3d22 626c 6f62 222c  ode_type="blob",
+00008ca0: 0d0a 2020 2020 2020 2020 6865 6c70 3d22  ..        help="
+00008cb0: 222c 0d0a 2020 2020 290d 0a20 2020 2064  ",..    )..    d
+00008cc0: 6566 2072 656d 6f76 655f 7479 7065 5f62  ef remove_type_b
+00008cd0: 6c6f 6228 6e6f 6465 2c20 2a2a 6b77 6172  lob(node, **kwar
+00008ce0: 6773 293a 0d0a 2020 2020 2020 2020 7365  gs):..        se
+00008cf0: 6c66 2e73 6574 5f65 6d70 6861 7369 7328  lf.set_emphasis(
+00008d00: 4e6f 6e65 290d 0a20 2020 2020 2020 206e  None)..        n
+00008d10: 6f64 652e 7265 6d6f 7665 5f6e 6f64 6528  ode.remove_node(
+00008d20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00008d30: 7369 676e 616c 2822 6f70 6572 6174 696f  signal("operatio
+00008d40: 6e5f 7265 6d6f 7665 6422 290d 0a0d 0a20  n_removed").... 
+00008d50: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
+00008d60: 6f6e 616c 280d 0a20 2020 2020 2020 206c  onal(..        l
+00008d70: 616d 6264 6120 636f 6e64 3a20 6c65 6e28  ambda cond: len(
+00008d80: 6c69 7374 2873 656c 662e 666c 6174 2873  list(self.flat(s
+00008d90: 656c 6563 7465 643d 5472 7565 2c20 6361  elected=True, ca
+00008da0: 7363 6164 653d 4661 6c73 652c 2074 7970  scade=False, typ
+00008db0: 6573 3d6f 705f 6e6f 6465 7329 2929 0d0a  es=op_nodes)))..
+00008dc0: 2020 2020 2020 2020 3e20 310d 0a20 2020          > 1..   
+00008dd0: 2029 0d0a 2020 2020 4074 7265 655f 6361   )..    @tree_ca
+00008de0: 6c63 280d 0a20 2020 2020 2020 2022 6563  lc(..        "ec
+00008df0: 6f75 6e74 222c 0d0a 2020 2020 2020 2020  ount",..        
+00008e00: 6c61 6d62 6461 2069 3a20 6c65 6e28 6c69  lambda i: len(li
+00008e10: 7374 2873 656c 662e 666c 6174 2873 656c  st(self.flat(sel
+00008e20: 6563 7465 643d 5472 7565 2c20 6361 7363  ected=True, casc
+00008e30: 6164 653d 4661 6c73 652c 2074 7970 6573  ade=False, types
+00008e40: 3d6f 705f 6e6f 6465 7329 2929 2c0d 0a20  =op_nodes))),.. 
+00008e50: 2020 2029 0d0a 2020 2020 4074 7265 655f     )..    @tree_
+00008e60: 6f70 6572 6174 696f 6e28 0d0a 2020 2020  operation(..    
+00008e70: 2020 2020 5f28 2244 656c 6574 6520 7b65      _("Delete {e
+00008e80: 636f 756e 747d 206f 7065 7261 7469 6f6e  count} operation
+00008e90: 7320 6675 6c6c 7922 292c 0d0a 2020 2020  s fully"),..    
+00008ea0: 2020 2020 6e6f 6465 5f74 7970 653d 6f70      node_type=op
+00008eb0: 5f6e 6f64 6573 2c0d 0a20 2020 2020 2020  _nodes,..       
+00008ec0: 2068 656c 703d 2222 2c0d 0a20 2020 2029   help="",..    )
+00008ed0: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+00008ee0: 5f74 7970 655f 6f70 5f6d 756c 7469 706c  _type_op_multipl
+00008ef0: 6528 6e6f 6465 2c20 2a2a 6b77 6172 6773  e(node, **kwargs
+00008f00: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00008f10: 6f70 2069 6e20 6c69 7374 2873 656c 662e  op in list(self.
+00008f20: 666c 6174 2873 656c 6563 7465 643d 5472  flat(selected=Tr
+00008f30: 7565 2c20 6361 7363 6164 653d 4661 6c73  ue, cascade=Fals
+00008f40: 652c 2074 7970 6573 3d6f 705f 6e6f 6465  e, types=op_node
+00008f50: 7329 293a 0d0a 2020 2020 2020 2020 2020  s)):..          
+00008f60: 2020 6f70 2e72 656d 6f76 655f 6e6f 6465    op.remove_node
+00008f70: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+00008f80: 2e73 6574 5f65 6d70 6861 7369 7328 4e6f  .set_emphasis(No
+00008f90: 6e65 290d 0a20 2020 2020 2020 2073 656c  ne)..        sel
+00008fa0: 662e 7369 676e 616c 2822 6f70 6572 6174  f.signal("operat
+00008fb0: 696f 6e5f 7265 6d6f 7665 6422 290d 0a0d  ion_removed")...
+00008fc0: 0a20 2020 2064 6566 2063 6f6e 7461 696e  .    def contain
+00008fd0: 735f 6e6f 5f75 6e72 656d 6f76 6162 6c65  s_no_unremovable
+00008fe0: 5f69 7465 6d73 2829 3a0d 0a20 2020 2020  _items():..     
+00008ff0: 2020 206e 6f6c 6f63 6b20 3d20 5472 7565     nolock = True
+00009000: 0d0a 2020 2020 2020 2020 666f 7220 6520  ..        for e 
+00009010: 696e 206c 6973 7428 7365 6c66 2e66 6c61  in list(self.fla
+00009020: 7428 7365 6c65 6374 6564 3d54 7275 652c  t(selected=True,
+00009030: 2063 6173 6361 6465 3d54 7275 6529 293a   cascade=True)):
+00009040: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00009050: 2068 6173 6174 7472 2865 2c20 2263 616e   hasattr(e, "can
+00009060: 5f72 656d 6f76 6522 2920 616e 6420 6e6f  _remove") and no
+00009070: 7420 652e 6361 6e5f 7265 6d6f 7665 3a0d  t e.can_remove:.
+00009080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009090: 206e 6f6c 6f63 6b20 3d20 4661 6c73 650d   nolock = False.
+000090a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000090b0: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+000090c0: 7265 7475 726e 206e 6f6c 6f63 6b0d 0a0d  return nolock...
+000090d0: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
+000090e0: 7469 6f6e 616c 286c 616d 6264 6120 636f  tional(lambda co
+000090f0: 6e64 3a20 636f 6e74 6169 6e73 5f6e 6f5f  nd: contains_no_
+00009100: 756e 7265 6d6f 7661 626c 655f 6974 656d  unremovable_item
+00009110: 7328 2929 0d0a 2020 2020 4074 7265 655f  s())..    @tree_
+00009120: 636f 6e64 6974 696f 6e61 6c28 0d0a 2020  conditional(..  
+00009130: 2020 2020 2020 6c61 6d62 6461 2063 6f6e        lambda con
+00009140: 643a 206c 656e 280d 0a20 2020 2020 2020  d: len(..       
+00009150: 2020 2020 206c 6973 7428 7365 6c66 2e66       list(self.f
+00009160: 6c61 7428 7365 6c65 6374 6564 3d54 7275  lat(selected=Tru
+00009170: 652c 2063 6173 6361 6465 3d46 616c 7365  e, cascade=False
+00009180: 2c20 7479 7065 733d 2822 6669 6c65 222c  , types=("file",
+00009190: 2022 6772 6f75 7022 2929 290d 0a20 2020   "group")))..   
+000091a0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000091b0: 3d3d 2031 0d0a 2020 2020 290d 0a20 2020  == 1..    )..   
+000091c0: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+000091d0: 280d 0a20 2020 2020 2020 205f 2822 4465  (..        _("De
+000091e0: 6c65 7465 2067 726f 7570 2027 7b6e 616d  lete group '{nam
+000091f0: 657d 2720 616e 6420 616c 6c20 6974 7320  e}' and all its 
+00009200: 6368 696c 642d 656c 656d 656e 7473 2066  child-elements f
+00009210: 756c 6c79 2229 2c0d 0a20 2020 2020 2020  ully"),..       
+00009220: 206e 6f64 655f 7479 7065 3d22 6772 6f75   node_type="grou
+00009230: 7022 2c0d 0a20 2020 2020 2020 2068 656c  p",..        hel
+00009240: 703d 2222 2c0d 0a20 2020 2029 0d0a 2020  p="",..    )..  
+00009250: 2020 6465 6620 7265 6d6f 7665 5f74 7970    def remove_typ
+00009260: 655f 6772 7028 6e6f 6465 2c20 2a2a 6b77  e_grp(node, **kw
+00009270: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00009280: 7365 6c66 2e73 6574 5f65 6d70 6861 7369  self.set_emphasi
+00009290: 7328 4e6f 6e65 290d 0a20 2020 2020 2020  s(None)..       
+000092a0: 206e 6f64 652e 7265 6d6f 7665 5f6e 6f64   node.remove_nod
+000092b0: 6528 290d 0a0d 0a20 2020 2040 7472 6565  e()....    @tree
+000092c0: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
+000092d0: 6264 6120 636f 6e64 3a20 636f 6e74 6169  bda cond: contai
+000092e0: 6e73 5f6e 6f5f 756e 7265 6d6f 7661 626c  ns_no_unremovabl
+000092f0: 655f 6974 656d 7328 2929 0d0a 2020 2020  e_items())..    
+00009300: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
+00009310: 6c28 0d0a 2020 2020 2020 2020 6c61 6d62  l(..        lamb
+00009320: 6461 2063 6f6e 643a 206c 656e 280d 0a20  da cond: len(.. 
+00009330: 2020 2020 2020 2020 2020 206c 6973 7428             list(
+00009340: 7365 6c66 2e66 6c61 7428 7365 6c65 6374  self.flat(select
+00009350: 6564 3d54 7275 652c 2063 6173 6361 6465  ed=True, cascade
+00009360: 3d46 616c 7365 2c20 7479 7065 733d 2822  =False, types=("
+00009370: 6669 6c65 222c 2022 6772 6f75 7022 2929  file", "group"))
+00009380: 290d 0a20 2020 2020 2020 2029 0d0a 2020  )..        )..  
+00009390: 2020 2020 2020 3d3d 2031 0d0a 2020 2020        == 1..    
+000093a0: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+000093b0: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
+000093c0: 205f 2822 5265 6d6f 7665 206c 6f61 6465   _("Remove loade
+000093d0: 6420 6669 6c65 2027 7b6e 616d 657d 2720  d file '{name}' 
+000093e0: 616e 6420 616c 6c20 6974 7320 6368 696c  and all its chil
+000093f0: 642d 656c 656d 656e 7473 2066 756c 6c79  d-elements fully
+00009400: 2229 2c0d 0a20 2020 2020 2020 206e 6f64  "),..        nod
+00009410: 655f 7479 7065 3d22 6669 6c65 222c 0d0a  e_type="file",..
+00009420: 2020 2020 2020 2020 6865 6c70 3d22 222c          help="",
+00009430: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
+00009440: 2072 656d 6f76 655f 7479 7065 5f66 696c   remove_type_fil
+00009450: 6528 6e6f 6465 2c20 2a2a 6b77 6172 6773  e(node, **kwargs
+00009460: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00009470: 2e73 6574 5f65 6d70 6861 7369 7328 4e6f  .set_emphasis(No
+00009480: 6e65 290d 0a20 2020 2020 2020 206e 6f64  ne)..        nod
+00009490: 652e 7265 6d6f 7665 5f6e 6f64 6528 290d  e.remove_node().
+000094a0: 0a0d 0a20 2020 2040 7472 6565 5f63 6f6e  ...    @tree_con
+000094b0: 6469 7469 6f6e 616c 286c 616d 6264 6120  ditional(lambda 
+000094c0: 6e6f 6465 3a20 6e6f 7420 6973 5f72 6567  node: not is_reg
+000094d0: 6d61 726b 286e 6f64 6529 290d 0a20 2020  mark(node))..   
+000094e0: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+000094f0: 280d 0a20 2020 2020 2020 205f 2822 5265  (..        _("Re
+00009500: 6d6f 7665 2074 7261 6e73 7061 7265 6e74  move transparent
+00009510: 206f 626a 6563 7473 2229 2c0d 0a20 2020   objects"),..   
+00009520: 2020 2020 206e 6f64 655f 7479 7065 3d28       node_type=(
+00009530: 2267 726f 7570 222c 2022 6669 6c65 2229  "group", "file")
+00009540: 2c0d 0a20 2020 2020 2020 2068 656c 703d  ,..        help=
+00009550: 5f28 2252 656d 6f76 6520 616c 6c20 656c  _("Remove all el
+00009560: 656d 656e 7473 2074 6861 7420 6e65 6974  ements that neit
+00009570: 6865 7220 6861 7665 2061 2062 6f72 6465  her have a borde
+00009580: 7220 6e6f 7220 6120 6669 6c6c 2063 6f6c  r nor a fill col
+00009590: 6f72 2229 2c0d 0a20 2020 2029 0d0a 2020  or"),..    )..  
+000095a0: 2020 6465 6620 7265 6d6f 7665 5f74 7261    def remove_tra
+000095b0: 6e73 7061 7265 6e74 286e 6f64 652c 202a  nsparent(node, *
+000095c0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+000095d0: 2020 2072 6573 203d 2030 0d0a 2020 2020     res = 0..    
+000095e0: 2020 2020 746f 5f72 656d 6f76 6520 3d20      to_remove = 
+000095f0: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+00009600: 656e 6f64 6520 696e 2073 656c 662e 666c  enode in self.fl
+00009610: 6174 280d 0a20 2020 2020 2020 2020 2020  at(..           
+00009620: 2073 656c 6563 7465 643d 5472 7565 2c0d   selected=True,.
+00009630: 0a20 2020 2020 2020 2020 2020 2063 6173  .            cas
+00009640: 6361 6465 3d54 7275 652c 0d0a 2020 2020  cade=True,..    
+00009650: 2020 2020 2020 2020 7479 7065 733d 280d          types=(.
+00009660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009670: 2022 656c 656d 2072 6563 7422 2c0d 0a20   "elem rect",.. 
+00009680: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00009690: 656c 656d 2065 6c6c 6970 7365 222c 0d0a  elem ellipse",..
+000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096b0: 2265 6c65 6d20 7061 7468 222c 0d0a 2020  "elem path",..  
+000096c0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+000096d0: 6c65 6d20 6c69 6e65 222c 0d0a 2020 2020  lem line",..    
+000096e0: 2020 2020 2020 2020 2020 2020 2265 6c65              "ele
+000096f0: 6d20 706f 6c79 6c69 6e65 222c 0d0a 2020  m polyline",..  
+00009700: 2020 2020 2020 2020 2020 292c 0d0a 2020            ),..  
+00009710: 2020 2020 2020 293a 0d0a 2020 2020 2020        ):..      
+00009720: 2020 2020 2020 636f 6c6f 7265 6420 3d20        colored = 
+00009730: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+00009740: 2020 2069 6620 280d 0a20 2020 2020 2020     if (..       
+00009750: 2020 2020 2020 2020 2068 6173 6174 7472           hasattr
+00009760: 2865 6e6f 6465 2c20 2266 696c 6c22 290d  (enode, "fill").
+00009770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009780: 2061 6e64 2065 6e6f 6465 2e66 696c 6c20   and enode.fill 
+00009790: 6973 206e 6f74 204e 6f6e 650d 0a20 2020  is not None..   
+000097a0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+000097b0: 2065 6e6f 6465 2e66 696c 6c2e 6172 6762   enode.fill.argb
+000097c0: 2069 7320 6e6f 7420 4e6f 6e65 0d0a 2020   is not None..  
+000097d0: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
+000097e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000097f0: 6c6f 7265 6420 3d20 5472 7565 0d0a 2020  lored = True..  
+00009800: 2020 2020 2020 2020 2020 6966 2028 0d0a            if (..
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 6861 7361 7474 7228 656e 6f64 652c 2022  hasattr(enode, "
+00009830: 7374 726f 6b65 2229 0d0a 2020 2020 2020  stroke")..      
+00009840: 2020 2020 2020 2020 2020 616e 6420 656e            and en
+00009850: 6f64 652e 7374 726f 6b65 2069 7320 6e6f  ode.stroke is no
+00009860: 7420 4e6f 6e65 0d0a 2020 2020 2020 2020  t None..        
+00009870: 2020 2020 2020 2020 616e 6420 656e 6f64          and enod
+00009880: 652e 7374 726f 6b65 2e61 7267 6220 6973  e.stroke.argb is
+00009890: 206e 6f74 204e 6f6e 650d 0a20 2020 2020   not None..     
+000098a0: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+000098b0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+000098c0: 6564 203d 2054 7275 650d 0a20 2020 2020  ed = True..     
+000098d0: 2020 2020 2020 2069 6620 6e6f 7420 636f         if not co
+000098e0: 6c6f 7265 643a 0d0a 2020 2020 2020 2020  lored:..        
+000098f0: 2020 2020 2020 2020 7265 7320 2b3d 2031          res += 1
+00009900: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009910: 2020 656e 6f64 652e 7265 6d6f 7665 5f6e    enode.remove_n
+00009920: 6f64 6528 290d 0a0d 0a20 2020 2020 2020  ode()....       
+00009930: 2069 6620 7265 7320 3e20 303a 0d0a 2020   if res > 0:..  
+00009940: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00009950: 6967 6e61 6c28 2272 6562 7569 6c64 5f74  ignal("rebuild_t
+00009960: 7265 6522 290d 0a0d 0a20 2020 2023 203d  ree")....    # =
+00009970: 3d3d 3d3d 3d3d 3d3d 3d0d 0a20 2020 2023  =========..    #
+00009980: 2052 656d 6f76 6520 4f70 6572 6174 696f   Remove Operatio
+00009990: 6e73 2028 4966 204e 6f20 5472 6565 2053  ns (If No Tree S
+000099a0: 656c 6563 7465 6429 0d0a 2020 2020 2320  elected)..    # 
+000099b0: 4e6f 7465 3a20 5468 6973 2063 6f64 6520  Note: This code 
+000099c0: 776f 756c 6420 7261 7265 6c79 206d 6174  would rarely mat
+000099d0: 6368 2061 6e79 7468 696e 6720 7369 6e63  ch anything sinc
+000099e0: 6520 7468 6520 7472 6565 2073 656c 6563  e the tree selec
+000099f0: 7465 6420 7769 6c6c 2061 6c6d 6f73 7420  ted will almost 
+00009a00: 616c 7761 7973 2062 6520 7472 7565 2069  always be true i
+00009a10: 6620 7765 2068 6176 650d 0a20 2020 2023  f we have..    #
+00009a20: 206d 6174 6368 2074 6869 7320 636f 6e64   match this cond
+00009a30: 6974 696f 6e61 6c2e 2054 6865 2074 7265  itional. The tre
+00009a40: 652d 7365 6c65 6374 6564 2064 656c 6574  e-selected delet
+00009a50: 6520 6675 6e63 7469 6f6e 7320 6172 6520  e functions are 
+00009a60: 7375 7065 7269 6f72 2e0d 0a20 2020 2023  superior...    #
+00009a70: 203d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20 2020   ==========..   
+00009a80: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
+00009a90: 616c 280d 0a20 2020 2020 2020 206c 616d  al(..        lam
+00009aa0: 6264 6120 636f 6e64 3a20 6c65 6e28 0d0a  bda cond: len(..
+00009ab0: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+00009ac0: 2873 656c 662e 666c 6174 2873 656c 6563  (self.flat(selec
+00009ad0: 7465 643d 5472 7565 2c20 6361 7363 6164  ted=True, cascad
+00009ae0: 653d 4661 6c73 652c 2074 7970 6573 3d6e  e=False, types=n
+00009af0: 6f6e 5f73 7472 7563 7475 7261 6c5f 6e6f  on_structural_no
+00009b00: 6465 7329 290d 0a20 2020 2020 2020 2029  des))..        )
+00009b10: 0d0a 2020 2020 2020 2020 3d3d 2030 0d0a  ..        == 0..
+00009b20: 2020 2020 290d 0a20 2020 2040 7472 6565      )..    @tree
+00009b30: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
+00009b40: 6264 6120 6e6f 6465 3a20 6c65 6e28 6c69  bda node: len(li
+00009b50: 7374 2873 656c 662e 6f70 7328 7365 6c65  st(self.ops(sele
+00009b60: 6374 6564 3d54 7275 6529 2929 203e 2031  cted=True))) > 1
+00009b70: 290d 0a20 2020 2040 7472 6565 5f63 616c  )..    @tree_cal
+00009b80: 6328 2265 636f 756e 7422 2c20 6c61 6d62  c("ecount", lamb
+00009b90: 6461 2069 3a20 6c65 6e28 6c69 7374 2873  da i: len(list(s
+00009ba0: 656c 662e 6f70 7328 7365 6c65 6374 6564  elf.ops(selected
+00009bb0: 3d54 7275 6529 2929 290d 0a20 2020 2040  =True))))..    @
+00009bc0: 7472 6565 5f6f 7065 7261 7469 6f6e 280d  tree_operation(.
+00009bd0: 0a20 2020 2020 2020 205f 2822 4465 6c65  .        _("Dele
+00009be0: 7465 207b 6563 6f75 6e74 7d20 6f70 6572  te {ecount} oper
+00009bf0: 6174 696f 6e73 2229 2c0d 0a20 2020 2020  ations"),..     
+00009c00: 2020 206e 6f64 655f 7479 7065 3d28 0d0a     node_type=(..
+00009c10: 2020 2020 2020 2020 2020 2020 226f 7020              "op 
+00009c20: 6375 7422 2c0d 0a20 2020 2020 2020 2020  cut",..         
+00009c30: 2020 2022 6f70 2072 6173 7465 7222 2c0d     "op raster",.
+00009c40: 0a20 2020 2020 2020 2020 2020 2022 6f70  .            "op
+00009c50: 2069 6d61 6765 222c 0d0a 2020 2020 2020   image",..      
+00009c60: 2020 2020 2020 226f 7020 656e 6772 6176        "op engrav
+00009c70: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+00009c80: 2022 6f70 2064 6f74 7322 2c0d 0a20 2020   "op dots",..   
+00009c90: 2020 2020 2020 2020 2022 6f70 2068 6174           "op hat
+00009ca0: 6368 222c 0d0a 2020 2020 2020 2020 2020  ch",..          
+00009cb0: 2020 2275 7469 6c20 636f 6e73 6f6c 6522    "util console"
+00009cc0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00009cd0: 7574 696c 2077 6169 7422 2c0d 0a20 2020  util wait",..   
+00009ce0: 2020 2020 2020 2020 2022 7574 696c 2068           "util h
+00009cf0: 6f6d 6522 2c0d 0a20 2020 2020 2020 2020  ome",..         
+00009d00: 2020 2022 7574 696c 2067 6f74 6f22 2c0d     "util goto",.
+00009d10: 0a20 2020 2020 2020 2020 2020 2022 7574  .            "ut
+00009d20: 696c 206f 7574 7075 7422 2c0d 0a20 2020  il output",..   
+00009d30: 2020 2020 2020 2020 2022 7574 696c 2069           "util i
+00009d40: 6e70 7574 222c 0d0a 2020 2020 2020 2020  nput",..        
+00009d50: 2020 2020 226c 6173 6572 636f 6465 222c      "lasercode",
+00009d60: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
+00009d70: 7574 636f 6465 222c 0d0a 2020 2020 2020  utcode",..      
+00009d80: 2020 2020 2020 2262 6c6f 6222 2c0d 0a20        "blob",.. 
+00009d90: 2020 2020 2020 2029 2c0d 0a20 2020 2020         ),..     
+00009da0: 2020 2068 656c 703d 2222 2c0d 0a20 2020     help="",..   
+00009db0: 2029 0d0a 2020 2020 6465 6620 7265 6d6f   )..    def remo
+00009dc0: 7665 5f6e 5f6f 7073 286e 6f64 652c 202a  ve_n_ops(node, *
+00009dd0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00009de0: 2020 2073 656c 6628 226f 7065 7261 7469     self("operati
+00009df0: 6f6e 2064 656c 6574 655c 6e22 290d 0a0d  on delete\n")...
+00009e00: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
+00009e10: 7469 6f6e 280d 0a20 2020 2020 2020 205f  tion(..        _
+00009e20: 2822 5365 6c65 6374 2061 6c6c 2065 6c65  ("Select all ele
+00009e30: 6d65 6e74 7320 6f66 2073 616d 6520 7479  ments of same ty
+00009e40: 7065 2229 2c0d 0a20 2020 2020 2020 206e  pe"),..        n
+00009e50: 6f64 655f 7479 7065 3d65 6c65 6d5f 6e6f  ode_type=elem_no
+00009e60: 6465 732c 0d0a 2020 2020 2020 2020 6865  des,..        he
+00009e70: 6c70 3d5f 2822 5365 6c65 6374 2061 6c6c  lp=_("Select all
+00009e80: 2065 6c65 6d65 6e74 7320 696e 2073 6365   elements in sce
+00009e90: 6e65 2c20 7468 6174 2068 6176 6520 7468  ne, that have th
+00009ea0: 6520 7361 6d65 2074 7970 6520 6173 2074  e same type as t
+00009eb0: 6869 7320 6e6f 6465 2229 2c0d 0a20 2020  his node"),..   
+00009ec0: 2029 0d0a 2020 2020 6465 6620 7365 6c65   )..    def sele
+00009ed0: 6374 5f73 696d 696c 6172 286e 6f64 652c  ct_similar(node,
+00009ee0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+00009ef0: 2020 2020 206e 7479 7065 203d 206e 6f64       ntype = nod
+00009f00: 652e 7479 7065 0d0a 2020 2020 2020 2020  e.type..        
+00009f10: 6368 616e 6765 7320 3d20 4661 6c73 650d  changes = False.
+00009f20: 0a20 2020 2020 2020 2066 6f72 2065 2069  .        for e i
+00009f30: 6e20 7365 6c66 2e65 6c65 6d73 2829 3a0d  n self.elems():.
+00009f40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009f50: 652e 7479 7065 203d 3d20 6e74 7970 6520  e.type == ntype 
+00009f60: 616e 6420 6e6f 7420 652e 656d 7068 6173  and not e.emphas
+00009f70: 697a 6564 2061 6e64 2065 2e63 616e 5f65  ized and e.can_e
+00009f80: 6d70 6861 7369 7a65 3a0d 0a20 2020 2020  mphasize:..     
+00009f90: 2020 2020 2020 2020 2020 2065 2e65 6d70             e.emp
+00009fa0: 6861 7369 7a65 6420 3d20 5472 7565 0d0a  hasized = True..
+00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fc0: 652e 7365 6c65 6374 6564 203d 2054 7275  e.selected = Tru
+00009fd0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00009fe0: 2020 2063 6861 6e67 6573 203d 2054 7275     changes = Tru
+00009ff0: 650d 0a20 2020 2020 2020 2069 6620 6368  e..        if ch
+0000a000: 616e 6765 733a 0d0a 2020 2020 2020 2020  anges:..        
+0000a010: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+0000a020: 655f 7365 6c65 6374 6564 5f61 7265 6128  e_selected_area(
+0000a030: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+0000a040: 656c 662e 7369 676e 616c 2822 7265 6672  elf.signal("refr
+0000a050: 6573 685f 7363 656e 6522 2c20 2253 6365  esh_scene", "Sce
+0000a060: 6e65 2229 0d0a 0d0a 2020 2020 2320 3d3d  ne")....    # ==
+0000a070: 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020 2320  ========..    # 
+0000a080: 5245 4d4f 5645 2045 4c45 4d45 4e54 530d  REMOVE ELEMENTS.
+0000a090: 0a20 2020 2023 203d 3d3d 3d3d 3d3d 3d3d  .    # =========
+0000a0a0: 3d0d 0a20 2020 2023 204d 6f72 6520 7468  =..    # More th
+0000a0b0: 616e 206f 6e65 2c20 7370 6563 6961 6c20  an one, special 
+0000a0c0: 6361 7365 203d 3d20 3120 616c 7265 6164  case == 1 alread
+0000a0d0: 7920 6465 616c 7420 7769 7468 0d0a 2020  y dealt with..  
+0000a0e0: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
+0000a0f0: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
+0000a100: 206c 656e 286c 6973 7428 7365 6c66 2e65   len(list(self.e
+0000a110: 6c65 6d73 2865 6d70 6861 7369 7a65 643d  lems(emphasized=
+0000a120: 5472 7565 2929 2920 3e20 3129 0d0a 2020  True))) > 1)..  
+0000a130: 2020 4074 7265 655f 6361 6c63 2822 6563    @tree_calc("ec
+0000a140: 6f75 6e74 222c 206c 616d 6264 6120 693a  ount", lambda i:
+0000a150: 206c 656e 286c 6973 7428 7365 6c66 2e65   len(list(self.e
+0000a160: 6c65 6d73 2865 6d70 6861 7369 7a65 643d  lems(emphasized=
+0000a170: 5472 7565 2929 2929 0d0a 2020 2020 4074  True))))..    @t
+0000a180: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
+0000a190: 2020 2020 2020 2020 5f28 2244 656c 6574          _("Delet
+0000a1a0: 6520 7b65 636f 756e 747d 2065 6c65 6d65  e {ecount} eleme
+0000a1b0: 6e74 732c 2061 7320 7365 6c65 6374 6564  nts, as selected
+0000a1c0: 2069 6e20 7363 656e 6522 292c 0d0a 2020   in scene"),..  
+0000a1d0: 2020 2020 2020 6e6f 6465 5f74 7970 653d        node_type=
+0000a1e0: 656c 656d 5f67 726f 7570 5f6e 6f64 6573  elem_group_nodes
+0000a1f0: 2c0d 0a20 2020 2020 2020 2068 656c 703d  ,..        help=
+0000a200: 2222 2c0d 0a20 2020 2029 0d0a 2020 2020  "",..    )..    
+0000a210: 6465 6620 7265 6d6f 7665 5f6e 5f65 6c65  def remove_n_ele
+0000a220: 6d65 6e74 7328 6e6f 6465 2c20 2a2a 6b77  ments(node, **kw
+0000a230: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+0000a240: 7365 6c66 2822 656c 656d 656e 7420 6465  self("element de
+0000a250: 6c65 7465 5c6e 2229 0d0a 0d0a 2020 2020  lete\n")....    
+0000a260: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+0000a270: 0d0a 2020 2020 2020 2020 5f28 2242 6563  ..        _("Bec
+0000a280: 6f6d 6520 7265 6665 7265 6e63 6520 6f62  ome reference ob
+0000a290: 6a65 6374 2229 2c0d 0a20 2020 2020 2020  ject"),..       
+0000a2a0: 206e 6f64 655f 7479 7065 3d65 6c65 6d5f   node_type=elem_
+0000a2b0: 6e6f 6465 732c 0d0a 2020 2020 2020 2020  nodes,..        
+0000a2c0: 6865 6c70 3d22 222c 0d0a 2020 2020 290d  help="",..    ).
+0000a2d0: 0a20 2020 2064 6566 206d 616b 655f 6e6f  .    def make_no
+0000a2e0: 6465 5f72 6566 6572 656e 6365 286e 6f64  de_reference(nod
+0000a2f0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+0000a300: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+0000a310: 616c 2822 6d61 6b65 5f72 6566 6572 656e  al("make_referen
+0000a320: 6365 222c 206e 6f64 6529 0d0a 0d0a 2020  ce", node)....  
+0000a330: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
+0000a340: 6e61 6c28 0d0a 2020 2020 2020 2020 6c61  nal(..        la
+0000a350: 6d62 6461 206e 6f64 653a 2069 7369 6e73  mbda node: isins
+0000a360: 7461 6e63 6528 6e6f 6465 2e73 6861 7065  tance(node.shape
+0000a370: 2c20 506f 6c79 676f 6e29 2061 6e64 206c  , Polygon) and l
+0000a380: 656e 286e 6f64 652e 7368 6170 652e 706f  en(node.shape.po
+0000a390: 696e 7473 2920 3e3d 2033 0d0a 2020 2020  ints) >= 3..    
+0000a3a0: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+0000a3b0: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
+0000a3c0: 205f 2822 4d61 6b65 2050 6f6c 7967 6f6e   _("Make Polygon
+0000a3d0: 2072 6567 756c 6172 2229 2c0d 0a20 2020   regular"),..   
+0000a3e0: 2020 2020 206e 6f64 655f 7479 7065 3d22       node_type="
+0000a3f0: 656c 656d 2070 6f6c 796c 696e 6522 2c0d  elem polyline",.
+0000a400: 0a20 2020 2020 2020 2068 656c 703d 2222  .        help=""
+0000a410: 2c0d 0a20 2020 2029 0d0a 2020 2020 6465  ,..    )..    de
+0000a420: 6620 6d61 6b65 5f70 6f6c 7967 6f6e 5f72  f make_polygon_r
+0000a430: 6567 756c 6172 286e 6f64 652c 202a 2a6b  egular(node, **k
+0000a440: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+0000a450: 2023 2066 726f 6d20 2e75 6e69 7473 2069   # from .units i
+0000a460: 6d70 6f72 7420 4c65 6e67 7468 0d0a 2020  mport Length..  
+0000a470: 2020 2020 2020 2320 6672 6f6d 202e 2e73        # from ..s
+0000a480: 7667 656c 656d 656e 7473 2069 6d70 6f72  vgelements impor
+0000a490: 7420 436f 6c6f 720d 0a0d 0a20 2020 2020  t Color....     
+0000a4a0: 2020 2023 2064 6566 206d 6b5f 6465 6275     # def mk_debu
+0000a4b0: 675f 706f 696e 7428 782c 2079 2c20 636f  g_point(x, y, co
+0000a4c0: 6c29 3a0d 0a20 2020 2020 2020 2023 2020  l):..        #  
+0000a4d0: 2020 2063 6972 6320 3d20 456c 6c69 7073     circ = Ellips
+0000a4e0: 6528 6378 3d78 2c20 6379 3d79 2c20 723d  e(cx=x, cy=y, r=
+0000a4f0: 666c 6f61 7428 4c65 6e67 7468 2822 316d  float(Length("1m
+0000a500: 6d22 2929 290d 0a20 2020 2020 2020 2023  m")))..        #
+0000a510: 2020 2020 2063 6972 632e 7472 616e 7366       circ.transf
+0000a520: 6f72 6d20 3d20 636f 7079 286e 6f64 652e  orm = copy(node.
+0000a530: 7368 6170 652e 7472 616e 7366 6f72 6d29  shape.transform)
+0000a540: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0000a550: 7365 6c66 2e65 6c65 6d5f 6272 616e 6368  self.elem_branch
+0000a560: 2e61 6464 280d 0a20 2020 2020 2020 2023  .add(..        #
+0000a570: 2020 2020 2020 2020 2073 6861 7065 3d63           shape=c
+0000a580: 6972 632c 0d0a 2020 2020 2020 2020 2320  irc,..        # 
+0000a590: 2020 2020 2020 2020 7479 7065 3d22 656c          type="el
+0000a5a0: 656d 2065 6c6c 6970 7365 222c 0d0a 2020  em ellipse",..  
+0000a5b0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0000a5c0: 7374 726f 6b65 3d43 6f6c 6f72 2863 6f6c  stroke=Color(col
+0000a5d0: 292c 0d0a 2020 2020 2020 2020 2320 2020  ),..        #   
+0000a5e0: 2020 2020 2020 6669 6c6c 3d43 6f6c 6f72        fill=Color
+0000a5f0: 2863 6f6c 292c 0d0a 2020 2020 2020 2020  (col),..        
+0000a600: 2320 2020 2020 2020 2020 6d61 7472 6978  #         matrix
+0000a610: 3d63 6f70 7928 6e6f 6465 2e6d 6174 7269  =copy(node.matri
+0000a620: 7829 2c0d 0a20 2020 2020 2020 2023 2020  x),..        #  
+0000a630: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+0000a640: 6966 206e 6f64 6520 6973 204e 6f6e 6520  if node is None 
+0000a650: 6f72 206e 6f64 652e 7479 7065 2021 3d20  or node.type != 
+0000a660: 2265 6c65 6d20 706f 6c79 6c69 6e65 223a  "elem polyline":
+0000a670: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0000a680: 7475 726e 0d0a 2020 2020 2020 2020 6e75  turn..        nu
+0000a690: 6d62 6572 5f70 6f69 6e74 7320 3d20 6c65  mber_points = le
+0000a6a0: 6e28 6e6f 6465 2e73 6861 7065 2e70 6f69  n(node.shape.poi
+0000a6b0: 6e74 7329 0d0a 2020 2020 2020 2020 2320  nts)..        # 
+0000a6c0: 7072 696e 7420 2866 224e 756d 6265 7220  print (f"Number 
+0000a6d0: 6f66 2070 6f69 6e74 733a 207b 6e75 6d62  of points: {numb
+0000a6e0: 6572 5f70 6f69 6e74 737d 2229 0d0a 2020  er_points}")..  
+0000a6f0: 2020 2020 2020 2320 666f 7220 7072 6f70        # for prop
+0000a700: 2069 6e20 6469 7228 6e6f 6465 293a 0d0a   in dir(node):..
+0000a710: 2020 2020 2020 2020 2320 2020 2020 7072          #     pr
+0000a720: 696e 7420 2866 227b 7072 6f70 7d20 2d20  int (f"{prop} - 
+0000a730: 7b67 6574 6174 7472 286e 6f64 652c 2027  {getattr(node, '
+0000a740: 7072 6f70 272c 2027 2729 7d22 290d 0a20  prop', '')}").. 
+0000a750: 2020 2020 2020 2023 2066 6f72 2069 6478         # for idx
+0000a760: 2c20 7074 2069 6e20 656e 756d 6572 6174  , pt in enumerat
+0000a770: 6528 6e6f 6465 2e73 6861 7065 2e70 6f69  e(node.shape.poi
+0000a780: 6e74 7329 3a0d 0a20 2020 2020 2020 2023  nts):..        #
+0000a790: 2020 2020 2070 7269 6e74 2028 6622 7b69       print (f"{i
+0000a7a0: 6478 7d3a 207b 7074 2e78 3a2e 3166 7d2c  dx}: {pt.x:.1f},
+0000a7b0: 207b 7074 2e79 3a2e 3166 7d22 290d 0a20   {pt.y:.1f}").. 
+0000a7c0: 2020 2020 2020 2069 6620 6e75 6d62 6572         if number
+0000a7d0: 5f70 6f69 6e74 7320 3c20 3320 6f72 206e  _points < 3 or n
+0000a7e0: 6f74 2069 7369 6e73 7461 6e63 6528 6e6f  ot isinstance(no
+0000a7f0: 6465 2e73 6861 7065 2c20 506f 6c79 676f  de.shape, Polygo
+0000a800: 6e29 3a0d 0a20 2020 2020 2020 2020 2020  n):..           
+0000a810: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
+0000a820: 2070 7473 203d 206e 6f64 652e 7368 6170   pts = node.shap
+0000a830: 652e 706f 696e 7473 0d0a 2020 2020 2020  e.points..      
+0000a840: 2020 6478 203d 2070 7473 5b31 5d2e 7820    dx = pts[1].x 
+0000a850: 2d20 7074 735b 305d 2e78 0d0a 2020 2020  - pts[0].x..    
+0000a860: 2020 2020 6479 203d 2070 7473 5b31 5d2e      dy = pts[1].
+0000a870: 7920 2d20 7074 735b 305d 2e79 0d0a 2020  y - pts[0].y..  
+0000a880: 2020 2020 2020 6261 7365 6c69 6e65 203d        baseline =
+0000a890: 206d 6174 682e 7371 7274 2864 7820 2a20   math.sqrt(dx * 
+0000a8a0: 6478 202b 2064 7920 2a20 6479 290d 0a20  dx + dy * dy).. 
+0000a8b0: 2020 2020 2020 2061 706f 7468 656d 203d         apothem =
+0000a8c0: 2062 6173 656c 696e 6520 2f20 2832 202a   baseline / (2 *
+0000a8d0: 206d 6174 682e 7461 6e28 6d61 7468 2e74   math.tan(math.t
+0000a8e0: 6175 202f 2028 3220 2a20 6e75 6d62 6572  au / (2 * number
+0000a8f0: 5f70 6f69 6e74 7329 2929 0d0a 2020 2020  _points)))..    
+0000a900: 2020 2020 6369 7263 756d 7261 6469 7573      circumradius
+0000a910: 203d 2062 6173 656c 696e 6520 2f20 2832   = baseline / (2
+0000a920: 202a 206d 6174 682e 7369 6e28 6d61 7468   * math.sin(math
+0000a930: 2e74 6175 202f 2028 3220 2a20 6e75 6d62  .tau / (2 * numb
+0000a940: 6572 5f70 6f69 6e74 7329 2929 0d0a 2020  er_points)))..  
+0000a950: 2020 2020 2020 6d69 6470 6f69 6e74 203d        midpoint =
+0000a960: 2050 6f69 6e74 2870 7473 5b30 5d2e 7820   Point(pts[0].x 
+0000a970: 2b20 302e 3520 2a20 6478 2c20 7074 735b  + 0.5 * dx, pts[
+0000a980: 305d 2e79 202b 2030 2e35 202a 2064 7929  0].y + 0.5 * dy)
+0000a990: 0d0a 2020 2020 2020 2020 2320 206d 6b5f  ..        #  mk_
+0000a9a0: 6465 6275 675f 706f 696e 7428 6d69 6470  debug_point(midp
+0000a9b0: 6f69 6e74 2e78 2c20 6d69 6470 6f69 6e74  oint.x, midpoint
+0000a9c0: 2e79 2c20 2262 6c61 636b 2229 0d0a 2020  .y, "black")..  
+0000a9d0: 2020 2020 2020 6178 203d 2030 0d0a 2020        ax = 0..  
+0000a9e0: 2020 2020 2020 6179 203d 2030 0d0a 2020        ay = 0..  
+0000a9f0: 2020 2020 2020 666f 7220 6964 782c 2070        for idx, p
+0000aa00: 7420 696e 2065 6e75 6d65 7261 7465 2870  t in enumerate(p
+0000aa10: 7473 293a 0d0a 2020 2020 2020 2020 2020  ts):..          
+0000aa20: 2020 6178 202b 3d20 7074 2e78 0d0a 2020    ax += pt.x..  
+0000aa30: 2020 2020 2020 2020 2020 6179 202b 3d20            ay += 
+0000aa40: 7074 2e79 0d0a 2020 2020 2020 2020 6178  pt.y..        ax
+0000aa50: 202f 3d20 6e75 6d62 6572 5f70 6f69 6e74   /= number_point
+0000aa60: 730d 0a20 2020 2020 2020 2061 7920 2f3d  s..        ay /=
+0000aa70: 206e 756d 6265 725f 706f 696e 7473 0d0a   number_points..
+0000aa80: 2020 2020 2020 2020 2320 5468 6520 6172          # The ar
+0000aa90: 6974 686d 6574 6963 2063 656e 7465 7220  ithmetic center 
+0000aaa0: 2861 782c 2061 7929 2069 6e64 6963 6174  (ax, ay) indicat
+0000aab0: 6573 2074 6f20 7768 6963 680d 0a20 2020  es to which..   
+0000aac0: 2020 2020 2023 2027 7369 6465 2720 6f66       # 'side' of
+0000aad0: 2074 6865 2062 6173 656c 696e 6520 7468   the baseline th
+0000aae0: 6520 706f 6c79 676f 6e20 6e65 6564 7320  e polygon needs 
+0000aaf0: 746f 2062 6520 636f 6e73 7472 7563 7465  to be constructe
+0000ab00: 640d 0a20 2020 2020 2020 2061 7269 7468  d..        arith
+0000ab10: 6d65 7469 635f 6365 6e74 6572 203d 2050  metic_center = P
+0000ab20: 6f69 6e74 2861 782c 2061 7929 0d0a 2020  oint(ax, ay)..  
+0000ab30: 2020 2020 2020 2320 6d6b 5f64 6562 7567        # mk_debug
+0000ab40: 5f70 6f69 6e74 2861 782c 2061 792c 2022  _point(ax, ay, "
+0000ab50: 6772 6565 6e22 290d 0a20 2020 2020 2020  green")..       
+0000ab60: 2061 6e67 6c65 203d 2070 7473 5b30 5d2e   angle = pts[0].
+0000ab70: 616e 676c 655f 746f 2870 7473 5b31 5d29  angle_to(pts[1])
+0000ab80: 0d0a 2020 2020 2020 2020 6d69 6461 6e67  ..        midang
+0000ab90: 6c65 203d 206d 6964 706f 696e 742e 616e  le = midpoint.an
+0000aba0: 676c 655f 746f 2861 7269 7468 6d65 7469  gle_to(arithmeti
+0000abb0: 635f 6365 6e74 6572 290d 0a20 2020 2020  c_center)..     
+0000abc0: 2020 2061 6e67 6c65 202b 3d20 6d61 7468     angle += math
+0000abd0: 2e74 6175 202f 2034 0d0a 2020 2020 2020  .tau / 4..      
+0000abe0: 2020 6669 7273 745f 706f 696e 7420 3d20    first_point = 
+0000abf0: 506f 696e 742e 706f 6c61 7228 6d69 6470  Point.polar(midp
+0000ac00: 6f69 6e74 2c20 616e 676c 652c 2061 706f  oint, angle, apo
+0000ac10: 7468 656d 290d 0a20 2020 2020 2020 2073  them)..        s
+0000ac20: 6563 6f6e 645f 706f 696e 7420 3d20 506f  econd_point = Po
+0000ac30: 696e 742e 706f 6c61 7228 6d69 6470 6f69  int.polar(midpoi
+0000ac40: 6e74 2c20 616e 676c 6520 2b20 6d61 7468  nt, angle + math
+0000ac50: 2e74 6175 202f 2032 2c20 6170 6f74 6865  .tau / 2, apothe
+0000ac60: 6d29 0d0a 2020 2020 2020 2020 2320 6d6b  m)..        # mk
+0000ac70: 5f64 6562 7567 5f70 6f69 6e74 2866 6972  _debug_point(fir
+0000ac80: 7374 5f70 6f69 6e74 2e78 2c20 6669 7273  st_point.x, firs
+0000ac90: 745f 706f 696e 742e 792c 2022 7965 6c6c  t_point.y, "yell
+0000aca0: 6f77 2229 0d0a 2020 2020 2020 2020 2320  ow")..        # 
+0000acb0: 6d6b 5f64 6562 7567 5f70 6f69 6e74 2873  mk_debug_point(s
+0000acc0: 6563 6f6e 645f 706f 696e 742e 782c 2073  econd_point.x, s
+0000acd0: 6563 6f6e 645f 706f 696e 742e 792c 2022  econd_point.y, "
+0000ace0: 6379 616e 2229 0d0a 2020 2020 2020 2020  cyan")..        
+0000acf0: 6465 6c74 6161 6e67 6c65 203d 206d 6174  deltaangle = mat
+0000ad00: 682e 7461 7520 2f20 6e75 6d62 6572 5f70  h.tau / number_p
+0000ad10: 6f69 6e74 730d 0a20 2020 2020 2020 2064  oints..        d
+0000ad20: 3120 3d20 6172 6974 686d 6574 6963 5f63  1 = arithmetic_c
+0000ad30: 656e 7465 722e 6469 7374 616e 6365 5f74  enter.distance_t
+0000ad40: 6f28 6669 7273 745f 706f 696e 7429 0d0a  o(first_point)..
+0000ad50: 2020 2020 2020 2020 6432 203d 2061 7269          d2 = ari
+0000ad60: 7468 6d65 7469 635f 6365 6e74 6572 2e64  thmetic_center.d
+0000ad70: 6973 7461 6e63 655f 746f 2873 6563 6f6e  istance_to(secon
+0000ad80: 645f 706f 696e 7429 0d0a 2020 2020 2020  d_point)..      
+0000ad90: 2020 6966 2064 3120 3c20 6432 3a0d 0a20    if d1 < d2:.. 
+0000ada0: 2020 2020 2020 2020 2020 2063 656e 7465             cente
+0000adb0: 725f 706f 696e 7420 3d20 636f 7079 2866  r_point = copy(f
+0000adc0: 6972 7374 5f70 6f69 6e74 290d 0a20 2020  irst_point)..   
+0000add0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000ade0: 2020 2020 2020 2020 6365 6e74 6572 5f70          center_p
+0000adf0: 6f69 6e74 203d 2063 6f70 7928 7365 636f  oint = copy(seco
+0000ae00: 6e64 5f70 6f69 6e74 290d 0a20 2020 2020  nd_point)..     
+0000ae10: 2020 2023 206d 6b5f 6465 6275 675f 706f     # mk_debug_po
+0000ae20: 696e 7428 6365 6e74 6572 5f70 6f69 6e74  int(center_point
+0000ae30: 2e78 2c20 6365 6e74 6572 5f70 6f69 6e74  .x, center_point
+0000ae40: 2e79 2c20 2272 6564 2229 0d0a 0d0a 2020  .y, "red")....  
+0000ae50: 2020 2020 2020 6966 2063 656e 7465 725f        if center_
+0000ae60: 706f 696e 742e 616e 676c 655f 746f 2870  point.angle_to(p
+0000ae70: 7473 5b30 5d29 203e 2063 656e 7465 725f  ts[0]) > center_
+0000ae80: 706f 696e 742e 616e 676c 655f 746f 2870  point.angle_to(p
+0000ae90: 7473 5b31 5d29 3a0d 0a20 2020 2020 2020  ts[1]):..       
+0000aea0: 2020 2020 2064 656c 7461 616e 676c 6520       deltaangle 
+0000aeb0: 2a3d 202d 310d 0a20 2020 2020 2020 2061  *= -1..        a
+0000aec0: 6e67 6c65 203d 2063 656e 7465 725f 706f  ngle = center_po
+0000aed0: 696e 742e 616e 676c 655f 746f 2870 7473  int.angle_to(pts
+0000aee0: 5b30 5d29 0d0a 2020 2020 2020 2020 666f  [0])..        fo
+0000aef0: 7220 6964 7820 696e 2072 616e 6765 286e  r idx in range(n
+0000af00: 756d 6265 725f 706f 696e 7473 293a 0d0a  umber_points):..
+0000af10: 2020 2020 2020 2020 2020 2020 2320 6966              # if
+0000af20: 2069 6478 203e 2031 3a0d 0a20 2020 2020   idx > 1:..     
+0000af30: 2020 2020 2020 2070 7420 3d20 506f 696e         pt = Poin
+0000af40: 742e 706f 6c61 7228 6365 6e74 6572 5f70  t.polar(center_p
+0000af50: 6f69 6e74 2c20 616e 676c 652c 2063 6972  oint, angle, cir
+0000af60: 6375 6d72 6164 6975 7329 0d0a 2020 2020  cumradius)..    
+0000af70: 2020 2020 2020 2020 7074 735b 6964 785d          pts[idx]
+0000af80: 2e78 203d 2070 742e 780d 0a20 2020 2020  .x = pt.x..     
+0000af90: 2020 2020 2020 2070 7473 5b69 6478 5d2e         pts[idx].
+0000afa0: 7920 3d20 7074 2e79 0d0a 2020 2020 2020  y = pt.y..      
+0000afb0: 2020 2020 2020 616e 676c 6520 2b3d 2064        angle += d
+0000afc0: 656c 7461 616e 676c 650d 0a20 2020 2020  eltaangle..     
+0000afd0: 2020 206e 6f64 652e 616c 7465 7265 6428     node.altered(
+0000afe0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000aff0: 7369 676e 616c 2822 7265 6672 6573 685f  signal("refresh_
+0000b000: 7363 656e 6522 2c20 2253 6365 6e65 2229  scene", "Scene")
+0000b010: 0d0a 0d0a 2020 2020 2320 3d3d 3d3d 3d3d  ....    # ======
+0000b020: 3d3d 3d3d 0d0a 2020 2020 2320 434f 4e56  ====..    # CONV
+0000b030: 4552 5420 5452 4545 204f 5045 5241 5449  ERT TREE OPERATI
+0000b040: 4f4e 530d 0a20 2020 2023 203d 3d3d 3d3d  ONS..    # =====
+0000b050: 3d3d 3d3d 3d0d 0a20 2020 2040 7472 6565  =====..    @tree
+0000b060: 5f6f 7065 7261 7469 6f6e 280d 0a20 2020  _operation(..   
+0000b070: 2020 2020 205f 2822 436f 6e76 6572 7420       _("Convert 
+0000b080: 746f 2043 7574 636f 6465 2229 2c0d 0a20  to Cutcode"),.. 
+0000b090: 2020 2020 2020 206e 6f64 655f 7479 7065         node_type
+0000b0a0: 3d22 6c61 7365 7263 6f64 6522 2c0d 0a20  ="lasercode",.. 
+0000b0b0: 2020 2020 2020 2068 656c 703d 2222 2c0d         help="",.
+0000b0c0: 0a20 2020 2029 0d0a 2020 2020 6465 6620  .    )..    def 
+0000b0d0: 6c61 7365 7263 6f64 6532 6375 7428 6e6f  lasercode2cut(no
+0000b0e0: 6465 2c20 2a2a 6b77 6172 6773 293a 0d0a  de, **kwargs):..
+0000b0f0: 2020 2020 2020 2020 6e6f 6465 2e72 6570          node.rep
+0000b100: 6c61 6365 5f6e 6f64 6528 4375 7443 6f64  lace_node(CutCod
+0000b110: 652e 6672 6f6d 5f6c 6173 6572 636f 6465  e.from_lasercode
+0000b120: 286e 6f64 652e 636f 6d6d 616e 6473 292c  (node.commands),
+0000b130: 2074 7970 653d 2263 7574 636f 6465 2229   type="cutcode")
+0000b140: 0d0a 0d0a 2020 2020 4074 7265 655f 636f  ....    @tree_co
+0000b150: 6e64 6974 696f 6e61 6c5f 7472 7928 0d0a  nditional_try(..
+0000b160: 2020 2020 2020 2020 6c61 6d62 6461 206e          lambda n
+0000b170: 6f64 653a 206b 6572 6e65 6c2e 6c6f 6f6b  ode: kernel.look
+0000b180: 7570 2866 2273 706f 6f6c 6572 6a6f 622f  up(f"spoolerjob/
+0000b190: 7b6e 6f64 652e 6461 7461 5f74 7970 657d  {node.data_type}
+0000b1a0: 2229 2069 7320 6e6f 7420 4e6f 6e65 0d0a  ") is not None..
+0000b1b0: 2020 2020 290d 0a20 2020 2040 7472 6565      )..    @tree
+0000b1c0: 5f6f 7065 7261 7469 6f6e 280d 0a20 2020  _operation(..   
+0000b1d0: 2020 2020 205f 2822 436f 6e76 6572 7420       _("Convert 
+0000b1e0: 746f 2045 6c65 6d65 6e74 7322 292c 0d0a  to Elements"),..
+0000b1f0: 2020 2020 2020 2020 6e6f 6465 5f74 7970          node_typ
+0000b200: 653d 2262 6c6f 6222 2c0d 0a20 2020 2020  e="blob",..     
+0000b210: 2020 2068 656c 703d 5f28 2243 6f6e 7665     help=_("Conve
+0000b220: 7274 2061 7474 6163 6865 6420 6269 6e61  rt attached bina
+0000b230: 7279 206f 626a 6563 7420 746f 2065 6c65  ry object to ele
+0000b240: 6d65 6e74 7322 292c 0d0a 2020 2020 290d  ments"),..    ).
+0000b250: 0a20 2020 2064 6566 2062 6c6f 6232 7061  .    def blob2pa
+0000b260: 7468 286e 6f64 652c 202a 2a6b 7761 7267  th(node, **kwarg
+0000b270: 7329 3a0d 0a20 2020 2020 2020 2063 616e  s):..        can
+0000b280: 6365 6c6c 6564 203d 2046 616c 7365 0d0a  celled = False..
+0000b290: 2020 2020 2020 2020 6672 6f6d 206d 6565          from mee
+0000b2a0: 726b 3430 742e 746f 6f6c 732e 6472 6976  rk40t.tools.driv
+0000b2b0: 6572 5f74 6f5f 7061 7468 2069 6d70 6f72  er_to_path impor
+0000b2c0: 7420 4472 6976 6572 546f 5061 7468 0d0a  t DriverToPath..
+0000b2d0: 0d0a 2020 2020 2020 2020 6432 7020 3d20  ..        d2p = 
+0000b2e0: 4472 6976 6572 546f 5061 7468 2829 0d0a  DriverToPath()..
+0000b2f0: 2020 2020 2020 2020 6469 616c 6f67 5f63          dialog_c
+0000b300: 6c61 7373 203d 206b 6572 6e65 6c2e 6c6f  lass = kernel.lo
+0000b310: 6f6b 7570 2822 6469 616c 6f67 2f6f 7074  okup("dialog/opt
+0000b320: 696f 6e73 2229 0d0a 2020 2020 2020 2020  ions")..        
+0000b330: 6966 2064 6961 6c6f 675f 636c 6173 7320  if dialog_class 
+0000b340: 616e 6420 6861 7361 7474 7228 6432 702c  and hasattr(d2p,
+0000b350: 2022 6f70 7469 6f6e 7322 293a 0d0a 2020   "options"):..  
+0000b360: 2020 2020 2020 2020 2020 6368 6f69 6365            choice
+0000b370: 7320 3d20 6765 7461 7474 7228 6432 702c  s = getattr(d2p,
+0000b380: 2022 6f70 7469 6f6e 7322 2c20 4e6f 6e65   "options", None
+0000b390: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000b3a0: 6620 6368 6f69 6365 7320 6973 206e 6f74  f choices is not
+0000b3b0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000b3c0: 2020 2020 2020 2020 666f 7220 656e 7472          for entr
+0000b3d0: 7920 696e 2063 686f 6963 6573 3a0d 0a20  y in choices:.. 
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 2069 6620 226c 6162 656c 2220 696e     if "label" in
+0000b400: 2065 6e74 7279 3a0d 0a20 2020 2020 2020   entry:..       
 0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b420: 2020 2065 6e74 7279 5b22 6c61 6265 6c22     entry["label"
-0000b430: 5d20 3d20 5f28 656e 7472 795b 226c 6162  ] = _(entry["lab
-0000b440: 656c 225d 290d 0a20 2020 2020 2020 2020  el"])..         
-0000b450: 2020 2020 2020 2020 2020 2069 6620 2274             if "t
-0000b460: 6970 2220 696e 2065 6e74 7279 3a0d 0a20  ip" in entry:.. 
+0000b420: 2065 6e74 7279 5b22 6c61 6265 6c22 5d20   entry["label"] 
+0000b430: 3d20 5f28 656e 7472 795b 226c 6162 656c  = _(entry["label
+0000b440: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
+0000b450: 2020 2020 2020 2020 2069 6620 2274 6970           if "tip
+0000b460: 2220 696e 2065 6e74 7279 3a0d 0a20 2020  " in entry:..   
 0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 2020 2020 2020 2065 6e74 7279 5b22 7469         entry["ti
-0000b490: 7022 5d20 3d20 5f28 656e 7472 795b 2274  p"] = _(entry["t
-0000b4a0: 6970 225d 290d 0a20 2020 2020 2020 2020  ip"])..         
-0000b4b0: 2020 2020 2020 2020 2020 2069 6620 2264             if "d
-0000b4c0: 6973 706c 6179 2220 696e 2065 6e74 7279  isplay" in entry
-0000b4d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000b4e0: 2020 2020 2020 2020 2020 206e 6577 6469             newdi
-0000b4f0: 7370 6c61 7920 3d20 5b5d 0d0a 2020 2020  splay = []..    
+0000b480: 2020 2020 2065 6e74 7279 5b22 7469 7022       entry["tip"
+0000b490: 5d20 3d20 5f28 656e 7472 795b 2274 6970  ] = _(entry["tip
+0000b4a0: 225d 290d 0a20 2020 2020 2020 2020 2020  "])..           
+0000b4b0: 2020 2020 2020 2020 2069 6620 2264 6973           if "dis
+0000b4c0: 706c 6179 2220 696e 2065 6e74 7279 3a0d  play" in entry:.
+0000b4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b4e0: 2020 2020 2020 2020 206e 6577 6469 7370           newdisp
+0000b4f0: 6c61 7920 3d20 5b5d 0d0a 2020 2020 2020  lay = []..      
 0000b500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b510: 2020 2020 666f 7220 6465 6e74 7279 2069      for dentry i
-0000b520: 6e20 656e 7472 795b 2264 6973 706c 6179  n entry["display
-0000b530: 225d 3a0d 0a20 2020 2020 2020 2020 2020  "]:..           
-0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 206e 6577 6469 7370 6c61 792e 6170 7065   newdisplay.appe
-0000b560: 6e64 285f 2864 656e 7472 7929 290d 0a20  nd(_(dentry)).. 
+0000b510: 2020 666f 7220 6465 6e74 7279 2069 6e20    for dentry in 
+0000b520: 656e 7472 795b 2264 6973 706c 6179 225d  entry["display"]
+0000b530: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000b540: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000b550: 6577 6469 7370 6c61 792e 6170 7065 6e64  ewdisplay.append
+0000b560: 285f 2864 656e 7472 7929 290d 0a20 2020  (_(dentry))..   
 0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b580: 2020 2020 2020 2065 6e74 7279 5b22 6469         entry["di
-0000b590: 7370 6c61 7922 5d20 3d20 6e65 7764 6973  splay"] = newdis
-0000b5a0: 706c 6179 0d0a 2020 2020 2020 2020 2020  play..          
-0000b5b0: 2020 2020 2020 6469 616c 6f67 203d 2064        dialog = d
-0000b5c0: 6961 6c6f 675f 636c 6173 7328 7365 6c66  ialog_class(self
-0000b5d0: 2e6b 6572 6e65 6c2c 2063 686f 6963 6573  .kernel, choices
-0000b5e0: 3d63 686f 6963 6573 290d 0a20 2020 2020  =choices)..     
-0000b5f0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-0000b600: 2064 6961 6c6f 672e 6469 616c 6f67 5f6f   dialog.dialog_o
-0000b610: 7074 696f 6e73 280d 0a20 2020 2020 2020  ptions(..       
-0000b620: 2020 2020 2020 2020 2020 2020 2074 6974               tit
-0000b630: 6c65 3d5f 2822 426c 6f62 2d43 6f6e 7665  le=_("Blob-Conve
-0000b640: 7273 696f 6e22 292c 0d0a 2020 2020 2020  rsion"),..      
-0000b650: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000b660: 7472 6f3d 5f28 0d0a 2020 2020 2020 2020  tro=_(..        
-0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b680: 2259 6f75 2063 616e 2069 6e66 6c75 656e  "You can influen
-0000b690: 6365 2074 6865 2077 6179 204d 4b20 7769  ce the way MK wi
-0000b6a0: 6c6c 2070 726f 6365 7373 2074 6865 2061  ll process the a
-0000b6b0: 7474 6163 6865 6420 6269 6e61 7279 2064  ttached binary d
-0000b6c0: 6174 613a 220d 0a20 2020 2020 2020 2020  ata:"..         
-0000b6d0: 2020 2020 2020 2020 2020 2029 2c0d 0a20             ),.. 
-0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000b6f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b700: 2020 6966 206e 6f74 2072 6573 3a0d 0a20    if not res:.. 
+0000b580: 2020 2020 2065 6e74 7279 5b22 6469 7370       entry["disp
+0000b590: 6c61 7922 5d20 3d20 6e65 7764 6973 706c  lay"] = newdispl
+0000b5a0: 6179 0d0a 2020 2020 2020 2020 2020 2020  ay..            
+0000b5b0: 2020 2020 6469 616c 6f67 203d 2064 6961      dialog = dia
+0000b5c0: 6c6f 675f 636c 6173 7328 7365 6c66 2e6b  log_class(self.k
+0000b5d0: 6572 6e65 6c2c 2063 686f 6963 6573 3d63  ernel, choices=c
+0000b5e0: 686f 6963 6573 290d 0a20 2020 2020 2020  hoices)..       
+0000b5f0: 2020 2020 2020 2020 2072 6573 203d 2064           res = d
+0000b600: 6961 6c6f 672e 6469 616c 6f67 5f6f 7074  ialog.dialog_opt
+0000b610: 696f 6e73 280d 0a20 2020 2020 2020 2020  ions(..         
+0000b620: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+0000b630: 3d5f 2822 426c 6f62 2d43 6f6e 7665 7273  =_("Blob-Convers
+0000b640: 696f 6e22 292c 0d0a 2020 2020 2020 2020  ion"),..        
+0000b650: 2020 2020 2020 2020 2020 2020 696e 7472              intr
+0000b660: 6f3d 5f28 0d0a 2020 2020 2020 2020 2020  o=_(..          
+0000b670: 2020 2020 2020 2020 2020 2020 2020 2259                "Y
+0000b680: 6f75 2063 616e 2069 6e66 6c75 656e 6365  ou can influence
+0000b690: 2074 6865 2077 6179 204d 4b20 7769 6c6c   the way MK will
+0000b6a0: 2070 726f 6365 7373 2074 6865 2061 7474   process the att
+0000b6b0: 6163 6865 6420 6269 6e61 7279 2064 6174  ached binary dat
+0000b6c0: 613a 220d 0a20 2020 2020 2020 2020 2020  a:"..           
+0000b6d0: 2020 2020 2020 2020 2029 2c0d 0a20 2020           ),..   
+0000b6e0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0000b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b700: 6966 206e 6f74 2072 6573 3a0d 0a20 2020  if not res:..   
 0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b720: 2020 2063 616e 6365 6c6c 6564 203d 2054     cancelled = T
-0000b730: 7275 650d 0a20 2020 2020 2020 2069 6620  rue..        if 
-0000b740: 6e6f 7420 6361 6e63 656c 6c65 643a 0d0a  not cancelled:..
-0000b750: 2020 2020 2020 2020 2020 2020 6432 702e              d2p.
-0000b760: 7061 7273 6528 6e6f 6465 2e64 6174 615f  parse(node.data_
-0000b770: 7479 7065 2c20 6e6f 6465 2e64 6174 612c  type, node.data,
-0000b780: 2073 656c 6629 0d0a 2020 2020 2020 2020   self)..        
-0000b790: 7265 7475 726e 2054 7275 650d 0a0d 0a20  return True.... 
-0000b7a0: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
-0000b7b0: 6f6e 616c 5f74 7279 280d 0a20 2020 2020  onal_try(..     
-0000b7c0: 2020 206c 616d 6264 6120 6e6f 6465 3a20     lambda node: 
-0000b7d0: 6b65 726e 656c 2e6c 6f6f 6b75 7028 6622  kernel.lookup(f"
-0000b7e0: 7370 6f6f 6c65 726a 6f62 2f7b 6e6f 6465  spoolerjob/{node
-0000b7f0: 2e64 6174 615f 7479 7065 7d22 2920 6973  .data_type}") is
-0000b800: 206e 6f74 204e 6f6e 650d 0a20 2020 2029   not None..    )
-0000b810: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
-0000b820: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
-0000b830: 5f28 2245 7865 6375 7465 2042 6c6f 6222  _("Execute Blob"
-0000b840: 292c 0d0a 2020 2020 2020 2020 6e6f 6465  ),..        node
-0000b850: 5f74 7970 653d 2262 6c6f 6222 2c0d 0a20  _type="blob",.. 
-0000b860: 2020 2020 2020 2068 656c 703d 5f28 2252         help=_("R
-0000b870: 756e 2074 6865 2067 6976 656e 2062 6c6f  un the given blo
-0000b880: 6220 6f6e 2074 6865 2063 7572 7265 6e74  b on the current
-0000b890: 2064 6576 6963 6522 292c 0d0a 2020 2020   device"),..    
-0000b8a0: 290d 0a20 2020 2064 6566 2062 6c6f 625f  )..    def blob_
-0000b8b0: 6578 6563 7574 6528 6e6f 6465 2c20 2a2a  execute(node, **
-0000b8c0: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-0000b8d0: 2020 7370 6f6f 6c65 725f 6a6f 6220 3d20    spooler_job = 
-0000b8e0: 7365 6c66 2e6c 6f6f 6b75 7028 6622 7370  self.lookup(f"sp
-0000b8f0: 6f6f 6c65 726a 6f62 2f7b 6e6f 6465 2e64  oolerjob/{node.d
-0000b900: 6174 615f 7479 7065 7d22 290d 0a20 2020  ata_type}")..   
-0000b910: 2020 2020 206d 6174 7269 7820 3d20 7365       matrix = se
-0000b920: 6c66 2e64 6576 6963 652e 7363 656e 655f  lf.device.scene_
-0000b930: 746f 5f64 6576 6963 655f 6d61 7472 6978  to_device_matrix
-0000b940: 2829 0d0a 2020 2020 2020 2020 6a6f 625f  ()..        job_
-0000b950: 6f62 6a65 6374 203d 2073 706f 6f6c 6572  object = spooler
-0000b960: 5f6a 6f62 2873 656c 662e 6465 7669 6365  _job(self.device
-0000b970: 2e64 7269 7665 722c 206d 6174 7269 7829  .driver, matrix)
-0000b980: 0d0a 2020 2020 2020 2020 6a6f 625f 6f62  ..        job_ob
-0000b990: 6a65 6374 2e77 7269 7465 5f62 6c6f 6228  ject.write_blob(
-0000b9a0: 6e6f 6465 2e64 6174 6129 0d0a 2020 2020  node.data)..    
-0000b9b0: 2020 2020 7365 6c66 2e64 6576 6963 652e      self.device.
-0000b9c0: 7370 6f6f 6c65 722e 7365 6e64 286a 6f62  spooler.send(job
-0000b9d0: 5f6f 626a 6563 7429 0d0a 0d0a 2020 2020  _object)....    
-0000b9e0: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
-0000b9f0: 6c5f 7472 7928 6c61 6d62 6461 206e 6f64  l_try(lambda nod
-0000ba00: 653a 2068 6173 6174 7472 286e 6f64 652c  e: hasattr(node,
-0000ba10: 2022 6173 5f63 7574 6f62 6a65 6374 7322   "as_cutobjects"
-0000ba20: 2929 0d0a 2020 2020 4074 7265 655f 6f70  ))..    @tree_op
-0000ba30: 6572 6174 696f 6e28 0d0a 2020 2020 2020  eration(..      
-0000ba40: 2020 5f28 2243 6f6e 7665 7274 2074 6f20    _("Convert to 
-0000ba50: 4375 7463 6f64 6522 292c 0d0a 2020 2020  Cutcode"),..    
-0000ba60: 2020 2020 6e6f 6465 5f74 7970 653d 2262      node_type="b
-0000ba70: 6c6f 6222 2c0d 0a20 2020 2020 2020 2068  lob",..        h
-0000ba80: 656c 703d 2222 2c0d 0a20 2020 2029 0d0a  elp="",..    )..
-0000ba90: 2020 2020 6465 6620 626c 6f62 3263 7574      def blob2cut
-0000baa0: 286e 6f64 652c 202a 2a6b 7761 7267 7329  (node, **kwargs)
-0000bab0: 3a0d 0a20 2020 2020 2020 206e 6f64 652e  :..        node.
-0000bac0: 7265 706c 6163 655f 6e6f 6465 286e 6f64  replace_node(nod
-0000bad0: 652e 6173 5f63 7574 6f62 6a65 6374 7328  e.as_cutobjects(
-0000bae0: 292c 2074 7970 653d 2263 7574 636f 6465  ), type="cutcode
-0000baf0: 2229 0d0a 0d0a 2020 2020 4074 7265 655f  ")....    @tree_
-0000bb00: 6f70 6572 6174 696f 6e28 0d0a 2020 2020  operation(..    
-0000bb10: 2020 2020 5f28 2243 6f6e 7665 7274 2074      _("Convert t
-0000bb20: 6f20 5061 7468 2229 2c0d 0a20 2020 2020  o Path"),..     
-0000bb30: 2020 206e 6f64 655f 7479 7065 3d22 6375     node_type="cu
-0000bb40: 7463 6f64 6522 2c0d 0a20 2020 2020 2020  tcode",..       
-0000bb50: 2068 656c 703d 2222 2c0d 0a20 2020 2029   help="",..    )
-0000bb60: 0d0a 2020 2020 6465 6620 6375 7463 6f64  ..    def cutcod
-0000bb70: 6532 7061 7468 6375 7428 6e6f 6465 2c20  e2pathcut(node, 
-0000bb80: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-0000bb90: 2020 2020 6375 7463 6f64 6520 3d20 6e6f      cutcode = no
-0000bba0: 6465 2e63 7574 636f 6465 0d0a 2020 2020  de.cutcode..    
-0000bbb0: 2020 2020 6966 2063 7574 636f 6465 2069      if cutcode i
-0000bbc0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-0000bbd0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-0000bbe0: 2020 2020 2065 6c65 6d65 6e74 7320 3d20       elements = 
-0000bbf0: 6c69 7374 2863 7574 636f 6465 2e61 735f  list(cutcode.as_
-0000bc00: 656c 656d 656e 7473 2829 290d 0a20 2020  elements())..   
-0000bc10: 2020 2020 206e 203d 204e 6f6e 650d 0a20       n = None.. 
-0000bc20: 2020 2020 2020 2066 6f72 2065 6c65 6d65         for eleme
-0000bc30: 6e74 2069 6e20 656c 656d 656e 7473 3a0d  nt in elements:.
-0000bc40: 0a20 2020 2020 2020 2020 2020 206e 203d  .            n =
-0000bc50: 2073 656c 662e 656c 656d 5f62 7261 6e63   self.elem_branc
-0000bc60: 682e 6164 6428 7479 7065 3d22 656c 656d  h.add(type="elem
-0000bc70: 2070 6174 6822 2c20 7061 7468 3d65 6c65   path", path=ele
-0000bc80: 6d65 6e74 290d 0a20 2020 2020 2020 206e  ment)..        n
-0000bc90: 6f64 652e 7265 6d6f 7665 5f6e 6f64 6528  ode.remove_node(
-0000bca0: 290d 0a20 2020 2020 2020 2069 6620 6e20  )..        if n 
-0000bcb0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-0000bcc0: 2020 2020 2020 2020 2020 6e2e 666f 6375            n.focu
-0000bcd0: 7328 290d 0a0d 0a20 2020 2040 7472 6565  s()....    @tree
-0000bce0: 5f73 7562 6d65 6e75 285f 2822 436c 6f6e  _submenu(_("Clon
-0000bcf0: 6520 7265 6665 7265 6e63 6522 2929 0d0a  e reference"))..
-0000bd00: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-0000bd10: 696f 6e28 5f28 224d 616b 6520 3120 636f  ion(_("Make 1 co
-0000bd20: 7079 2229 2c20 6e6f 6465 5f74 7970 653d  py"), node_type=
-0000bd30: 2822 7265 6665 7265 6e63 6522 2c29 2c20  ("reference",), 
-0000bd40: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
-0000bd50: 6620 636c 6f6e 655f 7369 6e67 6c65 5f65  f clone_single_e
-0000bd60: 6c65 6d65 6e74 5f6f 7028 6e6f 6465 2c20  lement_op(node, 
-0000bd70: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-0000bd80: 2020 2020 636c 6f6e 655f 656c 656d 656e      clone_elemen
-0000bd90: 745f 6f70 286e 6f64 652c 2063 6f70 6965  t_op(node, copie
-0000bda0: 733d 312c 202a 2a6b 7761 7267 7329 0d0a  s=1, **kwargs)..
-0000bdb0: 0d0a 2020 2020 4074 7265 655f 7375 626d  ..    @tree_subm
-0000bdc0: 656e 7528 5f28 2243 6c6f 6e65 2072 6566  enu(_("Clone ref
-0000bdd0: 6572 656e 6365 2229 290d 0a20 2020 2040  erence"))..    @
-0000bde0: 7472 6565 5f69 7465 7261 7465 2822 636f  tree_iterate("co
-0000bdf0: 7069 6573 222c 2032 2c20 3130 290d 0a20  pies", 2, 10).. 
-0000be00: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-0000be10: 6f6e 285f 2822 4d61 6b65 207b 636f 7069  on(_("Make {copi
-0000be20: 6573 7d20 636f 7069 6573 2229 2c20 6e6f  es} copies"), no
-0000be30: 6465 5f74 7970 653d 2822 7265 6665 7265  de_type=("refere
-0000be40: 6e63 6522 2c29 2c20 6865 6c70 3d22 2229  nce",), help="")
-0000be50: 0d0a 2020 2020 6465 6620 636c 6f6e 655f  ..    def clone_
-0000be60: 656c 656d 656e 745f 6f70 286e 6f64 652c  element_op(node,
-0000be70: 2063 6f70 6965 733d 312c 202a 2a6b 7761   copies=1, **kwa
-0000be80: 7267 7329 3a0d 0a20 2020 2020 2020 2077  rgs):..        w
-0000be90: 6974 6820 7365 6c66 2e73 7461 7469 6328  ith self.static(
-0000bea0: 2263 6c6f 6e65 5f65 6c65 6d5f 6f70 2229  "clone_elem_op")
-0000beb0: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
-0000bec0: 6f64 6573 203d 206c 6973 7428 7365 6c66  odes = list(self
-0000bed0: 2e66 6c61 7428 7365 6c65 6374 6564 3d54  .flat(selected=T
-0000bee0: 7275 652c 2063 6173 6361 6465 3d46 616c  rue, cascade=Fal
-0000bef0: 7365 2c20 7479 7065 733d 2272 6566 6572  se, types="refer
-0000bf00: 656e 6365 2229 290d 0a20 2020 2020 2020  ence"))..       
-0000bf10: 2020 2020 2066 6f72 2073 6e6f 6465 2069       for snode i
-0000bf20: 6e20 6e6f 6465 733a 0d0a 2020 2020 2020  n nodes:..      
-0000bf30: 2020 2020 2020 2020 2020 696e 6465 7820            index 
-0000bf40: 3d20 736e 6f64 652e 7061 7265 6e74 2e63  = snode.parent.c
-0000bf50: 6869 6c64 7265 6e2e 696e 6465 7828 736e  hildren.index(sn
-0000bf60: 6f64 6529 0d0a 2020 2020 2020 2020 2020  ode)..          
-0000bf70: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000bf80: 616e 6765 2863 6f70 6965 7329 3a0d 0a20  ange(copies):.. 
+0000b720: 2063 616e 6365 6c6c 6564 203d 2054 7275   cancelled = Tru
+0000b730: 650d 0a20 2020 2020 2020 2069 6620 6e6f  e..        if no
+0000b740: 7420 6361 6e63 656c 6c65 643a 0d0a 2020  t cancelled:..  
+0000b750: 2020 2020 2020 2020 2020 6432 702e 7061            d2p.pa
+0000b760: 7273 6528 6e6f 6465 2e64 6174 615f 7479  rse(node.data_ty
+0000b770: 7065 2c20 6e6f 6465 2e64 6174 612c 2073  pe, node.data, s
+0000b780: 656c 6629 0d0a 2020 2020 2020 2020 7265  elf)..        re
+0000b790: 7475 726e 2054 7275 650d 0a0d 0a20 2020  turn True....   
+0000b7a0: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
+0000b7b0: 616c 5f74 7279 280d 0a20 2020 2020 2020  al_try(..       
+0000b7c0: 206c 616d 6264 6120 6e6f 6465 3a20 6b65   lambda node: ke
+0000b7d0: 726e 656c 2e6c 6f6f 6b75 7028 6622 7370  rnel.lookup(f"sp
+0000b7e0: 6f6f 6c65 726a 6f62 2f7b 6e6f 6465 2e64  oolerjob/{node.d
+0000b7f0: 6174 615f 7479 7065 7d22 2920 6973 206e  ata_type}") is n
+0000b800: 6f74 204e 6f6e 650d 0a20 2020 2029 0d0a  ot None..    )..
+0000b810: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
+0000b820: 696f 6e28 0d0a 2020 2020 2020 2020 5f28  ion(..        _(
+0000b830: 2245 7865 6375 7465 2042 6c6f 6222 292c  "Execute Blob"),
+0000b840: 0d0a 2020 2020 2020 2020 6e6f 6465 5f74  ..        node_t
+0000b850: 7970 653d 2262 6c6f 6222 2c0d 0a20 2020  ype="blob",..   
+0000b860: 2020 2020 2068 656c 703d 5f28 2252 756e       help=_("Run
+0000b870: 2074 6865 2067 6976 656e 2062 6c6f 6220   the given blob 
+0000b880: 6f6e 2074 6865 2063 7572 7265 6e74 2064  on the current d
+0000b890: 6576 6963 6522 292c 0d0a 2020 2020 290d  evice"),..    ).
+0000b8a0: 0a20 2020 2064 6566 2062 6c6f 625f 6578  .    def blob_ex
+0000b8b0: 6563 7574 6528 6e6f 6465 2c20 2a2a 6b77  ecute(node, **kw
+0000b8c0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+0000b8d0: 7370 6f6f 6c65 725f 6a6f 6220 3d20 7365  spooler_job = se
+0000b8e0: 6c66 2e6c 6f6f 6b75 7028 6622 7370 6f6f  lf.lookup(f"spoo
+0000b8f0: 6c65 726a 6f62 2f7b 6e6f 6465 2e64 6174  lerjob/{node.dat
+0000b900: 615f 7479 7065 7d22 290d 0a20 2020 2020  a_type}")..     
+0000b910: 2020 206d 6174 7269 7820 3d20 7365 6c66     matrix = self
+0000b920: 2e64 6576 6963 652e 7363 656e 655f 746f  .device.scene_to
+0000b930: 5f64 6576 6963 655f 6d61 7472 6978 2829  _device_matrix()
+0000b940: 0d0a 2020 2020 2020 2020 6a6f 625f 6f62  ..        job_ob
+0000b950: 6a65 6374 203d 2073 706f 6f6c 6572 5f6a  ject = spooler_j
+0000b960: 6f62 2873 656c 662e 6465 7669 6365 2e64  ob(self.device.d
+0000b970: 7269 7665 722c 206d 6174 7269 7829 0d0a  river, matrix)..
+0000b980: 2020 2020 2020 2020 6a6f 625f 6f62 6a65          job_obje
+0000b990: 6374 2e77 7269 7465 5f62 6c6f 6228 6e6f  ct.write_blob(no
+0000b9a0: 6465 2e64 6174 6129 0d0a 2020 2020 2020  de.data)..      
+0000b9b0: 2020 7365 6c66 2e64 6576 6963 652e 7370    self.device.sp
+0000b9c0: 6f6f 6c65 722e 7365 6e64 286a 6f62 5f6f  ooler.send(job_o
+0000b9d0: 626a 6563 7429 0d0a 0d0a 2020 2020 4074  bject)....    @t
+0000b9e0: 7265 655f 636f 6e64 6974 696f 6e61 6c5f  ree_conditional_
+0000b9f0: 7472 7928 6c61 6d62 6461 206e 6f64 653a  try(lambda node:
+0000ba00: 2068 6173 6174 7472 286e 6f64 652c 2022   hasattr(node, "
+0000ba10: 6173 5f63 7574 6f62 6a65 6374 7322 2929  as_cutobjects"))
+0000ba20: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+0000ba30: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
+0000ba40: 5f28 2243 6f6e 7665 7274 2074 6f20 4375  _("Convert to Cu
+0000ba50: 7463 6f64 6522 292c 0d0a 2020 2020 2020  tcode"),..      
+0000ba60: 2020 6e6f 6465 5f74 7970 653d 2262 6c6f    node_type="blo
+0000ba70: 6222 2c0d 0a20 2020 2020 2020 2068 656c  b",..        hel
+0000ba80: 703d 2222 2c0d 0a20 2020 2029 0d0a 2020  p="",..    )..  
+0000ba90: 2020 6465 6620 626c 6f62 3263 7574 286e    def blob2cut(n
+0000baa0: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
+0000bab0: 0a20 2020 2020 2020 206e 6f64 652e 7265  .        node.re
+0000bac0: 706c 6163 655f 6e6f 6465 286e 6f64 652e  place_node(node.
+0000bad0: 6173 5f63 7574 6f62 6a65 6374 7328 292c  as_cutobjects(),
+0000bae0: 2074 7970 653d 2263 7574 636f 6465 2229   type="cutcode")
+0000baf0: 0d0a 0d0a 2020 2020 4074 7265 655f 6f70  ....    @tree_op
+0000bb00: 6572 6174 696f 6e28 0d0a 2020 2020 2020  eration(..      
+0000bb10: 2020 5f28 2243 6f6e 7665 7274 2074 6f20    _("Convert to 
+0000bb20: 5061 7468 2229 2c0d 0a20 2020 2020 2020  Path"),..       
+0000bb30: 206e 6f64 655f 7479 7065 3d22 6375 7463   node_type="cutc
+0000bb40: 6f64 6522 2c0d 0a20 2020 2020 2020 2068  ode",..        h
+0000bb50: 656c 703d 2222 2c0d 0a20 2020 2029 0d0a  elp="",..    )..
+0000bb60: 2020 2020 6465 6620 6375 7463 6f64 6532      def cutcode2
+0000bb70: 7061 7468 6375 7428 6e6f 6465 2c20 2a2a  pathcut(node, **
+0000bb80: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+0000bb90: 2020 6375 7463 6f64 6520 3d20 6e6f 6465    cutcode = node
+0000bba0: 2e63 7574 636f 6465 0d0a 2020 2020 2020  .cutcode..      
+0000bbb0: 2020 6966 2063 7574 636f 6465 2069 7320    if cutcode is 
+0000bbc0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+0000bbd0: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
+0000bbe0: 2020 2065 6c65 6d65 6e74 7320 3d20 6c69     elements = li
+0000bbf0: 7374 2863 7574 636f 6465 2e61 735f 656c  st(cutcode.as_el
+0000bc00: 656d 656e 7473 2829 290d 0a20 2020 2020  ements())..     
+0000bc10: 2020 206e 203d 204e 6f6e 650d 0a20 2020     n = None..   
+0000bc20: 2020 2020 2066 6f72 2065 6c65 6d65 6e74       for element
+0000bc30: 2069 6e20 656c 656d 656e 7473 3a0d 0a20   in elements:.. 
+0000bc40: 2020 2020 2020 2020 2020 206e 203d 2073             n = s
+0000bc50: 656c 662e 656c 656d 5f62 7261 6e63 682e  elf.elem_branch.
+0000bc60: 6164 6428 7479 7065 3d22 656c 656d 2070  add(type="elem p
+0000bc70: 6174 6822 2c20 7061 7468 3d65 6c65 6d65  ath", path=eleme
+0000bc80: 6e74 290d 0a20 2020 2020 2020 206e 6f64  nt)..        nod
+0000bc90: 652e 7265 6d6f 7665 5f6e 6f64 6528 290d  e.remove_node().
+0000bca0: 0a20 2020 2020 2020 2069 6620 6e20 6973  .        if n is
+0000bcb0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+0000bcc0: 2020 2020 2020 2020 6e2e 666f 6375 7328          n.focus(
+0000bcd0: 290d 0a0d 0a20 2020 2040 7472 6565 5f73  )....    @tree_s
+0000bce0: 7562 6d65 6e75 285f 2822 436c 6f6e 6520  ubmenu(_("Clone 
+0000bcf0: 7265 6665 7265 6e63 6522 2929 0d0a 2020  reference"))..  
+0000bd00: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
+0000bd10: 6e28 5f28 224d 616b 6520 3120 636f 7079  n(_("Make 1 copy
+0000bd20: 2229 2c20 6e6f 6465 5f74 7970 653d 2822  "), node_type=("
+0000bd30: 7265 6665 7265 6e63 6522 2c29 2c20 6865  reference",), he
+0000bd40: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+0000bd50: 636c 6f6e 655f 7369 6e67 6c65 5f65 6c65  clone_single_ele
+0000bd60: 6d65 6e74 5f6f 7028 6e6f 6465 2c20 2a2a  ment_op(node, **
+0000bd70: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+0000bd80: 2020 636c 6f6e 655f 656c 656d 656e 745f    clone_element_
+0000bd90: 6f70 286e 6f64 652c 2063 6f70 6965 733d  op(node, copies=
+0000bda0: 312c 202a 2a6b 7761 7267 7329 0d0a 0d0a  1, **kwargs)....
+0000bdb0: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
+0000bdc0: 7528 5f28 2243 6c6f 6e65 2072 6566 6572  u(_("Clone refer
+0000bdd0: 656e 6365 2229 290d 0a20 2020 2040 7472  ence"))..    @tr
+0000bde0: 6565 5f69 7465 7261 7465 2822 636f 7069  ee_iterate("copi
+0000bdf0: 6573 222c 2032 2c20 3130 290d 0a20 2020  es", 2, 10)..   
+0000be00: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+0000be10: 285f 2822 4d61 6b65 207b 636f 7069 6573  (_("Make {copies
+0000be20: 7d20 636f 7069 6573 2229 2c20 6e6f 6465  } copies"), node
+0000be30: 5f74 7970 653d 2822 7265 6665 7265 6e63  _type=("referenc
+0000be40: 6522 2c29 2c20 6865 6c70 3d22 2229 0d0a  e",), help="")..
+0000be50: 2020 2020 6465 6620 636c 6f6e 655f 656c      def clone_el
+0000be60: 656d 656e 745f 6f70 286e 6f64 652c 2063  ement_op(node, c
+0000be70: 6f70 6965 733d 312c 202a 2a6b 7761 7267  opies=1, **kwarg
+0000be80: 7329 3a0d 0a20 2020 2020 2020 2077 6974  s):..        wit
+0000be90: 6820 7365 6c66 2e73 7461 7469 6328 2263  h self.static("c
+0000bea0: 6c6f 6e65 5f65 6c65 6d5f 6f70 2229 3a0d  lone_elem_op"):.
+0000beb0: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
+0000bec0: 6573 203d 206c 6973 7428 7365 6c66 2e66  es = list(self.f
+0000bed0: 6c61 7428 7365 6c65 6374 6564 3d54 7275  lat(selected=Tru
+0000bee0: 652c 2063 6173 6361 6465 3d46 616c 7365  e, cascade=False
+0000bef0: 2c20 7479 7065 733d 2272 6566 6572 656e  , types="referen
+0000bf00: 6365 2229 290d 0a20 2020 2020 2020 2020  ce"))..         
+0000bf10: 2020 2066 6f72 2073 6e6f 6465 2069 6e20     for snode in 
+0000bf20: 6e6f 6465 733a 0d0a 2020 2020 2020 2020  nodes:..        
+0000bf30: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
+0000bf40: 736e 6f64 652e 7061 7265 6e74 2e63 6869  snode.parent.chi
+0000bf50: 6c64 7265 6e2e 696e 6465 7828 736e 6f64  ldren.index(snod
+0000bf60: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+0000bf70: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0000bf80: 6765 2863 6f70 6965 7329 3a0d 0a20 2020  ge(copies):..   
 0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 2020 2073 6e6f 6465 2e70 6172 656e 742e     snode.parent.
-0000bfb0: 6164 645f 7265 6665 7265 6e63 6528 736e  add_reference(sn
-0000bfc0: 6f64 652e 6e6f 6465 2c20 706f 733d 696e  ode.node, pos=in
-0000bfd0: 6465 7829 0d0a 2020 2020 2020 2020 2020  dex)..          
-0000bfe0: 2020 2020 2020 736e 6f64 652e 6d6f 6469        snode.modi
-0000bff0: 6669 6564 2829 0d0a 0d0a 2020 2020 4074  fied()....    @t
-0000c000: 7265 655f 636f 6e64 6974 696f 6e61 6c28  ree_conditional(
-0000c010: 6c61 6d62 6461 206e 6f64 653a 206e 6f64  lambda node: nod
-0000c020: 652e 636f 756e 745f 6368 696c 6472 656e  e.count_children
-0000c030: 2829 203e 2031 290d 0a20 2020 2040 7472  () > 1)..    @tr
-0000c040: 6565 5f6f 7065 7261 7469 6f6e 280d 0a20  ee_operation(.. 
-0000c050: 2020 2020 2020 205f 2822 5265 7665 7273         _("Revers
-0000c060: 6520 7375 6269 7465 6d73 206f 7264 6572  e subitems order
-0000c070: 2229 2c0d 0a20 2020 2020 2020 206e 6f64  "),..        nod
-0000c080: 655f 7479 7065 3d28 0d0a 2020 2020 2020  e_type=(..      
-0000c090: 2020 2020 2020 226f 7020 6375 7422 2c0d        "op cut",.
-0000c0a0: 0a20 2020 2020 2020 2020 2020 2022 6f70  .            "op
-0000c0b0: 2072 6173 7465 7222 2c0d 0a20 2020 2020   raster",..     
-0000c0c0: 2020 2020 2020 2022 6f70 2069 6d61 6765         "op image
-0000c0d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-0000c0e0: 226f 7020 656e 6772 6176 6522 2c0d 0a20  "op engrave",.. 
-0000c0f0: 2020 2020 2020 2020 2020 2022 6f70 2064             "op d
-0000c100: 6f74 7322 2c0d 0a20 2020 2020 2020 2020  ots",..         
-0000c110: 2020 2022 6f70 2068 6174 6368 222c 0d0a     "op hatch",..
-0000c120: 2020 2020 2020 2020 2020 2020 2267 726f              "gro
-0000c130: 7570 222c 0d0a 2020 2020 2020 2020 2020  up",..          
-0000c140: 2020 2262 7261 6e63 6820 656c 656d 7322    "branch elems"
-0000c150: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-0000c160: 6669 6c65 222c 0d0a 2020 2020 2020 2020  file",..        
-0000c170: 2020 2020 2262 7261 6e63 6820 6f70 7322      "branch ops"
-0000c180: 2c0d 0a20 2020 2020 2020 2029 2c0d 0a20  ,..        ),.. 
-0000c190: 2020 2020 2020 2068 656c 703d 5f28 2252         help=_("R
-0000c1a0: 6576 6572 7365 2074 6865 2069 7465 6d73  everse the items
-0000c1b0: 2077 6974 6869 6e20 7468 6973 2073 7562   within this sub
-0000c1c0: 6974 656d 2229 2c0d 0a20 2020 2029 0d0a  item"),..    )..
-0000c1d0: 2020 2020 6465 6620 7265 7665 7273 655f      def reverse_
-0000c1e0: 6c61 7965 725f 6f72 6465 7228 6e6f 6465  layer_order(node
-0000c1f0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
-0000c200: 2020 2020 2020 6e6f 6465 2e72 6576 6572        node.rever
-0000c210: 7365 2829 0d0a 2020 2020 2020 2020 7365  se()..        se
-0000c220: 6c66 2e73 6967 6e61 6c28 2272 6566 7265  lf.signal("refre
-0000c230: 7368 5f74 7265 6522 2c20 6c69 7374 2873  sh_tree", list(s
-0000c240: 656c 662e 666c 6174 2874 7970 6573 3d22  elf.flat(types="
-0000c250: 7265 6665 7265 6e63 6522 2929 290d 0a0d  reference")))...
-0000c260: 0a20 2020 2040 7472 6565 5f73 6570 6172  .    @tree_separ
-0000c270: 6174 6f72 5f61 6674 6572 2829 0d0a 2020  ator_after()..  
-0000c280: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
-0000c290: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
-0000c2a0: 2073 656c 662e 636c 6173 7369 6679 5f61   self.classify_a
-0000c2b0: 7574 6f67 656e 6572 6174 6529 0d0a 2020  utogenerate)..  
-0000c2c0: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-0000c2d0: 6e28 0d0a 2020 2020 2020 2020 5f28 2252  n(..        _("R
-0000c2e0: 6566 7265 7368 2063 6c61 7373 6966 6963  efresh classific
-0000c2f0: 6174 696f 6e22 292c 0d0a 2020 2020 2020  ation"),..      
-0000c300: 2020 6e6f 6465 5f74 7970 653d 2262 7261    node_type="bra
-0000c310: 6e63 6820 6f70 7322 2c0d 0a20 2020 2020  nch ops",..     
-0000c320: 2020 2068 656c 703d 5f28 2252 6563 6c61     help=_("Recla
-0000c330: 7373 6966 7920 656c 656d 656e 7473 2061  ssify elements a
-0000c340: 6e64 2063 7265 6174 6520 6f70 6572 6174  nd create operat
-0000c350: 696f 6e73 2069 6620 6e65 6365 7373 6172  ions if necessar
-0000c360: 7922 292c 0d0a 2020 2020 290d 0a20 2020  y"),..    )..   
-0000c370: 2064 6566 2072 6566 7265 7368 5f63 6c61   def refresh_cla
-0000c380: 7369 6669 6361 7469 6f6e 735f 3128 6e6f  sifications_1(no
-0000c390: 6465 2c20 2a2a 6b77 6172 6773 293a 0d0a  de, **kwargs):..
-0000c3a0: 2020 2020 2020 2020 7365 6c66 2e72 656d          self.rem
-0000c3b0: 6f76 655f 656c 656d 656e 7473 5f66 726f  ove_elements_fro
-0000c3c0: 6d5f 6f70 6572 6174 696f 6e73 286c 6973  m_operations(lis
-0000c3d0: 7428 7365 6c66 2e65 6c65 6d73 2829 2929  t(self.elems()))
-0000c3e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-0000c3f0: 6c61 7373 6966 7928 6c69 7374 2873 656c  lassify(list(sel
-0000c400: 662e 656c 656d 7328 2929 290d 0a20 2020  f.elems()))..   
-0000c410: 2020 2020 2073 656c 662e 7369 676e 616c       self.signal
-0000c420: 2822 7265 6672 6573 685f 7472 6565 222c  ("refresh_tree",
-0000c430: 206c 6973 7428 7365 6c66 2e66 6c61 7428   list(self.flat(
-0000c440: 7479 7065 733d 2272 6566 6572 656e 6365  types="reference
-0000c450: 2229 2929 0d0a 0d0a 2020 2020 4074 7265  ")))....    @tre
-0000c460: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
-0000c470: 6d62 6461 206e 6f64 653a 206e 6f74 2073  mbda node: not s
-0000c480: 656c 662e 636c 6173 7369 6679 5f61 7574  elf.classify_aut
-0000c490: 6f67 656e 6572 6174 6529 0d0a 2020 2020  ogenerate)..    
-0000c4a0: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
-0000c4b0: 0d0a 2020 2020 2020 2020 5f28 2252 6566  ..        _("Ref
-0000c4c0: 7265 7368 2063 6c61 7373 6966 6963 6174  resh classificat
-0000c4d0: 696f 6e22 292c 0d0a 2020 2020 2020 2020  ion"),..        
-0000c4e0: 6e6f 6465 5f74 7970 653d 2262 7261 6e63  node_type="branc
-0000c4f0: 6820 6f70 7322 2c0d 0a20 2020 2020 2020  h ops",..       
-0000c500: 2068 656c 703d 5f28 2252 6563 6c61 7373   help=_("Reclass
-0000c510: 6966 7920 656c 656d 656e 7473 2061 6e64  ify elements and
-0000c520: 2075 7365 206f 6e6c 7920 6578 6973 7469   use only existi
-0000c530: 6e67 206f 7065 7261 7469 6f6e 7322 292c  ng operations"),
-0000c540: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
-0000c550: 2072 6566 7265 7368 5f63 6c61 7369 6669   refresh_clasifi
-0000c560: 6361 7469 6f6e 735f 3228 6e6f 6465 2c20  cations_2(node, 
-0000c570: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-0000c580: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
-0000c590: 656c 656d 656e 7473 5f66 726f 6d5f 6f70  elements_from_op
-0000c5a0: 6572 6174 696f 6e73 286c 6973 7428 7365  erations(list(se
-0000c5b0: 6c66 2e65 6c65 6d73 2829 2929 0d0a 2020  lf.elems()))..  
-0000c5c0: 2020 2020 2020 7365 6c66 2e63 6c61 7373        self.class
-0000c5d0: 6966 7928 6c69 7374 2873 656c 662e 656c  ify(list(self.el
-0000c5e0: 656d 7328 2929 290d 0a20 2020 2020 2020  ems()))..       
-0000c5f0: 2073 656c 662e 7369 676e 616c 2822 7265   self.signal("re
-0000c600: 6672 6573 685f 7472 6565 222c 206c 6973  fresh_tree", lis
-0000c610: 7428 7365 6c66 2e66 6c61 7428 7479 7065  t(self.flat(type
-0000c620: 733d 2272 6566 6572 656e 6365 2229 2929  s="reference")))
-0000c630: 0d0a 0d0a 2020 2020 4074 7265 655f 7365  ....    @tree_se
-0000c640: 7061 7261 746f 725f 6166 7465 7228 290d  parator_after().
-0000c650: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
-0000c660: 7469 6f6e 616c 286c 616d 6264 6120 6e6f  tional(lambda no
-0000c670: 6465 3a20 6e6f 7420 7365 6c66 2e63 6c61  de: not self.cla
-0000c680: 7373 6966 795f 6175 746f 6765 6e65 7261  ssify_autogenera
-0000c690: 7465 290d 0a20 2020 2040 7472 6565 5f6f  te)..    @tree_o
-0000c6a0: 7065 7261 7469 6f6e 280d 0a20 2020 2020  peration(..     
-0000c6b0: 2020 205f 2822 5265 6672 6573 6820 2e2e     _("Refresh ..
-0000c6c0: 2e20 2869 6e63 6c20 6175 746f 6765 6e65  . (incl autogene
-0000c6d0: 7261 7469 6f6e 2922 292c 0d0a 2020 2020  ration)"),..    
-0000c6e0: 2020 2020 6e6f 6465 5f74 7970 653d 2262      node_type="b
-0000c6f0: 7261 6e63 6820 6f70 7322 2c0d 0a20 2020  ranch ops",..   
-0000c700: 2020 2020 2068 656c 703d 5f28 2252 6563       help=_("Rec
-0000c710: 6c61 7373 6966 7920 656c 656d 656e 7473  lassify elements
-0000c720: 2061 6e64 2063 7265 6174 6520 6f70 6572   and create oper
-0000c730: 6174 696f 6e73 2069 6620 6e65 6365 7373  ations if necess
-0000c740: 6172 7922 292c 0d0a 2020 2020 290d 0a20  ary"),..    ).. 
-0000c750: 2020 2064 6566 2072 6566 7265 7368 5f63     def refresh_c
-0000c760: 6c61 7369 6669 6361 7469 6f6e 735f 3328  lasifications_3(
-0000c770: 6e6f 6465 2c20 2a2a 6b77 6172 6773 293a  node, **kwargs):
-0000c780: 0d0a 2020 2020 2020 2020 7072 6576 696f  ..        previo
-0000c790: 7573 203d 2073 656c 662e 636c 6173 7369  us = self.classi
-0000c7a0: 6679 5f61 7574 6f67 656e 6572 6174 650d  fy_autogenerate.
-0000c7b0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-0000c7c0: 6173 7369 6679 5f61 7574 6f67 656e 6572  assify_autogener
-0000c7d0: 6174 6520 3d20 5472 7565 0d0a 2020 2020  ate = True..    
-0000c7e0: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
-0000c7f0: 656c 656d 656e 7473 5f66 726f 6d5f 6f70  elements_from_op
-0000c800: 6572 6174 696f 6e73 286c 6973 7428 7365  erations(list(se
-0000c810: 6c66 2e65 6c65 6d73 2829 2929 0d0a 2020  lf.elems()))..  
-0000c820: 2020 2020 2020 7365 6c66 2e63 6c61 7373        self.class
-0000c830: 6966 7928 6c69 7374 2873 656c 662e 656c  ify(list(self.el
-0000c840: 656d 7328 2929 290d 0a20 2020 2020 2020  ems()))..       
-0000c850: 2073 656c 662e 636c 6173 7369 6679 5f61   self.classify_a
-0000c860: 7574 6f67 656e 6572 6174 6520 3d20 7072  utogenerate = pr
-0000c870: 6576 696f 7573 0d0a 2020 2020 2020 2020  evious..        
-0000c880: 7365 6c66 2e73 6967 6e61 6c28 2272 6566  self.signal("ref
-0000c890: 7265 7368 5f74 7265 6522 2c20 6c69 7374  resh_tree", list
-0000c8a0: 2873 656c 662e 666c 6174 2874 7970 6573  (self.flat(types
-0000c8b0: 3d22 7265 6665 7265 6e63 6522 2929 290d  ="reference"))).
-0000c8c0: 0a0d 0a20 2020 2040 7472 6565 5f63 6f6e  ...    @tree_con
-0000c8d0: 6469 7469 6f6e 616c 286c 616d 6264 6120  ditional(lambda 
-0000c8e0: 636f 6e64 3a20 7365 6c66 2e68 6176 655f  cond: self.have_
-0000c8f0: 756e 6173 7369 676e 6564 5f65 6c65 6d65  unassigned_eleme
-0000c900: 6e74 7328 2929 0d0a 2020 2020 4074 7265  nts())..    @tre
-0000c910: 655f 6f70 6572 6174 696f 6e28 0d0a 2020  e_operation(..  
-0000c920: 2020 2020 2020 5f28 2253 656c 6563 7420        _("Select 
-0000c930: 756e 6173 7369 676e 6564 2065 6c65 6d65  unassigned eleme
-0000c940: 6e74 7322 292c 0d0a 2020 2020 2020 2020  nts"),..        
-0000c950: 6e6f 6465 5f74 7970 653d 2262 7261 6e63  node_type="branc
-0000c960: 6820 6f70 7322 2c0d 0a20 2020 2020 2020  h ops",..       
-0000c970: 2068 656c 703d 5f28 2253 656c 6563 7420   help=_("Select 
-0000c980: 616c 6c20 656c 656d 656e 7473 2074 6861  all elements tha
-0000c990: 7420 776f 6e27 7420 6265 2062 7572 6e65  t won't be burne
-0000c9a0: 6422 292c 0d0a 2020 2020 290d 0a20 2020  d"),..    )..   
-0000c9b0: 2064 6566 2073 656c 6563 745f 756e 6173   def select_unas
-0000c9c0: 7369 676e 6564 286e 6f64 652c 202a 2a6b  signed(node, **k
-0000c9d0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-0000c9e0: 2063 6861 6e67 6573 203d 2046 616c 7365   changes = False
-0000c9f0: 0d0a 2020 2020 2020 2020 666f 7220 6e6f  ..        for no
-0000ca00: 6465 2069 6e20 7365 6c66 2e65 6c65 6d73  de in self.elems
-0000ca10: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
-0000ca20: 2065 6d70 6861 7369 7320 3d20 626f 6f6c   emphasis = bool
-0000ca30: 286c 656e 286e 6f64 652e 7265 6665 7265  (len(node.refere
-0000ca40: 6e63 6573 2920 3d3d 2030 290d 0a20 2020  nces) == 0)..   
-0000ca50: 2020 2020 2020 2020 2069 6620 6e6f 6465           if node
-0000ca60: 2e65 6d70 6861 7369 7a65 6420 213d 2065  .emphasized != e
-0000ca70: 6d70 6861 7369 7320 616e 6420 6e6f 6465  mphasis and node
-0000ca80: 2e63 616e 5f65 6d70 6861 7369 7a65 3a0d  .can_emphasize:.
-0000ca90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000caa0: 2063 6861 6e67 6573 203d 2054 7275 650d   changes = True.
-0000cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cac0: 206e 6f64 652e 656d 7068 6173 697a 6564   node.emphasized
-0000cad0: 203d 2065 6d70 6861 7369 730d 0a20 2020   = emphasis..   
-0000cae0: 2020 2020 2069 6620 6368 616e 6765 733a       if changes:
-0000caf0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0000cb00: 6c66 2e76 616c 6964 6174 655f 7365 6c65  lf.validate_sele
-0000cb10: 6374 6564 5f61 7265 6128 290d 0a20 2020  cted_area()..   
-0000cb20: 2020 2020 2020 2020 2073 656c 662e 7369           self.si
-0000cb30: 676e 616c 2822 7265 6672 6573 685f 7363  gnal("refresh_sc
-0000cb40: 656e 6522 2c20 2253 6365 6e65 2229 0d0a  ene", "Scene")..
-0000cb50: 0d0a 2020 2020 6d61 7465 7269 616c 7320  ..    materials 
-0000cb60: 3d20 5b0d 0a20 2020 2020 2020 205f 2822  = [..        _("
-0000cb70: 576f 6f64 2229 2c0d 0a20 2020 2020 2020  Wood"),..       
-0000cb80: 205f 2822 4163 7279 6c69 6322 292c 0d0a   _("Acrylic"),..
-0000cb90: 2020 2020 2020 2020 5f28 2246 6f61 6d22          _("Foam"
-0000cba0: 292c 0d0a 2020 2020 2020 2020 5f28 224c  ),..        _("L
-0000cbb0: 6561 7468 6572 2229 2c0d 0a20 2020 2020  eather"),..     
-0000cbc0: 2020 205f 2822 4361 7264 626f 6172 6422     _("Cardboard"
-0000cbd0: 292c 0d0a 2020 2020 2020 2020 5f28 2243  ),..        _("C
-0000cbe0: 6f72 6b22 292c 0d0a 2020 2020 2020 2020  ork"),..        
-0000cbf0: 5f28 2254 6578 7469 6c65 7322 292c 0d0a  _("Textiles"),..
-0000cc00: 2020 2020 2020 2020 5f28 2250 6170 6572          _("Paper
-0000cc10: 2229 2c0d 0a20 2020 2020 2020 205f 2822  "),..        _("
-0000cc20: 5361 7665 2d31 2229 2c0d 0a20 2020 2020  Save-1"),..     
-0000cc30: 2020 205f 2822 5361 7665 2d32 2229 2c0d     _("Save-2"),.
-0000cc40: 0a20 2020 2020 2020 205f 2822 5361 7665  .        _("Save
-0000cc50: 2d33 2229 2c0d 0a20 2020 205d 0d0a 0d0a  -3"),..    ]....
-0000cc60: 2020 2020 6465 6620 756e 696f 6e5f 6d61      def union_ma
-0000cc70: 7465 7269 616c 735f 7361 7665 6428 293a  terials_saved():
-0000cc80: 0d0a 2020 2020 2020 2020 756e 696f 6e20  ..        union 
-0000cc90: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-0000cca0: 2064 0d0a 2020 2020 2020 2020 2020 2020   d..            
-0000ccb0: 666f 7220 6420 696e 2073 656c 662e 6f70  for d in self.op
-0000ccc0: 5f64 6174 612e 7365 6374 696f 6e5f 7365  _data.section_se
-0000ccd0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-0000cce0: 2069 6620 6420 6e6f 7420 696e 206d 6174   if d not in mat
-0000ccf0: 6572 6961 6c73 2061 6e64 2064 2021 3d20  erials and d != 
-0000cd00: 2270 7265 7669 6f75 7322 0d0a 2020 2020  "previous"..    
-0000cd10: 2020 2020 5d0d 0a20 2020 2020 2020 2075      ]..        u
-0000cd20: 6e69 6f6e 2e65 7874 656e 6428 6d61 7465  nion.extend(mate
-0000cd30: 7269 616c 7329 0d0a 2020 2020 2020 2020  rials)..        
-0000cd40: 7265 7475 726e 2075 6e69 6f6e 0d0a 0d0a  return union....
-0000cd50: 2020 2020 6465 6620 6469 6666 6572 656e      def differen
-0000cd60: 6365 5f6d 6174 6572 6961 6c73 5f73 6176  ce_materials_sav
-0000cd70: 6564 2829 3a0d 0a20 2020 2020 2020 2073  ed():..        s
-0000cd80: 6563 7320 3d20 7365 6c66 2e6f 705f 6461  ecs = self.op_da
-0000cd90: 7461 2e73 6563 7469 6f6e 5f73 6574 2829  ta.section_set()
-0000cda0: 0d0a 2020 2020 2020 2020 6469 6666 6572  ..        differ
-0000cdb0: 656e 6365 203d 205b 6d20 666f 7220 6d20  ence = [m for m 
-0000cdc0: 696e 206d 6174 6572 6961 6c73 2069 6620  in materials if 
-0000cdd0: 6d20 6e6f 7420 696e 2073 6563 735d 0d0a  m not in secs]..
-0000cde0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-0000cdf0: 6966 6665 7265 6e63 650d 0a0d 0a20 2020  ifference....   
-0000ce00: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
-0000ce10: 2822 4c6f 6164 2229 290d 0a20 2020 2040  ("Load"))..    @
-0000ce20: 7472 6565 5f76 616c 7565 7328 226f 706e  tree_values("opn
-0000ce30: 616d 6522 2c20 7661 6c75 6573 3d73 656c  ame", values=sel
-0000ce40: 662e 6f70 5f64 6174 612e 7365 6374 696f  f.op_data.sectio
-0000ce50: 6e5f 7365 7429 0d0a 2020 2020 4074 7265  n_set)..    @tre
-0000ce60: 655f 6f70 6572 6174 696f 6e28 227b 6f70  e_operation("{op
-0000ce70: 6e61 6d65 7d22 2c20 6e6f 6465 5f74 7970  name}", node_typ
-0000ce80: 653d 2262 7261 6e63 6820 6f70 7322 2c20  e="branch ops", 
-0000ce90: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
-0000cea0: 6620 6c6f 6164 5f6f 7073 286e 6f64 652c  f load_ops(node,
-0000ceb0: 206f 706e 616d 652c 202a 2a6b 7761 7267   opname, **kwarg
-0000cec0: 7329 3a0d 0a20 2020 2020 2020 2073 656c  s):..        sel
-0000ced0: 6628 6622 6d61 7465 7269 616c 206c 6f61  f(f"material loa
-0000cee0: 6420 7b6f 706e 616d 657d 5c6e 2229 0d0a  d {opname}\n")..
-0000cef0: 0d0a 2020 2020 4074 7265 655f 7365 7061  ..    @tree_sepa
-0000cf00: 7261 746f 725f 6265 666f 7265 2829 0d0a  rator_before()..
-0000cf10: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-0000cf20: 7528 5f28 224c 6f61 6422 2929 0d0a 2020  u(_("Load"))..  
-0000cf30: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-0000cf40: 6e28 5f28 224f 7468 6572 2f42 6c75 652f  n(_("Other/Blue/
-0000cf50: 5265 6422 292c 206e 6f64 655f 7479 7065  Red"), node_type
-0000cf60: 3d22 6272 616e 6368 206f 7073 222c 2068  ="branch ops", h
-0000cf70: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
-0000cf80: 2064 6566 6175 6c74 5f63 6c61 7373 6966   default_classif
-0000cf90: 6963 6174 696f 6e73 286e 6f64 652c 202a  ications(node, *
-0000cfa0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-0000cfb0: 2020 2073 656c 662e 6c6f 6164 5f64 6566     self.load_def
-0000cfc0: 6175 6c74 2870 6572 666f 726d 636c 6173  ault(performclas
-0000cfd0: 7369 6679 3d54 7275 6529 0d0a 0d0a 2020  sify=True)....  
-0000cfe0: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
-0000cff0: 5f28 224c 6f61 6422 2929 0d0a 2020 2020  _("Load"))..    
-0000d000: 4074 7265 655f 7365 7061 7261 746f 725f  @tree_separator_
-0000d010: 6166 7465 7228 290d 0a20 2020 2040 7472  after()..    @tr
-0000d020: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-0000d030: 4261 7369 6322 292c 206e 6f64 655f 7479  Basic"), node_ty
-0000d040: 7065 3d22 6272 616e 6368 206f 7073 222c  pe="branch ops",
-0000d050: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-0000d060: 6566 2062 6173 6963 5f63 6c61 7373 6966  ef basic_classif
-0000d070: 6963 6174 696f 6e73 286e 6f64 652c 202a  ications(node, *
-0000d080: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-0000d090: 2020 2073 656c 662e 6c6f 6164 5f64 6566     self.load_def
-0000d0a0: 6175 6c74 3228 7065 7266 6f72 6d63 6c61  ault2(performcla
-0000d0b0: 7373 6966 793d 5472 7565 290d 0a0d 0a20  ssify=True).... 
-0000d0c0: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
-0000d0d0: 285f 2822 5361 7665 2229 290d 0a20 2020  (_("Save"))..   
-0000d0e0: 2040 7472 6565 5f76 616c 7565 7328 226f   @tree_values("o
-0000d0f0: 706e 616d 6522 2c20 7661 6c75 6573 3d73  pname", values=s
-0000d100: 656c 662e 6f70 5f64 6174 612e 7365 6374  elf.op_data.sect
-0000d110: 696f 6e5f 7365 7429 0d0a 2020 2020 4074  ion_set)..    @t
-0000d120: 7265 655f 6f70 6572 6174 696f 6e28 227b  ree_operation("{
-0000d130: 6f70 6e61 6d65 7d22 2c20 6e6f 6465 5f74  opname}", node_t
-0000d140: 7970 653d 2262 7261 6e63 6820 6f70 7322  ype="branch ops"
-0000d150: 2c20 6865 6c70 3d22 2229 0d0a 2020 2020  , help="")..    
-0000d160: 6465 6620 7361 7665 5f6d 6174 6572 6961  def save_materia
-0000d170: 6c73 286e 6f64 652c 206f 706e 616d 653d  ls(node, opname=
-0000d180: 2273 6176 6564 222c 202a 2a6b 7761 7267  "saved", **kwarg
-0000d190: 7329 3a0d 0a20 2020 2020 2020 2073 656c  s):..        sel
-0000d1a0: 6628 6622 6d61 7465 7269 616c 2073 6176  f(f"material sav
-0000d1b0: 6520 7b6f 706e 616d 657d 5c6e 2229 0d0a  e {opname}\n")..
-0000d1c0: 0d0a 2020 2020 4074 7265 655f 7365 7061  ..    @tree_sepa
-0000d1d0: 7261 746f 725f 6265 666f 7265 2829 0d0a  rator_before()..
-0000d1e0: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-0000d1f0: 7528 5f28 2253 6176 6522 2929 0d0a 2020  u(_("Save"))..  
-0000d200: 2020 4074 7265 655f 7072 6f6d 7074 2822    @tree_prompt("
-0000d210: 6f70 6e61 6d65 222c 205f 2822 4e61 6d65  opname", _("Name
-0000d220: 2074 6f20 7374 6f72 6520 6375 7272 656e   to store curren
-0000d230: 7420 6f70 6572 6174 696f 6e73 2075 6e64  t operations und
-0000d240: 6572 3f22 2929 0d0a 2020 2020 4074 7265  er?"))..    @tre
-0000d250: 655f 6f70 6572 6174 696f 6e28 5f28 224e  e_operation(_("N
-0000d260: 6577 2229 2c20 6e6f 6465 5f74 7970 653d  ew"), node_type=
-0000d270: 2262 7261 6e63 6820 6f70 7322 2c20 6865  "branch ops", he
-0000d280: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
-0000d290: 7361 7665 5f6d 6174 6572 6961 6c5f 6375  save_material_cu
-0000d2a0: 7374 6f6d 286e 6f64 652c 206f 706e 616d  stom(node, opnam
-0000d2b0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-0000d2c0: 2020 2020 2020 2073 656c 6628 6622 6d61         self(f"ma
-0000d2d0: 7465 7269 616c 2073 6176 6520 7b6f 706e  terial save {opn
-0000d2e0: 616d 652e 7265 706c 6163 6528 2720 272c  ame.replace(' ',
-0000d2f0: 2027 5f27 297d 5c6e 2229 0d0a 0d0a 2020   '_')}\n")....  
-0000d300: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
-0000d310: 5f28 2244 656c 6574 6522 2929 0d0a 2020  _("Delete"))..  
-0000d320: 2020 4074 7265 655f 7661 6c75 6573 2822    @tree_values("
-0000d330: 6f70 6e61 6d65 222c 2076 616c 7565 733d  opname", values=
-0000d340: 7365 6c66 2e6f 705f 6461 7461 2e73 6563  self.op_data.sec
-0000d350: 7469 6f6e 5f73 6574 290d 0a20 2020 2040  tion_set)..    @
-0000d360: 7472 6565 5f6f 7065 7261 7469 6f6e 2822  tree_operation("
-0000d370: 7b6f 706e 616d 657d 222c 206e 6f64 655f  {opname}", node_
-0000d380: 7479 7065 3d22 6272 616e 6368 206f 7073  type="branch ops
-0000d390: 222c 2068 656c 703d 2222 290d 0a20 2020  ", help="")..   
-0000d3a0: 2064 6566 2072 656d 6f76 655f 6f70 7328   def remove_ops(
-0000d3b0: 6e6f 6465 2c20 6f70 6e61 6d65 3d22 7361  node, opname="sa
-0000d3c0: 7665 6422 2c20 2a2a 6b77 6172 6773 293a  ved", **kwargs):
-0000d3d0: 0d0a 2020 2020 2020 2020 7365 6c66 2866  ..        self(f
-0000d3e0: 226d 6174 6572 6961 6c20 6465 6c65 7465  "material delete
-0000d3f0: 207b 6f70 6e61 6d65 7d5c 6e22 290d 0a0d   {opname}\n")...
-0000d400: 0a20 2020 2040 7472 6565 5f73 6570 6172  .    @tree_separ
-0000d410: 6174 6f72 5f62 6566 6f72 6528 290d 0a20  ator_before().. 
-0000d420: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
-0000d430: 285f 2822 4170 7065 6e64 206f 7065 7261  (_("Append opera
-0000d440: 7469 6f6e 2229 290d 0a20 2020 2040 7472  tion"))..    @tr
-0000d450: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-0000d460: 4170 7065 6e64 2049 6d61 6765 2229 2c20  Append Image"), 
-0000d470: 6e6f 6465 5f74 7970 653d 2262 7261 6e63  node_type="branc
-0000d480: 6820 6f70 7322 2c20 6865 6c70 3d22 2229  h ops", help="")
-0000d490: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
-0000d4a0: 5f6f 7065 7261 7469 6f6e 5f69 6d61 6765  _operation_image
-0000d4b0: 286e 6f64 652c 2070 6f73 3d4e 6f6e 652c  (node, pos=None,
-0000d4c0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-0000d4d0: 2020 2020 2073 656c 662e 6f70 5f62 7261       self.op_bra
-0000d4e0: 6e63 682e 6164 6428 226f 7020 696d 6167  nch.add("op imag
-0000d4f0: 6522 2c20 706f 733d 706f 7329 0d0a 2020  e", pos=pos)..  
-0000d500: 2020 2020 2020 7365 6c66 2e73 6967 6e61        self.signa
-0000d510: 6c28 2275 7064 6174 656f 705f 7472 6565  l("updateop_tree
-0000d520: 2229 0d0a 0d0a 2020 2020 4074 7265 655f  ")....    @tree_
-0000d530: 7375 626d 656e 7528 5f28 2241 7070 656e  submenu(_("Appen
-0000d540: 6420 6f70 6572 6174 696f 6e22 2929 0d0a  d operation"))..
-0000d550: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-0000d560: 696f 6e28 5f28 2241 7070 656e 6420 5261  ion(_("Append Ra
-0000d570: 7374 6572 2229 2c20 6e6f 6465 5f74 7970  ster"), node_typ
-0000d580: 653d 2262 7261 6e63 6820 6f70 7322 2c20  e="branch ops", 
-0000d590: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
-0000d5a0: 6620 6170 7065 6e64 5f6f 7065 7261 7469  f append_operati
-0000d5b0: 6f6e 5f72 6173 7465 7228 6e6f 6465 2c20  on_raster(node, 
-0000d5c0: 706f 733d 4e6f 6e65 2c20 2a2a 6b77 6172  pos=None, **kwar
-0000d5d0: 6773 293a 0d0a 2020 2020 2020 2020 7365  gs):..        se
-0000d5e0: 6c66 2e6f 705f 6272 616e 6368 2e61 6464  lf.op_branch.add
-0000d5f0: 2822 6f70 2072 6173 7465 7222 2c20 706f  ("op raster", po
-0000d600: 733d 706f 7329 0d0a 2020 2020 2020 2020  s=pos)..        
-0000d610: 7365 6c66 2e73 6967 6e61 6c28 2275 7064  self.signal("upd
-0000d620: 6174 656f 705f 7472 6565 2229 0d0a 0d0a  ateop_tree")....
-0000d630: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-0000d640: 7528 5f28 2241 7070 656e 6420 6f70 6572  u(_("Append oper
-0000d650: 6174 696f 6e22 2929 0d0a 2020 2020 4074  ation"))..    @t
-0000d660: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
-0000d670: 2241 7070 656e 6420 456e 6772 6176 6522  "Append Engrave"
-0000d680: 292c 206e 6f64 655f 7479 7065 3d22 6272  ), node_type="br
-0000d690: 616e 6368 206f 7073 222c 2068 656c 703d  anch ops", help=
-0000d6a0: 2222 290d 0a20 2020 2064 6566 2061 7070  "")..    def app
-0000d6b0: 656e 645f 6f70 6572 6174 696f 6e5f 656e  end_operation_en
-0000d6c0: 6772 6176 6528 6e6f 6465 2c20 706f 733d  grave(node, pos=
-0000d6d0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-0000d6e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-0000d6f0: 705f 6272 616e 6368 2e61 6464 2822 6f70  p_branch.add("op
-0000d700: 2065 6e67 7261 7665 222c 2070 6f73 3d70   engrave", pos=p
-0000d710: 6f73 290d 0a20 2020 2020 2020 2073 656c  os)..        sel
-0000d720: 662e 7369 676e 616c 2822 7570 6461 7465  f.signal("update
-0000d730: 6f70 5f74 7265 6522 290d 0a0d 0a20 2020  op_tree")....   
-0000d740: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
-0000d750: 2822 4170 7065 6e64 206f 7065 7261 7469  ("Append operati
-0000d760: 6f6e 2229 290d 0a20 2020 2040 7472 6565  on"))..    @tree
-0000d770: 5f6f 7065 7261 7469 6f6e 285f 2822 4170  _operation(_("Ap
-0000d780: 7065 6e64 2043 7574 2229 2c20 6e6f 6465  pend Cut"), node
-0000d790: 5f74 7970 653d 2262 7261 6e63 6820 6f70  _type="branch op
-0000d7a0: 7322 2c20 6865 6c70 3d22 2229 0d0a 2020  s", help="")..  
-0000d7b0: 2020 6465 6620 6170 7065 6e64 5f6f 7065    def append_ope
-0000d7c0: 7261 7469 6f6e 5f63 7574 286e 6f64 652c  ration_cut(node,
-0000d7d0: 2070 6f73 3d4e 6f6e 652c 202a 2a6b 7761   pos=None, **kwa
-0000d7e0: 7267 7329 3a0d 0a20 2020 2020 2020 2073  rgs):..        s
-0000d7f0: 656c 662e 6f70 5f62 7261 6e63 682e 6164  elf.op_branch.ad
-0000d800: 6428 226f 7020 6375 7422 2c20 706f 733d  d("op cut", pos=
-0000d810: 706f 7329 0d0a 2020 2020 2020 2020 7365  pos)..        se
-0000d820: 6c66 2e73 6967 6e61 6c28 2275 7064 6174  lf.signal("updat
-0000d830: 656f 705f 7472 6565 2229 0d0a 0d0a 2020  eop_tree")....  
-0000d840: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
-0000d850: 5f28 2241 7070 656e 6420 6f70 6572 6174  _("Append operat
-0000d860: 696f 6e22 2929 0d0a 2020 2020 4074 7265  ion"))..    @tre
-0000d870: 655f 6f70 6572 6174 696f 6e28 5f28 2241  e_operation(_("A
-0000d880: 7070 656e 6420 4861 7463 6822 292c 206e  ppend Hatch"), n
-0000d890: 6f64 655f 7479 7065 3d22 6272 616e 6368  ode_type="branch
-0000d8a0: 206f 7073 222c 2068 656c 703d 2222 290d   ops", help="").
-0000d8b0: 0a20 2020 2064 6566 2061 7070 656e 645f  .    def append_
-0000d8c0: 6f70 6572 6174 696f 6e5f 6861 7463 6828  operation_hatch(
-0000d8d0: 6e6f 6465 2c20 706f 733d 4e6f 6e65 2c20  node, pos=None, 
-0000d8e0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-0000d8f0: 2020 2020 7365 6c66 2e6f 705f 6272 616e      self.op_bran
-0000d900: 6368 2e61 6464 2822 6f70 2068 6174 6368  ch.add("op hatch
-0000d910: 222c 2070 6f73 3d70 6f73 290d 0a20 2020  ", pos=pos)..   
-0000d920: 2020 2020 2073 656c 662e 7369 676e 616c       self.signal
-0000d930: 2822 7570 6461 7465 6f70 5f74 7265 6522  ("updateop_tree"
-0000d940: 290d 0a0d 0a20 2020 2040 7472 6565 5f73  )....    @tree_s
-0000d950: 7562 6d65 6e75 285f 2822 4170 7065 6e64  ubmenu(_("Append
-0000d960: 206f 7065 7261 7469 6f6e 2229 290d 0a20   operation")).. 
-0000d970: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-0000d980: 6f6e 285f 2822 4170 7065 6e64 2044 6f74  on(_("Append Dot
-0000d990: 7322 292c 206e 6f64 655f 7479 7065 3d22  s"), node_type="
-0000d9a0: 6272 616e 6368 206f 7073 222c 2068 656c  branch ops", hel
-0000d9b0: 703d 2222 290d 0a20 2020 2064 6566 2061  p="")..    def a
-0000d9c0: 7070 656e 645f 6f70 6572 6174 696f 6e5f  ppend_operation_
-0000d9d0: 646f 7473 286e 6f64 652c 2070 6f73 3d4e  dots(node, pos=N
-0000d9e0: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0d  one, **kwargs):.
-0000d9f0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-0000da00: 5f62 7261 6e63 682e 6164 6428 226f 7020  _branch.add("op 
-0000da10: 646f 7473 222c 2070 6f73 3d70 6f73 290d  dots", pos=pos).
-0000da20: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-0000da30: 676e 616c 2822 7570 6461 7465 6f70 5f74  gnal("updateop_t
-0000da40: 7265 6522 290d 0a0d 0a20 2020 2040 7472  ree")....    @tr
-0000da50: 6565 5f73 7562 6d65 6e75 285f 2822 4170  ee_submenu(_("Ap
-0000da60: 7065 6e64 2073 7065 6369 616c 206f 7065  pend special ope
-0000da70: 7261 7469 6f6e 2873 2922 2929 0d0a 2020  ration(s)"))..  
-0000da80: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-0000da90: 6e28 5f28 2241 7070 656e 6420 486f 6d65  n(_("Append Home
-0000daa0: 2229 2c20 6e6f 6465 5f74 7970 653d 2262  "), node_type="b
-0000dab0: 7261 6e63 6820 6f70 7322 2c20 6865 6c70  ranch ops", help
-0000dac0: 3d22 2229 0d0a 2020 2020 6465 6620 6170  ="")..    def ap
-0000dad0: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f68  pend_operation_h
-0000dae0: 6f6d 6528 6e6f 6465 2c20 706f 733d 4e6f  ome(node, pos=No
-0000daf0: 6e65 2c20 2a2a 6b77 6172 6773 293a 0d0a  ne, **kwargs):..
-0000db00: 2020 2020 2020 2020 7365 6c66 2e6f 705f          self.op_
-0000db10: 6272 616e 6368 2e61 6464 2874 7970 653d  branch.add(type=
-0000db20: 2275 7469 6c20 686f 6d65 222c 2070 6f73  "util home", pos
-0000db30: 3d70 6f73 290d 0a20 2020 2020 2020 2073  =pos)..        s
-0000db40: 656c 662e 7369 676e 616c 2822 7570 6461  elf.signal("upda
-0000db50: 7465 6f70 5f74 7265 6522 290d 0a0d 0a20  teop_tree").... 
-0000db60: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
-0000db70: 285f 2822 4170 7065 6e64 2073 7065 6369  (_("Append speci
-0000db80: 616c 206f 7065 7261 7469 6f6e 2873 2922  al operation(s)"
-0000db90: 2929 0d0a 2020 2020 4074 7265 655f 6f70  ))..    @tree_op
-0000dba0: 6572 6174 696f 6e28 5f28 2241 7070 656e  eration(_("Appen
-0000dbb0: 6420 5265 7475 726e 2074 6f20 4f72 6967  d Return to Orig
-0000dbc0: 696e 2229 2c20 6e6f 6465 5f74 7970 653d  in"), node_type=
-0000dbd0: 2262 7261 6e63 6820 6f70 7322 2c20 6865  "branch ops", he
-0000dbe0: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
-0000dbf0: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
-0000dc00: 5f67 6f74 6f28 6e6f 6465 2c20 706f 733d  _goto(node, pos=
-0000dc10: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-0000dc20: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-0000dc30: 705f 6272 616e 6368 2e61 6464 2874 7970  p_branch.add(typ
-0000dc40: 653d 2275 7469 6c20 676f 746f 222c 2070  e="util goto", p
-0000dc50: 6f73 3d70 6f73 2c20 783d 302c 2079 3d30  os=pos, x=0, y=0
-0000dc60: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000dc70: 7369 676e 616c 2822 7570 6461 7465 6f70  signal("updateop
-0000dc80: 5f74 7265 6522 290d 0a0d 0a20 2020 2040  _tree")....    @
-0000dc90: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
-0000dca0: 4170 7065 6e64 2073 7065 6369 616c 206f  Append special o
-0000dcb0: 7065 7261 7469 6f6e 2873 2922 2929 0d0a  peration(s)"))..
-0000dcc0: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-0000dcd0: 696f 6e28 5f28 2241 7070 656e 6420 4265  ion(_("Append Be
-0000dce0: 6570 2229 2c20 6e6f 6465 5f74 7970 653d  ep"), node_type=
-0000dcf0: 2262 7261 6e63 6820 6f70 7322 2c20 6865  "branch ops", he
-0000dd00: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
-0000dd10: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
-0000dd20: 5f62 6565 7028 6e6f 6465 2c20 706f 733d  _beep(node, pos=
-0000dd30: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-0000dd40: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-0000dd50: 705f 6272 616e 6368 2e61 6464 280d 0a20  p_branch.add(.. 
-0000dd60: 2020 2020 2020 2020 2020 2074 7970 653d             type=
-0000dd70: 2275 7469 6c20 636f 6e73 6f6c 6522 2c0d  "util console",.
-0000dd80: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
-0000dd90: 3d70 6f73 2c0d 0a20 2020 2020 2020 2020  =pos,..         
-0000dda0: 2020 2063 6f6d 6d61 6e64 3d22 6265 6570     command="beep
-0000ddb0: 222c 0d0a 2020 2020 2020 2020 290d 0a20  ",..        ).. 
-0000ddc0: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
-0000ddd0: 616c 2822 7570 6461 7465 6f70 5f74 7265  al("updateop_tre
-0000dde0: 6522 290d 0a0d 0a20 2020 2040 7472 6565  e")....    @tree
-0000ddf0: 5f73 7562 6d65 6e75 285f 2822 4170 7065  _submenu(_("Appe
-0000de00: 6e64 2073 7065 6369 616c 206f 7065 7261  nd special opera
-0000de10: 7469 6f6e 2873 2922 2929 0d0a 2020 2020  tion(s)"))..    
-0000de20: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
-0000de30: 5f28 2241 7070 656e 6420 496e 7465 7272  _("Append Interr
-0000de40: 7570 7422 292c 206e 6f64 655f 7479 7065  upt"), node_type
-0000de50: 3d22 6272 616e 6368 206f 7073 222c 2068  ="branch ops", h
-0000de60: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
-0000de70: 2061 7070 656e 645f 6f70 6572 6174 696f   append_operatio
-0000de80: 6e5f 696e 7465 7272 7570 7428 6e6f 6465  n_interrupt(node
-0000de90: 2c20 706f 733d 4e6f 6e65 2c20 2a2a 6b77  , pos=None, **kw
-0000dea0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-0000deb0: 7365 6c66 2e6f 705f 6272 616e 6368 2e61  self.op_branch.a
-0000dec0: 6464 280d 0a20 2020 2020 2020 2020 2020  dd(..           
-0000ded0: 2074 7970 653d 2275 7469 6c20 636f 6e73   type="util cons
-0000dee0: 6f6c 6522 2c0d 0a20 2020 2020 2020 2020  ole",..         
-0000def0: 2020 2070 6f73 3d70 6f73 2c0d 0a20 2020     pos=pos,..   
-0000df00: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
-0000df10: 3d27 696e 7465 7272 7570 7420 2253 706f  ='interrupt "Spo
-0000df20: 6f6c 696e 6720 7761 7320 696e 7465 7272  oling was interr
-0000df30: 7570 7465 6422 272c 0d0a 2020 2020 2020  upted"',..      
-0000df40: 2020 290d 0a20 2020 2020 2020 2073 656c    )..        sel
-0000df50: 662e 7369 676e 616c 2822 7570 6461 7465  f.signal("update
-0000df60: 6f70 5f74 7265 6522 290d 0a0d 0a20 2020  op_tree")....   
-0000df70: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
-0000df80: 2822 4170 7065 6e64 2073 7065 6369 616c  ("Append special
-0000df90: 206f 7065 7261 7469 6f6e 2873 2922 2929   operation(s)"))
-0000dfa0: 0d0a 2020 2020 4074 7265 655f 7072 6f6d  ..    @tree_prom
-0000dfb0: 7074 2822 7761 6974 5f74 696d 6522 2c20  pt("wait_time", 
-0000dfc0: 5f28 2257 6169 7420 666f 7220 686f 7720  _("Wait for how 
-0000dfd0: 6c6f 6e67 2028 696e 2073 6563 6f6e 6473  long (in seconds
-0000dfe0: 293f 2229 2c20 6461 7461 5f74 7970 653d  )?"), data_type=
-0000dff0: 666c 6f61 7429 0d0a 2020 2020 4074 7265  float)..    @tre
-0000e000: 655f 6f70 6572 6174 696f 6e28 5f28 2241  e_operation(_("A
-0000e010: 7070 656e 6420 5761 6974 2229 2c20 6e6f  ppend Wait"), no
-0000e020: 6465 5f74 7970 653d 2262 7261 6e63 6820  de_type="branch 
-0000e030: 6f70 7322 2c20 6865 6c70 3d22 2229 0d0a  ops", help="")..
-0000e040: 2020 2020 6465 6620 6170 7065 6e64 5f6f      def append_o
-0000e050: 7065 7261 7469 6f6e 5f77 6169 7428 6e6f  peration_wait(no
-0000e060: 6465 2c20 7761 6974 5f74 696d 652c 2070  de, wait_time, p
-0000e070: 6f73 3d4e 6f6e 652c 202a 2a6b 7761 7267  os=None, **kwarg
-0000e080: 7329 3a0d 0a20 2020 2020 2020 2073 656c  s):..        sel
-0000e090: 662e 6f70 5f62 7261 6e63 682e 6164 6428  f.op_branch.add(
-0000e0a0: 0d0a 2020 2020 2020 2020 2020 2020 7479  ..            ty
-0000e0b0: 7065 3d22 7574 696c 2077 6169 7422 2c0d  pe="util wait",.
-0000e0c0: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
-0000e0d0: 3d70 6f73 2c0d 0a20 2020 2020 2020 2020  =pos,..         
-0000e0e0: 2020 2077 6169 743d 7761 6974 5f74 696d     wait=wait_tim
-0000e0f0: 652c 0d0a 2020 2020 2020 2020 290d 0a20  e,..        ).. 
-0000e100: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
-0000e110: 616c 2822 7570 6461 7465 6f70 5f74 7265  al("updateop_tre
-0000e120: 6522 290d 0a0d 0a20 2020 2040 7472 6565  e")....    @tree
-0000e130: 5f73 7562 6d65 6e75 285f 2822 4170 7065  _submenu(_("Appe
-0000e140: 6e64 2073 7065 6369 616c 206f 7065 7261  nd special opera
-0000e150: 7469 6f6e 2873 2922 2929 0d0a 2020 2020  tion(s)"))..    
-0000e160: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
-0000e170: 5f28 2241 7070 656e 6420 4f75 7470 7574  _("Append Output
-0000e180: 2229 2c20 6e6f 6465 5f74 7970 653d 2262  "), node_type="b
-0000e190: 7261 6e63 6820 6f70 7322 2c20 6865 6c70  ranch ops", help
-0000e1a0: 3d22 2229 0d0a 2020 2020 6465 6620 6170  ="")..    def ap
-0000e1b0: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f6f  pend_operation_o
-0000e1c0: 7574 7075 7428 6e6f 6465 2c20 706f 733d  utput(node, pos=
-0000e1d0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-0000e1e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
-0000e1f0: 705f 6272 616e 6368 2e61 6464 280d 0a20  p_branch.add(.. 
-0000e200: 2020 2020 2020 2020 2020 2074 7970 653d             type=
-0000e210: 2275 7469 6c20 6f75 7470 7574 222c 0d0a  "util output",..
-0000e220: 2020 2020 2020 2020 2020 2020 706f 733d              pos=
-0000e230: 706f 732c 0d0a 2020 2020 2020 2020 2020  pos,..          
-0000e240: 2020 6f75 7470 7574 5f6d 6173 6b3d 302c    output_mask=0,
-0000e250: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
-0000e260: 7470 7574 5f76 616c 7565 3d30 2c0d 0a20  tput_value=0,.. 
-0000e270: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-0000e280: 745f 6d65 7373 6167 653d 4e6f 6e65 2c0d  t_message=None,.
-0000e290: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-0000e2a0: 2020 2020 7365 6c66 2e73 6967 6e61 6c28      self.signal(
-0000e2b0: 2275 7064 6174 656f 705f 7472 6565 2229  "updateop_tree")
-0000e2c0: 0d0a 0d0a 2020 2020 4074 7265 655f 7375  ....    @tree_su
-0000e2d0: 626d 656e 7528 5f28 2241 7070 656e 6420  bmenu(_("Append 
-0000e2e0: 7370 6563 6961 6c20 6f70 6572 6174 696f  special operatio
-0000e2f0: 6e28 7329 2229 290d 0a20 2020 2040 7472  n(s)"))..    @tr
-0000e300: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-0000e310: 4170 7065 6e64 2049 6e70 7574 2229 2c20  Append Input"), 
-0000e320: 6e6f 6465 5f74 7970 653d 2262 7261 6e63  node_type="branc
-0000e330: 6820 6f70 7322 2c20 6865 6c70 3d22 2229  h ops", help="")
-0000e340: 0d0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
-0000e350: 5f6f 7065 7261 7469 6f6e 5f69 6e70 7574  _operation_input
-0000e360: 286e 6f64 652c 2070 6f73 3d4e 6f6e 652c  (node, pos=None,
-0000e370: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-0000e380: 2020 2020 2073 656c 662e 6f70 5f62 7261       self.op_bra
-0000e390: 6e63 682e 6164 6428 0d0a 2020 2020 2020  nch.add(..      
-0000e3a0: 2020 2020 2020 7479 7065 3d22 7574 696c        type="util
-0000e3b0: 2069 6e70 7574 222c 0d0a 2020 2020 2020   input",..      
-0000e3c0: 2020 2020 2020 706f 733d 706f 732c 0d0a        pos=pos,..
-0000e3d0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-0000e3e0: 745f 6d61 736b 3d30 2c0d 0a20 2020 2020  t_mask=0,..     
-0000e3f0: 2020 2020 2020 2069 6e70 7574 5f76 616c         input_val
-0000e400: 7565 3d30 2c0d 0a20 2020 2020 2020 2020  ue=0,..         
-0000e410: 2020 2069 6e70 7574 5f6d 6573 7361 6765     input_message
-0000e420: 3d4e 6f6e 652c 0d0a 2020 2020 2020 2020  =None,..        
-0000e430: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000e440: 7369 676e 616c 2822 7570 6461 7465 6f70  signal("updateop
-0000e450: 5f74 7265 6522 290d 0a0d 0a20 2020 2040  _tree")....    @
-0000e460: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
-0000e470: 4170 7065 6e64 2073 7065 6369 616c 206f  Append special o
-0000e480: 7065 7261 7469 6f6e 2873 2922 2929 0d0a  peration(s)"))..
-0000e490: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-0000e4a0: 696f 6e28 5f28 2241 7070 656e 6420 486f  ion(_("Append Ho
-0000e4b0: 6d65 2f42 6565 702f 496e 7465 7272 7570  me/Beep/Interrup
-0000e4c0: 7422 292c 206e 6f64 655f 7479 7065 3d22  t"), node_type="
-0000e4d0: 6272 616e 6368 206f 7073 222c 2068 656c  branch ops", hel
-0000e4e0: 703d 2222 290d 0a20 2020 2064 6566 2061  p="")..    def a
-0000e4f0: 7070 656e 645f 6f70 6572 6174 696f 6e5f  ppend_operation_
-0000e500: 686f 6d65 5f62 6565 705f 696e 7465 7272  home_beep_interr
-0000e510: 7570 7428 6e6f 6465 2c20 2a2a 6b77 6172  upt(node, **kwar
-0000e520: 6773 293a 0d0a 2020 2020 2020 2020 6170  gs):..        ap
-0000e530: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f68  pend_operation_h
-0000e540: 6f6d 6528 6e6f 6465 2c20 2a2a 6b77 6172  ome(node, **kwar
-0000e550: 6773 290d 0a20 2020 2020 2020 2061 7070  gs)..        app
-0000e560: 656e 645f 6f70 6572 6174 696f 6e5f 6265  end_operation_be
-0000e570: 6570 286e 6f64 652c 202a 2a6b 7761 7267  ep(node, **kwarg
-0000e580: 7329 0d0a 2020 2020 2020 2020 6170 7065  s)..        appe
-0000e590: 6e64 5f6f 7065 7261 7469 6f6e 5f69 6e74  nd_operation_int
-0000e5a0: 6572 7275 7074 286e 6f64 652c 202a 2a6b  errupt(node, **k
-0000e5b0: 7761 7267 7329 0d0a 2020 2020 2020 2020  wargs)..        
-0000e5c0: 7365 6c66 2e73 6967 6e61 6c28 2275 7064  self.signal("upd
-0000e5d0: 6174 656f 705f 7472 6565 2229 0d0a 0d0a  ateop_tree")....
-0000e5e0: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-0000e5f0: 7528 5f28 2241 7070 656e 6420 7370 6563  u(_("Append spec
-0000e600: 6961 6c20 6f70 6572 6174 696f 6e28 7329  ial operation(s)
-0000e610: 2229 290d 0a20 2020 2040 7472 6565 5f6f  "))..    @tree_o
-0000e620: 7065 7261 7469 6f6e 285f 2822 4170 7065  peration(_("Appe
-0000e630: 6e64 204f 7269 6769 6e2f 4265 6570 2f49  nd Origin/Beep/I
-0000e640: 6e74 6572 7275 7074 2229 2c20 6e6f 6465  nterrupt"), node
-0000e650: 5f74 7970 653d 2262 7261 6e63 6820 6f70  _type="branch op
-0000e660: 7322 2c20 6865 6c70 3d22 2229 0d0a 2020  s", help="")..  
-0000e670: 2020 6465 6620 6170 7065 6e64 5f6f 7065    def append_ope
-0000e680: 7261 7469 6f6e 5f6f 7269 6769 6e5f 6265  ration_origin_be
-0000e690: 6570 5f69 6e74 6572 7275 7074 286e 6f64  ep_interrupt(nod
-0000e6a0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-0000e6b0: 2020 2020 2020 2061 7070 656e 645f 6f70         append_op
-0000e6c0: 6572 6174 696f 6e5f 676f 746f 286e 6f64  eration_goto(nod
-0000e6d0: 652c 202a 2a6b 7761 7267 7329 0d0a 2020  e, **kwargs)..  
-0000e6e0: 2020 2020 2020 6170 7065 6e64 5f6f 7065        append_ope
-0000e6f0: 7261 7469 6f6e 5f62 6565 7028 6e6f 6465  ration_beep(node
-0000e700: 2c20 2a2a 6b77 6172 6773 290d 0a20 2020  , **kwargs)..   
-0000e710: 2020 2020 2061 7070 656e 645f 6f70 6572       append_oper
-0000e720: 6174 696f 6e5f 696e 7465 7272 7570 7428  ation_interrupt(
-0000e730: 6e6f 6465 2c20 2a2a 6b77 6172 6773 290d  node, **kwargs).
-0000e740: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-0000e750: 676e 616c 2822 7570 6461 7465 6f70 5f74  gnal("updateop_t
-0000e760: 7265 6522 290d 0a0d 0a20 2020 2040 7472  ree")....    @tr
-0000e770: 6565 5f73 7562 6d65 6e75 285f 2822 4170  ee_submenu(_("Ap
-0000e780: 7065 6e64 2073 7065 6369 616c 206f 7065  pend special ope
-0000e790: 7261 7469 6f6e 2873 2922 2929 0d0a 2020  ration(s)"))..  
-0000e7a0: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-0000e7b0: 6e28 5f28 2241 7070 656e 6420 5368 7574  n(_("Append Shut
-0000e7c0: 646f 776e 2229 2c20 6e6f 6465 5f74 7970  down"), node_typ
-0000e7d0: 653d 2262 7261 6e63 6820 6f70 7322 2c20  e="branch ops", 
-0000e7e0: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
-0000e7f0: 6620 6170 7065 6e64 5f6f 7065 7261 7469  f append_operati
-0000e800: 6f6e 5f73 6875 7464 6f77 6e28 6e6f 6465  on_shutdown(node
-0000e810: 2c20 706f 733d 4e6f 6e65 2c20 2a2a 6b77  , pos=None, **kw
-0000e820: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-0000e830: 7365 6c66 2e6f 705f 6272 616e 6368 2e61  self.op_branch.a
-0000e840: 6464 280d 0a20 2020 2020 2020 2020 2020  dd(..           
-0000e850: 2074 7970 653d 2275 7469 6c20 636f 6e73   type="util cons
-0000e860: 6f6c 6522 2c0d 0a20 2020 2020 2020 2020  ole",..         
-0000e870: 2020 2070 6f73 3d70 6f73 2c0d 0a20 2020     pos=pos,..   
-0000e880: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
-0000e890: 3d22 7175 6974 222c 0d0a 2020 2020 2020  ="quit",..      
-0000e8a0: 2020 290d 0a20 2020 2020 2020 2073 656c    )..        sel
-0000e8b0: 662e 7369 676e 616c 2822 7570 6461 7465  f.signal("update
-0000e8c0: 6f70 5f74 7265 6522 290d 0a0d 0a20 2020  op_tree")....   
-0000e8d0: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
-0000e8e0: 2822 4170 7065 6e64 2073 7065 6369 616c  ("Append special
-0000e8f0: 206f 7065 7261 7469 6f6e 2873 2922 2929   operation(s)"))
-0000e900: 0d0a 2020 2020 4074 7265 655f 7072 6f6d  ..    @tree_prom
-0000e910: 7074 2822 6f70 6e61 6d65 222c 205f 2822  pt("opname", _("
-0000e920: 436f 6e73 6f6c 6520 636f 6d6d 616e 6420  Console command 
-0000e930: 746f 2061 7070 656e 6420 746f 206f 7065  to append to ope
-0000e940: 7261 7469 6f6e 733f 2229 290d 0a20 2020  rations?"))..   
-0000e950: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
-0000e960: 285f 2822 4170 7065 6e64 2043 6f6e 736f  (_("Append Conso
-0000e970: 6c65 2229 2c20 6e6f 6465 5f74 7970 653d  le"), node_type=
-0000e980: 2262 7261 6e63 6820 6f70 7322 2c20 6865  "branch ops", he
-0000e990: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
-0000e9a0: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
-0000e9b0: 5f63 7573 746f 6d28 6e6f 6465 2c20 6f70  _custom(node, op
-0000e9c0: 6e61 6d65 2c20 706f 733d 4e6f 6e65 2c20  name, pos=None, 
-0000e9d0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-0000e9e0: 2020 2020 7365 6c66 2e6f 705f 6272 616e      self.op_bran
-0000e9f0: 6368 2e61 6464 280d 0a20 2020 2020 2020  ch.add(..       
-0000ea00: 2020 2020 2074 7970 653d 2275 7469 6c20       type="util 
-0000ea10: 636f 6e73 6f6c 6522 2c0d 0a20 2020 2020  console",..     
-0000ea20: 2020 2020 2020 2070 6f73 3d70 6f73 2c0d         pos=pos,.
-0000ea30: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
-0000ea40: 6d61 6e64 3d6f 706e 616d 652c 0d0a 2020  mand=opname,..  
-0000ea50: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0000ea60: 2073 656c 662e 7369 676e 616c 2822 7570   self.signal("up
-0000ea70: 6461 7465 6f70 5f74 7265 6522 290d 0a0d  dateop_tree")...
-0000ea80: 0a20 2020 2040 7472 6565 5f73 7562 6d65  .    @tree_subme
-0000ea90: 6e75 285f 2822 4170 7065 6e64 2073 7065  nu(_("Append spe
-0000eaa0: 6369 616c 206f 7065 7261 7469 6f6e 2873  cial operation(s
-0000eab0: 2922 2929 0d0a 2020 2020 4074 7265 655f  )"))..    @tree_
-0000eac0: 7072 6f6d 7074 2822 7922 2c20 5f28 2259  prompt("y", _("Y
-0000ead0: 2d43 6f6f 7264 696e 6174 6520 666f 7220  -Coordinate for 
-0000eae0: 706c 6163 656d 656e 7420 746f 2061 7070  placement to app
-0000eaf0: 656e 643f 2229 290d 0a20 2020 2040 7472  end?"))..    @tr
-0000eb00: 6565 5f70 726f 6d70 7428 2278 222c 205f  ee_prompt("x", _
-0000eb10: 2822 582d 436f 6f72 6469 6e61 7465 2066  ("X-Coordinate f
-0000eb20: 6f72 2070 6c61 6365 6d65 6e74 2074 6f20  or placement to 
-0000eb30: 6170 7065 6e64 3f22 2929 0d0a 2020 2020  append?"))..    
-0000eb40: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
-0000eb50: 5f28 2241 7070 656e 6420 506c 6163 656d  _("Append Placem
-0000eb60: 656e 7422 292c 206e 6f64 655f 7479 7065  ent"), node_type
-0000eb70: 3d22 6272 616e 6368 206f 7073 222c 2068  ="branch ops", h
-0000eb80: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
-0000eb90: 2061 7070 656e 645f 6f70 6572 6174 696f   append_operatio
-0000eba0: 6e5f 706c 6163 656d 656e 7428 6e6f 6465  n_placement(node
-0000ebb0: 2c20 792c 2078 2c20 706f 733d 4e6f 6e65  , y, x, pos=None
-0000ebc0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
-0000ebd0: 2020 2020 2020 7365 6c66 2e6f 705f 6272        self.op_br
-0000ebe0: 616e 6368 2e61 6464 280d 0a20 2020 2020  anch.add(..     
-0000ebf0: 2020 2020 2020 2074 7970 653d 2270 6c61         type="pla
-0000ec00: 6365 2070 6f69 6e74 222c 0d0a 2020 2020  ce point",..    
-0000ec10: 2020 2020 2020 2020 706f 733d 706f 732c          pos=pos,
-0000ec20: 0d0a 2020 2020 2020 2020 2020 2020 783d  ..            x=
-0000ec30: 782c 0d0a 2020 2020 2020 2020 2020 2020  x,..            
-0000ec40: 793d 792c 0d0a 2020 2020 2020 2020 2020  y=y,..          
-0000ec50: 2020 726f 7461 7469 6f6e 3d30 2c0d 0a20    rotation=0,.. 
-0000ec60: 2020 2020 2020 2020 2020 2063 6f72 6e65             corne
-0000ec70: 723d 302c 0d0a 2020 2020 2020 2020 290d  r=0,..        ).
-0000ec80: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-0000ec90: 676e 616c 2822 7570 6461 7465 6f70 5f74  gnal("updateop_t
-0000eca0: 7265 6522 290d 0a0d 0a20 2020 2040 7472  ree")....    @tr
-0000ecb0: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-0000ecc0: 5265 636c 6173 7369 6679 206f 7065 7261  Reclassify opera
-0000ecd0: 7469 6f6e 7322 292c 206e 6f64 655f 7479  tions"), node_ty
-0000ece0: 7065 3d22 6272 616e 6368 2065 6c65 6d73  pe="branch elems
-0000ecf0: 222c 2068 656c 703d 2222 290d 0a20 2020  ", help="")..   
-0000ed00: 2064 6566 2072 6563 6c61 7373 6966 795f   def reclassify_
-0000ed10: 6f70 6572 6174 696f 6e73 286e 6f64 652c  operations(node,
-0000ed20: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-0000ed30: 2020 2020 2065 6c65 6d73 203d 206c 6973       elems = lis
-0000ed40: 7428 7365 6c66 2e65 6c65 6d73 2829 290d  t(self.elems()).
-0000ed50: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0000ed60: 6d6f 7665 5f65 6c65 6d65 6e74 735f 6672  move_elements_fr
-0000ed70: 6f6d 5f6f 7065 7261 7469 6f6e 7328 656c  om_operations(el
-0000ed80: 656d 7329 0d0a 2020 2020 2020 2020 7365  ems)..        se
-0000ed90: 6c66 2e63 6c61 7373 6966 7928 6c69 7374  lf.classify(list
-0000eda0: 2873 656c 662e 656c 656d 7328 2929 290d  (self.elems())).
-0000edb0: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-0000edc0: 676e 616c 2822 7265 6672 6573 685f 7472  gnal("refresh_tr
-0000edd0: 6565 2229 0d0a 0d0a 2020 2020 4074 7265  ee")....    @tre
-0000ede0: 655f 6f70 6572 6174 696f 6e28 0d0a 2020  e_operation(..  
-0000edf0: 2020 2020 2020 5f28 2252 656d 6f76 6520        _("Remove 
-0000ee00: 616c 6c20 6173 7369 676e 6d65 6e74 7320  all assignments 
-0000ee10: 6672 6f6d 206f 7065 7261 7469 6f6e 7322  from operations"
-0000ee20: 292c 0d0a 2020 2020 2020 2020 6e6f 6465  ),..        node
-0000ee30: 5f74 7970 653d 2262 7261 6e63 6820 656c  _type="branch el
-0000ee40: 656d 7322 2c0d 0a20 2020 2020 2020 2068  ems",..        h
-0000ee50: 656c 703d 5f28 2241 6e79 2065 7869 7374  elp=_("Any exist
-0000ee60: 696e 6720 6173 7369 676e 6d65 6e74 206f  ing assignment o
-0000ee70: 6620 656c 656d 656e 7473 2074 6f20 6f70  f elements to op
-0000ee80: 6572 6174 696f 6e73 2077 696c 6c20 6265  erations will be
-0000ee90: 2072 656d 6f76 6564 2229 2c0d 0a20 2020   removed"),..   
-0000eea0: 2029 0d0a 2020 2020 6465 6620 7265 6d6f   )..    def remo
-0000eeb0: 7665 5f61 6c6c 5f61 7373 6967 6e6d 656e  ve_all_assignmen
-0000eec0: 7473 286e 6f64 652c 202a 2a6b 7761 7267  ts(node, **kwarg
-0000eed0: 7329 3a0d 0a20 2020 2020 2020 2077 6974  s):..        wit
-0000eee0: 6820 7365 6c66 2e73 7461 7469 6328 2272  h self.static("r
-0000eef0: 656d 6f76 655f 616c 6c5f 6173 7369 676e  emove_all_assign
-0000ef00: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-0000ef10: 2066 6f72 206e 6f64 6520 696e 2073 656c   for node in sel
-0000ef20: 662e 656c 656d 7328 293a 0d0a 2020 2020  f.elems():..    
-0000ef30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000ef40: 7265 6620 696e 206c 6973 7428 6e6f 6465  ref in list(node
-0000ef50: 2e72 6566 6572 656e 6365 7329 3a0d 0a20  .references):.. 
+0000bfa0: 2073 6e6f 6465 2e70 6172 656e 742e 6164   snode.parent.ad
+0000bfb0: 645f 7265 6665 7265 6e63 6528 736e 6f64  d_reference(snod
+0000bfc0: 652e 6e6f 6465 2c20 706f 733d 696e 6465  e.node, pos=inde
+0000bfd0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+0000bfe0: 2020 2020 736e 6f64 652e 6d6f 6469 6669      snode.modifi
+0000bff0: 6564 2829 0d0a 0d0a 2020 2020 4074 7265  ed()....    @tre
+0000c000: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
+0000c010: 6d62 6461 206e 6f64 653a 206e 6f64 652e  mbda node: node.
+0000c020: 636f 756e 745f 6368 696c 6472 656e 2829  count_children()
+0000c030: 203e 2031 290d 0a20 2020 2040 7472 6565   > 1)..    @tree
+0000c040: 5f6f 7065 7261 7469 6f6e 280d 0a20 2020  _operation(..   
+0000c050: 2020 2020 205f 2822 5265 7665 7273 6520       _("Reverse 
+0000c060: 7375 6269 7465 6d73 206f 7264 6572 2229  subitems order")
+0000c070: 2c0d 0a20 2020 2020 2020 206e 6f64 655f  ,..        node_
+0000c080: 7479 7065 3d28 0d0a 2020 2020 2020 2020  type=(..        
+0000c090: 2020 2020 226f 7020 6375 7422 2c0d 0a20      "op cut",.. 
+0000c0a0: 2020 2020 2020 2020 2020 2022 6f70 2072             "op r
+0000c0b0: 6173 7465 7222 2c0d 0a20 2020 2020 2020  aster",..       
+0000c0c0: 2020 2020 2022 6f70 2069 6d61 6765 222c       "op image",
+0000c0d0: 0d0a 2020 2020 2020 2020 2020 2020 226f  ..            "o
+0000c0e0: 7020 656e 6772 6176 6522 2c0d 0a20 2020  p engrave",..   
+0000c0f0: 2020 2020 2020 2020 2022 6f70 2064 6f74           "op dot
+0000c100: 7322 2c0d 0a20 2020 2020 2020 2020 2020  s",..           
+0000c110: 2022 6f70 2068 6174 6368 222c 0d0a 2020   "op hatch",..  
+0000c120: 2020 2020 2020 2020 2020 2267 726f 7570            "group
+0000c130: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+0000c140: 2262 7261 6e63 6820 656c 656d 7322 2c0d  "branch elems",.
+0000c150: 0a20 2020 2020 2020 2020 2020 2022 6669  .            "fi
+0000c160: 6c65 222c 0d0a 2020 2020 2020 2020 2020  le",..          
+0000c170: 2020 2262 7261 6e63 6820 6f70 7322 2c0d    "branch ops",.
+0000c180: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
+0000c190: 2020 2020 2068 656c 703d 5f28 2252 6576       help=_("Rev
+0000c1a0: 6572 7365 2074 6865 2069 7465 6d73 2077  erse the items w
+0000c1b0: 6974 6869 6e20 7468 6973 2073 7562 6974  ithin this subit
+0000c1c0: 656d 2229 2c0d 0a20 2020 2029 0d0a 2020  em"),..    )..  
+0000c1d0: 2020 6465 6620 7265 7665 7273 655f 6c61    def reverse_la
+0000c1e0: 7965 725f 6f72 6465 7228 6e6f 6465 2c20  yer_order(node, 
+0000c1f0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+0000c200: 2020 2020 6e6f 6465 2e72 6576 6572 7365      node.reverse
+0000c210: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0000c220: 2e73 6967 6e61 6c28 2272 6566 7265 7368  .signal("refresh
+0000c230: 5f74 7265 6522 2c20 6c69 7374 2873 656c  _tree", list(sel
+0000c240: 662e 666c 6174 2874 7970 6573 3d22 7265  f.flat(types="re
+0000c250: 6665 7265 6e63 6522 2929 290d 0a0d 0a20  ference"))).... 
+0000c260: 2020 2040 7472 6565 5f73 6570 6172 6174     @tree_separat
+0000c270: 6f72 5f61 6674 6572 2829 0d0a 2020 2020  or_after()..    
+0000c280: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
+0000c290: 6c28 6c61 6d62 6461 206e 6f64 653a 2073  l(lambda node: s
+0000c2a0: 656c 662e 636c 6173 7369 6679 5f61 7574  elf.classify_aut
+0000c2b0: 6f67 656e 6572 6174 6529 0d0a 2020 2020  ogenerate)..    
+0000c2c0: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+0000c2d0: 0d0a 2020 2020 2020 2020 5f28 2252 6566  ..        _("Ref
+0000c2e0: 7265 7368 2063 6c61 7373 6966 6963 6174  resh classificat
+0000c2f0: 696f 6e22 292c 0d0a 2020 2020 2020 2020  ion"),..        
+0000c300: 6e6f 6465 5f74 7970 653d 2262 7261 6e63  node_type="branc
+0000c310: 6820 6f70 7322 2c0d 0a20 2020 2020 2020  h ops",..       
+0000c320: 2068 656c 703d 5f28 2252 6563 6c61 7373   help=_("Reclass
+0000c330: 6966 7920 656c 656d 656e 7473 2061 6e64  ify elements and
+0000c340: 2063 7265 6174 6520 6f70 6572 6174 696f   create operatio
+0000c350: 6e73 2069 6620 6e65 6365 7373 6172 7922  ns if necessary"
+0000c360: 292c 0d0a 2020 2020 290d 0a20 2020 2064  ),..    )..    d
+0000c370: 6566 2072 6566 7265 7368 5f63 6c61 7369  ef refresh_clasi
+0000c380: 6669 6361 7469 6f6e 735f 3128 6e6f 6465  fications_1(node
+0000c390: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+0000c3a0: 2020 2020 2020 7365 6c66 2e72 656d 6f76        self.remov
+0000c3b0: 655f 656c 656d 656e 7473 5f66 726f 6d5f  e_elements_from_
+0000c3c0: 6f70 6572 6174 696f 6e73 286c 6973 7428  operations(list(
+0000c3d0: 7365 6c66 2e65 6c65 6d73 2829 2929 0d0a  self.elems()))..
+0000c3e0: 2020 2020 2020 2020 7365 6c66 2e63 6c61          self.cla
+0000c3f0: 7373 6966 7928 6c69 7374 2873 656c 662e  ssify(list(self.
+0000c400: 656c 656d 7328 2929 290d 0a20 2020 2020  elems()))..     
+0000c410: 2020 2073 656c 662e 7369 676e 616c 2822     self.signal("
+0000c420: 7265 6672 6573 685f 7472 6565 222c 206c  refresh_tree", l
+0000c430: 6973 7428 7365 6c66 2e66 6c61 7428 7479  ist(self.flat(ty
+0000c440: 7065 733d 2272 6566 6572 656e 6365 2229  pes="reference")
+0000c450: 2929 0d0a 0d0a 2020 2020 4074 7265 655f  ))....    @tree_
+0000c460: 636f 6e64 6974 696f 6e61 6c28 6c61 6d62  conditional(lamb
+0000c470: 6461 206e 6f64 653a 206e 6f74 2073 656c  da node: not sel
+0000c480: 662e 636c 6173 7369 6679 5f61 7574 6f67  f.classify_autog
+0000c490: 656e 6572 6174 6529 0d0a 2020 2020 4074  enerate)..    @t
+0000c4a0: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
+0000c4b0: 2020 2020 2020 2020 5f28 2252 6566 7265          _("Refre
+0000c4c0: 7368 2063 6c61 7373 6966 6963 6174 696f  sh classificatio
+0000c4d0: 6e22 292c 0d0a 2020 2020 2020 2020 6e6f  n"),..        no
+0000c4e0: 6465 5f74 7970 653d 2262 7261 6e63 6820  de_type="branch 
+0000c4f0: 6f70 7322 2c0d 0a20 2020 2020 2020 2068  ops",..        h
+0000c500: 656c 703d 5f28 2252 6563 6c61 7373 6966  elp=_("Reclassif
+0000c510: 7920 656c 656d 656e 7473 2061 6e64 2075  y elements and u
+0000c520: 7365 206f 6e6c 7920 6578 6973 7469 6e67  se only existing
+0000c530: 206f 7065 7261 7469 6f6e 7322 292c 0d0a   operations"),..
+0000c540: 2020 2020 290d 0a20 2020 2064 6566 2072      )..    def r
+0000c550: 6566 7265 7368 5f63 6c61 7369 6669 6361  efresh_clasifica
+0000c560: 7469 6f6e 735f 3228 6e6f 6465 2c20 2a2a  tions_2(node, **
+0000c570: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+0000c580: 2020 7365 6c66 2e72 656d 6f76 655f 656c    self.remove_el
+0000c590: 656d 656e 7473 5f66 726f 6d5f 6f70 6572  ements_from_oper
+0000c5a0: 6174 696f 6e73 286c 6973 7428 7365 6c66  ations(list(self
+0000c5b0: 2e65 6c65 6d73 2829 2929 0d0a 2020 2020  .elems()))..    
+0000c5c0: 2020 2020 7365 6c66 2e63 6c61 7373 6966      self.classif
+0000c5d0: 7928 6c69 7374 2873 656c 662e 656c 656d  y(list(self.elem
+0000c5e0: 7328 2929 290d 0a20 2020 2020 2020 2073  s()))..        s
+0000c5f0: 656c 662e 7369 676e 616c 2822 7265 6672  elf.signal("refr
+0000c600: 6573 685f 7472 6565 222c 206c 6973 7428  esh_tree", list(
+0000c610: 7365 6c66 2e66 6c61 7428 7479 7065 733d  self.flat(types=
+0000c620: 2272 6566 6572 656e 6365 2229 2929 0d0a  "reference")))..
+0000c630: 0d0a 2020 2020 4074 7265 655f 7365 7061  ..    @tree_sepa
+0000c640: 7261 746f 725f 6166 7465 7228 290d 0a20  rator_after().. 
+0000c650: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
+0000c660: 6f6e 616c 286c 616d 6264 6120 6e6f 6465  onal(lambda node
+0000c670: 3a20 6e6f 7420 7365 6c66 2e63 6c61 7373  : not self.class
+0000c680: 6966 795f 6175 746f 6765 6e65 7261 7465  ify_autogenerate
+0000c690: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+0000c6a0: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
+0000c6b0: 205f 2822 5265 6672 6573 6820 2e2e 2e20   _("Refresh ... 
+0000c6c0: 2869 6e63 6c20 6175 746f 6765 6e65 7261  (incl autogenera
+0000c6d0: 7469 6f6e 2922 292c 0d0a 2020 2020 2020  tion)"),..      
+0000c6e0: 2020 6e6f 6465 5f74 7970 653d 2262 7261    node_type="bra
+0000c6f0: 6e63 6820 6f70 7322 2c0d 0a20 2020 2020  nch ops",..     
+0000c700: 2020 2068 656c 703d 5f28 2252 6563 6c61     help=_("Recla
+0000c710: 7373 6966 7920 656c 656d 656e 7473 2061  ssify elements a
+0000c720: 6e64 2063 7265 6174 6520 6f70 6572 6174  nd create operat
+0000c730: 696f 6e73 2069 6620 6e65 6365 7373 6172  ions if necessar
+0000c740: 7922 292c 0d0a 2020 2020 290d 0a20 2020  y"),..    )..   
+0000c750: 2064 6566 2072 6566 7265 7368 5f63 6c61   def refresh_cla
+0000c760: 7369 6669 6361 7469 6f6e 735f 3328 6e6f  sifications_3(no
+0000c770: 6465 2c20 2a2a 6b77 6172 6773 293a 0d0a  de, **kwargs):..
+0000c780: 2020 2020 2020 2020 7072 6576 696f 7573          previous
+0000c790: 203d 2073 656c 662e 636c 6173 7369 6679   = self.classify
+0000c7a0: 5f61 7574 6f67 656e 6572 6174 650d 0a20  _autogenerate.. 
+0000c7b0: 2020 2020 2020 2073 656c 662e 636c 6173         self.clas
+0000c7c0: 7369 6679 5f61 7574 6f67 656e 6572 6174  sify_autogenerat
+0000c7d0: 6520 3d20 5472 7565 0d0a 2020 2020 2020  e = True..      
+0000c7e0: 2020 7365 6c66 2e72 656d 6f76 655f 656c    self.remove_el
+0000c7f0: 656d 656e 7473 5f66 726f 6d5f 6f70 6572  ements_from_oper
+0000c800: 6174 696f 6e73 286c 6973 7428 7365 6c66  ations(list(self
+0000c810: 2e65 6c65 6d73 2829 2929 0d0a 2020 2020  .elems()))..    
+0000c820: 2020 2020 7365 6c66 2e63 6c61 7373 6966      self.classif
+0000c830: 7928 6c69 7374 2873 656c 662e 656c 656d  y(list(self.elem
+0000c840: 7328 2929 290d 0a20 2020 2020 2020 2073  s()))..        s
+0000c850: 656c 662e 636c 6173 7369 6679 5f61 7574  elf.classify_aut
+0000c860: 6f67 656e 6572 6174 6520 3d20 7072 6576  ogenerate = prev
+0000c870: 696f 7573 0d0a 2020 2020 2020 2020 7365  ious..        se
+0000c880: 6c66 2e73 6967 6e61 6c28 2272 6566 7265  lf.signal("refre
+0000c890: 7368 5f74 7265 6522 2c20 6c69 7374 2873  sh_tree", list(s
+0000c8a0: 656c 662e 666c 6174 2874 7970 6573 3d22  elf.flat(types="
+0000c8b0: 7265 6665 7265 6e63 6522 2929 290d 0a0d  reference")))...
+0000c8c0: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
+0000c8d0: 7469 6f6e 616c 286c 616d 6264 6120 636f  tional(lambda co
+0000c8e0: 6e64 3a20 7365 6c66 2e68 6176 655f 756e  nd: self.have_un
+0000c8f0: 6173 7369 676e 6564 5f65 6c65 6d65 6e74  assigned_element
+0000c900: 7328 2929 0d0a 2020 2020 4074 7265 655f  s())..    @tree_
+0000c910: 6f70 6572 6174 696f 6e28 0d0a 2020 2020  operation(..    
+0000c920: 2020 2020 5f28 2253 656c 6563 7420 756e      _("Select un
+0000c930: 6173 7369 676e 6564 2065 6c65 6d65 6e74  assigned element
+0000c940: 7322 292c 0d0a 2020 2020 2020 2020 6e6f  s"),..        no
+0000c950: 6465 5f74 7970 653d 2262 7261 6e63 6820  de_type="branch 
+0000c960: 6f70 7322 2c0d 0a20 2020 2020 2020 2068  ops",..        h
+0000c970: 656c 703d 5f28 2253 656c 6563 7420 616c  elp=_("Select al
+0000c980: 6c20 656c 656d 656e 7473 2074 6861 7420  l elements that 
+0000c990: 776f 6e27 7420 6265 2062 7572 6e65 6422  won't be burned"
+0000c9a0: 292c 0d0a 2020 2020 290d 0a20 2020 2064  ),..    )..    d
+0000c9b0: 6566 2073 656c 6563 745f 756e 6173 7369  ef select_unassi
+0000c9c0: 676e 6564 286e 6f64 652c 202a 2a6b 7761  gned(node, **kwa
+0000c9d0: 7267 7329 3a0d 0a20 2020 2020 2020 2063  rgs):..        c
+0000c9e0: 6861 6e67 6573 203d 2046 616c 7365 0d0a  hanges = False..
+0000c9f0: 2020 2020 2020 2020 666f 7220 6e6f 6465          for node
+0000ca00: 2069 6e20 7365 6c66 2e65 6c65 6d73 2829   in self.elems()
+0000ca10: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
+0000ca20: 6d70 6861 7369 7320 3d20 626f 6f6c 286c  mphasis = bool(l
+0000ca30: 656e 286e 6f64 652e 7265 6665 7265 6e63  en(node.referenc
+0000ca40: 6573 2920 3d3d 2030 290d 0a20 2020 2020  es) == 0)..     
+0000ca50: 2020 2020 2020 2069 6620 6e6f 6465 2e65         if node.e
+0000ca60: 6d70 6861 7369 7a65 6420 213d 2065 6d70  mphasized != emp
+0000ca70: 6861 7369 7320 616e 6420 6e6f 6465 2e63  hasis and node.c
+0000ca80: 616e 5f65 6d70 6861 7369 7a65 3a0d 0a20  an_emphasize:.. 
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000caa0: 6861 6e67 6573 203d 2054 7275 650d 0a20  hanges = True.. 
+0000cab0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000cac0: 6f64 652e 656d 7068 6173 697a 6564 203d  ode.emphasized =
+0000cad0: 2065 6d70 6861 7369 730d 0a20 2020 2020   emphasis..     
+0000cae0: 2020 2069 6620 6368 616e 6765 733a 0d0a     if changes:..
+0000caf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cb00: 2e76 616c 6964 6174 655f 7365 6c65 6374  .validate_select
+0000cb10: 6564 5f61 7265 6128 290d 0a20 2020 2020  ed_area()..     
+0000cb20: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+0000cb30: 616c 2822 7265 6672 6573 685f 7363 656e  al("refresh_scen
+0000cb40: 6522 2c20 2253 6365 6e65 2229 0d0a 0d0a  e", "Scene")....
+0000cb50: 2020 2020 6d61 7465 7269 616c 7320 3d20      materials = 
+0000cb60: 5b0d 0a20 2020 2020 2020 205f 2822 576f  [..        _("Wo
+0000cb70: 6f64 2229 2c0d 0a20 2020 2020 2020 205f  od"),..        _
+0000cb80: 2822 4163 7279 6c69 6322 292c 0d0a 2020  ("Acrylic"),..  
+0000cb90: 2020 2020 2020 5f28 2246 6f61 6d22 292c        _("Foam"),
+0000cba0: 0d0a 2020 2020 2020 2020 5f28 224c 6561  ..        _("Lea
+0000cbb0: 7468 6572 2229 2c0d 0a20 2020 2020 2020  ther"),..       
+0000cbc0: 205f 2822 4361 7264 626f 6172 6422 292c   _("Cardboard"),
+0000cbd0: 0d0a 2020 2020 2020 2020 5f28 2243 6f72  ..        _("Cor
+0000cbe0: 6b22 292c 0d0a 2020 2020 2020 2020 5f28  k"),..        _(
+0000cbf0: 2254 6578 7469 6c65 7322 292c 0d0a 2020  "Textiles"),..  
+0000cc00: 2020 2020 2020 5f28 2250 6170 6572 2229        _("Paper")
+0000cc10: 2c0d 0a20 2020 2020 2020 205f 2822 5361  ,..        _("Sa
+0000cc20: 7665 2d31 2229 2c0d 0a20 2020 2020 2020  ve-1"),..       
+0000cc30: 205f 2822 5361 7665 2d32 2229 2c0d 0a20   _("Save-2"),.. 
+0000cc40: 2020 2020 2020 205f 2822 5361 7665 2d33         _("Save-3
+0000cc50: 2229 2c0d 0a20 2020 205d 0d0a 0d0a 2020  "),..    ]....  
+0000cc60: 2020 6465 6620 756e 696f 6e5f 6d61 7465    def union_mate
+0000cc70: 7269 616c 735f 7361 7665 6428 293a 0d0a  rials_saved():..
+0000cc80: 2020 2020 2020 2020 756e 696f 6e20 3d20          union = 
+0000cc90: 5b0d 0a20 2020 2020 2020 2020 2020 2064  [..            d
+0000cca0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000ccb0: 7220 6420 696e 2073 656c 662e 6f70 5f64  r d in self.op_d
+0000ccc0: 6174 612e 7365 6374 696f 6e5f 7365 7428  ata.section_set(
+0000ccd0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000cce0: 6620 6420 6e6f 7420 696e 206d 6174 6572  f d not in mater
+0000ccf0: 6961 6c73 2061 6e64 2064 2021 3d20 2270  ials and d != "p
+0000cd00: 7265 7669 6f75 7322 0d0a 2020 2020 2020  revious"..      
+0000cd10: 2020 5d0d 0a20 2020 2020 2020 2075 6e69    ]..        uni
+0000cd20: 6f6e 2e65 7874 656e 6428 6d61 7465 7269  on.extend(materi
+0000cd30: 616c 7329 0d0a 2020 2020 2020 2020 7265  als)..        re
+0000cd40: 7475 726e 2075 6e69 6f6e 0d0a 0d0a 2020  turn union....  
+0000cd50: 2020 6465 6620 6469 6666 6572 656e 6365    def difference
+0000cd60: 5f6d 6174 6572 6961 6c73 5f73 6176 6564  _materials_saved
+0000cd70: 2829 3a0d 0a20 2020 2020 2020 2073 6563  ():..        sec
+0000cd80: 7320 3d20 7365 6c66 2e6f 705f 6461 7461  s = self.op_data
+0000cd90: 2e73 6563 7469 6f6e 5f73 6574 2829 0d0a  .section_set()..
+0000cda0: 2020 2020 2020 2020 6469 6666 6572 656e          differen
+0000cdb0: 6365 203d 205b 6d20 666f 7220 6d20 696e  ce = [m for m in
+0000cdc0: 206d 6174 6572 6961 6c73 2069 6620 6d20   materials if m 
+0000cdd0: 6e6f 7420 696e 2073 6563 735d 0d0a 2020  not in secs]..  
+0000cde0: 2020 2020 2020 7265 7475 726e 2064 6966        return dif
+0000cdf0: 6665 7265 6e63 650d 0a0d 0a20 2020 2040  ference....    @
+0000ce00: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
+0000ce10: 4c6f 6164 2229 290d 0a20 2020 2040 7472  Load"))..    @tr
+0000ce20: 6565 5f76 616c 7565 7328 226f 706e 616d  ee_values("opnam
+0000ce30: 6522 2c20 7661 6c75 6573 3d73 656c 662e  e", values=self.
+0000ce40: 6f70 5f64 6174 612e 7365 6374 696f 6e5f  op_data.section_
+0000ce50: 7365 7429 0d0a 2020 2020 4074 7265 655f  set)..    @tree_
+0000ce60: 6f70 6572 6174 696f 6e28 227b 6f70 6e61  operation("{opna
+0000ce70: 6d65 7d22 2c20 6e6f 6465 5f74 7970 653d  me}", node_type=
+0000ce80: 2262 7261 6e63 6820 6f70 7322 2c20 6865  "branch ops", he
+0000ce90: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+0000cea0: 6c6f 6164 5f6f 7073 286e 6f64 652c 206f  load_ops(node, o
+0000ceb0: 706e 616d 652c 202a 2a6b 7761 7267 7329  pname, **kwargs)
+0000cec0: 3a0d 0a20 2020 2020 2020 2073 656c 6628  :..        self(
+0000ced0: 6622 6d61 7465 7269 616c 206c 6f61 6420  f"material load 
+0000cee0: 7b6f 706e 616d 657d 5c6e 2229 0d0a 0d0a  {opname}\n")....
+0000cef0: 2020 2020 4074 7265 655f 7365 7061 7261      @tree_separa
+0000cf00: 746f 725f 6265 666f 7265 2829 0d0a 2020  tor_before()..  
+0000cf10: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+0000cf20: 5f28 224c 6f61 6422 2929 0d0a 2020 2020  _("Load"))..    
+0000cf30: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+0000cf40: 5f28 224f 7468 6572 2f42 6c75 652f 5265  _("Other/Blue/Re
+0000cf50: 6422 292c 206e 6f64 655f 7479 7065 3d22  d"), node_type="
+0000cf60: 6272 616e 6368 206f 7073 222c 2068 656c  branch ops", hel
+0000cf70: 703d 2222 290d 0a20 2020 2064 6566 2064  p="")..    def d
+0000cf80: 6566 6175 6c74 5f63 6c61 7373 6966 6963  efault_classific
+0000cf90: 6174 696f 6e73 286e 6f64 652c 202a 2a6b  ations(node, **k
+0000cfa0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+0000cfb0: 2073 656c 662e 6c6f 6164 5f64 6566 6175   self.load_defau
+0000cfc0: 6c74 2870 6572 666f 726d 636c 6173 7369  lt(performclassi
+0000cfd0: 6679 3d54 7275 6529 0d0a 0d0a 2020 2020  fy=True)....    
+0000cfe0: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
+0000cff0: 224c 6f61 6422 2929 0d0a 2020 2020 4074  "Load"))..    @t
+0000d000: 7265 655f 7365 7061 7261 746f 725f 6166  ree_separator_af
+0000d010: 7465 7228 290d 0a20 2020 2040 7472 6565  ter()..    @tree
+0000d020: 5f6f 7065 7261 7469 6f6e 285f 2822 4261  _operation(_("Ba
+0000d030: 7369 6322 292c 206e 6f64 655f 7479 7065  sic"), node_type
+0000d040: 3d22 6272 616e 6368 206f 7073 222c 2068  ="branch ops", h
+0000d050: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
+0000d060: 2062 6173 6963 5f63 6c61 7373 6966 6963   basic_classific
+0000d070: 6174 696f 6e73 286e 6f64 652c 202a 2a6b  ations(node, **k
+0000d080: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+0000d090: 2073 656c 662e 6c6f 6164 5f64 6566 6175   self.load_defau
+0000d0a0: 6c74 3228 7065 7266 6f72 6d63 6c61 7373  lt2(performclass
+0000d0b0: 6966 793d 5472 7565 290d 0a0d 0a20 2020  ify=True)....   
+0000d0c0: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
+0000d0d0: 2822 5361 7665 2229 290d 0a20 2020 2040  ("Save"))..    @
+0000d0e0: 7472 6565 5f76 616c 7565 7328 226f 706e  tree_values("opn
+0000d0f0: 616d 6522 2c20 7661 6c75 6573 3d73 656c  ame", values=sel
+0000d100: 662e 6f70 5f64 6174 612e 7365 6374 696f  f.op_data.sectio
+0000d110: 6e5f 7365 7429 0d0a 2020 2020 4074 7265  n_set)..    @tre
+0000d120: 655f 6f70 6572 6174 696f 6e28 227b 6f70  e_operation("{op
+0000d130: 6e61 6d65 7d22 2c20 6e6f 6465 5f74 7970  name}", node_typ
+0000d140: 653d 2262 7261 6e63 6820 6f70 7322 2c20  e="branch ops", 
+0000d150: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
+0000d160: 6620 7361 7665 5f6d 6174 6572 6961 6c73  f save_materials
+0000d170: 286e 6f64 652c 206f 706e 616d 653d 2273  (node, opname="s
+0000d180: 6176 6564 222c 202a 2a6b 7761 7267 7329  aved", **kwargs)
+0000d190: 3a0d 0a20 2020 2020 2020 2073 656c 6628  :..        self(
+0000d1a0: 6622 6d61 7465 7269 616c 2073 6176 6520  f"material save 
+0000d1b0: 7b6f 706e 616d 657d 5c6e 2229 0d0a 0d0a  {opname}\n")....
+0000d1c0: 2020 2020 4074 7265 655f 7365 7061 7261      @tree_separa
+0000d1d0: 746f 725f 6265 666f 7265 2829 0d0a 2020  tor_before()..  
+0000d1e0: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+0000d1f0: 5f28 2253 6176 6522 2929 0d0a 2020 2020  _("Save"))..    
+0000d200: 4074 7265 655f 7072 6f6d 7074 2822 6f70  @tree_prompt("op
+0000d210: 6e61 6d65 222c 205f 2822 4e61 6d65 2074  name", _("Name t
+0000d220: 6f20 7374 6f72 6520 6375 7272 656e 7420  o store current 
+0000d230: 6f70 6572 6174 696f 6e73 2075 6e64 6572  operations under
+0000d240: 3f22 2929 0d0a 2020 2020 4074 7265 655f  ?"))..    @tree_
+0000d250: 6f70 6572 6174 696f 6e28 5f28 224e 6577  operation(_("New
+0000d260: 2229 2c20 6e6f 6465 5f74 7970 653d 2262  "), node_type="b
+0000d270: 7261 6e63 6820 6f70 7322 2c20 6865 6c70  ranch ops", help
+0000d280: 3d22 2229 0d0a 2020 2020 6465 6620 7361  ="")..    def sa
+0000d290: 7665 5f6d 6174 6572 6961 6c5f 6375 7374  ve_material_cust
+0000d2a0: 6f6d 286e 6f64 652c 206f 706e 616d 652c  om(node, opname,
+0000d2b0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+0000d2c0: 2020 2020 2073 656c 6628 6622 6d61 7465       self(f"mate
+0000d2d0: 7269 616c 2073 6176 6520 7b6f 706e 616d  rial save {opnam
+0000d2e0: 652e 7265 706c 6163 6528 2720 272c 2027  e.replace(' ', '
+0000d2f0: 5f27 297d 5c6e 2229 0d0a 0d0a 2020 2020  _')}\n")....    
+0000d300: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
+0000d310: 2244 656c 6574 6522 2929 0d0a 2020 2020  "Delete"))..    
+0000d320: 4074 7265 655f 7661 6c75 6573 2822 6f70  @tree_values("op
+0000d330: 6e61 6d65 222c 2076 616c 7565 733d 7365  name", values=se
+0000d340: 6c66 2e6f 705f 6461 7461 2e73 6563 7469  lf.op_data.secti
+0000d350: 6f6e 5f73 6574 290d 0a20 2020 2040 7472  on_set)..    @tr
+0000d360: 6565 5f6f 7065 7261 7469 6f6e 2822 7b6f  ee_operation("{o
+0000d370: 706e 616d 657d 222c 206e 6f64 655f 7479  pname}", node_ty
+0000d380: 7065 3d22 6272 616e 6368 206f 7073 222c  pe="branch ops",
+0000d390: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
+0000d3a0: 6566 2072 656d 6f76 655f 6f70 7328 6e6f  ef remove_ops(no
+0000d3b0: 6465 2c20 6f70 6e61 6d65 3d22 7361 7665  de, opname="save
+0000d3c0: 6422 2c20 2a2a 6b77 6172 6773 293a 0d0a  d", **kwargs):..
+0000d3d0: 2020 2020 2020 2020 7365 6c66 2866 226d          self(f"m
+0000d3e0: 6174 6572 6961 6c20 6465 6c65 7465 207b  aterial delete {
+0000d3f0: 6f70 6e61 6d65 7d5c 6e22 290d 0a0d 0a20  opname}\n").... 
+0000d400: 2020 2040 7472 6565 5f73 6570 6172 6174     @tree_separat
+0000d410: 6f72 5f62 6566 6f72 6528 290d 0a20 2020  or_before()..   
+0000d420: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
+0000d430: 2822 4170 7065 6e64 206f 7065 7261 7469  ("Append operati
+0000d440: 6f6e 2229 290d 0a20 2020 2040 7472 6565  on"))..    @tree
+0000d450: 5f6f 7065 7261 7469 6f6e 285f 2822 4170  _operation(_("Ap
+0000d460: 7065 6e64 2049 6d61 6765 2229 2c20 6e6f  pend Image"), no
+0000d470: 6465 5f74 7970 653d 2262 7261 6e63 6820  de_type="branch 
+0000d480: 6f70 7322 2c20 6865 6c70 3d22 2229 0d0a  ops", help="")..
+0000d490: 2020 2020 6465 6620 6170 7065 6e64 5f6f      def append_o
+0000d4a0: 7065 7261 7469 6f6e 5f69 6d61 6765 286e  peration_image(n
+0000d4b0: 6f64 652c 2070 6f73 3d4e 6f6e 652c 202a  ode, pos=None, *
+0000d4c0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+0000d4d0: 2020 2073 656c 662e 6f70 5f62 7261 6e63     self.op_branc
+0000d4e0: 682e 6164 6428 226f 7020 696d 6167 6522  h.add("op image"
+0000d4f0: 2c20 706f 733d 706f 7329 0d0a 2020 2020  , pos=pos)..    
+0000d500: 2020 2020 7365 6c66 2e73 6967 6e61 6c28      self.signal(
+0000d510: 2275 7064 6174 656f 705f 7472 6565 2229  "updateop_tree")
+0000d520: 0d0a 0d0a 2020 2020 4074 7265 655f 7375  ....    @tree_su
+0000d530: 626d 656e 7528 5f28 2241 7070 656e 6420  bmenu(_("Append 
+0000d540: 6f70 6572 6174 696f 6e22 2929 0d0a 2020  operation"))..  
+0000d550: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
+0000d560: 6e28 5f28 2241 7070 656e 6420 5261 7374  n(_("Append Rast
+0000d570: 6572 2229 2c20 6e6f 6465 5f74 7970 653d  er"), node_type=
+0000d580: 2262 7261 6e63 6820 6f70 7322 2c20 6865  "branch ops", he
+0000d590: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+0000d5a0: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
+0000d5b0: 5f72 6173 7465 7228 6e6f 6465 2c20 706f  _raster(node, po
+0000d5c0: 733d 4e6f 6e65 2c20 2a2a 6b77 6172 6773  s=None, **kwargs
+0000d5d0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+0000d5e0: 2e6f 705f 6272 616e 6368 2e61 6464 2822  .op_branch.add("
+0000d5f0: 6f70 2072 6173 7465 7222 2c20 706f 733d  op raster", pos=
+0000d600: 706f 7329 0d0a 2020 2020 2020 2020 7365  pos)..        se
+0000d610: 6c66 2e73 6967 6e61 6c28 2275 7064 6174  lf.signal("updat
+0000d620: 656f 705f 7472 6565 2229 0d0a 0d0a 2020  eop_tree")....  
+0000d630: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+0000d640: 5f28 2241 7070 656e 6420 6f70 6572 6174  _("Append operat
+0000d650: 696f 6e22 2929 0d0a 2020 2020 4074 7265  ion"))..    @tre
+0000d660: 655f 6f70 6572 6174 696f 6e28 5f28 2241  e_operation(_("A
+0000d670: 7070 656e 6420 456e 6772 6176 6522 292c  ppend Engrave"),
+0000d680: 206e 6f64 655f 7479 7065 3d22 6272 616e   node_type="bran
+0000d690: 6368 206f 7073 222c 2068 656c 703d 2222  ch ops", help=""
+0000d6a0: 290d 0a20 2020 2064 6566 2061 7070 656e  )..    def appen
+0000d6b0: 645f 6f70 6572 6174 696f 6e5f 656e 6772  d_operation_engr
+0000d6c0: 6176 6528 6e6f 6465 2c20 706f 733d 4e6f  ave(node, pos=No
+0000d6d0: 6e65 2c20 2a2a 6b77 6172 6773 293a 0d0a  ne, **kwargs):..
+0000d6e0: 2020 2020 2020 2020 7365 6c66 2e6f 705f          self.op_
+0000d6f0: 6272 616e 6368 2e61 6464 2822 6f70 2065  branch.add("op e
+0000d700: 6e67 7261 7665 222c 2070 6f73 3d70 6f73  ngrave", pos=pos
+0000d710: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000d720: 7369 676e 616c 2822 7570 6461 7465 6f70  signal("updateop
+0000d730: 5f74 7265 6522 290d 0a0d 0a20 2020 2040  _tree")....    @
+0000d740: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
+0000d750: 4170 7065 6e64 206f 7065 7261 7469 6f6e  Append operation
+0000d760: 2229 290d 0a20 2020 2040 7472 6565 5f6f  "))..    @tree_o
+0000d770: 7065 7261 7469 6f6e 285f 2822 4170 7065  peration(_("Appe
+0000d780: 6e64 2043 7574 2229 2c20 6e6f 6465 5f74  nd Cut"), node_t
+0000d790: 7970 653d 2262 7261 6e63 6820 6f70 7322  ype="branch ops"
+0000d7a0: 2c20 6865 6c70 3d22 2229 0d0a 2020 2020  , help="")..    
+0000d7b0: 6465 6620 6170 7065 6e64 5f6f 7065 7261  def append_opera
+0000d7c0: 7469 6f6e 5f63 7574 286e 6f64 652c 2070  tion_cut(node, p
+0000d7d0: 6f73 3d4e 6f6e 652c 202a 2a6b 7761 7267  os=None, **kwarg
+0000d7e0: 7329 3a0d 0a20 2020 2020 2020 2073 656c  s):..        sel
+0000d7f0: 662e 6f70 5f62 7261 6e63 682e 6164 6428  f.op_branch.add(
+0000d800: 226f 7020 6375 7422 2c20 706f 733d 706f  "op cut", pos=po
+0000d810: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
+0000d820: 2e73 6967 6e61 6c28 2275 7064 6174 656f  .signal("updateo
+0000d830: 705f 7472 6565 2229 0d0a 0d0a 2020 2020  p_tree")....    
+0000d840: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
+0000d850: 2241 7070 656e 6420 6f70 6572 6174 696f  "Append operatio
+0000d860: 6e22 2929 0d0a 2020 2020 4074 7265 655f  n"))..    @tree_
+0000d870: 6f70 6572 6174 696f 6e28 5f28 2241 7070  operation(_("App
+0000d880: 656e 6420 4861 7463 6822 292c 206e 6f64  end Hatch"), nod
+0000d890: 655f 7479 7065 3d22 6272 616e 6368 206f  e_type="branch o
+0000d8a0: 7073 222c 2068 656c 703d 2222 290d 0a20  ps", help="").. 
+0000d8b0: 2020 2064 6566 2061 7070 656e 645f 6f70     def append_op
+0000d8c0: 6572 6174 696f 6e5f 6861 7463 6828 6e6f  eration_hatch(no
+0000d8d0: 6465 2c20 706f 733d 4e6f 6e65 2c20 2a2a  de, pos=None, **
+0000d8e0: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+0000d8f0: 2020 7365 6c66 2e6f 705f 6272 616e 6368    self.op_branch
+0000d900: 2e61 6464 2822 6f70 2068 6174 6368 222c  .add("op hatch",
+0000d910: 2070 6f73 3d70 6f73 290d 0a20 2020 2020   pos=pos)..     
+0000d920: 2020 2073 656c 662e 7369 676e 616c 2822     self.signal("
+0000d930: 7570 6461 7465 6f70 5f74 7265 6522 290d  updateop_tree").
+0000d940: 0a0d 0a20 2020 2040 7472 6565 5f73 7562  ...    @tree_sub
+0000d950: 6d65 6e75 285f 2822 4170 7065 6e64 206f  menu(_("Append o
+0000d960: 7065 7261 7469 6f6e 2229 290d 0a20 2020  peration"))..   
+0000d970: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+0000d980: 285f 2822 4170 7065 6e64 2044 6f74 7322  (_("Append Dots"
+0000d990: 292c 206e 6f64 655f 7479 7065 3d22 6272  ), node_type="br
+0000d9a0: 616e 6368 206f 7073 222c 2068 656c 703d  anch ops", help=
+0000d9b0: 2222 290d 0a20 2020 2064 6566 2061 7070  "")..    def app
+0000d9c0: 656e 645f 6f70 6572 6174 696f 6e5f 646f  end_operation_do
+0000d9d0: 7473 286e 6f64 652c 2070 6f73 3d4e 6f6e  ts(node, pos=Non
+0000d9e0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+0000d9f0: 2020 2020 2020 2073 656c 662e 6f70 5f62         self.op_b
+0000da00: 7261 6e63 682e 6164 6428 226f 7020 646f  ranch.add("op do
+0000da10: 7473 222c 2070 6f73 3d70 6f73 290d 0a20  ts", pos=pos).. 
+0000da20: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+0000da30: 616c 2822 7570 6461 7465 6f70 5f74 7265  al("updateop_tre
+0000da40: 6522 290d 0a0d 0a20 2020 2040 7472 6565  e")....    @tree
+0000da50: 5f73 7562 6d65 6e75 285f 2822 4170 7065  _submenu(_("Appe
+0000da60: 6e64 2073 7065 6369 616c 206f 7065 7261  nd special opera
+0000da70: 7469 6f6e 2873 2922 2929 0d0a 2020 2020  tion(s)"))..    
+0000da80: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+0000da90: 5f28 2241 7070 656e 6420 486f 6d65 2229  _("Append Home")
+0000daa0: 2c20 6e6f 6465 5f74 7970 653d 2262 7261  , node_type="bra
+0000dab0: 6e63 6820 6f70 7322 2c20 6865 6c70 3d22  nch ops", help="
+0000dac0: 2229 0d0a 2020 2020 6465 6620 6170 7065  ")..    def appe
+0000dad0: 6e64 5f6f 7065 7261 7469 6f6e 5f68 6f6d  nd_operation_hom
+0000dae0: 6528 6e6f 6465 2c20 706f 733d 4e6f 6e65  e(node, pos=None
+0000daf0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+0000db00: 2020 2020 2020 7365 6c66 2e6f 705f 6272        self.op_br
+0000db10: 616e 6368 2e61 6464 2874 7970 653d 2275  anch.add(type="u
+0000db20: 7469 6c20 686f 6d65 222c 2070 6f73 3d70  til home", pos=p
+0000db30: 6f73 290d 0a20 2020 2020 2020 2073 656c  os)..        sel
+0000db40: 662e 7369 676e 616c 2822 7570 6461 7465  f.signal("update
+0000db50: 6f70 5f74 7265 6522 290d 0a0d 0a20 2020  op_tree")....   
+0000db60: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
+0000db70: 2822 4170 7065 6e64 2073 7065 6369 616c  ("Append special
+0000db80: 206f 7065 7261 7469 6f6e 2873 2922 2929   operation(s)"))
+0000db90: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+0000dba0: 6174 696f 6e28 5f28 2241 7070 656e 6420  ation(_("Append 
+0000dbb0: 5265 7475 726e 2074 6f20 4f72 6967 696e  Return to Origin
+0000dbc0: 2229 2c20 6e6f 6465 5f74 7970 653d 2262  "), node_type="b
+0000dbd0: 7261 6e63 6820 6f70 7322 2c20 6865 6c70  ranch ops", help
+0000dbe0: 3d22 2229 0d0a 2020 2020 6465 6620 6170  ="")..    def ap
+0000dbf0: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f67  pend_operation_g
+0000dc00: 6f74 6f28 6e6f 6465 2c20 706f 733d 4e6f  oto(node, pos=No
+0000dc10: 6e65 2c20 2a2a 6b77 6172 6773 293a 0d0a  ne, **kwargs):..
+0000dc20: 2020 2020 2020 2020 7365 6c66 2e6f 705f          self.op_
+0000dc30: 6272 616e 6368 2e61 6464 2874 7970 653d  branch.add(type=
+0000dc40: 2275 7469 6c20 676f 746f 222c 2070 6f73  "util goto", pos
+0000dc50: 3d70 6f73 2c20 783d 302c 2079 3d30 290d  =pos, x=0, y=0).
+0000dc60: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
+0000dc70: 676e 616c 2822 7570 6461 7465 6f70 5f74  gnal("updateop_t
+0000dc80: 7265 6522 290d 0a0d 0a20 2020 2040 7472  ree")....    @tr
+0000dc90: 6565 5f73 7562 6d65 6e75 285f 2822 4170  ee_submenu(_("Ap
+0000dca0: 7065 6e64 2073 7065 6369 616c 206f 7065  pend special ope
+0000dcb0: 7261 7469 6f6e 2873 2922 2929 0d0a 2020  ration(s)"))..  
+0000dcc0: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
+0000dcd0: 6e28 5f28 2241 7070 656e 6420 4265 6570  n(_("Append Beep
+0000dce0: 2229 2c20 6e6f 6465 5f74 7970 653d 2262  "), node_type="b
+0000dcf0: 7261 6e63 6820 6f70 7322 2c20 6865 6c70  ranch ops", help
+0000dd00: 3d22 2229 0d0a 2020 2020 6465 6620 6170  ="")..    def ap
+0000dd10: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f62  pend_operation_b
+0000dd20: 6565 7028 6e6f 6465 2c20 706f 733d 4e6f  eep(node, pos=No
+0000dd30: 6e65 2c20 2a2a 6b77 6172 6773 293a 0d0a  ne, **kwargs):..
+0000dd40: 2020 2020 2020 2020 7365 6c66 2e6f 705f          self.op_
+0000dd50: 6272 616e 6368 2e61 6464 280d 0a20 2020  branch.add(..   
+0000dd60: 2020 2020 2020 2020 2074 7970 653d 2275           type="u
+0000dd70: 7469 6c20 636f 6e73 6f6c 6522 2c0d 0a20  til console",.. 
+0000dd80: 2020 2020 2020 2020 2020 2070 6f73 3d70             pos=p
+0000dd90: 6f73 2c0d 0a20 2020 2020 2020 2020 2020  os,..           
+0000dda0: 2063 6f6d 6d61 6e64 3d22 6265 6570 222c   command="beep",
+0000ddb0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+0000ddc0: 2020 2020 2073 656c 662e 7369 676e 616c       self.signal
+0000ddd0: 2822 7570 6461 7465 6f70 5f74 7265 6522  ("updateop_tree"
+0000dde0: 290d 0a0d 0a20 2020 2040 7472 6565 5f73  )....    @tree_s
+0000ddf0: 7562 6d65 6e75 285f 2822 4170 7065 6e64  ubmenu(_("Append
+0000de00: 2073 7065 6369 616c 206f 7065 7261 7469   special operati
+0000de10: 6f6e 2873 2922 2929 0d0a 2020 2020 4074  on(s)"))..    @t
+0000de20: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
+0000de30: 2241 7070 656e 6420 496e 7465 7272 7570  "Append Interrup
+0000de40: 7422 292c 206e 6f64 655f 7479 7065 3d22  t"), node_type="
+0000de50: 6272 616e 6368 206f 7073 222c 2068 656c  branch ops", hel
+0000de60: 703d 2222 290d 0a20 2020 2064 6566 2061  p="")..    def a
+0000de70: 7070 656e 645f 6f70 6572 6174 696f 6e5f  ppend_operation_
+0000de80: 696e 7465 7272 7570 7428 6e6f 6465 2c20  interrupt(node, 
+0000de90: 706f 733d 4e6f 6e65 2c20 2a2a 6b77 6172  pos=None, **kwar
+0000dea0: 6773 293a 0d0a 2020 2020 2020 2020 7365  gs):..        se
+0000deb0: 6c66 2e6f 705f 6272 616e 6368 2e61 6464  lf.op_branch.add
+0000dec0: 280d 0a20 2020 2020 2020 2020 2020 2074  (..            t
+0000ded0: 7970 653d 2275 7469 6c20 636f 6e73 6f6c  ype="util consol
+0000dee0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+0000def0: 2070 6f73 3d70 6f73 2c0d 0a20 2020 2020   pos=pos,..     
+0000df00: 2020 2020 2020 2063 6f6d 6d61 6e64 3d27         command='
+0000df10: 696e 7465 7272 7570 7420 2253 706f 6f6c  interrupt "Spool
+0000df20: 696e 6720 7761 7320 696e 7465 7272 7570  ing was interrup
+0000df30: 7465 6422 272c 0d0a 2020 2020 2020 2020  ted"',..        
+0000df40: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000df50: 7369 676e 616c 2822 7570 6461 7465 6f70  signal("updateop
+0000df60: 5f74 7265 6522 290d 0a0d 0a20 2020 2040  _tree")....    @
+0000df70: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
+0000df80: 4170 7065 6e64 2073 7065 6369 616c 206f  Append special o
+0000df90: 7065 7261 7469 6f6e 2873 2922 2929 0d0a  peration(s)"))..
+0000dfa0: 2020 2020 4074 7265 655f 7072 6f6d 7074      @tree_prompt
+0000dfb0: 2822 7761 6974 5f74 696d 6522 2c20 5f28  ("wait_time", _(
+0000dfc0: 2257 6169 7420 666f 7220 686f 7720 6c6f  "Wait for how lo
+0000dfd0: 6e67 2028 696e 2073 6563 6f6e 6473 293f  ng (in seconds)?
+0000dfe0: 2229 2c20 6461 7461 5f74 7970 653d 666c  "), data_type=fl
+0000dff0: 6f61 7429 0d0a 2020 2020 4074 7265 655f  oat)..    @tree_
+0000e000: 6f70 6572 6174 696f 6e28 5f28 2241 7070  operation(_("App
+0000e010: 656e 6420 5761 6974 2229 2c20 6e6f 6465  end Wait"), node
+0000e020: 5f74 7970 653d 2262 7261 6e63 6820 6f70  _type="branch op
+0000e030: 7322 2c20 6865 6c70 3d22 2229 0d0a 2020  s", help="")..  
+0000e040: 2020 6465 6620 6170 7065 6e64 5f6f 7065    def append_ope
+0000e050: 7261 7469 6f6e 5f77 6169 7428 6e6f 6465  ration_wait(node
+0000e060: 2c20 7761 6974 5f74 696d 652c 2070 6f73  , wait_time, pos
+0000e070: 3d4e 6f6e 652c 202a 2a6b 7761 7267 7329  =None, **kwargs)
+0000e080: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+0000e090: 6f70 5f62 7261 6e63 682e 6164 6428 0d0a  op_branch.add(..
+0000e0a0: 2020 2020 2020 2020 2020 2020 7479 7065              type
+0000e0b0: 3d22 7574 696c 2077 6169 7422 2c0d 0a20  ="util wait",.. 
+0000e0c0: 2020 2020 2020 2020 2020 2070 6f73 3d70             pos=p
+0000e0d0: 6f73 2c0d 0a20 2020 2020 2020 2020 2020  os,..           
+0000e0e0: 2077 6169 743d 7761 6974 5f74 696d 652c   wait=wait_time,
+0000e0f0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+0000e100: 2020 2020 2073 656c 662e 7369 676e 616c       self.signal
+0000e110: 2822 7570 6461 7465 6f70 5f74 7265 6522  ("updateop_tree"
+0000e120: 290d 0a0d 0a20 2020 2040 7472 6565 5f73  )....    @tree_s
+0000e130: 7562 6d65 6e75 285f 2822 4170 7065 6e64  ubmenu(_("Append
+0000e140: 2073 7065 6369 616c 206f 7065 7261 7469   special operati
+0000e150: 6f6e 2873 2922 2929 0d0a 2020 2020 4074  on(s)"))..    @t
+0000e160: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
+0000e170: 2241 7070 656e 6420 4f75 7470 7574 2229  "Append Output")
+0000e180: 2c20 6e6f 6465 5f74 7970 653d 2262 7261  , node_type="bra
+0000e190: 6e63 6820 6f70 7322 2c20 6865 6c70 3d22  nch ops", help="
+0000e1a0: 2229 0d0a 2020 2020 6465 6620 6170 7065  ")..    def appe
+0000e1b0: 6e64 5f6f 7065 7261 7469 6f6e 5f6f 7574  nd_operation_out
+0000e1c0: 7075 7428 6e6f 6465 2c20 706f 733d 4e6f  put(node, pos=No
+0000e1d0: 6e65 2c20 2a2a 6b77 6172 6773 293a 0d0a  ne, **kwargs):..
+0000e1e0: 2020 2020 2020 2020 7365 6c66 2e6f 705f          self.op_
+0000e1f0: 6272 616e 6368 2e61 6464 280d 0a20 2020  branch.add(..   
+0000e200: 2020 2020 2020 2020 2074 7970 653d 2275           type="u
+0000e210: 7469 6c20 6f75 7470 7574 222c 0d0a 2020  til output",..  
+0000e220: 2020 2020 2020 2020 2020 706f 733d 706f            pos=po
+0000e230: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+0000e240: 6f75 7470 7574 5f6d 6173 6b3d 302c 0d0a  output_mask=0,..
+0000e250: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+0000e260: 7574 5f76 616c 7565 3d30 2c0d 0a20 2020  ut_value=0,..   
+0000e270: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+0000e280: 6d65 7373 6167 653d 4e6f 6e65 2c0d 0a20  message=None,.. 
+0000e290: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+0000e2a0: 2020 7365 6c66 2e73 6967 6e61 6c28 2275    self.signal("u
+0000e2b0: 7064 6174 656f 705f 7472 6565 2229 0d0a  pdateop_tree")..
+0000e2c0: 0d0a 2020 2020 4074 7265 655f 7375 626d  ..    @tree_subm
+0000e2d0: 656e 7528 5f28 2241 7070 656e 6420 7370  enu(_("Append sp
+0000e2e0: 6563 6961 6c20 6f70 6572 6174 696f 6e28  ecial operation(
+0000e2f0: 7329 2229 290d 0a20 2020 2040 7472 6565  s)"))..    @tree
+0000e300: 5f6f 7065 7261 7469 6f6e 285f 2822 4170  _operation(_("Ap
+0000e310: 7065 6e64 2049 6e70 7574 2229 2c20 6e6f  pend Input"), no
+0000e320: 6465 5f74 7970 653d 2262 7261 6e63 6820  de_type="branch 
+0000e330: 6f70 7322 2c20 6865 6c70 3d22 2229 0d0a  ops", help="")..
+0000e340: 2020 2020 6465 6620 6170 7065 6e64 5f6f      def append_o
+0000e350: 7065 7261 7469 6f6e 5f69 6e70 7574 286e  peration_input(n
+0000e360: 6f64 652c 2070 6f73 3d4e 6f6e 652c 202a  ode, pos=None, *
+0000e370: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+0000e380: 2020 2073 656c 662e 6f70 5f62 7261 6e63     self.op_branc
+0000e390: 682e 6164 6428 0d0a 2020 2020 2020 2020  h.add(..        
+0000e3a0: 2020 2020 7479 7065 3d22 7574 696c 2069      type="util i
+0000e3b0: 6e70 7574 222c 0d0a 2020 2020 2020 2020  nput",..        
+0000e3c0: 2020 2020 706f 733d 706f 732c 0d0a 2020      pos=pos,..  
+0000e3d0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+0000e3e0: 6d61 736b 3d30 2c0d 0a20 2020 2020 2020  mask=0,..       
+0000e3f0: 2020 2020 2069 6e70 7574 5f76 616c 7565       input_value
+0000e400: 3d30 2c0d 0a20 2020 2020 2020 2020 2020  =0,..           
+0000e410: 2069 6e70 7574 5f6d 6573 7361 6765 3d4e   input_message=N
+0000e420: 6f6e 652c 0d0a 2020 2020 2020 2020 290d  one,..        ).
+0000e430: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
+0000e440: 676e 616c 2822 7570 6461 7465 6f70 5f74  gnal("updateop_t
+0000e450: 7265 6522 290d 0a0d 0a20 2020 2040 7472  ree")....    @tr
+0000e460: 6565 5f73 7562 6d65 6e75 285f 2822 4170  ee_submenu(_("Ap
+0000e470: 7065 6e64 2073 7065 6369 616c 206f 7065  pend special ope
+0000e480: 7261 7469 6f6e 2873 2922 2929 0d0a 2020  ration(s)"))..  
+0000e490: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
+0000e4a0: 6e28 5f28 2241 7070 656e 6420 486f 6d65  n(_("Append Home
+0000e4b0: 2f42 6565 702f 496e 7465 7272 7570 7422  /Beep/Interrupt"
+0000e4c0: 292c 206e 6f64 655f 7479 7065 3d22 6272  ), node_type="br
+0000e4d0: 616e 6368 206f 7073 222c 2068 656c 703d  anch ops", help=
+0000e4e0: 2222 290d 0a20 2020 2064 6566 2061 7070  "")..    def app
+0000e4f0: 656e 645f 6f70 6572 6174 696f 6e5f 686f  end_operation_ho
+0000e500: 6d65 5f62 6565 705f 696e 7465 7272 7570  me_beep_interrup
+0000e510: 7428 6e6f 6465 2c20 2a2a 6b77 6172 6773  t(node, **kwargs
+0000e520: 293a 0d0a 2020 2020 2020 2020 6170 7065  ):..        appe
+0000e530: 6e64 5f6f 7065 7261 7469 6f6e 5f68 6f6d  nd_operation_hom
+0000e540: 6528 6e6f 6465 2c20 2a2a 6b77 6172 6773  e(node, **kwargs
+0000e550: 290d 0a20 2020 2020 2020 2061 7070 656e  )..        appen
+0000e560: 645f 6f70 6572 6174 696f 6e5f 6265 6570  d_operation_beep
+0000e570: 286e 6f64 652c 202a 2a6b 7761 7267 7329  (node, **kwargs)
+0000e580: 0d0a 2020 2020 2020 2020 6170 7065 6e64  ..        append
+0000e590: 5f6f 7065 7261 7469 6f6e 5f69 6e74 6572  _operation_inter
+0000e5a0: 7275 7074 286e 6f64 652c 202a 2a6b 7761  rupt(node, **kwa
+0000e5b0: 7267 7329 0d0a 2020 2020 2020 2020 7365  rgs)..        se
+0000e5c0: 6c66 2e73 6967 6e61 6c28 2275 7064 6174  lf.signal("updat
+0000e5d0: 656f 705f 7472 6565 2229 0d0a 0d0a 2020  eop_tree")....  
+0000e5e0: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+0000e5f0: 5f28 2241 7070 656e 6420 7370 6563 6961  _("Append specia
+0000e600: 6c20 6f70 6572 6174 696f 6e28 7329 2229  l operation(s)")
+0000e610: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+0000e620: 7261 7469 6f6e 285f 2822 4170 7065 6e64  ration(_("Append
+0000e630: 204f 7269 6769 6e2f 4265 6570 2f49 6e74   Origin/Beep/Int
+0000e640: 6572 7275 7074 2229 2c20 6e6f 6465 5f74  errupt"), node_t
+0000e650: 7970 653d 2262 7261 6e63 6820 6f70 7322  ype="branch ops"
+0000e660: 2c20 6865 6c70 3d22 2229 0d0a 2020 2020  , help="")..    
+0000e670: 6465 6620 6170 7065 6e64 5f6f 7065 7261  def append_opera
+0000e680: 7469 6f6e 5f6f 7269 6769 6e5f 6265 6570  tion_origin_beep
+0000e690: 5f69 6e74 6572 7275 7074 286e 6f64 652c  _interrupt(node,
+0000e6a0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+0000e6b0: 2020 2020 2061 7070 656e 645f 6f70 6572       append_oper
+0000e6c0: 6174 696f 6e5f 676f 746f 286e 6f64 652c  ation_goto(node,
+0000e6d0: 202a 2a6b 7761 7267 7329 0d0a 2020 2020   **kwargs)..    
+0000e6e0: 2020 2020 6170 7065 6e64 5f6f 7065 7261      append_opera
+0000e6f0: 7469 6f6e 5f62 6565 7028 6e6f 6465 2c20  tion_beep(node, 
+0000e700: 2a2a 6b77 6172 6773 290d 0a20 2020 2020  **kwargs)..     
+0000e710: 2020 2061 7070 656e 645f 6f70 6572 6174     append_operat
+0000e720: 696f 6e5f 696e 7465 7272 7570 7428 6e6f  ion_interrupt(no
+0000e730: 6465 2c20 2a2a 6b77 6172 6773 290d 0a20  de, **kwargs).. 
+0000e740: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+0000e750: 616c 2822 7570 6461 7465 6f70 5f74 7265  al("updateop_tre
+0000e760: 6522 290d 0a0d 0a20 2020 2040 7472 6565  e")....    @tree
+0000e770: 5f73 7562 6d65 6e75 285f 2822 4170 7065  _submenu(_("Appe
+0000e780: 6e64 2073 7065 6369 616c 206f 7065 7261  nd special opera
+0000e790: 7469 6f6e 2873 2922 2929 0d0a 2020 2020  tion(s)"))..    
+0000e7a0: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+0000e7b0: 5f28 2241 7070 656e 6420 5368 7574 646f  _("Append Shutdo
+0000e7c0: 776e 2229 2c20 6e6f 6465 5f74 7970 653d  wn"), node_type=
+0000e7d0: 2262 7261 6e63 6820 6f70 7322 2c20 6865  "branch ops", he
+0000e7e0: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+0000e7f0: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
+0000e800: 5f73 6875 7464 6f77 6e28 6e6f 6465 2c20  _shutdown(node, 
+0000e810: 706f 733d 4e6f 6e65 2c20 2a2a 6b77 6172  pos=None, **kwar
+0000e820: 6773 293a 0d0a 2020 2020 2020 2020 7365  gs):..        se
+0000e830: 6c66 2e6f 705f 6272 616e 6368 2e61 6464  lf.op_branch.add
+0000e840: 280d 0a20 2020 2020 2020 2020 2020 2074  (..            t
+0000e850: 7970 653d 2275 7469 6c20 636f 6e73 6f6c  ype="util consol
+0000e860: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+0000e870: 2070 6f73 3d70 6f73 2c0d 0a20 2020 2020   pos=pos,..     
+0000e880: 2020 2020 2020 2063 6f6d 6d61 6e64 3d22         command="
+0000e890: 7175 6974 222c 0d0a 2020 2020 2020 2020  quit",..        
+0000e8a0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0000e8b0: 7369 676e 616c 2822 7570 6461 7465 6f70  signal("updateop
+0000e8c0: 5f74 7265 6522 290d 0a0d 0a20 2020 2040  _tree")....    @
+0000e8d0: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
+0000e8e0: 4170 7065 6e64 2073 7065 6369 616c 206f  Append special o
+0000e8f0: 7065 7261 7469 6f6e 2873 2922 2929 0d0a  peration(s)"))..
+0000e900: 2020 2020 4074 7265 655f 7072 6f6d 7074      @tree_prompt
+0000e910: 2822 6f70 6e61 6d65 222c 205f 2822 436f  ("opname", _("Co
+0000e920: 6e73 6f6c 6520 636f 6d6d 616e 6420 746f  nsole command to
+0000e930: 2061 7070 656e 6420 746f 206f 7065 7261   append to opera
+0000e940: 7469 6f6e 733f 2229 290d 0a20 2020 2040  tions?"))..    @
+0000e950: 7472 6565 5f6f 7065 7261 7469 6f6e 285f  tree_operation(_
+0000e960: 2822 4170 7065 6e64 2043 6f6e 736f 6c65  ("Append Console
+0000e970: 2229 2c20 6e6f 6465 5f74 7970 653d 2262  "), node_type="b
+0000e980: 7261 6e63 6820 6f70 7322 2c20 6865 6c70  ranch ops", help
+0000e990: 3d22 2229 0d0a 2020 2020 6465 6620 6170  ="")..    def ap
+0000e9a0: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f63  pend_operation_c
+0000e9b0: 7573 746f 6d28 6e6f 6465 2c20 6f70 6e61  ustom(node, opna
+0000e9c0: 6d65 2c20 706f 733d 4e6f 6e65 2c20 2a2a  me, pos=None, **
+0000e9d0: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+0000e9e0: 2020 7365 6c66 2e6f 705f 6272 616e 6368    self.op_branch
+0000e9f0: 2e61 6464 280d 0a20 2020 2020 2020 2020  .add(..         
+0000ea00: 2020 2074 7970 653d 2275 7469 6c20 636f     type="util co
+0000ea10: 6e73 6f6c 6522 2c0d 0a20 2020 2020 2020  nsole",..       
+0000ea20: 2020 2020 2070 6f73 3d70 6f73 2c0d 0a20       pos=pos,.. 
+0000ea30: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
+0000ea40: 6e64 3d6f 706e 616d 652c 0d0a 2020 2020  nd=opname,..    
+0000ea50: 2020 2020 290d 0a20 2020 2020 2020 2073      )..        s
+0000ea60: 656c 662e 7369 676e 616c 2822 7570 6461  elf.signal("upda
+0000ea70: 7465 6f70 5f74 7265 6522 290d 0a0d 0a20  teop_tree").... 
+0000ea80: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
+0000ea90: 285f 2822 4170 7065 6e64 2073 7065 6369  (_("Append speci
+0000eaa0: 616c 206f 7065 7261 7469 6f6e 2873 2922  al operation(s)"
+0000eab0: 2929 0d0a 2020 2020 4074 7265 655f 7072  ))..    @tree_pr
+0000eac0: 6f6d 7074 2822 7922 2c20 5f28 2259 2d43  ompt("y", _("Y-C
+0000ead0: 6f6f 7264 696e 6174 6520 666f 7220 706c  oordinate for pl
+0000eae0: 6163 656d 656e 7420 746f 2061 7070 656e  acement to appen
+0000eaf0: 643f 2229 290d 0a20 2020 2040 7472 6565  d?"))..    @tree
+0000eb00: 5f70 726f 6d70 7428 2278 222c 205f 2822  _prompt("x", _("
+0000eb10: 582d 436f 6f72 6469 6e61 7465 2066 6f72  X-Coordinate for
+0000eb20: 2070 6c61 6365 6d65 6e74 2074 6f20 6170   placement to ap
+0000eb30: 7065 6e64 3f22 2929 0d0a 2020 2020 4074  pend?"))..    @t
+0000eb40: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
+0000eb50: 2241 7070 656e 6420 506c 6163 656d 656e  "Append Placemen
+0000eb60: 7422 292c 206e 6f64 655f 7479 7065 3d22  t"), node_type="
+0000eb70: 6272 616e 6368 206f 7073 222c 2068 656c  branch ops", hel
+0000eb80: 703d 2222 290d 0a20 2020 2064 6566 2061  p="")..    def a
+0000eb90: 7070 656e 645f 6f70 6572 6174 696f 6e5f  ppend_operation_
+0000eba0: 706c 6163 656d 656e 7428 6e6f 6465 2c20  placement(node, 
+0000ebb0: 792c 2078 2c20 706f 733d 4e6f 6e65 2c20  y, x, pos=None, 
+0000ebc0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+0000ebd0: 2020 2020 7365 6c66 2e6f 705f 6272 616e      self.op_bran
+0000ebe0: 6368 2e61 6464 280d 0a20 2020 2020 2020  ch.add(..       
+0000ebf0: 2020 2020 2074 7970 653d 2270 6c61 6365       type="place
+0000ec00: 2070 6f69 6e74 222c 0d0a 2020 2020 2020   point",..      
+0000ec10: 2020 2020 2020 706f 733d 706f 732c 0d0a        pos=pos,..
+0000ec20: 2020 2020 2020 2020 2020 2020 783d 782c              x=x,
+0000ec30: 0d0a 2020 2020 2020 2020 2020 2020 793d  ..            y=
+0000ec40: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
+0000ec50: 726f 7461 7469 6f6e 3d30 2c0d 0a20 2020  rotation=0,..   
+0000ec60: 2020 2020 2020 2020 2063 6f72 6e65 723d           corner=
+0000ec70: 302c 0d0a 2020 2020 2020 2020 290d 0a20  0,..        ).. 
+0000ec80: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+0000ec90: 616c 2822 7570 6461 7465 6f70 5f74 7265  al("updateop_tre
+0000eca0: 6522 290d 0a0d 0a20 2020 2040 7472 6565  e")....    @tree
+0000ecb0: 5f6f 7065 7261 7469 6f6e 285f 2822 5265  _operation(_("Re
+0000ecc0: 636c 6173 7369 6679 206f 7065 7261 7469  classify operati
+0000ecd0: 6f6e 7322 292c 206e 6f64 655f 7479 7065  ons"), node_type
+0000ece0: 3d22 6272 616e 6368 2065 6c65 6d73 222c  ="branch elems",
+0000ecf0: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
+0000ed00: 6566 2072 6563 6c61 7373 6966 795f 6f70  ef reclassify_op
+0000ed10: 6572 6174 696f 6e73 286e 6f64 652c 202a  erations(node, *
+0000ed20: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+0000ed30: 2020 2065 6c65 6d73 203d 206c 6973 7428     elems = list(
+0000ed40: 7365 6c66 2e65 6c65 6d73 2829 290d 0a20  self.elems()).. 
+0000ed50: 2020 2020 2020 2073 656c 662e 7265 6d6f         self.remo
+0000ed60: 7665 5f65 6c65 6d65 6e74 735f 6672 6f6d  ve_elements_from
+0000ed70: 5f6f 7065 7261 7469 6f6e 7328 656c 656d  _operations(elem
+0000ed80: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
+0000ed90: 2e63 6c61 7373 6966 7928 6c69 7374 2873  .classify(list(s
+0000eda0: 656c 662e 656c 656d 7328 2929 290d 0a20  elf.elems())).. 
+0000edb0: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+0000edc0: 616c 2822 7265 6672 6573 685f 7472 6565  al("refresh_tree
+0000edd0: 2229 0d0a 0d0a 2020 2020 4074 7265 655f  ")....    @tree_
+0000ede0: 6f70 6572 6174 696f 6e28 0d0a 2020 2020  operation(..    
+0000edf0: 2020 2020 5f28 2252 656d 6f76 6520 616c      _("Remove al
+0000ee00: 6c20 6173 7369 676e 6d65 6e74 7320 6672  l assignments fr
+0000ee10: 6f6d 206f 7065 7261 7469 6f6e 7322 292c  om operations"),
+0000ee20: 0d0a 2020 2020 2020 2020 6e6f 6465 5f74  ..        node_t
+0000ee30: 7970 653d 2262 7261 6e63 6820 656c 656d  ype="branch elem
+0000ee40: 7322 2c0d 0a20 2020 2020 2020 2068 656c  s",..        hel
+0000ee50: 703d 5f28 2241 6e79 2065 7869 7374 696e  p=_("Any existin
+0000ee60: 6720 6173 7369 676e 6d65 6e74 206f 6620  g assignment of 
+0000ee70: 656c 656d 656e 7473 2074 6f20 6f70 6572  elements to oper
+0000ee80: 6174 696f 6e73 2077 696c 6c20 6265 2072  ations will be r
+0000ee90: 656d 6f76 6564 2229 2c0d 0a20 2020 2029  emoved"),..    )
+0000eea0: 0d0a 2020 2020 6465 6620 7265 6d6f 7665  ..    def remove
+0000eeb0: 5f61 6c6c 5f61 7373 6967 6e6d 656e 7473  _all_assignments
+0000eec0: 286e 6f64 652c 202a 2a6b 7761 7267 7329  (node, **kwargs)
+0000eed0: 3a0d 0a20 2020 2020 2020 2077 6974 6820  :..        with 
+0000eee0: 7365 6c66 2e73 7461 7469 6328 2272 656d  self.static("rem
+0000eef0: 6f76 655f 616c 6c5f 6173 7369 676e 2229  ove_all_assign")
+0000ef00: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+0000ef10: 6f72 206e 6f64 6520 696e 2073 656c 662e  or node in self.
+0000ef20: 656c 656d 7328 293a 0d0a 2020 2020 2020  elems():..      
+0000ef30: 2020 2020 2020 2020 2020 666f 7220 7265            for re
+0000ef40: 6620 696e 206c 6973 7428 6e6f 6465 2e72  f in list(node.r
+0000ef50: 6566 6572 656e 6365 7329 3a0d 0a20 2020  eferences):..   
 0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef70: 2020 2072 6566 2e72 656d 6f76 655f 6e6f     ref.remove_no
-0000ef80: 6465 2829 0d0a 2020 2020 2020 2020 7365  de()..        se
-0000ef90: 6c66 2e73 6967 6e61 6c28 2272 6566 7265  lf.signal("refre
-0000efa0: 7368 5f74 7265 6522 290d 0a0d 0a20 2020  sh_tree")....   
-0000efb0: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
-0000efc0: 280d 0a20 2020 2020 2020 205f 2822 4475  (..        _("Du
-0000efd0: 706c 6963 6174 6520 6f70 6572 6174 696f  plicate operatio
-0000efe0: 6e28 7329 2229 2c0d 0a20 2020 2020 2020  n(s)"),..       
-0000eff0: 206e 6f64 655f 7479 7065 3d6f 705f 6e6f   node_type=op_no
-0000f000: 6465 732c 0d0a 2020 2020 2020 2020 6865  des,..        he
-0000f010: 6c70 3d5f 2822 6475 706c 6963 6174 6520  lp=_("duplicate 
-0000f020: 6f70 6572 6174 696f 6e20 6e6f 6465 7322  operation nodes"
-0000f030: 292c 0d0a 2020 2020 290d 0a20 2020 2064  ),..    )..    d
-0000f040: 6566 2064 7570 6c69 6361 7465 5f6f 7065  ef duplicate_ope
-0000f050: 7261 7469 6f6e 286e 6f64 652c 202a 2a6b  ration(node, **k
-0000f060: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-0000f070: 2077 6974 6820 7365 6c66 2e73 7461 7469   with self.stati
-0000f080: 6328 2264 7570 6c69 6361 7465 5f6f 7065  c("duplicate_ope
-0000f090: 7261 7469 6f6e 2229 3a0d 0a20 2020 2020  ration"):..     
-0000f0a0: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
-0000f0b0: 7320 3d20 7365 6c66 2e5f 7472 6565 2e67  s = self._tree.g
-0000f0c0: 6574 2874 7970 653d 2262 7261 6e63 6820  et(type="branch 
-0000f0d0: 6f70 7322 292e 6368 696c 6472 656e 0d0a  ops").children..
-0000f0e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000f0f0: 6f70 2069 6e20 7365 6c66 2e6f 7073 2873  op in self.ops(s
-0000f100: 656c 6563 7465 643d 5472 7565 293a 0d0a  elected=True):..
-0000f110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f120: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0000f130: 2020 2020 2020 2020 2020 706f 7320 3d20            pos = 
-0000f140: 6f70 6572 6174 696f 6e73 2e69 6e64 6578  operations.index
-0000f150: 286f 7029 202b 2031 0d0a 2020 2020 2020  (op) + 1..      
-0000f160: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0000f170: 2056 616c 7565 4572 726f 723a 0d0a 2020   ValueError:..  
+0000ef70: 2072 6566 2e72 656d 6f76 655f 6e6f 6465   ref.remove_node
+0000ef80: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+0000ef90: 2e73 6967 6e61 6c28 2272 6566 7265 7368  .signal("refresh
+0000efa0: 5f74 7265 6522 290d 0a0d 0a20 2020 2040  _tree")....    @
+0000efb0: 7472 6565 5f6f 7065 7261 7469 6f6e 280d  tree_operation(.
+0000efc0: 0a20 2020 2020 2020 205f 2822 4475 706c  .        _("Dupl
+0000efd0: 6963 6174 6520 6f70 6572 6174 696f 6e28  icate operation(
+0000efe0: 7329 2229 2c0d 0a20 2020 2020 2020 206e  s)"),..        n
+0000eff0: 6f64 655f 7479 7065 3d6f 705f 6e6f 6465  ode_type=op_node
+0000f000: 732c 0d0a 2020 2020 2020 2020 6865 6c70  s,..        help
+0000f010: 3d5f 2822 6475 706c 6963 6174 6520 6f70  =_("duplicate op
+0000f020: 6572 6174 696f 6e20 6e6f 6465 7322 292c  eration nodes"),
+0000f030: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
+0000f040: 2064 7570 6c69 6361 7465 5f6f 7065 7261   duplicate_opera
+0000f050: 7469 6f6e 286e 6f64 652c 202a 2a6b 7761  tion(node, **kwa
+0000f060: 7267 7329 3a0d 0a20 2020 2020 2020 2077  rgs):..        w
+0000f070: 6974 6820 7365 6c66 2e73 7461 7469 6328  ith self.static(
+0000f080: 2264 7570 6c69 6361 7465 5f6f 7065 7261  "duplicate_opera
+0000f090: 7469 6f6e 2229 3a0d 0a20 2020 2020 2020  tion"):..       
+0000f0a0: 2020 2020 206f 7065 7261 7469 6f6e 7320       operations 
+0000f0b0: 3d20 7365 6c66 2e5f 7472 6565 2e67 6574  = self._tree.get
+0000f0c0: 2874 7970 653d 2262 7261 6e63 6820 6f70  (type="branch op
+0000f0d0: 7322 292e 6368 696c 6472 656e 0d0a 2020  s").children..  
+0000f0e0: 2020 2020 2020 2020 2020 666f 7220 6f70            for op
+0000f0f0: 2069 6e20 7365 6c66 2e6f 7073 2873 656c   in self.ops(sel
+0000f100: 6563 7465 643d 5472 7565 293a 0d0a 2020  ected=True):..  
+0000f110: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000f120: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000f130: 2020 2020 2020 2020 706f 7320 3d20 6f70          pos = op
+0000f140: 6572 6174 696f 6e73 2e69 6e64 6578 286f  erations.index(o
+0000f150: 7029 202b 2031 0d0a 2020 2020 2020 2020  p) + 1..        
+0000f160: 2020 2020 2020 2020 6578 6365 7074 2056          except V
+0000f170: 616c 7565 4572 726f 723a 0d0a 2020 2020  alueError:..    
 0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f190: 2020 706f 7320 3d20 4e6f 6e65 0d0a 2020    pos = None..  
-0000f1a0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000f1b0: 7079 5f6f 7020 3d20 636f 7079 286f 7029  py_op = copy(op)
-0000f1c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f1d0: 2020 7365 6c66 2e61 6464 5f6f 7028 636f    self.add_op(co
-0000f1e0: 7079 5f6f 702c 2070 6f73 3d70 6f73 290d  py_op, pos=pos).
-0000f1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f200: 2066 6f72 2063 6869 6c64 2069 6e20 6f70   for child in op
-0000f210: 2e63 6869 6c64 7265 6e3a 0d0a 2020 2020  .children:..    
-0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f230: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0000f240: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000f250: 7079 5f6f 702e 6164 645f 7265 6665 7265  py_op.add_refere
-0000f260: 6e63 6528 6368 696c 642e 6e6f 6465 290d  nce(child.node).
-0000f270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f280: 2020 2020 2065 7863 6570 7420 4174 7472       except Attr
-0000f290: 6962 7574 6545 7272 6f72 3a0d 0a20 2020  ibuteError:..   
+0000f190: 706f 7320 3d20 4e6f 6e65 0d0a 2020 2020  pos = None..    
+0000f1a0: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+0000f1b0: 5f6f 7020 3d20 636f 7079 286f 7029 0d0a  _op = copy(op)..
+0000f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1d0: 7365 6c66 2e61 6464 5f6f 7028 636f 7079  self.add_op(copy
+0000f1e0: 5f6f 702c 2070 6f73 3d70 6f73 290d 0a20  _op, pos=pos).. 
+0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f200: 6f72 2063 6869 6c64 2069 6e20 6f70 2e63  or child in op.c
+0000f210: 6869 6c64 7265 6e3a 0d0a 2020 2020 2020  hildren:..      
+0000f220: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0000f230: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0000f240: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+0000f250: 5f6f 702e 6164 645f 7265 6665 7265 6e63  _op.add_referenc
+0000f260: 6528 6368 696c 642e 6e6f 6465 290d 0a20  e(child.node).. 
+0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f280: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
+0000f290: 7574 6545 7272 6f72 3a0d 0a20 2020 2020  uteError:..     
 0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2b0: 2020 2020 2070 6173 730d 0a0d 0a20 2020       pass....   
-0000f2c0: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
-0000f2d0: 616c 286c 616d 6264 6120 6e6f 6465 3a20  al(lambda node: 
-0000f2e0: 6e6f 6465 2e63 6f75 6e74 5f63 6869 6c64  node.count_child
-0000f2f0: 7265 6e28 2920 3e20 3129 0d0a 2020 2020  ren() > 1)..    
-0000f300: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
-0000f310: 2250 6173 7365 7322 2929 0d0a 2020 2020  "Passes"))..    
-0000f320: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
-0000f330: 0d0a 2020 2020 2020 2020 5f28 2241 6464  ..        _("Add
-0000f340: 2031 2070 6173 7322 292c 0d0a 2020 2020   1 pass"),..    
-0000f350: 2020 2020 6e6f 6465 5f74 7970 653d 2822      node_type=("
-0000f360: 6f70 2069 6d61 6765 222c 2022 6f70 2065  op image", "op e
-0000f370: 6e67 7261 7665 222c 2022 6f70 2063 7574  ngrave", "op cut
-0000f380: 222c 2022 6f70 2068 6174 6368 2229 2c0d  ", "op hatch"),.
-0000f390: 0a20 2020 2020 2020 2068 656c 703d 2222  .        help=""
-0000f3a0: 2c0d 0a20 2020 2029 0d0a 2020 2020 6465  ,..    )..    de
-0000f3b0: 6620 6164 645f 315f 7061 7373 286e 6f64  f add_1_pass(nod
-0000f3c0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-0000f3d0: 2020 2020 2020 2061 6464 5f6e 5f70 6173         add_n_pas
-0000f3e0: 7365 7328 6e6f 6465 2c20 636f 7069 6573  ses(node, copies
-0000f3f0: 3d31 2c20 2a2a 6b77 6172 6773 290d 0a0d  =1, **kwargs)...
-0000f400: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
-0000f410: 7469 6f6e 616c 286c 616d 6264 6120 6e6f  tional(lambda no
-0000f420: 6465 3a20 6e6f 6465 2e63 6f75 6e74 5f63  de: node.count_c
-0000f430: 6869 6c64 7265 6e28 2920 3e20 3129 0d0a  hildren() > 1)..
-0000f440: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-0000f450: 7528 5f28 2250 6173 7365 7322 2929 0d0a  u(_("Passes"))..
-0000f460: 2020 2020 4074 7265 655f 6974 6572 6174      @tree_iterat
-0000f470: 6528 2263 6f70 6965 7322 2c20 322c 2031  e("copies", 2, 1
-0000f480: 3029 0d0a 2020 2020 4074 7265 655f 6f70  0)..    @tree_op
-0000f490: 6572 6174 696f 6e28 0d0a 2020 2020 2020  eration(..      
-0000f4a0: 2020 5f28 2241 6464 207b 636f 7069 6573    _("Add {copies
-0000f4b0: 7d20 7061 7373 6573 2229 2c0d 0a20 2020  } passes"),..   
-0000f4c0: 2020 2020 206e 6f64 655f 7479 7065 3d28       node_type=(
-0000f4d0: 226f 7020 696d 6167 6522 2c20 226f 7020  "op image", "op 
-0000f4e0: 656e 6772 6176 6522 2c20 226f 7020 6375  engrave", "op cu
-0000f4f0: 7422 2c20 226f 7020 6861 7463 6822 292c  t", "op hatch"),
-0000f500: 0d0a 2020 2020 2020 2020 6865 6c70 3d22  ..        help="
-0000f510: 222c 0d0a 2020 2020 290d 0a20 2020 2064  ",..    )..    d
-0000f520: 6566 2061 6464 5f6e 5f70 6173 7365 7328  ef add_n_passes(
-0000f530: 6e6f 6465 2c20 636f 7069 6573 3d31 2c20  node, copies=1, 
-0000f540: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-0000f550: 2020 2020 6164 645f 6e6f 6465 7320 3d20      add_nodes = 
-0000f560: 6c69 7374 286e 6f64 652e 6368 696c 6472  list(node.childr
-0000f570: 656e 290d 0a0d 0a20 2020 2020 2020 2072  en)....        r
-0000f580: 656d 6f76 6564 203d 2046 616c 7365 0d0a  emoved = False..
-0000f590: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0000f5a0: 2072 616e 6765 2830 2c20 6c65 6e28 6164   range(0, len(ad
-0000f5b0: 645f 6e6f 6465 7329 293a 0d0a 2020 2020  d_nodes)):..    
-0000f5c0: 2020 2020 2020 2020 666f 7220 7120 696e          for q in
-0000f5d0: 2072 616e 6765 2830 2c20 6929 3a0d 0a20   range(0, i):.. 
-0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f5f0: 6620 6164 645f 6e6f 6465 735b 715d 2069  f add_nodes[q] i
-0000f600: 7320 6164 645f 6e6f 6465 735b 695d 3a0d  s add_nodes[i]:.
-0000f610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f620: 2020 2020 2061 6464 5f6e 6f64 6573 5b69       add_nodes[i
-0000f630: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 2020  ] = None..      
-0000f640: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000f650: 6d6f 7665 6420 3d20 5472 7565 0d0a 2020  moved = True..  
-0000f660: 2020 2020 2020 6966 2072 656d 6f76 6564        if removed
-0000f670: 3a0d 0a20 2020 2020 2020 2020 2020 2061  :..            a
-0000f680: 6464 5f6e 6f64 6573 203d 205b 6320 666f  dd_nodes = [c fo
-0000f690: 7220 6320 696e 2061 6464 5f6e 6f64 6573  r c in add_nodes
-0000f6a0: 2069 6620 6320 6973 206e 6f74 204e 6f6e   if c is not Non
-0000f6b0: 655d 0d0a 2020 2020 2020 2020 6164 645f  e]..        add_
-0000f6c0: 6e6f 6465 7320 2a3d 2063 6f70 6965 730d  nodes *= copies.
-0000f6d0: 0a20 2020 2020 2020 2066 6f72 206e 2069  .        for n i
-0000f6e0: 6e20 6164 645f 6e6f 6465 733a 0d0a 2020  n add_nodes:..  
-0000f6f0: 2020 2020 2020 2020 2020 6e6f 6465 2e61            node.a
-0000f700: 6464 5f72 6566 6572 656e 6365 286e 2e6e  dd_reference(n.n
-0000f710: 6f64 6529 0d0a 2020 2020 2020 2020 7365  ode)..        se
-0000f720: 6c66 2e73 6967 6e61 6c28 2272 6562 7569  lf.signal("rebui
-0000f730: 6c64 5f74 7265 6522 290d 0a0d 0a20 2020  ld_tree")....   
-0000f740: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
-0000f750: 616c 286c 616d 6264 6120 6e6f 6465 3a20  al(lambda node: 
-0000f760: 6e6f 6465 2e63 6f75 6e74 5f63 6869 6c64  node.count_child
-0000f770: 7265 6e28 2920 3e20 3129 0d0a 2020 2020  ren() > 1)..    
-0000f780: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
-0000f790: 2244 7570 6c69 6361 7465 2065 6c65 6d65  "Duplicate eleme
-0000f7a0: 6e74 2873 2922 2929 0d0a 2020 2020 4074  nt(s)"))..    @t
-0000f7b0: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
-0000f7c0: 2020 2020 2020 2020 5f28 2244 7570 6c69          _("Dupli
-0000f7d0: 6361 7465 2065 6c65 6d65 6e74 7320 3120  cate elements 1 
-0000f7e0: 7469 6d65 2229 2c0d 0a20 2020 2020 2020  time"),..       
-0000f7f0: 206e 6f64 655f 7479 7065 3d28 226f 7020   node_type=("op 
-0000f800: 696d 6167 6522 2c20 226f 7020 656e 6772  image", "op engr
-0000f810: 6176 6522 2c20 226f 7020 6375 7422 292c  ave", "op cut"),
-0000f820: 0d0a 2020 2020 2020 2020 6865 6c70 3d22  ..        help="
-0000f830: 222c 0d0a 2020 2020 290d 0a20 2020 2064  ",..    )..    d
-0000f840: 6566 2064 7570 5f31 5f63 6f70 7928 6e6f  ef dup_1_copy(no
-0000f850: 6465 2c20 2a2a 6b77 6172 6773 293a 0d0a  de, **kwargs):..
-0000f860: 2020 2020 2020 2020 6475 705f 6e5f 636f          dup_n_co
-0000f870: 7069 6573 286e 6f64 652c 2063 6f70 6965  pies(node, copie
-0000f880: 733d 312c 202a 2a6b 7761 7267 7329 0d0a  s=1, **kwargs)..
-0000f890: 0d0a 2020 2020 4074 7265 655f 636f 6e64  ..    @tree_cond
-0000f8a0: 6974 696f 6e61 6c28 6c61 6d62 6461 206e  itional(lambda n
-0000f8b0: 6f64 653a 206e 6f64 652e 636f 756e 745f  ode: node.count_
-0000f8c0: 6368 696c 6472 656e 2829 203e 2031 290d  children() > 1).
-0000f8d0: 0a20 2020 2040 7472 6565 5f73 7562 6d65  .    @tree_subme
-0000f8e0: 6e75 285f 2822 4475 706c 6963 6174 6520  nu(_("Duplicate 
-0000f8f0: 656c 656d 656e 7428 7329 2229 290d 0a20  element(s)")).. 
-0000f900: 2020 2040 7472 6565 5f69 7465 7261 7465     @tree_iterate
-0000f910: 2822 636f 7069 6573 222c 2032 2c20 3130  ("copies", 2, 10
-0000f920: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
-0000f930: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
-0000f940: 205f 2822 4475 706c 6963 6174 6520 656c   _("Duplicate el
-0000f950: 656d 656e 7473 207b 636f 7069 6573 7d20  ements {copies} 
-0000f960: 7469 6d65 7322 292c 0d0a 2020 2020 2020  times"),..      
-0000f970: 2020 6e6f 6465 5f74 7970 653d 2822 6f70    node_type=("op
-0000f980: 2069 6d61 6765 222c 2022 6f70 2065 6e67   image", "op eng
-0000f990: 7261 7665 222c 2022 6f70 2063 7574 2229  rave", "op cut")
-0000f9a0: 2c0d 0a20 2020 2020 2020 2068 656c 703d  ,..        help=
-0000f9b0: 2222 2c0d 0a20 2020 2029 0d0a 2020 2020  "",..    )..    
-0000f9c0: 6465 6620 6475 705f 6e5f 636f 7069 6573  def dup_n_copies
-0000f9d0: 286e 6f64 652c 2063 6f70 6965 733d 312c  (node, copies=1,
-0000f9e0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-0000f9f0: 2020 2020 2023 2043 6f64 6520 696e 2073       # Code in s
-0000fa00: 6572 6965 732e 0d0a 2020 2020 2020 2020  eries...        
-0000fa10: 2320 6164 645f 6e6f 6465 7320 3d20 6c69  # add_nodes = li
-0000fa20: 7374 286e 6f64 652e 6368 696c 6472 656e  st(node.children
-0000fa30: 290d 0a20 2020 2020 2020 2023 2061 6464  )..        # add
-0000fa40: 5f6e 6f64 6573 202a 3d20 636f 7069 6573  _nodes *= copies
-0000fa50: 0d0a 2020 2020 2020 2020 2320 666f 7220  ..        # for 
-0000fa60: 6e20 696e 2061 6464 5f6e 6f64 6573 3a0d  n in add_nodes:.
-0000fa70: 0a20 2020 2020 2020 2023 2020 2020 206e  .        #     n
-0000fa80: 6f64 652e 6164 645f 7265 6665 7265 6e63  ode.add_referenc
-0000fa90: 6528 6e2e 6e6f 6465 290d 0a0d 0a20 2020  e(n.node)....   
-0000faa0: 2020 2020 2023 2043 6f64 6520 696e 2070       # Code in p
-0000fab0: 6172 616c 6c65 6c2e 0d0a 2020 2020 2020  arallel...      
-0000fac0: 2020 6164 645f 6e6f 6465 7320 3d20 6c69    add_nodes = li
-0000fad0: 7374 286e 6f64 652e 6368 696c 6472 656e  st(node.children
-0000fae0: 290d 0a20 2020 2020 2020 2066 6f72 2069  )..        for i
-0000faf0: 2069 6e20 7261 6e67 6528 6c65 6e28 6164   in range(len(ad
-0000fb00: 645f 6e6f 6465 7329 202d 2031 2c20 2d31  d_nodes) - 1, -1
-0000fb10: 2c20 2d31 293a 0d0a 2020 2020 2020 2020  , -1):..        
-0000fb20: 2020 2020 6e20 3d20 6164 645f 6e6f 6465      n = add_node
-0000fb30: 735b 695d 0d0a 2020 2020 2020 2020 2020  s[i]..          
-0000fb40: 2020 666f 7220 6b20 696e 2072 616e 6765    for k in range
-0000fb50: 2863 6f70 6965 7329 3a0d 0a20 2020 2020  (copies):..     
-0000fb60: 2020 2020 2020 2020 2020 206e 6f64 652e             node.
-0000fb70: 6164 645f 7265 6665 7265 6e63 6528 6e2e  add_reference(n.
-0000fb80: 6e6f 6465 2c20 706f 733d 6929 0d0a 0d0a  node, pos=i)....
-0000fb90: 2020 2020 2020 2020 7365 6c66 2e73 6967          self.sig
-0000fba0: 6e61 6c28 2272 6566 7265 7368 5f74 7265  nal("refresh_tre
-0000fbb0: 6522 290d 0a0d 0a20 2020 2040 7472 6565  e")....    @tree
-0000fbc0: 5f6f 7065 7261 7469 6f6e 280d 0a20 2020  _operation(..   
-0000fbd0: 2020 2020 205f 2822 4d61 6b65 2072 6173       _("Make ras
-0000fbe0: 7465 7220 696d 6167 6522 292c 0d0a 2020  ter image"),..  
-0000fbf0: 2020 2020 2020 6e6f 6465 5f74 7970 653d        node_type=
-0000fc00: 2822 6f70 2069 6d61 6765 222c 2022 6f70  ("op image", "op
-0000fc10: 2072 6173 7465 7222 292c 0d0a 2020 2020   raster"),..    
-0000fc20: 2020 2020 6865 6c70 3d5f 2822 4372 6561      help=_("Crea
-0000fc30: 7465 2061 6e20 696d 6167 6520 6672 6f6d  te an image from
-0000fc40: 2074 6865 2061 7373 6967 6e65 6420 656c   the assigned el
-0000fc50: 656d 656e 7473 2e22 292c 0d0a 2020 2020  ements."),..    
-0000fc60: 290d 0a20 2020 2064 6566 206d 616b 655f  )..    def make_
-0000fc70: 7261 7374 6572 5f69 6d61 6765 286e 6f64  raster_image(nod
-0000fc80: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-0000fc90: 2020 2020 2020 2064 6174 6120 3d20 6c69         data = li
-0000fca0: 7374 286e 6f64 652e 666c 6174 2874 7970  st(node.flat(typ
-0000fcb0: 6573 3d65 6c65 6d5f 7265 665f 6e6f 6465  es=elem_ref_node
-0000fcc0: 7329 290d 0a20 2020 2020 2020 2069 6620  s))..        if 
-0000fcd0: 6c65 6e28 6461 7461 2920 3d3d 2030 3a0d  len(data) == 0:.
-0000fce0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000fcf0: 7572 6e0d 0a20 2020 2020 2020 2074 7279  urn..        try
-0000fd00: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
-0000fd10: 6f75 6e64 7320 3d20 4e6f 6465 2e75 6e69  ounds = Node.uni
-0000fd20: 6f6e 5f62 6f75 6e64 7328 6461 7461 2c20  on_bounds(data, 
-0000fd30: 6174 7472 3d22 7061 696e 745f 626f 756e  attr="paint_boun
-0000fd40: 6473 2229 0d0a 2020 2020 2020 2020 2020  ds")..          
-0000fd50: 2020 7769 6474 6820 3d20 626f 756e 6473    width = bounds
-0000fd60: 5b32 5d20 2d20 626f 756e 6473 5b30 5d0d  [2] - bounds[0].
-0000fd70: 0a20 2020 2020 2020 2020 2020 2068 6569  .            hei
-0000fd80: 6768 7420 3d20 626f 756e 6473 5b33 5d20  ght = bounds[3] 
-0000fd90: 2d20 626f 756e 6473 5b31 5d0d 0a20 2020  - bounds[1]..   
-0000fda0: 2020 2020 2065 7863 6570 7420 5479 7065       except Type
-0000fdb0: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-0000fdc0: 2020 2020 7261 6973 6520 436f 6d6d 616e      raise Comman
-0000fdd0: 6453 796e 7461 7845 7272 6f72 0d0a 2020  dSyntaxError..  
-0000fde0: 2020 2020 2020 6d61 6b65 5f72 6173 7465        make_raste
-0000fdf0: 7220 3d20 7365 6c66 2e6c 6f6f 6b75 7028  r = self.lookup(
-0000fe00: 2272 656e 6465 722d 6f70 2f6d 616b 655f  "render-op/make_
-0000fe10: 7261 7374 6572 2229 0d0a 2020 2020 2020  raster")..      
-0000fe20: 2020 6966 206e 6f74 206d 616b 655f 7261    if not make_ra
-0000fe30: 7374 6572 3a0d 0a20 2020 2020 2020 2020  ster:..         
-0000fe40: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-0000fe50: 726f 7228 224e 6f20 7265 6e64 6572 6572  ror("No renderer
-0000fe60: 2069 7320 7265 6769 7374 6572 6564 2074   is registered t
-0000fe70: 6f20 7065 7266 6f72 6d20 7265 6e64 6572  o perform render
-0000fe80: 2e22 290d 0a0d 0a20 2020 2020 2020 2064  .")....        d
-0000fe90: 6f74 735f 7065 725f 756e 6974 7320 3d20  ots_per_units = 
-0000fea0: 6e6f 6465 2e64 7069 202f 2055 4e49 5453  node.dpi / UNITS
-0000feb0: 5f50 4552 5f49 4e43 480d 0a20 2020 2020  _PER_INCH..     
-0000fec0: 2020 206e 6577 5f77 6964 7468 203d 2077     new_width = w
-0000fed0: 6964 7468 202a 2064 6f74 735f 7065 725f  idth * dots_per_
-0000fee0: 756e 6974 730d 0a20 2020 2020 2020 206e  units..        n
-0000fef0: 6577 5f68 6569 6768 7420 3d20 6865 6967  ew_height = heig
-0000ff00: 6874 202a 2064 6f74 735f 7065 725f 756e  ht * dots_per_un
-0000ff10: 6974 730d 0a0d 0a20 2020 2020 2020 2069  its....        i
-0000ff20: 6d61 6765 203d 206d 616b 655f 7261 7374  mage = make_rast
-0000ff30: 6572 280d 0a20 2020 2020 2020 2020 2020  er(..           
-0000ff40: 2064 6174 612c 0d0a 2020 2020 2020 2020   data,..        
-0000ff50: 2020 2020 626f 756e 6473 3d62 6f75 6e64      bounds=bound
-0000ff60: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0000ff70: 7769 6474 683d 6e65 775f 7769 6474 682c  width=new_width,
-0000ff80: 0d0a 2020 2020 2020 2020 2020 2020 6865  ..            he
-0000ff90: 6967 6874 3d6e 6577 5f68 6569 6768 742c  ight=new_height,
-0000ffa0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-0000ffb0: 2020 2020 206d 6174 7269 7820 3d20 4d61       matrix = Ma
-0000ffc0: 7472 6978 2e73 6361 6c65 2877 6964 7468  trix.scale(width
-0000ffd0: 202f 206e 6577 5f77 6964 7468 2c20 6865   / new_width, he
-0000ffe0: 6967 6874 202f 206e 6577 5f68 6569 6768  ight / new_heigh
-0000fff0: 7429 0d0a 2020 2020 2020 2020 6d61 7472  t)..        matr
-00010000: 6978 2e70 6f73 745f 7472 616e 736c 6174  ix.post_translat
-00010010: 6528 626f 756e 6473 5b30 5d2c 2062 6f75  e(bounds[0], bou
-00010020: 6e64 735b 315d 290d 0a0d 0a20 2020 2020  nds[1])....     
-00010030: 2020 2069 6d61 6765 5f6e 6f64 6520 3d20     image_node = 
-00010040: 496d 6167 654e 6f64 6528 696d 6167 653d  ImageNode(image=
-00010050: 696d 6167 652c 206d 6174 7269 783d 6d61  image, matrix=ma
-00010060: 7472 6978 2c20 6470 693d 6e6f 6465 2e64  trix, dpi=node.d
-00010070: 7069 290d 0a20 2020 2020 2020 2073 656c  pi)..        sel
-00010080: 662e 656c 656d 5f62 7261 6e63 682e 6164  f.elem_branch.ad
-00010090: 645f 6e6f 6465 2869 6d61 6765 5f6e 6f64  d_node(image_nod
-000100a0: 6529 0d0a 2020 2020 2020 2020 6e6f 6465  e)..        node
-000100b0: 2e61 6464 5f72 6566 6572 656e 6365 2869  .add_reference(i
-000100c0: 6d61 6765 5f6e 6f64 6529 0d0a 2020 2020  mage_node)..    
-000100d0: 2020 2020 7365 6c66 2e73 6967 6e61 6c28      self.signal(
-000100e0: 2272 6566 7265 7368 5f73 6365 6e65 222c  "refresh_scene",
-000100f0: 2022 5363 656e 6522 290d 0a0d 0a20 2020   "Scene")....   
-00010100: 2064 6566 2061 6464 5f61 6674 6572 5f69   def add_after_i
-00010110: 6e64 6578 286e 6f64 653d 4e6f 6e65 293a  ndex(node=None):
-00010120: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00010130: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00010140: 6f64 6520 6973 204e 6f6e 653a 0d0a 2020  ode is None:..  
-00010150: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00010160: 6465 203d 206c 6973 7428 7365 6c66 2e6f  de = list(self.o
-00010170: 7073 2873 656c 6563 7465 643d 5472 7565  ps(selected=True
-00010180: 2929 5b2d 315d 0d0a 2020 2020 2020 2020  ))[-1]..        
-00010190: 2020 2020 6f70 6572 6174 696f 6e73 203d      operations =
-000101a0: 2073 656c 662e 5f74 7265 652e 6765 7428   self._tree.get(
-000101b0: 7479 7065 3d22 6272 616e 6368 206f 7073  type="branch ops
-000101c0: 2229 2e63 6869 6c64 7265 6e0d 0a20 2020  ").children..   
-000101d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000101e0: 6f70 6572 6174 696f 6e73 2e69 6e64 6578  operations.index
-000101f0: 286e 6f64 6529 202b 2031 0d0a 2020 2020  (node) + 1..    
-00010200: 2020 2020 6578 6365 7074 2028 5661 6c75      except (Valu
-00010210: 6545 7272 6f72 2c20 496e 6465 7845 7272  eError, IndexErr
-00010220: 6f72 293a 0d0a 2020 2020 2020 2020 2020  or):..          
-00010230: 2020 7265 7475 726e 204e 6f6e 650d 0a0d    return None...
-00010240: 0a20 2020 2040 7472 6565 5f73 6570 6172  .    @tree_separ
-00010250: 6174 6f72 5f62 6566 6f72 6528 290d 0a20  ator_before().. 
-00010260: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
-00010270: 285f 2822 496e 7365 7274 206f 7065 7261  (_("Insert opera
-00010280: 7469 6f6e 2229 290d 0a20 2020 2040 7472  tion"))..    @tr
-00010290: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-000102a0: 4164 6420 496d 6167 6522 292c 206e 6f64  Add Image"), nod
-000102b0: 655f 7479 7065 3d6f 705f 6e6f 6465 732c  e_type=op_nodes,
-000102c0: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-000102d0: 6566 2061 6464 5f6f 7065 7261 7469 6f6e  ef add_operation
-000102e0: 5f69 6d61 6765 286e 6f64 652c 202a 2a6b  _image(node, **k
-000102f0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00010300: 2061 7070 656e 645f 6f70 6572 6174 696f   append_operatio
-00010310: 6e5f 696d 6167 6528 6e6f 6465 2c20 706f  n_image(node, po
-00010320: 733d 6164 645f 6166 7465 725f 696e 6465  s=add_after_inde
-00010330: 7828 6e6f 6465 292c 202a 2a6b 7761 7267  x(node), **kwarg
-00010340: 7329 0d0a 0d0a 2020 2020 4074 7265 655f  s)....    @tree_
-00010350: 7375 626d 656e 7528 5f28 2249 6e73 6572  submenu(_("Inser
-00010360: 7420 6f70 6572 6174 696f 6e22 2929 0d0a  t operation"))..
-00010370: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-00010380: 696f 6e28 5f28 2241 6464 2052 6173 7465  ion(_("Add Raste
-00010390: 7222 292c 206e 6f64 655f 7479 7065 3d6f  r"), node_type=o
-000103a0: 705f 6e6f 6465 732c 2068 656c 703d 2222  p_nodes, help=""
-000103b0: 290d 0a20 2020 2064 6566 2061 6464 5f6f  )..    def add_o
-000103c0: 7065 7261 7469 6f6e 5f72 6173 7465 7228  peration_raster(
-000103d0: 6e6f 6465 2c20 2a2a 6b77 6172 6773 293a  node, **kwargs):
-000103e0: 0d0a 2020 2020 2020 2020 6170 7065 6e64  ..        append
-000103f0: 5f6f 7065 7261 7469 6f6e 5f72 6173 7465  _operation_raste
-00010400: 7228 6e6f 6465 2c20 706f 733d 6164 645f  r(node, pos=add_
-00010410: 6166 7465 725f 696e 6465 7828 6e6f 6465  after_index(node
-00010420: 292c 202a 2a6b 7761 7267 7329 0d0a 0d0a  ), **kwargs)....
-00010430: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-00010440: 7528 5f28 2249 6e73 6572 7420 6f70 6572  u(_("Insert oper
-00010450: 6174 696f 6e22 2929 0d0a 2020 2020 4074  ation"))..    @t
-00010460: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
-00010470: 2241 6464 2045 6e67 7261 7665 2229 2c20  "Add Engrave"), 
-00010480: 6e6f 6465 5f74 7970 653d 6f70 5f6e 6f64  node_type=op_nod
-00010490: 6573 2c20 6865 6c70 3d22 2229 0d0a 2020  es, help="")..  
-000104a0: 2020 6465 6620 6164 645f 6f70 6572 6174    def add_operat
-000104b0: 696f 6e5f 656e 6772 6176 6528 6e6f 6465  ion_engrave(node
-000104c0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
-000104d0: 2020 2020 2020 6170 7065 6e64 5f6f 7065        append_ope
-000104e0: 7261 7469 6f6e 5f65 6e67 7261 7665 286e  ration_engrave(n
-000104f0: 6f64 652c 2070 6f73 3d61 6464 5f61 6674  ode, pos=add_aft
-00010500: 6572 5f69 6e64 6578 286e 6f64 6529 2c20  er_index(node), 
-00010510: 2a2a 6b77 6172 6773 290d 0a0d 0a20 2020  **kwargs)....   
-00010520: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
-00010530: 2822 496e 7365 7274 206f 7065 7261 7469  ("Insert operati
-00010540: 6f6e 2229 290d 0a20 2020 2040 7472 6565  on"))..    @tree
-00010550: 5f6f 7065 7261 7469 6f6e 285f 2822 4164  _operation(_("Ad
-00010560: 6420 4375 7422 292c 206e 6f64 655f 7479  d Cut"), node_ty
-00010570: 7065 3d6f 705f 6e6f 6465 732c 2068 656c  pe=op_nodes, hel
-00010580: 703d 2222 290d 0a20 2020 2064 6566 2061  p="")..    def a
-00010590: 6464 5f6f 7065 7261 7469 6f6e 5f63 7574  dd_operation_cut
-000105a0: 286e 6f64 652c 202a 2a6b 7761 7267 7329  (node, **kwargs)
-000105b0: 3a0d 0a20 2020 2020 2020 2061 7070 656e  :..        appen
-000105c0: 645f 6f70 6572 6174 696f 6e5f 6375 7428  d_operation_cut(
-000105d0: 6e6f 6465 2c20 706f 733d 6164 645f 6166  node, pos=add_af
-000105e0: 7465 725f 696e 6465 7828 6e6f 6465 292c  ter_index(node),
-000105f0: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
-00010600: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
-00010610: 5f28 2249 6e73 6572 7420 6f70 6572 6174  _("Insert operat
-00010620: 696f 6e22 2929 0d0a 2020 2020 4074 7265  ion"))..    @tre
-00010630: 655f 6f70 6572 6174 696f 6e28 5f28 2241  e_operation(_("A
-00010640: 6464 2048 6174 6368 2229 2c20 6e6f 6465  dd Hatch"), node
-00010650: 5f74 7970 653d 6f70 5f6e 6f64 6573 2c20  _type=op_nodes, 
-00010660: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
-00010670: 6620 6164 645f 6f70 6572 6174 696f 6e5f  f add_operation_
-00010680: 6861 7463 6828 6e6f 6465 2c20 2a2a 6b77  hatch(node, **kw
-00010690: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-000106a0: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
-000106b0: 5f68 6174 6368 286e 6f64 652c 2070 6f73  _hatch(node, pos
-000106c0: 3d61 6464 5f61 6674 6572 5f69 6e64 6578  =add_after_index
-000106d0: 286e 6f64 6529 2c20 2a2a 6b77 6172 6773  (node), **kwargs
-000106e0: 290d 0a0d 0a20 2020 2040 7472 6565 5f73  )....    @tree_s
-000106f0: 7562 6d65 6e75 285f 2822 496e 7365 7274  ubmenu(_("Insert
-00010700: 206f 7065 7261 7469 6f6e 2229 290d 0a20   operation")).. 
-00010710: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-00010720: 6f6e 285f 2822 4164 6420 446f 7473 2229  on(_("Add Dots")
-00010730: 2c20 6e6f 6465 5f74 7970 653d 6f70 5f6e  , node_type=op_n
-00010740: 6f64 6573 2c20 6865 6c70 3d22 2229 0d0a  odes, help="")..
-00010750: 2020 2020 6465 6620 6164 645f 6f70 6572      def add_oper
-00010760: 6174 696f 6e5f 646f 7473 286e 6f64 652c  ation_dots(node,
-00010770: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00010780: 2020 2020 2061 7070 656e 645f 6f70 6572       append_oper
-00010790: 6174 696f 6e5f 646f 7473 286e 6f64 652c  ation_dots(node,
-000107a0: 2070 6f73 3d61 6464 5f61 6674 6572 5f69   pos=add_after_i
-000107b0: 6e64 6578 286e 6f64 6529 2c20 2a2a 6b77  ndex(node), **kw
-000107c0: 6172 6773 290d 0a0d 0a20 2020 2040 7472  args)....    @tr
-000107d0: 6565 5f73 7562 6d65 6e75 285f 2822 496e  ee_submenu(_("In
-000107e0: 7365 7274 2073 7065 6369 616c 206f 7065  sert special ope
-000107f0: 7261 7469 6f6e 2873 2922 2929 0d0a 2020  ration(s)"))..  
-00010800: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-00010810: 6e28 5f28 2241 6464 2048 6f6d 6522 292c  n(_("Add Home"),
-00010820: 206e 6f64 655f 7479 7065 3d6f 705f 6e6f   node_type=op_no
-00010830: 6465 732c 2068 656c 703d 2222 290d 0a20  des, help="").. 
-00010840: 2020 2064 6566 2061 6464 5f6f 7065 7261     def add_opera
-00010850: 7469 6f6e 5f68 6f6d 6528 6e6f 6465 2c20  tion_home(node, 
-00010860: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-00010870: 2020 2020 6170 7065 6e64 5f6f 7065 7261      append_opera
-00010880: 7469 6f6e 5f68 6f6d 6528 6e6f 6465 2c20  tion_home(node, 
-00010890: 706f 733d 6164 645f 6166 7465 725f 696e  pos=add_after_in
-000108a0: 6465 7828 6e6f 6465 292c 202a 2a6b 7761  dex(node), **kwa
-000108b0: 7267 7329 0d0a 0d0a 2020 2020 4074 7265  rgs)....    @tre
-000108c0: 655f 7375 626d 656e 7528 5f28 2249 6e73  e_submenu(_("Ins
-000108d0: 6572 7420 7370 6563 6961 6c20 6f70 6572  ert special oper
-000108e0: 6174 696f 6e28 7329 2229 290d 0a20 2020  ation(s)"))..   
-000108f0: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
-00010900: 285f 2822 4164 6420 5265 7475 726e 2074  (_("Add Return t
-00010910: 6f20 4f72 6967 696e 2229 2c20 6e6f 6465  o Origin"), node
-00010920: 5f74 7970 653d 6f70 5f6e 6f64 6573 2c20  _type=op_nodes, 
-00010930: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
-00010940: 6620 6164 645f 6f70 6572 6174 696f 6e5f  f add_operation_
-00010950: 6f72 6967 696e 286e 6f64 652c 202a 2a6b  origin(node, **k
-00010960: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00010970: 2061 7070 656e 645f 6f70 6572 6174 696f   append_operatio
-00010980: 6e5f 676f 746f 286e 6f64 652c 2070 6f73  n_goto(node, pos
-00010990: 3d61 6464 5f61 6674 6572 5f69 6e64 6578  =add_after_index
-000109a0: 286e 6f64 6529 2c20 2a2a 6b77 6172 6773  (node), **kwargs
-000109b0: 290d 0a0d 0a20 2020 2040 7472 6565 5f73  )....    @tree_s
-000109c0: 7562 6d65 6e75 285f 2822 496e 7365 7274  ubmenu(_("Insert
-000109d0: 2073 7065 6369 616c 206f 7065 7261 7469   special operati
-000109e0: 6f6e 2873 2922 2929 0d0a 2020 2020 4074  on(s)"))..    @t
-000109f0: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
-00010a00: 2241 6464 2042 6565 7022 292c 206e 6f64  "Add Beep"), nod
-00010a10: 655f 7479 7065 3d6f 705f 6e6f 6465 732c  e_type=op_nodes,
-00010a20: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-00010a30: 6566 2061 6464 5f6f 7065 7261 7469 6f6e  ef add_operation
-00010a40: 5f62 6565 7028 6e6f 6465 2c20 2a2a 6b77  _beep(node, **kw
-00010a50: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00010a60: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
-00010a70: 5f62 6565 7028 6e6f 6465 2c20 706f 733d  _beep(node, pos=
-00010a80: 6164 645f 6166 7465 725f 696e 6465 7828  add_after_index(
-00010a90: 6e6f 6465 292c 202a 2a6b 7761 7267 7329  node), **kwargs)
-00010aa0: 0d0a 0d0a 2020 2020 4074 7265 655f 7375  ....    @tree_su
-00010ab0: 626d 656e 7528 5f28 2249 6e73 6572 7420  bmenu(_("Insert 
-00010ac0: 7370 6563 6961 6c20 6f70 6572 6174 696f  special operatio
-00010ad0: 6e28 7329 2229 290d 0a20 2020 2040 7472  n(s)"))..    @tr
-00010ae0: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-00010af0: 4164 6420 496e 7465 7272 7570 7422 292c  Add Interrupt"),
-00010b00: 206e 6f64 655f 7479 7065 3d6f 705f 6e6f   node_type=op_no
-00010b10: 6465 732c 2068 656c 703d 2222 290d 0a20  des, help="").. 
-00010b20: 2020 2064 6566 2061 6464 5f6f 7065 7261     def add_opera
-00010b30: 7469 6f6e 5f69 6e74 6572 7275 7074 286e  tion_interrupt(n
-00010b40: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
-00010b50: 0a20 2020 2020 2020 2061 7070 656e 645f  .        append_
-00010b60: 6f70 6572 6174 696f 6e5f 696e 7465 7272  operation_interr
-00010b70: 7570 7428 6e6f 6465 2c20 706f 733d 6164  upt(node, pos=ad
-00010b80: 645f 6166 7465 725f 696e 6465 7828 6e6f  d_after_index(no
-00010b90: 6465 292c 202a 2a6b 7761 7267 7329 0d0a  de), **kwargs)..
-00010ba0: 0d0a 2020 2020 4074 7265 655f 7375 626d  ..    @tree_subm
-00010bb0: 656e 7528 5f28 2249 6e73 6572 7420 7370  enu(_("Insert sp
-00010bc0: 6563 6961 6c20 6f70 6572 6174 696f 6e28  ecial operation(
-00010bd0: 7329 2229 290d 0a20 2020 2040 7472 6565  s)"))..    @tree
-00010be0: 5f70 726f 6d70 7428 2277 6169 745f 7469  _prompt("wait_ti
-00010bf0: 6d65 222c 205f 2822 5761 6974 2066 6f72  me", _("Wait for
-00010c00: 2068 6f77 206c 6f6e 6720 2869 6e20 7365   how long (in se
-00010c10: 636f 6e64 7329 3f22 292c 2064 6174 615f  conds)?"), data_
-00010c20: 7479 7065 3d66 6c6f 6174 290d 0a20 2020  type=float)..   
-00010c30: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
-00010c40: 285f 2822 4164 6420 5761 6974 2229 2c20  (_("Add Wait"), 
-00010c50: 6e6f 6465 5f74 7970 653d 6f70 5f6e 6f64  node_type=op_nod
-00010c60: 6573 2c20 6865 6c70 3d22 2229 0d0a 2020  es, help="")..  
-00010c70: 2020 6465 6620 6164 645f 6f70 6572 6174    def add_operat
-00010c80: 696f 6e5f 7761 6974 286e 6f64 652c 2077  ion_wait(node, w
-00010c90: 6169 745f 7469 6d65 2c20 2a2a 6b77 6172  ait_time, **kwar
-00010ca0: 6773 293a 0d0a 2020 2020 2020 2020 6170  gs):..        ap
-00010cb0: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f77  pend_operation_w
-00010cc0: 6169 7428 0d0a 2020 2020 2020 2020 2020  ait(..          
-00010cd0: 2020 6e6f 6465 2c20 7761 6974 5f74 696d    node, wait_tim
-00010ce0: 653d 7761 6974 5f74 696d 652c 2070 6f73  e=wait_time, pos
-00010cf0: 3d61 6464 5f61 6674 6572 5f69 6e64 6578  =add_after_index
-00010d00: 286e 6f64 6529 2c20 2a2a 6b77 6172 6773  (node), **kwargs
-00010d10: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
-00010d20: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
-00010d30: 285f 2822 496e 7365 7274 2073 7065 6369  (_("Insert speci
-00010d40: 616c 206f 7065 7261 7469 6f6e 2873 2922  al operation(s)"
-00010d50: 2929 0d0a 2020 2020 4074 7265 655f 6f70  ))..    @tree_op
-00010d60: 6572 6174 696f 6e28 5f28 2241 6464 204f  eration(_("Add O
-00010d70: 7574 7075 7422 292c 206e 6f64 655f 7479  utput"), node_ty
-00010d80: 7065 3d6f 705f 6e6f 6465 732c 2068 656c  pe=op_nodes, hel
-00010d90: 703d 2222 290d 0a20 2020 2064 6566 2061  p="")..    def a
-00010da0: 6464 5f6f 7065 7261 7469 6f6e 5f6f 7574  dd_operation_out
-00010db0: 7075 7428 6e6f 6465 2c20 2a2a 6b77 6172  put(node, **kwar
-00010dc0: 6773 293a 0d0a 2020 2020 2020 2020 6170  gs):..        ap
-00010dd0: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f6f  pend_operation_o
-00010de0: 7574 7075 7428 6e6f 6465 2c20 706f 733d  utput(node, pos=
-00010df0: 6164 645f 6166 7465 725f 696e 6465 7828  add_after_index(
-00010e00: 6e6f 6465 292c 202a 2a6b 7761 7267 7329  node), **kwargs)
-00010e10: 0d0a 0d0a 2020 2020 4074 7265 655f 7375  ....    @tree_su
-00010e20: 626d 656e 7528 5f28 2249 6e73 6572 7420  bmenu(_("Insert 
-00010e30: 7370 6563 6961 6c20 6f70 6572 6174 696f  special operatio
-00010e40: 6e28 7329 2229 290d 0a20 2020 2040 7472  n(s)"))..    @tr
-00010e50: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-00010e60: 4164 6420 496e 7075 7422 292c 206e 6f64  Add Input"), nod
-00010e70: 655f 7479 7065 3d6f 705f 6e6f 6465 732c  e_type=op_nodes,
-00010e80: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-00010e90: 6566 2061 6464 5f6f 7065 7261 7469 6f6e  ef add_operation
-00010ea0: 5f69 6e70 7574 286e 6f64 652c 202a 2a6b  _input(node, **k
-00010eb0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00010ec0: 2061 7070 656e 645f 6f70 6572 6174 696f   append_operatio
-00010ed0: 6e5f 696e 7075 7428 6e6f 6465 2c20 706f  n_input(node, po
-00010ee0: 733d 6164 645f 6166 7465 725f 696e 6465  s=add_after_inde
-00010ef0: 7828 6e6f 6465 292c 202a 2a6b 7761 7267  x(node), **kwarg
-00010f00: 7329 0d0a 0d0a 2020 2020 4074 7265 655f  s)....    @tree_
-00010f10: 7375 626d 656e 7528 5f28 2249 6e73 6572  submenu(_("Inser
-00010f20: 7420 7370 6563 6961 6c20 6f70 6572 6174  t special operat
-00010f30: 696f 6e28 7329 2229 290d 0a20 2020 2040  ion(s)"))..    @
-00010f40: 7472 6565 5f6f 7065 7261 7469 6f6e 285f  tree_operation(_
-00010f50: 2822 4164 6420 486f 6d65 2f42 6565 702f  ("Add Home/Beep/
-00010f60: 496e 7465 7272 7570 7422 292c 206e 6f64  Interrupt"), nod
-00010f70: 655f 7479 7065 3d6f 705f 6e6f 6465 732c  e_type=op_nodes,
-00010f80: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-00010f90: 6566 2061 6464 5f6f 7065 7261 7469 6f6e  ef add_operation
-00010fa0: 5f68 6f6d 655f 6265 6570 5f69 6e74 6572  _home_beep_inter
-00010fb0: 7275 7074 286e 6f64 652c 202a 2a6b 7761  rupt(node, **kwa
-00010fc0: 7267 7329 3a0d 0a20 2020 2020 2020 2070  rgs):..        p
-00010fd0: 6f73 203d 2061 6464 5f61 6674 6572 5f69  os = add_after_i
-00010fe0: 6e64 6578 286e 6f64 6529 0d0a 2020 2020  ndex(node)..    
-00010ff0: 2020 2020 6170 7065 6e64 5f6f 7065 7261      append_opera
-00011000: 7469 6f6e 5f68 6f6d 6528 6e6f 6465 2c20  tion_home(node, 
-00011010: 706f 733d 706f 732c 202a 2a6b 7761 7267  pos=pos, **kwarg
-00011020: 7329 0d0a 2020 2020 2020 2020 6966 2070  s)..        if p
-00011030: 6f73 3a0d 0a20 2020 2020 2020 2020 2020  os:..           
-00011040: 2070 6f73 202b 3d20 310d 0a20 2020 2020   pos += 1..     
-00011050: 2020 2061 7070 656e 645f 6f70 6572 6174     append_operat
-00011060: 696f 6e5f 6265 6570 286e 6f64 652c 2070  ion_beep(node, p
-00011070: 6f73 3d70 6f73 2c20 2a2a 6b77 6172 6773  os=pos, **kwargs
-00011080: 290d 0a20 2020 2020 2020 2069 6620 706f  )..        if po
-00011090: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000110a0: 706f 7320 2b3d 2031 0d0a 2020 2020 2020  pos += 1..      
-000110b0: 2020 6170 7065 6e64 5f6f 7065 7261 7469    append_operati
-000110c0: 6f6e 5f69 6e74 6572 7275 7074 286e 6f64  on_interrupt(nod
-000110d0: 652c 2070 6f73 3d70 6f73 2c20 2a2a 6b77  e, pos=pos, **kw
-000110e0: 6172 6773 290d 0a0d 0a20 2020 2040 7472  args)....    @tr
-000110f0: 6565 5f73 7562 6d65 6e75 285f 2822 496e  ee_submenu(_("In
-00011100: 7365 7274 2073 7065 6369 616c 206f 7065  sert special ope
-00011110: 7261 7469 6f6e 2873 2922 2929 0d0a 2020  ration(s)"))..  
-00011120: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-00011130: 6e28 5f28 2241 6464 204f 7269 6769 6e2f  n(_("Add Origin/
-00011140: 4265 6570 2f49 6e74 6572 7275 7074 2229  Beep/Interrupt")
-00011150: 2c20 6e6f 6465 5f74 7970 653d 6f70 5f6e  , node_type=op_n
-00011160: 6f64 6573 2c20 6865 6c70 3d22 2229 0d0a  odes, help="")..
-00011170: 2020 2020 6465 6620 6164 645f 6f70 6572      def add_oper
-00011180: 6174 696f 6e5f 6f72 6967 696e 5f62 6565  ation_origin_bee
-00011190: 705f 696e 7465 7272 7570 7428 6e6f 6465  p_interrupt(node
-000111a0: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
-000111b0: 2020 2020 2020 706f 7320 3d20 6164 645f        pos = add_
-000111c0: 6166 7465 725f 696e 6465 7828 6e6f 6465  after_index(node
-000111d0: 290d 0a20 2020 2020 2020 2061 7070 656e  )..        appen
-000111e0: 645f 6f70 6572 6174 696f 6e5f 676f 746f  d_operation_goto
-000111f0: 286e 6f64 652c 2070 6f73 3d70 6f73 2c20  (node, pos=pos, 
-00011200: 2a2a 6b77 6172 6773 290d 0a20 2020 2020  **kwargs)..     
-00011210: 2020 2069 6620 706f 733a 0d0a 2020 2020     if pos:..    
-00011220: 2020 2020 2020 2020 706f 7320 2b3d 2031          pos += 1
-00011230: 0d0a 2020 2020 2020 2020 6170 7065 6e64  ..        append
-00011240: 5f6f 7065 7261 7469 6f6e 5f62 6565 7028  _operation_beep(
-00011250: 6e6f 6465 2c20 706f 733d 706f 732c 202a  node, pos=pos, *
-00011260: 2a6b 7761 7267 7329 0d0a 2020 2020 2020  *kwargs)..      
-00011270: 2020 6966 2070 6f73 3a0d 0a20 2020 2020    if pos:..     
-00011280: 2020 2020 2020 2070 6f73 202b 3d20 310d         pos += 1.
-00011290: 0a20 2020 2020 2020 2061 7070 656e 645f  .        append_
-000112a0: 6f70 6572 6174 696f 6e5f 696e 7465 7272  operation_interr
-000112b0: 7570 7428 6e6f 6465 2c20 706f 733d 706f  upt(node, pos=po
-000112c0: 732c 202a 2a6b 7761 7267 7329 0d0a 0d0a  s, **kwargs)....
-000112d0: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-000112e0: 696f 6e28 5f28 2252 656c 6f61 6420 277b  ion(_("Reload '{
-000112f0: 6e61 6d65 7d27 2229 2c20 6e6f 6465 5f74  name}'"), node_t
-00011300: 7970 653d 2266 696c 6522 2c20 6865 6c70  ype="file", help
-00011310: 3d22 2229 0d0a 2020 2020 6465 6620 7265  ="")..    def re
-00011320: 6c6f 6164 5f66 696c 6528 6e6f 6465 2c20  load_file(node, 
-00011330: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-00011340: 2020 2020 6669 6c65 7061 7468 203d 206e      filepath = n
-00011350: 6f64 652e 6669 6c65 7061 7468 0d0a 2020  ode.filepath..  
-00011360: 2020 2020 2020 6e6f 6465 2e72 656d 6f76        node.remov
-00011370: 655f 6e6f 6465 2829 0d0a 2020 2020 2020  e_node()..      
-00011380: 2020 7365 6c66 2e6c 6f61 6428 6669 6c65    self.load(file
-00011390: 7061 7468 290d 0a0d 0a20 2020 2040 7472  path)....    @tr
-000113a0: 6565 5f6f 7065 7261 7469 6f6e 280d 0a20  ee_operation(.. 
-000113b0: 2020 2020 2020 205f 2822 4f70 656e 2069         _("Open i
-000113c0: 6e20 5379 7374 656d 3a20 277b 6e61 6d65  n System: '{name
-000113d0: 7d27 2229 2c0d 0a20 2020 2020 2020 206e  }'"),..        n
-000113e0: 6f64 655f 7479 7065 3d22 6669 6c65 222c  ode_type="file",
-000113f0: 0d0a 2020 2020 2020 2020 6865 6c70 3d5f  ..        help=_
-00011400: 280d 0a20 2020 2020 2020 2020 2020 2022  (..            "
-00011410: 4f70 656e 2074 6869 7320 6669 6c65 2069  Open this file i
-00011420: 6e20 7468 6520 7379 7374 656d 2061 7070  n the system app
-00011430: 6c69 6361 7469 6f6e 2061 7373 6f63 6961  lication associa
-00011440: 7465 6420 7769 7468 2074 6869 7320 7479  ted with this ty
-00011450: 7065 206f 6620 6669 6c65 220d 0a20 2020  pe of file"..   
-00011460: 2020 2020 2029 2c0d 0a20 2020 2029 0d0a       ),..    )..
-00011470: 2020 2020 6465 6620 6f70 656e 5f73 7973      def open_sys
-00011480: 7465 6d5f 6669 6c65 286e 6f64 652c 202a  tem_file(node, *
-00011490: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-000114a0: 2020 2066 696c 6570 6174 6820 3d20 6e6f     filepath = no
-000114b0: 6465 2e66 696c 6570 6174 680d 0a20 2020  de.filepath..   
-000114c0: 2020 2020 206e 6f72 6d61 6c69 7a65 6420       normalized 
-000114d0: 3d20 6f73 2e70 6174 682e 7265 616c 7061  = os.path.realpa
-000114e0: 7468 2866 696c 6570 6174 6829 0d0a 0d0a  th(filepath)....
-000114f0: 2020 2020 2020 2020 696d 706f 7274 2070          import p
-00011500: 6c61 7466 6f72 6d0d 0a0d 0a20 2020 2020  latform....     
-00011510: 2020 2073 7973 7465 6d20 3d20 706c 6174     system = plat
-00011520: 666f 726d 2e73 7973 7465 6d28 290d 0a20  form.system().. 
-00011530: 2020 2020 2020 2069 6620 7379 7374 656d         if system
-00011540: 203d 3d20 2244 6172 7769 6e22 3a0d 0a20   == "Darwin":.. 
-00011550: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-00011560: 6f73 2069 6d70 6f72 7420 7379 7374 656d  os import system
-00011570: 2061 7320 6f70 656e 5f69 6e5f 7368 656c   as open_in_shel
-00011580: 6c0d 0a0d 0a20 2020 2020 2020 2020 2020  l....           
-00011590: 206f 7065 6e5f 696e 5f73 6865 6c6c 2866   open_in_shell(f
-000115a0: 226f 7065 6e20 277b 6e6f 726d 616c 697a  "open '{normaliz
-000115b0: 6564 7d27 2229 0d0a 2020 2020 2020 2020  ed}'")..        
-000115c0: 656c 6966 2073 7973 7465 6d20 3d3d 2022  elif system == "
-000115d0: 5769 6e64 6f77 7322 3a0d 0a20 2020 2020  Windows":..     
-000115e0: 2020 2020 2020 2066 726f 6d20 6f73 2069         from os i
-000115f0: 6d70 6f72 7420 7374 6172 7466 696c 6520  mport startfile 
-00011600: 6173 206f 7065 6e5f 696e 5f73 6865 6c6c  as open_in_shell
-00011610: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00011620: 6f70 656e 5f69 6e5f 7368 656c 6c28 6627  open_in_shell(f'
-00011630: 227b 6e6f 726d 616c 697a 6564 7d22 2729  "{normalized}"')
-00011640: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00011650: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-00011660: 6d20 6f73 2069 6d70 6f72 7420 7379 7374  m os import syst
-00011670: 656d 2061 7320 6f70 656e 5f69 6e5f 7368  em as open_in_sh
-00011680: 656c 6c0d 0a0d 0a20 2020 2020 2020 2020  ell....         
-00011690: 2020 206f 7065 6e5f 696e 5f73 6865 6c6c     open_in_shell
-000116a0: 2866 2278 6467 2d6f 7065 6e20 277b 6e6f  (f"xdg-open '{no
-000116b0: 726d 616c 697a 6564 7d27 2229 0d0a 0d0a  rmalized}'")....
-000116c0: 2020 2020 6465 6620 6765 745f 7661 6c75      def get_valu
-000116d0: 6573 2829 3a0d 0a20 2020 2020 2020 2072  es():..        r
-000116e0: 6574 7572 6e20 5b6f 2066 6f72 206f 2069  eturn [o for o i
-000116f0: 6e20 7365 6c66 2e6f 7073 2829 2069 6620  n self.ops() if 
-00011700: 6f2e 7479 7065 2e73 7461 7274 7377 6974  o.type.startswit
-00011710: 6828 226f 7022 295d 0d0a 0d0a 2020 2020  h("op")]....    
-00011720: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
-00011730: 6c28 6c61 6d62 6461 206e 6f64 653a 206e  l(lambda node: n
-00011740: 6f74 2069 735f 7265 676d 6172 6b28 6e6f  ot is_regmark(no
-00011750: 6465 2929 0d0a 2020 2020 4074 7265 655f  de))..    @tree_
-00011760: 7375 626d 656e 7528 5f28 2241 7373 6967  submenu(_("Assig
-00011770: 6e20 4f70 6572 6174 696f 6e22 2929 0d0a  n Operation"))..
-00011780: 2020 2020 4074 7265 655f 7661 6c75 6573      @tree_values
-00011790: 2822 6f70 5f61 7373 6967 6e22 2c20 7661  ("op_assign", va
-000117a0: 6c75 6573 3d67 6574 5f76 616c 7565 7329  lues=get_values)
-000117b0: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
-000117c0: 6174 696f 6e28 227b 6f70 5f61 7373 6967  ation("{op_assig
-000117d0: 6e7d 222c 206e 6f64 655f 7479 7065 3d65  n}", node_type=e
-000117e0: 6c65 6d5f 6e6f 6465 732c 2068 656c 703d  lem_nodes, help=
-000117f0: 2222 290d 0a20 2020 2064 6566 206d 656e  "")..    def men
-00011800: 755f 6173 7369 676e 5f6f 7065 7261 7469  u_assign_operati
-00011810: 6f6e 7328 6e6f 6465 2c20 6f70 5f61 7373  ons(node, op_ass
-00011820: 6967 6e2c 202a 2a6b 7761 7267 7329 3a0d  ign, **kwargs):.
-00011830: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00011840: 2e63 6c61 7373 6966 795f 696e 6865 7269  .classify_inheri
-00011850: 745f 7374 726f 6b65 3a0d 0a20 2020 2020  t_stroke:..     
-00011860: 2020 2020 2020 2069 6d70 6f73 6520 3d20         impose = 
-00011870: 2274 6f5f 6f70 220d 0a20 2020 2020 2020  "to_op"..       
-00011880: 2020 2020 2061 7474 7269 6220 3d20 2273       attrib = "s
-00011890: 7472 6f6b 6522 0d0a 2020 2020 2020 2020  troke"..        
-000118a0: 2020 2020 7369 6d69 6c61 7220 3d20 5472      similar = Tr
-000118b0: 7565 0d0a 2020 2020 2020 2020 656c 6966  ue..        elif
-000118c0: 2073 656c 662e 636c 6173 7369 6679 5f69   self.classify_i
-000118d0: 6e68 6572 6974 5f66 696c 6c3a 0d0a 2020  nherit_fill:..  
-000118e0: 2020 2020 2020 2020 2020 696d 706f 7365            impose
-000118f0: 203d 2022 746f 5f6f 7022 0d0a 2020 2020   = "to_op"..    
-00011900: 2020 2020 2020 2020 6174 7472 6962 203d          attrib =
-00011910: 2022 6669 6c6c 220d 0a20 2020 2020 2020   "fill"..       
-00011920: 2020 2020 2073 696d 696c 6172 203d 2054       similar = T
-00011930: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
-00011940: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00011950: 696d 706f 7365 203d 204e 6f6e 650d 0a20  impose = None.. 
-00011960: 2020 2020 2020 2020 2020 2061 7474 7269             attri
-00011970: 6220 3d20 4e6f 6e65 0d0a 2020 2020 2020  b = None..      
-00011980: 2020 2020 2020 7369 6d69 6c61 7220 3d20        similar = 
-00011990: 4661 6c73 650d 0a20 2020 2020 2020 2065  False..        e
-000119a0: 7863 6c75 7369 7665 203d 2073 656c 662e  xclusive = self.
-000119b0: 636c 6173 7369 6679 5f69 6e68 6572 6974  classify_inherit
-000119c0: 5f65 7863 6c75 7369 7665 0d0a 2020 2020  _exclusive..    
-000119d0: 2020 2020 6461 7461 203d 206c 6973 7428      data = list(
-000119e0: 7365 6c66 2e65 6c65 6d73 2865 6d70 6861  self.elems(empha
-000119f0: 7369 7a65 643d 5472 7565 2929 0d0a 2020  sized=True))..  
-00011a00: 2020 2020 2020 7365 6c66 2e61 7373 6967        self.assig
-00011a10: 6e5f 6f70 6572 6174 696f 6e28 0d0a 2020  n_operation(..  
-00011a20: 2020 2020 2020 2020 2020 6f70 5f61 7373            op_ass
-00011a30: 6967 6e3d 6f70 5f61 7373 6967 6e2c 0d0a  ign=op_assign,..
-00011a40: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00011a50: 3d64 6174 612c 0d0a 2020 2020 2020 2020  =data,..        
-00011a60: 2020 2020 696d 706f 7365 3d69 6d70 6f73      impose=impos
-00011a70: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00011a80: 6174 7472 6962 3d61 7474 7269 622c 0d0a  attrib=attrib,..
-00011a90: 2020 2020 2020 2020 2020 2020 7369 6d69              simi
-00011aa0: 6c61 723d 7369 6d69 6c61 722c 0d0a 2020  lar=similar,..  
-00011ab0: 2020 2020 2020 2020 2020 6578 636c 7573            exclus
-00011ac0: 6976 653d 6578 636c 7573 6976 652c 0d0a  ive=exclusive,..
-00011ad0: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00011ae0: 2064 6566 2065 7863 6c75 7369 7665 5f6d   def exclusive_m
-00011af0: 6174 6368 286e 6f64 652c 202a 2a6b 7761  atch(node, **kwa
-00011b00: 7267 7329 3a0d 0a20 2020 2020 2020 2072  rgs):..        r
-00011b10: 6574 7572 6e20 7365 6c66 2e63 6c61 7373  eturn self.class
-00011b20: 6966 795f 696e 6865 7269 745f 6578 636c  ify_inherit_excl
-00011b30: 7573 6976 650d 0a0d 0a20 2020 2040 7472  usive....    @tr
-00011b40: 6565 5f73 6570 6172 6174 6f72 5f62 6566  ee_separator_bef
-00011b50: 6f72 6528 290d 0a20 2020 2040 7472 6565  ore()..    @tree
-00011b60: 5f73 7562 6d65 6e75 285f 2822 4173 7369  _submenu(_("Assi
-00011b70: 676e 204f 7065 7261 7469 6f6e 2229 290d  gn Operation")).
-00011b80: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
-00011b90: 7469 6f6e 280d 0a20 2020 2020 2020 205f  tion(..        _
-00011ba0: 2822 5265 6d6f 7665 2061 6c6c 2061 7373  ("Remove all ass
-00011bb0: 6967 6e6d 656e 7473 2066 726f 6d20 6f70  ignments from op
-00011bc0: 6572 6174 696f 6e73 2229 2c0d 0a20 2020  erations"),..   
-00011bd0: 2020 2020 206e 6f64 655f 7479 7065 3d65       node_type=e
-00011be0: 6c65 6d5f 6772 6f75 705f 6e6f 6465 732c  lem_group_nodes,
-00011bf0: 0d0a 2020 2020 2020 2020 6865 6c70 3d5f  ..        help=_
-00011c00: 2822 416e 7920 6578 6973 7469 6e67 2061  ("Any existing a
-00011c10: 7373 6967 6e6d 656e 7420 6f66 2074 6869  ssignment of thi
-00011c20: 7320 656c 656d 656e 7420 746f 206f 7065  s element to ope
-00011c30: 7261 7469 6f6e 7320 7769 6c6c 2062 6520  rations will be 
-00011c40: 7265 6d6f 7665 6422 292c 0d0a 2020 2020  removed"),..    
-00011c50: 290d 0a20 2020 2064 6566 2072 656d 6f76  )..    def remov
-00011c60: 655f 6173 7369 676e 6d65 6e74 7328 7369  e_assignments(si
-00011c70: 6e67 6c65 6e6f 6465 2c20 2a2a 6b77 6172  nglenode, **kwar
-00011c80: 6773 293a 0d0a 2020 2020 2020 2020 6465  gs):..        de
-00011c90: 6620 7265 6d5f 6e6f 6465 2872 6e6f 6465  f rem_node(rnode
-00011ca0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00011cb0: 2320 7265 6375 7273 6976 656c 7920 7265  # recursively re
-00011cc0: 6d6f 7665 2061 7373 6967 6e6d 656e 7473  move assignments
-00011cd0: 2e2e 2e0d 0a20 2020 2020 2020 2020 2020  .....           
-00011ce0: 2069 6620 726e 6f64 652e 7479 7065 2069   if rnode.type i
-00011cf0: 6e20 2822 6669 6c65 222c 2022 6772 6f75  n ("file", "grou
-00011d00: 7022 293a 0d0a 2020 2020 2020 2020 2020  p"):..          
-00011d10: 2020 2020 2020 666f 7220 636e 6f64 6520        for cnode 
-00011d20: 696e 206c 6973 7428 726e 6f64 652e 5f63  in list(rnode._c
-00011d30: 6869 6c64 7265 6e29 3a0d 0a20 2020 2020  hildren):..     
-00011d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011d50: 656d 5f6e 6f64 6528 636e 6f64 6529 0d0a  em_node(cnode)..
-00011d60: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00011d70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00011d80: 2020 2066 6f72 2072 6566 2069 6e20 6c69     for ref in li
-00011d90: 7374 2872 6e6f 6465 2e72 6566 6572 656e  st(rnode.referen
-00011da0: 6365 7329 3a0d 0a20 2020 2020 2020 2020  ces):..         
-00011db0: 2020 2020 2020 2020 2020 2072 6566 2e72             ref.r
-00011dc0: 656d 6f76 655f 6e6f 6465 2829 0d0a 0d0a  emove_node()....
-00011dd0: 2020 2020 2020 2020 7769 7468 2073 656c          with sel
-00011de0: 662e 7374 6174 6963 2822 7265 6d6f 7665  f.static("remove
-00011df0: 5f61 7373 6967 6e22 293a 0d0a 2020 2020  _assign"):..    
-00011e00: 2020 2020 2020 2020 666f 7220 6e6f 6465          for node
-00011e10: 2069 6e20 6c69 7374 2873 656c 662e 656c   in list(self.el
-00011e20: 656d 7328 656d 7068 6173 697a 6564 3d54  ems(emphasized=T
-00011e30: 7275 6529 293a 0d0a 2020 2020 2020 2020  rue)):..        
-00011e40: 2020 2020 2020 2020 7265 6d5f 6e6f 6465          rem_node
-00011e50: 286e 6f64 6529 0d0a 2020 2020 2020 2020  (node)..        
-00011e60: 7365 6c66 2e73 6967 6e61 6c28 2272 6566  self.signal("ref
-00011e70: 7265 7368 5f74 7265 6522 290d 0a0d 0a20  resh_tree").... 
-00011e80: 2020 2040 7472 6565 5f73 6570 6172 6174     @tree_separat
-00011e90: 6f72 5f62 6566 6f72 6528 290d 0a20 2020  or_before()..   
-00011ea0: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
-00011eb0: 2822 4173 7369 676e 204f 7065 7261 7469  ("Assign Operati
-00011ec0: 6f6e 2229 290d 0a20 2020 2040 7472 6565  on"))..    @tree
-00011ed0: 5f63 6865 636b 2865 7863 6c75 7369 7665  _check(exclusive
-00011ee0: 5f6d 6174 6368 290d 0a20 2020 2040 7472  _match)..    @tr
-00011ef0: 6565 5f6f 7065 7261 7469 6f6e 280d 0a20  ee_operation(.. 
-00011f00: 2020 2020 2020 205f 2822 4578 636c 7573         _("Exclus
-00011f10: 6976 6520 6173 7369 676e 6d65 6e74 2229  ive assignment")
-00011f20: 2c0d 0a20 2020 2020 2020 206e 6f64 655f  ,..        node_
-00011f30: 7479 7065 3d65 6c65 6d5f 6e6f 6465 732c  type=elem_nodes,
-00011f40: 0d0a 2020 2020 2020 2020 6865 6c70 3d5f  ..        help=_
-00011f50: 280d 0a20 2020 2020 2020 2020 2020 2022  (..            "
-00011f60: 416e 2061 7373 6967 6e6d 656e 7420 7769  An assignment wi
-00011f70: 6c6c 2072 656d 6f76 6520 616c 6c20 6f74  ll remove all ot
-00011f80: 6865 7220 636c 6173 7369 6669 6361 7469  her classificati
-00011f90: 6f6e 7320 6f66 2074 6869 7320 656c 656d  ons of this elem
-00011fa0: 656e 7420 6966 2063 6865 636b 6564 220d  ent if checked".
-00011fb0: 0a20 2020 2020 2020 2029 2c0d 0a20 2020  .        ),..   
-00011fc0: 2029 0d0a 2020 2020 6465 6620 7365 745f   )..    def set_
-00011fd0: 6173 7369 676e 5f6f 7074 696f 6e5f 6578  assign_option_ex
-00011fe0: 636c 7573 6976 6528 6e6f 6465 2c20 2a2a  clusive(node, **
-00011ff0: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00012000: 2020 7365 6c66 2e63 6c61 7373 6966 795f    self.classify_
-00012010: 696e 6865 7269 745f 6578 636c 7573 6976  inherit_exclusiv
-00012020: 6520 3d20 6e6f 7420 7365 6c66 2e63 6c61  e = not self.cla
-00012030: 7373 6966 795f 696e 6865 7269 745f 6578  ssify_inherit_ex
-00012040: 636c 7573 6976 650d 0a0d 0a20 2020 2064  clusive....    d
-00012050: 6566 2073 7472 6f6b 655f 6d61 7463 6828  ef stroke_match(
-00012060: 6e6f 6465 2c20 2a2a 6b77 6172 6773 293a  node, **kwargs):
-00012070: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00012080: 2073 656c 662e 636c 6173 7369 6679 5f69   self.classify_i
-00012090: 6e68 6572 6974 5f73 7472 6f6b 650d 0a0d  nherit_stroke...
-000120a0: 0a20 2020 2040 7472 6565 5f73 6570 6172  .    @tree_separ
-000120b0: 6174 6f72 5f62 6566 6f72 6528 290d 0a20  ator_before().. 
-000120c0: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
-000120d0: 285f 2822 4173 7369 676e 204f 7065 7261  (_("Assign Opera
-000120e0: 7469 6f6e 2229 290d 0a20 2020 2040 7472  tion"))..    @tr
-000120f0: 6565 5f63 6865 636b 2873 7472 6f6b 655f  ee_check(stroke_
-00012100: 6d61 7463 6829 0d0a 2020 2020 4074 7265  match)..    @tre
-00012110: 655f 6f70 6572 6174 696f 6e28 0d0a 2020  e_operation(..  
-00012120: 2020 2020 2020 5f28 2249 6e68 6572 6974        _("Inherit
-00012130: 2073 7472 6f6b 6520 616e 6420 636c 6173   stroke and clas
-00012140: 7369 6679 2073 696d 696c 6172 2229 2c0d  sify similar"),.
-00012150: 0a20 2020 2020 2020 206e 6f64 655f 7479  .        node_ty
-00012160: 7065 3d65 6c65 6d5f 6e6f 6465 732c 0d0a  pe=elem_nodes,..
-00012170: 2020 2020 2020 2020 6865 6c70 3d5f 2822          help=_("
-00012180: 4f70 6572 6174 696f 6e20 7769 6c6c 2069  Operation will i
-00012190: 6e68 6572 6974 2065 6c65 6d65 6e74 2073  nherit element s
-000121a0: 7472 6f6b 6520 636f 6c6f 7222 292c 0d0a  troke color"),..
-000121b0: 2020 2020 290d 0a20 2020 2064 6566 2073      )..    def s
-000121c0: 6574 5f61 7373 6967 6e5f 6f70 7469 6f6e  et_assign_option
-000121d0: 5f73 7472 6f6b 6528 6e6f 6465 2c20 2a2a  _stroke(node, **
-000121e0: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-000121f0: 2020 7365 6c66 2e63 6c61 7373 6966 795f    self.classify_
-00012200: 696e 6865 7269 745f 7374 726f 6b65 203d  inherit_stroke =
-00012210: 206e 6f74 2073 656c 662e 636c 6173 7369   not self.classi
-00012220: 6679 5f69 6e68 6572 6974 5f73 7472 6f6b  fy_inherit_strok
-00012230: 650d 0a20 2020 2020 2020 2023 2050 6f6f  e..        # Poo
-00012240: 7220 6d61 6e73 2072 6164 696f 0d0a 2020  r mans radio..  
-00012250: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
-00012260: 6173 7369 6679 5f69 6e68 6572 6974 5f73  assify_inherit_s
-00012270: 7472 6f6b 653a 0d0a 2020 2020 2020 2020  troke:..        
-00012280: 2020 2020 7365 6c66 2e63 6c61 7373 6966      self.classif
-00012290: 795f 696e 6865 7269 745f 6669 6c6c 203d  y_inherit_fill =
-000122a0: 2046 616c 7365 0d0a 0d0a 2020 2020 6465   False....    de
-000122b0: 6620 6669 6c6c 5f6d 6174 6368 286e 6f64  f fill_match(nod
-000122c0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-000122d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000122e0: 6c66 2e63 6c61 7373 6966 795f 696e 6865  lf.classify_inhe
-000122f0: 7269 745f 6669 6c6c 0d0a 0d0a 2020 2020  rit_fill....    
-00012300: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
-00012310: 2241 7373 6967 6e20 4f70 6572 6174 696f  "Assign Operatio
-00012320: 6e22 2929 0d0a 2020 2020 4074 7265 655f  n"))..    @tree_
-00012330: 6368 6563 6b28 6669 6c6c 5f6d 6174 6368  check(fill_match
-00012340: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
-00012350: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
-00012360: 205f 2822 496e 6865 7269 7420 6669 6c6c   _("Inherit fill
-00012370: 2061 6e64 2063 6c61 7373 6966 7920 7369   and classify si
-00012380: 6d69 6c61 7222 292c 0d0a 2020 2020 2020  milar"),..      
-00012390: 2020 6e6f 6465 5f74 7970 653d 656c 656d    node_type=elem
-000123a0: 5f6e 6f64 6573 2c0d 0a20 2020 2020 2020  _nodes,..       
-000123b0: 2068 656c 703d 5f28 224f 7065 7261 7469   help=_("Operati
-000123c0: 6f6e 2077 696c 6c20 696e 6865 7269 7420  on will inherit 
-000123d0: 656c 656d 656e 7420 6669 6c6c 2063 6f6c  element fill col
-000123e0: 6f72 2229 2c0d 0a20 2020 2029 0d0a 2020  or"),..    )..  
-000123f0: 2020 6465 6620 7365 745f 6173 7369 676e    def set_assign
-00012400: 5f6f 7074 696f 6e5f 6669 6c6c 286e 6f64  _option_fill(nod
-00012410: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-00012420: 2020 2020 2020 2073 656c 662e 636c 6173         self.clas
-00012430: 7369 6679 5f69 6e68 6572 6974 5f66 696c  sify_inherit_fil
-00012440: 6c20 3d20 6e6f 7420 7365 6c66 2e63 6c61  l = not self.cla
-00012450: 7373 6966 795f 696e 6865 7269 745f 6669  ssify_inherit_fi
-00012460: 6c6c 0d0a 2020 2020 2020 2020 2320 506f  ll..        # Po
-00012470: 6f72 206d 616e 7320 7261 6469 6f0d 0a20  or mans radio.. 
-00012480: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00012490: 6c61 7373 6966 795f 696e 6865 7269 745f  lassify_inherit_
-000124a0: 6669 6c6c 3a0d 0a20 2020 2020 2020 2020  fill:..         
-000124b0: 2020 2073 656c 662e 636c 6173 7369 6679     self.classify
-000124c0: 5f69 6e68 6572 6974 5f73 7472 6f6b 6520  _inherit_stroke 
-000124d0: 3d20 4661 6c73 650d 0a0d 0a20 2020 2040  = False....    @
-000124e0: 7472 6565 5f63 6f6e 6469 7469 6f6e 616c  tree_conditional
-000124f0: 286c 616d 6264 6120 6e6f 6465 3a20 6e6f  (lambda node: no
-00012500: 7420 6973 5f72 6567 6d61 726b 286e 6f64  t is_regmark(nod
-00012510: 6529 290d 0a20 2020 2040 7472 6565 5f73  e))..    @tree_s
-00012520: 7562 6d65 6e75 285f 2822 4475 706c 6963  ubmenu(_("Duplic
-00012530: 6174 6520 656c 656d 656e 7428 7329 2229  ate element(s)")
-00012540: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
-00012550: 7261 7469 6f6e 285f 2822 4d61 6b65 2031  ration(_("Make 1
-00012560: 2063 6f70 7922 292c 206e 6f64 655f 7479   copy"), node_ty
-00012570: 7065 3d65 6c65 6d5f 6772 6f75 705f 6e6f  pe=elem_group_no
-00012580: 6465 732c 2068 656c 703d 2222 290d 0a20  des, help="").. 
-00012590: 2020 2064 6566 2064 7570 6c69 6361 7465     def duplicate
-000125a0: 5f65 6c65 6d65 6e74 5f31 286e 6f64 652c  _element_1(node,
-000125b0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-000125c0: 2020 2020 2064 7570 6c69 6361 7465 5f65       duplicate_e
-000125d0: 6c65 6d65 6e74 5f6e 286e 6f64 652c 2063  lement_n(node, c
-000125e0: 6f70 6965 733d 312c 202a 2a6b 7761 7267  opies=1, **kwarg
-000125f0: 7329 0d0a 0d0a 2020 2020 4074 7265 655f  s)....    @tree_
-00012600: 636f 6e64 6974 696f 6e61 6c28 6c61 6d62  conditional(lamb
-00012610: 6461 206e 6f64 653a 206e 6f74 2069 735f  da node: not is_
-00012620: 7265 676d 6172 6b28 6e6f 6465 2929 0d0a  regmark(node))..
-00012630: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-00012640: 7528 5f28 2244 7570 6c69 6361 7465 2065  u(_("Duplicate e
-00012650: 6c65 6d65 6e74 2873 2922 2929 0d0a 2020  lement(s)"))..  
-00012660: 2020 4074 7265 655f 6974 6572 6174 6528    @tree_iterate(
-00012670: 2263 6f70 6965 7322 2c20 322c 2031 3029  "copies", 2, 10)
-00012680: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
-00012690: 6174 696f 6e28 5f28 224d 616b 6520 7b63  ation(_("Make {c
-000126a0: 6f70 6965 737d 2063 6f70 6965 7322 292c  opies} copies"),
-000126b0: 206e 6f64 655f 7479 7065 3d65 6c65 6d5f   node_type=elem_
-000126c0: 6772 6f75 705f 6e6f 6465 732c 2068 656c  group_nodes, hel
-000126d0: 703d 2222 290d 0a20 2020 2064 6566 2064  p="")..    def d
-000126e0: 7570 6c69 6361 7465 5f65 6c65 6d65 6e74  uplicate_element
-000126f0: 5f6e 286e 6f64 652c 2063 6f70 6965 732c  _n(node, copies,
-00012700: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00012710: 2020 2020 2064 6566 2063 6f70 795f 7369       def copy_si
-00012720: 6e67 6c65 5f6e 6f64 6528 6f72 676e 6f64  ngle_node(orgnod
-00012730: 652c 206f 7267 7061 7265 6e74 2c20 7469  e, orgparent, ti
-00012740: 6d65 732c 2064 782c 2064 7929 3a0d 0a20  mes, dx, dy):.. 
-00012750: 2020 2020 2020 2020 2020 2064 656c 7461             delta
-00012760: 5f77 6f72 646c 6973 7420 3d20 300d 0a20  _wordlist = 0.. 
-00012770: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00012780: 2069 6e20 7261 6e67 6528 7469 6d65 7329   in range(times)
-00012790: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000127a0: 2020 2064 656c 7461 5f77 6f72 646c 6973     delta_wordlis
-000127b0: 7420 2b3d 2031 0d0a 0d0a 2020 2020 2020  t += 1....      
-000127c0: 2020 2020 2020 2020 2020 636f 7079 5f6e            copy_n
-000127d0: 6f64 6520 3d20 636f 7079 286f 7267 6e6f  ode = copy(orgno
-000127e0: 6465 290d 0a20 2020 2020 2020 2020 2020  de)..           
-000127f0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00012800: 636f 7079 5f6e 6f64 652c 2022 6d61 7472  copy_node, "matr
-00012810: 6978 2229 3a0d 0a20 2020 2020 2020 2020  ix"):..         
-00012820: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
-00012830: 6e6f 6465 2e6d 6174 7269 7820 2a3d 204d  node.matrix *= M
-00012840: 6174 7269 782e 7472 616e 736c 6174 6528  atrix.translate(
-00012850: 286e 202b 2031 2920 2a20 6478 2c20 286e  (n + 1) * dx, (n
-00012860: 202b 2031 2920 2a20 6479 290d 0a20 2020   + 1) * dy)..   
-00012870: 2020 2020 2020 2020 2020 2020 2068 6164               had
-00012880: 5f6f 7074 696f 6e61 6c20 3d20 4661 6c73  _optional = Fals
-00012890: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000128a0: 2020 2023 204e 6565 6420 746f 2061 6464     # Need to add
-000128b0: 2073 7472 6f6b 6520 616e 6420 6669 6c6c   stroke and fill
-000128c0: 2c20 6173 2063 6f70 7920 7769 6c6c 2074  , as copy will t
-000128d0: 616b 6520 7468 650d 0a20 2020 2020 2020  ake the..       
-000128e0: 2020 2020 2020 2020 2023 2064 6566 6175           # defau
-000128f0: 6c74 2076 616c 7565 7320 666f 7220 7468  lt values for th
-00012900: 6573 6520 6174 7472 6962 7574 6573 0d0a  ese attributes..
-00012910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012920: 666f 7220 6f70 7469 6f6e 616c 2069 6e20  for optional in 
-00012930: 2822 6669 6c6c 222c 2022 7374 726f 6b65  ("fill", "stroke
-00012940: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00012950: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
-00012960: 7474 7228 6f72 676e 6f64 652c 206f 7074  ttr(orgnode, opt
-00012970: 696f 6e61 6c29 3a0d 0a20 2020 2020 2020  ional):..       
-00012980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012990: 2073 6574 6174 7472 2863 6f70 795f 6e6f   setattr(copy_no
-000129a0: 6465 2c20 6f70 7469 6f6e 616c 2c20 6765  de, optional, ge
-000129b0: 7461 7474 7228 6f72 676e 6f64 652c 206f  tattr(orgnode, o
-000129c0: 7074 696f 6e61 6c29 290d 0a20 2020 2020  ptional))..     
-000129d0: 2020 2020 2020 2020 2020 2066 6f72 206f             for o
-000129e0: 7074 696f 6e61 6c20 696e 2028 2277 7866  ptional in ("wxf
-000129f0: 6f6e 7422 2c20 226d 6b74 6578 7422 2c20  ont", "mktext", 
-00012a00: 226d 6b66 6f6e 7422 2c20 226d 6b66 6f6e  "mkfont", "mkfon
-00012a10: 7473 697a 6522 293a 0d0a 2020 2020 2020  tsize"):..      
-00012a20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012a30: 2068 6173 6174 7472 286f 7267 6e6f 6465   hasattr(orgnode
-00012a40: 2c20 6f70 7469 6f6e 616c 293a 0d0a 2020  , optional):..  
-00012a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a60: 2020 2020 2020 6861 645f 6f70 7469 6f6e        had_option
-00012a70: 616c 203d 2054 7275 650d 0a20 2020 2020  al = True..     
-00012a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a90: 2020 2073 6574 6174 7472 2863 6f70 795f     setattr(copy_
-00012aa0: 6e6f 6465 2c20 6f70 7469 6f6e 616c 2c20  node, optional, 
-00012ab0: 6765 7461 7474 7228 6f72 676e 6f64 652c  getattr(orgnode,
-00012ac0: 206f 7074 696f 6e61 6c29 290d 0a20 2020   optional))..   
-00012ad0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012ae0: 7365 6c66 2e63 6f70 795f 696e 6372 6561  self.copy_increa
-00012af0: 7365 735f 776f 7264 6c69 7374 5f72 6566  ses_wordlist_ref
-00012b00: 6572 656e 6365 7320 616e 6420 6861 7361  erences and hasa
-00012b10: 7474 7228 6f72 676e 6f64 652c 2022 7465  ttr(orgnode, "te
-00012b20: 7874 2229 3a0d 0a20 2020 2020 2020 2020  xt"):..         
-00012b30: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
-00012b40: 6e6f 6465 2e74 6578 7420 3d20 7365 6c66  node.text = self
-00012b50: 2e77 6f72 646c 6973 745f 6465 6c74 6128  .wordlist_delta(
-00012b60: 6f72 676e 6f64 652e 7465 7874 2c20 6465  orgnode.text, de
-00012b70: 6c74 615f 776f 7264 6c69 7374 290d 0a20  lta_wordlist).. 
-00012b80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00012b90: 6c69 6620 7365 6c66 2e63 6f70 795f 696e  lif self.copy_in
-00012ba0: 6372 6561 7365 735f 776f 7264 6c69 7374  creases_wordlist
-00012bb0: 5f72 6566 6572 656e 6365 7320 616e 6420  _references and 
-00012bc0: 6861 7361 7474 7228 652c 2022 6d6b 7465  hasattr(e, "mkte
-00012bd0: 7874 2229 3a0d 0a20 2020 2020 2020 2020  xt"):..         
-00012be0: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
-00012bf0: 6e6f 6465 2e6d 6b74 6578 7420 3d20 7365  node.mktext = se
-00012c00: 6c66 2e77 6f72 646c 6973 745f 6465 6c74  lf.wordlist_delt
-00012c10: 6128 652e 6d6b 7465 7874 2c20 6465 6c74  a(e.mktext, delt
-00012c20: 615f 776f 7264 6c69 7374 290d 0a20 2020  a_wordlist)..   
-00012c30: 2020 2020 2020 2020 2020 2020 206f 7267               org
-00012c40: 7061 7265 6e74 2e61 6464 5f6e 6f64 6528  parent.add_node(
-00012c50: 636f 7079 5f6e 6f64 6529 0d0a 2020 2020  copy_node)..    
-00012c60: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-00012c70: 6164 5f6f 7074 696f 6e61 6c3a 0d0a 2020  ad_optional:..  
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c90: 2020 666f 7220 7072 6f70 6572 7479 5f6f    for property_o
-00012ca0: 7020 696e 2073 656c 662e 6b65 726e 656c  p in self.kernel
-00012cb0: 2e6c 6f6f 6b75 705f 616c 6c28 2270 6174  .lookup_all("pat
-00012cc0: 685f 7570 6461 7465 722f 2e2a 2229 3a0d  h_updater/.*"):.
-00012cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ce0: 2020 2020 2020 2020 2070 726f 7065 7274           propert
-00012cf0: 795f 6f70 2873 656c 662e 6b65 726e 656c  y_op(self.kernel
-00012d00: 2e72 6f6f 742c 2063 6f70 795f 6e6f 6465  .root, copy_node
-00012d10: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00012d20: 2020 2020 2063 6f70 795f 6e6f 6465 732e       copy_nodes.
-00012d30: 6170 7065 6e64 2863 6f70 795f 6e6f 6465  append(copy_node
-00012d40: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00012d50: 2020 2020 2069 6620 6f72 676e 6f64 652e       if orgnode.
-00012d60: 7479 7065 2069 6e20 2822 6669 6c65 222c  type in ("file",
-00012d70: 2022 6772 6f75 7022 293a 0d0a 2020 2020   "group"):..    
-00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d90: 6e65 7770 6172 656e 7420 3d20 636f 7079  newparent = copy
-00012da0: 5f6e 6f64 650d 0a20 2020 2020 2020 2020  _node..         
-00012db0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00012dc0: 6e6f 6465 2069 6e20 6f72 676e 6f64 652e  node in orgnode.
-00012dd0: 6368 696c 6472 656e 3a0d 0a20 2020 2020  children:..     
-00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 2020 2063 6f70 795f 7369 6e67 6c65 5f6e     copy_single_n
-00012e00: 6f64 6528 0d0a 2020 2020 2020 2020 2020  ode(..          
-00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 636e 6f64 652c 206e 6577 7061 7265    cnode, newpare
-00012e30: 6e74 2c20 312c 2028 6e20 2b20 3129 202a  nt, 1, (n + 1) *
-00012e40: 2064 782c 2028 6e20 2b20 3129 202a 2064   dx, (n + 1) * d
-00012e50: 790d 0a20 2020 2020 2020 2020 2020 2020  y..             
-00012e60: 2020 2020 2020 2020 2020 2029 0d0a 0d0a             )....
-00012e70: 2020 2020 2020 2020 636f 7079 5f6e 6f64          copy_nod
-00012e80: 6573 203d 206c 6973 7428 290d 0a20 2020  es = list()..   
-00012e90: 2020 2020 2064 7820 3d20 7365 6c66 2e6c       dx = self.l
-00012ea0: 656e 6774 685f 7828 2233 6d6d 2229 0d0a  ength_x("3mm")..
-00012eb0: 2020 2020 2020 2020 6479 203d 2073 656c          dy = sel
-00012ec0: 662e 6c65 6e67 7468 5f79 2822 336d 6d22  f.length_y("3mm"
-00012ed0: 290d 0a20 2020 2020 2020 2061 6c6c 6461  )..        allda
-00012ee0: 7461 203d 206c 6973 7428 7365 6c66 2e65  ta = list(self.e
-00012ef0: 6c65 6d73 2865 6d70 6861 7369 7a65 643d  lems(emphasized=
-00012f00: 5472 7565 2929 0d0a 2020 2020 2020 2020  True))..        
-00012f10: 6d69 6e69 6d61 6c64 6174 6120 3d20 7365  minimaldata = se
-00012f20: 6c66 2e63 6f6e 6465 6e73 655f 656c 656d  lf.condense_elem
-00012f30: 656e 7473 2861 6c6c 6461 7461 2c20 6578  ents(alldata, ex
-00012f40: 7061 6e64 5f61 745f 656e 643d 4661 6c73  pand_at_end=Fals
-00012f50: 6529 0d0a 2020 2020 2020 2020 666f 7220  e)..        for 
-00012f60: 6520 696e 206d 696e 696d 616c 6461 7461  e in minimaldata
-00012f70: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00012f80: 6172 656e 7420 3d20 652e 7061 7265 6e74  arent = e.parent
-00012f90: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00012fa0: 7079 5f73 696e 676c 655f 6e6f 6465 2865  py_single_node(e
-00012fb0: 2c20 7061 7265 6e74 2c20 636f 7069 6573  , parent, copies
-00012fc0: 2c20 6478 2c20 6479 290d 0a0d 0a20 2020  , dx, dy)....   
-00012fd0: 2020 2020 2069 6620 7365 6c66 2e63 6c61       if self.cla
-00012fe0: 7373 6966 795f 6e65 773a 0d0a 2020 2020  ssify_new:..    
-00012ff0: 2020 2020 2020 2020 7365 6c66 2e63 6c61          self.cla
-00013000: 7373 6966 7928 636f 7079 5f6e 6f64 6573  ssify(copy_nodes
-00013010: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
-00013020: 662e 7365 745f 656d 7068 6173 6973 284e  f.set_emphasis(N
-00013030: 6f6e 6529 0d0a 0d0a 2020 2020 6465 6620  one)....    def 
-00013040: 6861 735f 776f 7264 6c69 7374 286e 6f64  has_wordlist(nod
-00013050: 6529 3a0d 0a20 2020 2020 2020 2072 6573  e):..        res
-00013060: 756c 7420 3d20 4661 6c73 650d 0a20 2020  ult = False..   
-00013070: 2020 2020 2074 7874 203d 2022 220d 0a20       txt = "".. 
-00013080: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
-00013090: 7228 6e6f 6465 2c20 2274 6578 7422 2920  r(node, "text") 
-000130a0: 616e 6420 6e6f 6465 2e74 6578 7420 6973  and node.text is
-000130b0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-000130c0: 2020 2020 2020 2020 7478 7420 3d20 7374          txt = st
-000130d0: 7228 6e6f 6465 2e74 6578 7429 0d0a 2020  r(node.text)..  
-000130e0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-000130f0: 286e 6f64 652c 2022 6d6b 7465 7874 2229  (node, "mktext")
-00013100: 2061 6e64 206e 6f64 652e 6d6b 7465 7874   and node.mktext
-00013110: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
-00013120: 2020 2020 2020 2020 2020 2074 7874 203d             txt =
-00013130: 2073 7472 286e 6f64 652e 6d6b 7465 7874   str(node.mktext
-00013140: 290d 0a20 2020 2020 2020 2023 2056 6572  )..        # Ver
-00013150: 7920 7374 7570 6964 2c20 6275 7420 676f  y stupid, but go
-00013160: 6f64 2065 6e6f 7567 680d 0a20 2020 2020  od enough..     
-00013170: 2020 2069 6620 227b 2220 696e 2074 7874     if "{" in txt
-00013180: 2061 6e64 2022 7d22 2069 6e20 7478 743a   and "}" in txt:
-00013190: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000131a0: 7375 6c74 203d 2054 7275 650d 0a20 2020  sult = True..   
-000131b0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-000131c0: 6c74 0d0a 0d0a 2020 2020 4074 7265 655f  lt....    @tree_
-000131d0: 636f 6e64 6974 696f 6e61 6c28 6c61 6d62  conditional(lamb
-000131e0: 6461 206e 6f64 653a 2068 6173 5f77 6f72  da node: has_wor
-000131f0: 646c 6973 7428 6e6f 6465 2929 0d0a 2020  dlist(node))..  
-00013200: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-00013210: 6e28 0d0a 2020 2020 2020 2020 5f28 2249  n(..        _("I
-00013220: 6e63 7265 6173 6520 576f 7264 6c69 7374  ncrease Wordlist
-00013230: 2d52 6566 6572 656e 6365 2229 2c0d 0a20  -Reference"),.. 
-00013240: 2020 2020 2020 206e 6f64 655f 7479 7065         node_type
-00013250: 3d28 0d0a 2020 2020 2020 2020 2020 2020  =(..            
-00013260: 2265 6c65 6d20 7465 7874 222c 0d0a 2020  "elem text",..  
-00013270: 2020 2020 2020 2020 2020 2265 6c65 6d20            "elem 
-00013280: 7061 7468 222c 0d0a 2020 2020 2020 2020  path",..        
-00013290: 292c 0d0a 2020 2020 2020 2020 6865 6c70  ),..        help
-000132a0: 3d5f 2822 4164 6a75 7374 7320 7468 6520  =_("Adjusts the 
-000132b0: 7265 6665 7265 6e63 6520 7661 6c75 6520  reference value 
-000132c0: 666f 7220 6120 776f 7264 6c69 7374 2c20  for a wordlist, 
-000132d0: 6965 207b 6e61 6d65 7d20 746f 207b 6e61  ie {name} to {na
-000132e0: 6d65 232b 317d 2229 2c0d 0a20 2020 2029  me#+1}"),..    )
-000132f0: 0d0a 2020 2020 6465 6620 776c 6973 745f  ..    def wlist_
-00013300: 706c 7573 2873 696e 676c 656e 6f64 652c  plus(singlenode,
-00013310: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00013320: 2020 2020 2064 6174 6120 3d20 6c69 7374       data = list
-00013330: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
-00013340: 6e6f 6465 2069 6e20 6c69 7374 2873 656c  node in list(sel
-00013350: 662e 656c 656d 7328 656d 7068 6173 697a  f.elems(emphasiz
-00013360: 6564 3d54 7275 6529 293a 0d0a 2020 2020  ed=True)):..    
-00013370: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-00013380: 6173 5f77 6f72 646c 6973 7428 6e6f 6465  as_wordlist(node
-00013390: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000133a0: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
-000133b0: 2020 2020 2020 2020 2020 6465 6c74 615f            delta_
-000133c0: 776f 7264 6c69 7374 203d 2031 0d0a 2020  wordlist = 1..  
-000133d0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-000133e0: 6174 7472 286e 6f64 652c 2022 7465 7874  attr(node, "text
-000133f0: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00013400: 2020 2020 206e 6f64 652e 7465 7874 203d       node.text =
-00013410: 2073 656c 662e 776f 7264 6c69 7374 5f64   self.wordlist_d
-00013420: 656c 7461 286e 6f64 652e 7465 7874 2c20  elta(node.text, 
-00013430: 6465 6c74 615f 776f 7264 6c69 7374 290d  delta_wordlist).
-00013440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013450: 206e 6f64 652e 616c 7465 7265 6428 290d   node.altered().
-00013460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013470: 2064 6174 612e 6170 7065 6e64 286e 6f64   data.append(nod
-00013480: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00013490: 656c 6966 2068 6173 6174 7472 286e 6f64  elif hasattr(nod
-000134a0: 652c 2022 6d6b 7465 7874 2229 3a0d 0a20  e, "mktext"):.. 
-000134b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000134c0: 6f64 652e 6d6b 7465 7874 203d 2073 656c  ode.mktext = sel
-000134d0: 662e 776f 7264 6c69 7374 5f64 656c 7461  f.wordlist_delta
-000134e0: 286e 6f64 652e 6d6b 7465 7874 2c20 6465  (node.mktext, de
-000134f0: 6c74 615f 776f 7264 6c69 7374 290d 0a20  lta_wordlist).. 
-00013500: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013510: 6f72 2070 726f 7065 7274 795f 6f70 2069  or property_op i
-00013520: 6e20 7365 6c66 2e6b 6572 6e65 6c2e 6c6f  n self.kernel.lo
-00013530: 6f6b 7570 5f61 6c6c 2822 7061 7468 5f75  okup_all("path_u
-00013540: 7064 6174 6572 2f2e 2a22 293a 0d0a 2020  pdater/.*"):..  
-00013550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013560: 2020 7072 6f70 6572 7479 5f6f 7028 7365    property_op(se
-00013570: 6c66 2e6b 6572 6e65 6c2e 726f 6f74 2c20  lf.kernel.root, 
-00013580: 6e6f 6465 290d 0a20 2020 2020 2020 2020  node)..         
-00013590: 2020 2020 2020 2064 6174 612e 6170 7065         data.appe
-000135a0: 6e64 286e 6f64 6529 0d0a 2020 2020 2020  nd(node)..      
-000135b0: 2020 7365 6c66 2e73 6967 6e61 6c28 2265    self.signal("e
-000135c0: 6c65 6d65 6e74 5f70 726f 7065 7274 795f  lement_property_
-000135d0: 7570 6461 7465 222c 2064 6174 6129 0d0a  update", data)..
-000135e0: 0d0a 2020 2020 4074 7265 655f 636f 6e64  ..    @tree_cond
-000135f0: 6974 696f 6e61 6c28 6c61 6d62 6461 206e  itional(lambda n
-00013600: 6f64 653a 2068 6173 5f77 6f72 646c 6973  ode: has_wordlis
-00013610: 7428 6e6f 6465 2929 0d0a 2020 2020 4074  t(node))..    @t
-00013620: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
-00013630: 2020 2020 2020 2020 5f28 2244 6563 7265          _("Decre
-00013640: 6173 6520 576f 7264 6c69 7374 2d52 6566  ase Wordlist-Ref
-00013650: 6572 656e 6365 2229 2c0d 0a20 2020 2020  erence"),..     
-00013660: 2020 206e 6f64 655f 7479 7065 3d28 0d0a     node_type=(..
-00013670: 2020 2020 2020 2020 2020 2020 2265 6c65              "ele
-00013680: 6d20 7465 7874 222c 0d0a 2020 2020 2020  m text",..      
-00013690: 2020 2020 2020 2265 6c65 6d20 7061 7468        "elem path
-000136a0: 222c 0d0a 2020 2020 2020 2020 292c 0d0a  ",..        ),..
-000136b0: 2020 2020 2020 2020 6865 6c70 3d5f 2822          help=_("
-000136c0: 4164 6a75 7374 7320 7468 6520 7265 6665  Adjusts the refe
-000136d0: 7265 6e63 6520 7661 6c75 6520 666f 7220  rence value for 
-000136e0: 6120 776f 7264 6c69 7374 2c20 6965 207b  a wordlist, ie {
-000136f0: 6e61 6d65 232b 337d 2074 6f20 7b6e 616d  name#+3} to {nam
-00013700: 6523 2b32 7d22 292c 0d0a 2020 2020 290d  e#+2}"),..    ).
-00013710: 0a20 2020 2064 6566 2077 6c69 7374 5f6d  .    def wlist_m
-00013720: 696e 7573 2873 696e 676c 656e 6f64 652c  inus(singlenode,
-00013730: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00013740: 2020 2020 2064 6174 6120 3d20 6c69 7374       data = list
-00013750: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
-00013760: 6e6f 6465 2069 6e20 6c69 7374 2873 656c  node in list(sel
-00013770: 662e 656c 656d 7328 656d 7068 6173 697a  f.elems(emphasiz
-00013780: 6564 3d54 7275 6529 293a 0d0a 2020 2020  ed=True)):..    
-00013790: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-000137a0: 6173 5f77 6f72 646c 6973 7428 6e6f 6465  as_wordlist(node
-000137b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000137c0: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
-000137d0: 2020 2020 2020 2020 2020 6465 6c74 615f            delta_
-000137e0: 776f 7264 6c69 7374 203d 202d 310d 0a20  wordlist = -1.. 
-000137f0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-00013800: 7361 7474 7228 6e6f 6465 2c20 2274 6578  sattr(node, "tex
-00013810: 7422 293a 0d0a 2020 2020 2020 2020 2020  t"):..          
-00013820: 2020 2020 2020 6e6f 6465 2e74 6578 7420        node.text 
-00013830: 3d20 7365 6c66 2e77 6f72 646c 6973 745f  = self.wordlist_
-00013840: 6465 6c74 6128 6e6f 6465 2e74 6578 742c  delta(node.text,
-00013850: 2064 656c 7461 5f77 6f72 646c 6973 7429   delta_wordlist)
-00013860: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013870: 2020 6e6f 6465 2e61 6c74 6572 6564 2829    node.altered()
-00013880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013890: 2020 6461 7461 2e61 7070 656e 6428 6e6f    data.append(no
-000138a0: 6465 290d 0a20 2020 2020 2020 2020 2020  de)..           
-000138b0: 2065 6c69 6620 6861 7361 7474 7228 6e6f   elif hasattr(no
-000138c0: 6465 2c20 226d 6b74 6578 7422 293a 0d0a  de, "mktext"):..
-000138d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138e0: 6e6f 6465 2e6d 6b74 6578 7420 3d20 7365  node.mktext = se
-000138f0: 6c66 2e77 6f72 646c 6973 745f 6465 6c74  lf.wordlist_delt
-00013900: 6128 6e6f 6465 2e6d 6b74 6578 742c 2064  a(node.mktext, d
-00013910: 656c 7461 5f77 6f72 646c 6973 7429 0d0a  elta_wordlist)..
-00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013930: 666f 7220 7072 6f70 6572 7479 5f6f 7020  for property_op 
-00013940: 696e 2073 656c 662e 6b65 726e 656c 2e6c  in self.kernel.l
-00013950: 6f6f 6b75 705f 616c 6c28 2270 6174 685f  ookup_all("path_
-00013960: 7570 6461 7465 722f 2e2a 2229 3a0d 0a20  updater/.*"):.. 
-00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013980: 2020 2070 726f 7065 7274 795f 6f70 2873     property_op(s
-00013990: 656c 662e 6b65 726e 656c 2e72 6f6f 742c  elf.kernel.root,
-000139a0: 206e 6f64 6529 0d0a 2020 2020 2020 2020   node)..        
-000139b0: 2020 2020 2020 2020 6461 7461 2e61 7070          data.app
-000139c0: 656e 6428 6e6f 6465 290d 0a20 2020 2020  end(node)..     
-000139d0: 2020 2073 656c 662e 7369 676e 616c 2822     self.signal("
-000139e0: 656c 656d 656e 745f 7072 6f70 6572 7479  element_property
-000139f0: 5f75 7064 6174 6522 2c20 6461 7461 290d  _update", data).
-00013a00: 0a0d 0a20 2020 2040 7472 6565 5f63 6f6e  ...    @tree_con
-00013a10: 6469 7469 6f6e 616c 286c 616d 6264 6120  ditional(lambda 
-00013a20: 6e6f 6465 3a20 6861 735f 7665 6374 6f72  node: has_vector
-00013a30: 697a 6528 6e6f 6465 2929 0d0a 2020 2020  ize(node))..    
-00013a40: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
-00013a50: 224f 7574 6c69 6e65 2065 6c65 6d65 6e74  "Outline element
-00013a60: 2873 292e 2e2e 2229 290d 0a20 2020 2040  (s)..."))..    @
-00013a70: 7472 6565 5f69 7465 7261 7465 2822 6f66  tree_iterate("of
-00013a80: 6673 6574 222c 2031 2c20 3130 290d 0a20  fset", 1, 10).. 
-00013a90: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-00013aa0: 6f6e 280d 0a20 2020 2020 2020 205f 2822  on(..        _("
-00013ab0: 2e2e 2e77 6974 6820 7b6f 6666 7365 747d  ...with {offset}
-00013ac0: 6d6d 2064 6973 7461 6e63 6522 292c 0d0a  mm distance"),..
-00013ad0: 2020 2020 2020 2020 6e6f 6465 5f74 7970          node_typ
-00013ae0: 653d 656c 656d 5f6e 6f64 6573 2c0d 0a20  e=elem_nodes,.. 
-00013af0: 2020 2020 2020 2068 656c 703d 2222 2c0d         help="",.
-00013b00: 0a20 2020 2029 0d0a 2020 2020 6465 6620  .    )..    def 
-00013b10: 6d61 6b65 5f6f 7574 6c69 6e65 7328 6e6f  make_outlines(no
-00013b20: 6465 2c20 6f66 6673 6574 3d31 2c20 2a2a  de, offset=1, **
-00013b30: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00013b40: 2020 7365 6c66 2866 226f 7574 6c69 6e65    self(f"outline
-00013b50: 207b 6f66 6673 6574 7d6d 6d5c 6e22 290d   {offset}mm\n").
-00013b60: 0a20 2020 2020 2020 2073 656c 662e 7369  .        self.si
-00013b70: 676e 616c 2822 7265 6672 6573 685f 7472  gnal("refresh_tr
-00013b80: 6565 2229 0d0a 0d0a 2020 2020 6465 6620  ee")....    def 
-00013b90: 6861 735f 7665 6374 6f72 697a 6528 6e6f  has_vectorize(no
-00013ba0: 6465 293a 0d0a 2020 2020 2020 2020 7265  de):..        re
-00013bb0: 7375 6c74 203d 2046 616c 7365 0d0a 2020  sult = False..  
-00013bc0: 2020 2020 2020 6d61 6b65 5f76 6563 746f        make_vecto
-00013bd0: 7220 3d20 7365 6c66 2e6c 6f6f 6b75 7028  r = self.lookup(
-00013be0: 2272 656e 6465 722d 6f70 2f6d 616b 655f  "render-op/make_
-00013bf0: 7665 6374 6f72 2229 0d0a 2020 2020 2020  vector")..      
-00013c00: 2020 6966 206d 616b 655f 7665 6374 6f72    if make_vector
-00013c10: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00013c20: 6573 756c 7420 3d20 5472 7565 0d0a 2020  esult = True..  
-00013c30: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00013c40: 756c 740d 0a0d 0a20 2020 2040 7472 6565  ult....    @tree
-00013c50: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
-00013c60: 6264 6120 6e6f 6465 3a20 6861 735f 7665  bda node: has_ve
-00013c70: 6374 6f72 697a 6528 6e6f 6465 2929 0d0a  ctorize(node))..
-00013c80: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-00013c90: 696f 6e28 0d0a 2020 2020 2020 2020 5f28  ion(..        _(
-00013ca0: 2254 7261 6365 2062 6974 6d61 7022 292c  "Trace bitmap"),
-00013cb0: 0d0a 2020 2020 2020 2020 6e6f 6465 5f74  ..        node_t
-00013cc0: 7970 653d 280d 0a20 2020 2020 2020 2020  ype=(..         
-00013cd0: 2020 2022 656c 656d 2074 6578 7422 2c0d     "elem text",.
-00013ce0: 0a20 2020 2020 2020 2020 2020 2022 656c  .            "el
-00013cf0: 656d 2069 6d61 6765 222c 0d0a 2020 2020  em image",..    
-00013d00: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
-00013d10: 6865 6c70 3d5f 2822 5665 6374 6f72 697a  help=_("Vectoriz
-00013d20: 6520 7468 6520 6769 7665 6e20 656c 656d  e the given elem
-00013d30: 656e 7422 292c 0d0a 2020 2020 290d 0a20  ent"),..    ).. 
-00013d40: 2020 2064 6566 2074 7261 6365 5f62 6974     def trace_bit
-00013d50: 6d61 7028 6e6f 6465 2c20 2a2a 6b77 6172  map(node, **kwar
-00013d60: 6773 293a 0d0a 2020 2020 2020 2020 7365  gs):..        se
-00013d70: 6c66 2822 7665 6374 6f72 697a 655c 6e22  lf("vectorize\n"
-00013d80: 290d 0a0d 0a20 2020 2040 7472 6565 5f63  )....    @tree_c
-00013d90: 6f6e 6469 7469 6f6e 616c 286c 616d 6264  onditional(lambd
-00013da0: 6120 6e6f 6465 3a20 6e6f 7420 6973 5f72  a node: not is_r
-00013db0: 6567 6d61 726b 286e 6f64 6529 290d 0a20  egmark(node)).. 
-00013dc0: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-00013dd0: 6f6e 280d 0a20 2020 2020 2020 205f 2822  on(..        _("
-00013de0: 436f 6e76 6572 7420 746f 2070 6174 6822  Convert to path"
-00013df0: 292c 0d0a 2020 2020 2020 2020 6e6f 6465  ),..        node
-00013e00: 5f74 7970 653d 280d 0a20 2020 2020 2020  _type=(..       
-00013e10: 2020 2020 2022 656c 656d 2065 6c6c 6970       "elem ellip
-00013e20: 7365 222c 0d0a 2020 2020 2020 2020 2020  se",..          
-00013e30: 2020 2265 6c65 6d20 7061 7468 222c 0d0a    "elem path",..
-00013e40: 2020 2020 2020 2020 2020 2020 2265 6c65              "ele
-00013e50: 6d20 706f 6c79 6c69 6e65 222c 0d0a 2020  m polyline",..  
-00013e60: 2020 2020 2020 2020 2020 2265 6c65 6d20            "elem 
-00013e70: 7265 6374 222c 0d0a 2020 2020 2020 2020  rect",..        
-00013e80: 2020 2020 2265 6c65 6d20 6c69 6e65 222c      "elem line",
-00013e90: 0d0a 2020 2020 2020 2020 292c 0d0a 2020  ..        ),..  
-00013ea0: 2020 2020 2020 6865 6c70 3d22 222c 0d0a        help="",..
-00013eb0: 2020 2020 290d 0a20 2020 2064 6566 2063      )..    def c
-00013ec0: 6f6e 7665 7274 5f74 6f5f 7061 7468 2873  onvert_to_path(s
-00013ed0: 696e 676c 656e 6f64 652c 202a 2a6b 7761  inglenode, **kwa
-00013ee0: 7267 7329 3a0d 0a20 2020 2020 2020 2066  rgs):..        f
-00013ef0: 6f72 206e 6f64 6520 696e 206c 6973 7428  or node in list(
-00013f00: 7365 6c66 2e65 6c65 6d73 2865 6d70 6861  self.elems(empha
-00013f10: 7369 7a65 643d 5472 7565 2929 3a0d 0a20  sized=True)):.. 
-00013f20: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00013f30: 7420 6e6f 6465 206e 6f74 2069 6e20 280d  t node not in (.
-00013f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013f50: 2022 656c 656d 2065 6c6c 6970 7365 222c   "elem ellipse",
-00013f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013f70: 2020 2265 6c65 6d20 7061 7468 222c 0d0a    "elem path",..
-00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f90: 2265 6c65 6d20 706f 6c79 6c69 6e65 222c  "elem polyline",
-00013fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013fb0: 2020 2265 6c65 6d20 7265 6374 222c 0d0a    "elem rect",..
-00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fd0: 2265 6c65 6d20 6c69 6e65 222c 0d0a 2020  "elem line",..  
-00013fe0: 2020 2020 2020 2020 2020 293a 0d0a 2020            ):..  
-00013ff0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00014000: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00014010: 2020 2020 6f6c 6473 7475 6666 203d 205b      oldstuff = [
-00014020: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-00014030: 6f72 2061 7474 7269 6220 696e 2028 2273  or attrib in ("s
-00014040: 7472 6f6b 6522 2c20 2266 696c 6c22 2c20  troke", "fill", 
-00014050: 2273 7472 6f6b 655f 7769 6474 6822 2c20  "stroke_width", 
-00014060: 2273 7472 6f6b 655f 7363 616c 6564 2229  "stroke_scaled")
-00014070: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00014080: 2020 2069 6620 6861 7361 7474 7228 6e6f     if hasattr(no
-00014090: 6465 2c20 6174 7472 6962 293a 0d0a 2020  de, attrib):..  
-000140a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140b0: 2020 6f6c 6476 616c 203d 2067 6574 6174    oldval = getat
-000140c0: 7472 286e 6f64 652c 2061 7474 7269 622c  tr(node, attrib,
-000140d0: 204e 6f6e 6529 0d0a 2020 2020 2020 2020   None)..        
-000140e0: 2020 2020 2020 2020 2020 2020 6f6c 6473              olds
-000140f0: 7475 6666 2e61 7070 656e 6428 5b61 7474  tuff.append([att
-00014100: 7269 622c 206f 6c64 7661 6c5d 290d 0a20  rib, oldval]).. 
-00014110: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-00014120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014130: 2070 6174 6820 3d20 6e6f 6465 2e61 735f   path = node.as_
-00014140: 7061 7468 2829 0d0a 2020 2020 2020 2020  path()..        
-00014150: 2020 2020 2020 2020 2320 5468 6572 6520          # There 
-00014160: 6172 6520 736f 6d65 2063 6861 6c6c 656e  are some challen
-00014170: 6765 7320 6172 6f75 6e64 2074 6865 2074  ges around the t
-00014180: 7265 6174 6d65 6e74 0d0a 2020 2020 2020  reatment..      
-00014190: 2020 2020 2020 2020 2020 2320 6f66 2061            # of a
-000141a0: 7263 7320 7769 7468 696e 2073 7667 656c  rcs within svgel
-000141b0: 656d 656e 7473 2c20 736f 206c 6574 2773  ements, so let's
-000141c0: 2063 6972 6375 6d76 656e 740d 0a20 2020   circumvent..   
-000141d0: 2020 2020 2020 2020 2020 2020 2023 2074               # t
-000141e0: 6865 6d20 666f 7220 7468 6520 7469 6d65  hem for the time
-000141f0: 2062 6569 6e67 2028 756e 7469 6c20 7265   being (until re
-00014200: 736f 6c76 6564 290d 0a20 2020 2020 2020  solved)..       
-00014210: 2020 2020 2020 2020 2023 2062 7920 7265           # by re
-00014220: 706c 6163 696e 6720 6172 6320 7365 676d  placing arc segm
-00014230: 656e 7473 2077 6974 6820 6375 6269 6320  ents with cubic 
-00014240: 6265 7a69 6572 730d 0a20 2020 2020 2020  beziers..       
-00014250: 2020 2020 2020 2020 2069 6620 6e6f 6465           if node
-00014260: 2e74 7970 6520 696e 2028 2265 6c65 6d20  .type in ("elem 
-00014270: 7061 7468 222c 2022 656c 656d 2065 6c6c  path", "elem ell
-00014280: 6970 7365 2229 3a0d 0a20 2020 2020 2020  ipse"):..       
-00014290: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-000142a0: 682e 6170 7072 6f78 696d 6174 655f 6172  h.approximate_ar
-000142b0: 6373 5f77 6974 685f 6375 6269 6373 2829  cs_with_cubics()
-000142c0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-000142d0: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
-000142e0: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-000142f0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00014300: 2020 2020 2020 2020 2020 6e65 776e 6f64            newnod
-00014310: 6520 3d20 6e6f 6465 2e72 6570 6c61 6365  e = node.replace
-00014320: 5f6e 6f64 6528 7061 7468 3d70 6174 682c  _node(path=path,
-00014330: 2074 7970 653d 2265 6c65 6d20 7061 7468   type="elem path
-00014340: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00014350: 666f 7220 6974 656d 2069 6e20 6f6c 6473  for item in olds
-00014360: 7475 6666 3a0d 0a20 2020 2020 2020 2020  tuff:..         
-00014370: 2020 2020 2020 2073 6574 6174 7472 286e         setattr(n
-00014380: 6577 6e6f 6465 2c20 6974 656d 5b30 5d2c  ewnode, item[0],
-00014390: 2069 7465 6d5b 315d 290d 0a20 2020 2020   item[1])..     
-000143a0: 2020 2020 2020 206e 6577 6e6f 6465 2e61         newnode.a
-000143b0: 6c74 6572 6564 2829 0d0a 0d0a 2020 2020  ltered()....    
-000143c0: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
-000143d0: 2246 6c69 7022 2929 0d0a 2020 2020 4074  "Flip"))..    @t
-000143e0: 7265 655f 7365 7061 7261 746f 725f 6265  ree_separator_be
-000143f0: 666f 7265 2829 0d0a 2020 2020 4074 7265  fore()..    @tre
-00014400: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
-00014410: 6d62 6461 206e 6f64 653a 206e 6f74 2069  mbda node: not i
-00014420: 735f 7265 676d 6172 6b28 6e6f 6465 2929  s_regmark(node))
-00014430: 0d0a 2020 2020 4074 7265 655f 636f 6e64  ..    @tree_cond
-00014440: 6974 696f 6e61 6c5f 7472 7928 6c61 6d62  itional_try(lamb
-00014450: 6461 206e 6f64 653a 206e 6f64 652e 6361  da node: node.ca
-00014460: 6e5f 7363 616c 6529 0d0a 2020 2020 4074  n_scale)..    @t
-00014470: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
-00014480: 2020 2020 2020 2020 5f28 2248 6f72 697a          _("Horiz
-00014490: 6f6e 7461 6c6c 7922 292c 0d0a 2020 2020  ontally"),..    
-000144a0: 2020 2020 6e6f 6465 5f74 7970 653d 656c      node_type=el
-000144b0: 656d 5f67 726f 7570 5f6e 6f64 6573 2c0d  em_group_nodes,.
-000144c0: 0a20 2020 2020 2020 2068 656c 703d 5f28  .        help=_(
-000144d0: 224d 6972 726f 7220 486f 7269 7a6f 6e74  "Mirror Horizont
-000144e0: 616c 6c79 2229 2c0d 0a20 2020 2029 0d0a  ally"),..    )..
-000144f0: 2020 2020 6465 6620 6d69 7272 6f72 5f65      def mirror_e
-00014500: 6c65 6d28 6e6f 6465 2c20 2a2a 6b77 6172  lem(node, **kwar
-00014510: 6773 293a 0d0a 2020 2020 2020 2020 626f  gs):..        bo
-00014520: 756e 6473 203d 2073 656c 662e 5f65 6d70  unds = self._emp
-00014530: 6861 7369 7a65 645f 626f 756e 6473 0d0a  hasized_bounds..
-00014540: 2020 2020 2020 2020 6966 2062 6f75 6e64          if bound
-00014550: 7320 6973 204e 6f6e 653a 0d0a 2020 2020  s is None:..    
-00014560: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-00014570: 2020 2020 2020 2020 6365 6e74 6572 5f78          center_x
-00014580: 203d 2028 626f 756e 6473 5b32 5d20 2b20   = (bounds[2] + 
-00014590: 626f 756e 6473 5b30 5d29 202f 2032 2e30  bounds[0]) / 2.0
-000145a0: 0d0a 2020 2020 2020 2020 6365 6e74 6572  ..        center
-000145b0: 5f79 203d 2028 626f 756e 6473 5b33 5d20  _y = (bounds[3] 
-000145c0: 2b20 626f 756e 6473 5b31 5d29 202f 2032  + bounds[1]) / 2
-000145d0: 2e30 0d0a 2020 2020 2020 2020 7365 6c66  .0..        self
-000145e0: 2866 2273 6361 6c65 202d 3120 3120 7b63  (f"scale -1 1 {c
-000145f0: 656e 7465 725f 787d 207b 6365 6e74 6572  enter_x} {center
-00014600: 5f79 7d5c 6e22 290d 0a0d 0a20 2020 2040  _y}\n")....    @
-00014610: 7472 6565 5f63 6f6e 6469 7469 6f6e 616c  tree_conditional
-00014620: 286c 616d 6264 6120 6e6f 6465 3a20 6e6f  (lambda node: no
-00014630: 7420 6973 5f72 6567 6d61 726b 286e 6f64  t is_regmark(nod
-00014640: 6529 290d 0a20 2020 2040 7472 6565 5f73  e))..    @tree_s
-00014650: 7562 6d65 6e75 285f 2822 466c 6970 2229  ubmenu(_("Flip")
-00014660: 290d 0a20 2020 2040 7472 6565 5f63 6f6e  )..    @tree_con
-00014670: 6469 7469 6f6e 616c 5f74 7279 286c 616d  ditional_try(lam
-00014680: 6264 6120 6e6f 6465 3a20 6e6f 6465 2e63  bda node: node.c
-00014690: 616e 5f73 6361 6c65 290d 0a20 2020 2040  an_scale)..    @
-000146a0: 7472 6565 5f6f 7065 7261 7469 6f6e 280d  tree_operation(.
-000146b0: 0a20 2020 2020 2020 205f 2822 5665 7274  .        _("Vert
-000146c0: 6963 616c 6c79 2229 2c0d 0a20 2020 2020  ically"),..     
-000146d0: 2020 206e 6f64 655f 7479 7065 3d65 6c65     node_type=ele
-000146e0: 6d5f 6772 6f75 705f 6e6f 6465 732c 0d0a  m_group_nodes,..
-000146f0: 2020 2020 2020 2020 6865 6c70 3d5f 2822          help=_("
-00014700: 466c 6970 2056 6572 7469 6361 6c6c 7922  Flip Vertically"
-00014710: 292c 0d0a 2020 2020 290d 0a20 2020 2064  ),..    )..    d
-00014720: 6566 2066 6c69 705f 656c 656d 286e 6f64  ef flip_elem(nod
-00014730: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-00014740: 2020 2020 2020 2062 6f75 6e64 7320 3d20         bounds = 
-00014750: 7365 6c66 2e5f 656d 7068 6173 697a 6564  self._emphasized
-00014760: 5f62 6f75 6e64 730d 0a20 2020 2020 2020  _bounds..       
-00014770: 2069 6620 626f 756e 6473 2069 7320 4e6f   if bounds is No
-00014780: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00014790: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
-000147a0: 2063 656e 7465 725f 7820 3d20 2862 6f75   center_x = (bou
-000147b0: 6e64 735b 325d 202b 2062 6f75 6e64 735b  nds[2] + bounds[
-000147c0: 305d 2920 2f20 322e 300d 0a20 2020 2020  0]) / 2.0..     
-000147d0: 2020 2063 656e 7465 725f 7920 3d20 2862     center_y = (b
-000147e0: 6f75 6e64 735b 335d 202b 2062 6f75 6e64  ounds[3] + bound
-000147f0: 735b 315d 2920 2f20 322e 300d 0a20 2020  s[1]) / 2.0..   
-00014800: 2020 2020 2073 656c 6628 6622 7363 616c       self(f"scal
-00014810: 6520 3120 2d31 207b 6365 6e74 6572 5f78  e 1 -1 {center_x
-00014820: 7d20 7b63 656e 7465 725f 797d 5c6e 2229  } {center_y}\n")
-00014830: 0d0a 0d0a 2020 2020 4074 7265 655f 636f  ....    @tree_co
-00014840: 6e64 6974 696f 6e61 6c28 6c61 6d62 6461  nditional(lambda
-00014850: 206e 6f64 653a 206e 6f74 2069 735f 7265   node: not is_re
-00014860: 676d 6172 6b28 6e6f 6465 2929 0d0a 2020  gmark(node))..  
-00014870: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
-00014880: 6e61 6c5f 7472 7928 6c61 6d62 6461 206e  nal_try(lambda n
-00014890: 6f64 653a 206e 6f64 652e 6361 6e5f 7363  ode: node.can_sc
-000148a0: 616c 6529 0d0a 2020 2020 4074 7265 655f  ale)..    @tree_
-000148b0: 7375 626d 656e 7528 5f28 2253 6361 6c65  submenu(_("Scale
-000148c0: 2229 290d 0a20 2020 2040 7472 6565 5f69  "))..    @tree_i
-000148d0: 7465 7261 7465 2822 7363 616c 6522 2c20  terate("scale", 
-000148e0: 3235 2c20 312c 202d 3129 0d0a 2020 2020  25, 1, -1)..    
-000148f0: 4074 7265 655f 6361 6c63 2822 7363 616c  @tree_calc("scal
-00014900: 655f 7065 7263 656e 7422 2c20 6c61 6d62  e_percent", lamb
-00014910: 6461 2069 3a20 6622 7b28 3630 302e 3020  da i: f"{(600.0 
-00014920: 2f20 666c 6f61 7428 6929 293a 2e32 667d  / float(i)):.2f}
-00014930: 2229 0d0a 2020 2020 4074 7265 655f 6f70  ")..    @tree_op
-00014940: 6572 6174 696f 6e28 0d0a 2020 2020 2020  eration(..      
-00014950: 2020 5f28 2253 6361 6c65 207b 7363 616c    _("Scale {scal
-00014960: 655f 7065 7263 656e 747d 2522 292c 0d0a  e_percent}%"),..
-00014970: 2020 2020 2020 2020 6e6f 6465 5f74 7970          node_typ
-00014980: 653d 656c 656d 5f67 726f 7570 5f6e 6f64  e=elem_group_nod
-00014990: 6573 2c0d 0a20 2020 2020 2020 2068 656c  es,..        hel
-000149a0: 703d 5f28 2253 6361 6c65 2045 6c65 6d65  p=_("Scale Eleme
-000149b0: 6e74 2229 2c0d 0a20 2020 2029 0d0a 2020  nt"),..    )..  
-000149c0: 2020 6465 6620 7363 616c 655f 656c 656d    def scale_elem
-000149d0: 5f61 6d6f 756e 7428 6e6f 6465 2c20 7363  _amount(node, sc
-000149e0: 616c 652c 202a 2a6b 7761 7267 7329 3a0d  ale, **kwargs):.
-000149f0: 0a20 2020 2020 2020 2073 6361 6c65 203d  .        scale =
-00014a00: 2036 2e30 202f 2066 6c6f 6174 2873 6361   6.0 / float(sca
-00014a10: 6c65 290d 0a20 2020 2020 2020 2062 6f75  le)..        bou
-00014a20: 6e64 7320 3d20 7365 6c66 2e5f 656d 7068  nds = self._emph
-00014a30: 6173 697a 6564 5f62 6f75 6e64 730d 0a20  asized_bounds.. 
-00014a40: 2020 2020 2020 2069 6620 626f 756e 6473         if bounds
-00014a50: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
-00014a60: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-00014a70: 2020 2020 2020 2063 656e 7465 725f 7820         center_x 
-00014a80: 3d20 2862 6f75 6e64 735b 325d 202b 2062  = (bounds[2] + b
-00014a90: 6f75 6e64 735b 305d 2920 2f20 322e 300d  ounds[0]) / 2.0.
-00014aa0: 0a20 2020 2020 2020 2063 656e 7465 725f  .        center_
-00014ab0: 7920 3d20 2862 6f75 6e64 735b 335d 202b  y = (bounds[3] +
-00014ac0: 2062 6f75 6e64 735b 315d 2920 2f20 322e   bounds[1]) / 2.
-00014ad0: 300d 0a20 2020 2020 2020 2073 656c 6628  0..        self(
-00014ae0: 6622 7363 616c 6520 7b73 6361 6c65 7d20  f"scale {scale} 
-00014af0: 7b73 6361 6c65 7d20 7b63 656e 7465 725f  {scale} {center_
-00014b00: 787d 207b 6365 6e74 6572 5f79 7d5c 6e22  x} {center_y}\n"
-00014b10: 290d 0a0d 0a20 2020 2023 2040 7472 6565  )....    # @tree
-00014b20: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
-00014b30: 6264 6120 6e6f 6465 3a20 6973 696e 7374  bda node: isinst
-00014b40: 616e 6365 286e 6f64 652e 6f62 6a65 6374  ance(node.object
-00014b50: 2c20 5356 4745 6c65 6d65 6e74 2929 0d0a  , SVGElement))..
-00014b60: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
-00014b70: 696f 6e61 6c28 6c61 6d62 6461 206e 6f64  ional(lambda nod
-00014b80: 653a 206e 6f74 2069 735f 7265 676d 6172  e: not is_regmar
-00014b90: 6b28 6e6f 6465 2929 0d0a 2020 2020 4074  k(node))..    @t
-00014ba0: 7265 655f 636f 6e64 6974 696f 6e61 6c5f  ree_conditional_
-00014bb0: 7472 7928 6c61 6d62 6461 206e 6f64 653a  try(lambda node:
-00014bc0: 206e 6f64 652e 6361 6e5f 726f 7461 7465   node.can_rotate
-00014bd0: 290d 0a20 2020 2040 7472 6565 5f73 7562  )..    @tree_sub
-00014be0: 6d65 6e75 285f 2822 526f 7461 7465 2229  menu(_("Rotate")
-00014bf0: 290d 0a20 2020 2040 7472 6565 5f76 616c  )..    @tree_val
-00014c00: 7565 7328 0d0a 2020 2020 2020 2020 2261  ues(..        "a
-00014c10: 6e67 6c65 222c 0d0a 2020 2020 2020 2020  ngle",..        
-00014c20: 280d 0a20 2020 2020 2020 2020 2020 2031  (..            1
-00014c30: 3830 2c0d 0a20 2020 2020 2020 2020 2020  80,..           
-00014c40: 2031 3530 2c0d 0a20 2020 2020 2020 2020   150,..         
-00014c50: 2020 2031 3335 2c0d 0a20 2020 2020 2020     135,..       
-00014c60: 2020 2020 2031 3230 2c0d 0a20 2020 2020       120,..     
-00014c70: 2020 2020 2020 2039 302c 0d0a 2020 2020         90,..    
-00014c80: 2020 2020 2020 2020 3630 2c0d 0a20 2020          60,..   
-00014c90: 2020 2020 2020 2020 2034 352c 0d0a 2020           45,..  
-00014ca0: 2020 2020 2020 2020 2020 3330 2c0d 0a20            30,.. 
-00014cb0: 2020 2020 2020 2020 2020 2032 302c 0d0a             20,..
-00014cc0: 2020 2020 2020 2020 2020 2020 3135 2c0d              15,.
-00014cd0: 0a20 2020 2020 2020 2020 2020 2031 302c  .            10,
-00014ce0: 0d0a 2020 2020 2020 2020 2020 2020 352c  ..            5,
-00014cf0: 0d0a 2020 2020 2020 2020 2020 2020 342c  ..            4,
-00014d00: 0d0a 2020 2020 2020 2020 2020 2020 332c  ..            3,
-00014d10: 0d0a 2020 2020 2020 2020 2020 2020 322c  ..            2,
-00014d20: 0d0a 2020 2020 2020 2020 2020 2020 312c  ..            1,
-00014d30: 0d0a 2020 2020 2020 2020 2020 2020 2d31  ..            -1
-00014d40: 2c0d 0a20 2020 2020 2020 2020 2020 202d  ,..            -
-00014d50: 322c 0d0a 2020 2020 2020 2020 2020 2020  2,..            
-00014d60: 2d33 2c0d 0a20 2020 2020 2020 2020 2020  -3,..           
-00014d70: 202d 342c 0d0a 2020 2020 2020 2020 2020   -4,..          
-00014d80: 2020 2d35 2c0d 0a20 2020 2020 2020 2020    -5,..         
-00014d90: 2020 202d 3130 2c0d 0a20 2020 2020 2020     -10,..       
-00014da0: 2020 2020 202d 3135 2c0d 0a20 2020 2020       -15,..     
-00014db0: 2020 2020 2020 202d 3230 2c0d 0a20 2020         -20,..   
-00014dc0: 2020 2020 2020 2020 202d 3330 2c0d 0a20           -30,.. 
-00014dd0: 2020 2020 2020 2020 2020 202d 3435 2c0d             -45,.
-00014de0: 0a20 2020 2020 2020 2020 2020 202d 3630  .            -60
-00014df0: 2c0d 0a20 2020 2020 2020 2020 2020 202d  ,..            -
-00014e00: 3930 2c0d 0a20 2020 2020 2020 2029 2c0d  90,..        ),.
-00014e10: 0a20 2020 2029 0d0a 2020 2020 4074 7265  .    )..    @tre
-00014e20: 655f 6f70 6572 6174 696f 6e28 5f28 2252  e_operation(_("R
-00014e30: 6f74 6174 6520 7b61 6e67 6c65 7dc2 b022  otate {angle}.."
-00014e40: 292c 206e 6f64 655f 7479 7065 3d65 6c65  ), node_type=ele
-00014e50: 6d5f 6772 6f75 705f 6e6f 6465 732c 2068  m_group_nodes, h
-00014e60: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
-00014e70: 2072 6f74 6174 655f 656c 656d 5f61 6d6f   rotate_elem_amo
-00014e80: 756e 7428 6e6f 6465 2c20 616e 676c 652c  unt(node, angle,
-00014e90: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00014ea0: 2020 2020 2074 7572 6e73 203d 2066 6c6f       turns = flo
-00014eb0: 6174 2861 6e67 6c65 2920 2f20 3336 302e  at(angle) / 360.
-00014ec0: 300d 0a20 2020 2020 2020 2062 6f75 6e64  0..        bound
-00014ed0: 7320 3d20 7365 6c66 2e5f 656d 7068 6173  s = self._emphas
-00014ee0: 697a 6564 5f62 6f75 6e64 730d 0a20 2020  ized_bounds..   
-00014ef0: 2020 2020 2069 6620 626f 756e 6473 2069       if bounds i
-00014f00: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00014f10: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00014f20: 2020 2020 2063 656e 7465 725f 7820 3d20       center_x = 
-00014f30: 2862 6f75 6e64 735b 325d 202b 2062 6f75  (bounds[2] + bou
-00014f40: 6e64 735b 305d 2920 2f20 322e 300d 0a20  nds[0]) / 2.0.. 
-00014f50: 2020 2020 2020 2063 656e 7465 725f 7920         center_y 
-00014f60: 3d20 2862 6f75 6e64 735b 335d 202b 2062  = (bounds[3] + b
-00014f70: 6f75 6e64 735b 315d 2920 2f20 322e 300d  ounds[1]) / 2.0.
-00014f80: 0a20 2020 2020 2020 2073 656c 6628 6622  .        self(f"
-00014f90: 726f 7461 7465 207b 7475 726e 737d 7475  rotate {turns}tu
-00014fa0: 726e 207b 6365 6e74 6572 5f78 7d20 7b63  rn {center_x} {c
-00014fb0: 656e 7465 725f 797d 5c6e 2229 0d0a 2020  enter_y}\n")..  
-00014fc0: 2020 2020 2020 7365 6c66 2e73 6967 6e61        self.signa
-00014fd0: 6c28 2265 7874 2d6d 6f64 6966 6965 6422  l("ext-modified"
-00014fe0: 290d 0a0d 0a20 2020 2040 7472 6565 5f63  )....    @tree_c
-00014ff0: 6f6e 6469 7469 6f6e 616c 286c 616d 6264  onditional(lambd
-00015000: 6120 6e6f 6465 3a20 6e6f 7420 6973 5f72  a node: not is_r
-00015010: 6567 6d61 726b 286e 6f64 6529 290d 0a20  egmark(node)).. 
-00015020: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
-00015030: 6f6e 616c 286c 616d 6264 6120 6e6f 6465  onal(lambda node
-00015040: 3a20 6861 735f 6368 616e 6765 7328 6e6f  : has_changes(no
-00015050: 6465 2929 0d0a 2020 2020 4074 7265 655f  de))..    @tree_
-00015060: 636f 6e64 6974 696f 6e61 6c5f 7472 7928  conditional_try(
-00015070: 6c61 6d62 6461 206e 6f64 653a 206e 6f64  lambda node: nod
-00015080: 652e 6361 6e5f 6d6f 6469 6679 290d 0a20  e.can_modify).. 
-00015090: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-000150a0: 6f6e 285f 2822 5265 6966 7920 5573 6572  on(_("Reify User
-000150b0: 2043 6861 6e67 6573 2229 2c20 6e6f 6465   Changes"), node
-000150c0: 5f74 7970 653d 656c 656d 5f67 726f 7570  _type=elem_group
-000150d0: 5f6e 6f64 6573 2c20 6865 6c70 3d22 2229  _nodes, help="")
-000150e0: 0d0a 2020 2020 6465 6620 7265 6966 795f  ..    def reify_
-000150f0: 656c 656d 5f63 6861 6e67 6573 286e 6f64  elem_changes(nod
-00015100: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
-00015110: 2020 2020 2020 2073 656c 6628 2272 6569         self("rei
-00015120: 6679 5c6e 2229 0d0a 2020 2020 2020 2020  fy\n")..        
-00015130: 7365 6c66 2e73 6967 6e61 6c28 2265 7874  self.signal("ext
-00015140: 2d6d 6f64 6966 6965 6422 290d 0a0d 0a20  -modified").... 
-00015150: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
-00015160: 6f6e 616c 286c 616d 6264 6120 6e6f 6465  onal(lambda node
-00015170: 3a20 6e6f 7420 6973 5f72 6567 6d61 726b  : not is_regmark
-00015180: 286e 6f64 6529 290d 0a20 2020 2040 7472  (node))..    @tr
-00015190: 6565 5f63 6f6e 6469 7469 6f6e 616c 5f74  ee_conditional_t
-000151a0: 7279 286c 616d 6264 6120 6e6f 6465 3a20  ry(lambda node: 
-000151b0: 6e6f 6465 2e63 616e 5f6d 6f64 6966 7929  node.can_modify)
-000151c0: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
-000151d0: 6174 696f 6e28 5f28 2242 7265 616b 2053  ation(_("Break S
-000151e0: 7562 7061 7468 7322 292c 206e 6f64 655f  ubpaths"), node_
-000151f0: 7479 7065 3d22 656c 656d 2070 6174 6822  type="elem path"
-00015200: 2c20 6865 6c70 3d22 2229 0d0a 2020 2020  , help="")..    
-00015210: 6465 6620 6272 6561 6b5f 7375 6270 6174  def break_subpat
-00015220: 685f 656c 656d 286e 6f64 652c 202a 2a6b  h_elem(node, **k
-00015230: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00015240: 2073 656c 6628 2265 6c65 6d65 6e74 2073   self("element s
-00015250: 7562 7061 7468 5c6e 2229 0d0a 0d0a 2020  ubpath\n")....  
-00015260: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
-00015270: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
-00015280: 206e 6f74 2069 735f 7265 676d 6172 6b28   not is_regmark(
-00015290: 6e6f 6465 2929 0d0a 2020 2020 4074 7265  node))..    @tre
-000152a0: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
-000152b0: 6d62 6461 206e 6f64 653a 2068 6173 5f63  mbda node: has_c
-000152c0: 6861 6e67 6573 286e 6f64 6529 290d 0a20  hanges(node)).. 
-000152d0: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
-000152e0: 6f6e 616c 5f74 7279 286c 616d 6264 6120  onal_try(lambda 
-000152f0: 6e6f 6465 3a20 6e6f 6465 2e63 616e 5f6d  node: node.can_m
-00015300: 6f64 6966 7929 0d0a 2020 2020 4074 7265  odify)..    @tre
-00015310: 655f 6f70 6572 6174 696f 6e28 5f28 2252  e_operation(_("R
-00015320: 6573 6574 2075 7365 7220 6368 616e 6765  eset user change
-00015330: 7322 292c 206e 6f64 655f 7479 7065 3d65  s"), node_type=e
-00015340: 6c65 6d5f 6772 6f75 705f 6e6f 6465 732c  lem_group_nodes,
-00015350: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-00015360: 6566 2072 6573 6574 5f75 7365 725f 6368  ef reset_user_ch
-00015370: 616e 6765 7328 6e6f 6465 2c20 636f 7069  anges(node, copi
-00015380: 6573 3d31 2c20 2a2a 6b77 6172 6773 293a  es=1, **kwargs):
-00015390: 0d0a 2020 2020 2020 2020 7365 6c66 2822  ..        self("
-000153a0: 7265 7365 745c 6e22 290d 0a20 2020 2020  reset\n")..     
-000153b0: 2020 2073 656c 662e 7369 676e 616c 2822     self.signal("
-000153c0: 6578 742d 6d6f 6469 6669 6564 2229 0d0a  ext-modified")..
-000153d0: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
-000153e0: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
-000153f0: 5f28 224d 6572 6765 2069 7465 6d73 2229  _("Merge items")
-00015400: 2c0d 0a20 2020 2020 2020 206e 6f64 655f  ,..        node_
-00015410: 7479 7065 3d22 6772 6f75 7022 2c0d 0a20  type="group",.. 
-00015420: 2020 2020 2020 2068 656c 703d 5f28 224d         help=_("M
-00015430: 6572 6765 2074 6869 7320 6e6f 6465 2773  erge this node's
-00015440: 2063 6869 6c64 7265 6e20 696e 746f 2031   children into 1
-00015450: 2070 6174 682e 2229 2c0d 0a20 2020 2029   path."),..    )
-00015460: 0d0a 2020 2020 6465 6620 6d65 7267 655f  ..    def merge_
-00015470: 656c 656d 656e 7473 286e 6f64 652c 202a  elements(node, *
-00015480: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-00015490: 2020 2073 656c 6628 2265 6c65 6d65 6e74     self("element
-000154a0: 206d 6572 6765 5c6e 2229 0d0a 2020 2020   merge\n")..    
-000154b0: 2020 2020 2320 4973 2074 6865 2067 726f      # Is the gro
-000154c0: 7570 206e 6f77 2065 6d70 7479 3f20 2d2d  up now empty? --
-000154d0: 3e20 6465 6c65 7465 0d0a 2020 2020 2020  > delete..      
-000154e0: 2020 6966 206c 656e 286e 6f64 652e 6368    if len(node.ch
-000154f0: 696c 6472 656e 2920 3d3d 2030 3a0d 0a20  ildren) == 0:.. 
-00015500: 2020 2020 2020 2020 2020 206e 6f64 652e             node.
-00015510: 7265 6d6f 7665 5f6e 6f64 6528 290d 0a0d  remove_node()...
-00015520: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
-00015530: 7469 6f6e 616c 286c 616d 6264 6120 6e6f  tional(lambda no
-00015540: 6465 3a20 6e6f 6465 2e6c 6f63 6b29 0d0a  de: node.lock)..
-00015550: 2020 2020 4074 7265 655f 7365 7061 7261      @tree_separa
-00015560: 746f 725f 6265 666f 7265 2829 0d0a 2020  tor_before()..  
-00015570: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
-00015580: 6e28 0d0a 2020 2020 2020 2020 5f28 2255  n(..        _("U
-00015590: 6e6c 6f63 6b20 656c 656d 656e 742c 2061  nlock element, a
-000155a0: 6c6c 6f77 7320 6d61 6e69 7075 6c61 7469  llows manipulati
-000155b0: 6f6e 2229 2c20 6e6f 6465 5f74 7970 653d  on"), node_type=
-000155c0: 656c 656d 5f6e 6f64 6573 2c20 6865 6c70  elem_nodes, help
-000155d0: 3d22 220d 0a20 2020 2029 0d0a 2020 2020  =""..    )..    
-000155e0: 6465 6620 656c 656d 656e 745f 756e 6c6f  def element_unlo
-000155f0: 636b 5f6d 616e 6970 756c 6174 696f 6e73  ck_manipulations
-00015600: 286e 6f64 652c 202a 2a6b 7761 7267 7329  (node, **kwargs)
-00015610: 3a0d 0a20 2020 2020 2020 2073 656c 6628  :..        self(
-00015620: 2265 6c65 6d65 6e74 2075 6e6c 6f63 6b5c  "element unlock\
-00015630: 6e22 290d 0a0d 0a20 2020 2040 7472 6565  n")....    @tree
-00015640: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
-00015650: 6264 6120 6e6f 6465 3a20 6e6f 7420 6e6f  bda node: not no
-00015660: 6465 2e6c 6f63 6b29 0d0a 2020 2020 4074  de.lock)..    @t
-00015670: 7265 655f 7365 7061 7261 746f 725f 6265  ree_separator_be
-00015680: 666f 7265 2829 0d0a 2020 2020 4074 7265  fore()..    @tre
-00015690: 655f 6f70 6572 6174 696f 6e28 0d0a 2020  e_operation(..  
-000156a0: 2020 2020 2020 5f28 224c 6f63 6b20 656c        _("Lock el
-000156b0: 656d 656e 7473 2c20 7072 6576 656e 7473  ements, prevents
-000156c0: 206d 616e 6970 756c 6174 696f 6e73 2229   manipulations")
-000156d0: 2c20 6e6f 6465 5f74 7970 653d 656c 656d  , node_type=elem
-000156e0: 5f6e 6f64 6573 2c20 6865 6c70 3d22 220d  _nodes, help="".
-000156f0: 0a20 2020 2029 0d0a 2020 2020 6465 6620  .    )..    def 
-00015700: 656c 656d 656e 745f 6c6f 636b 5f6d 616e  element_lock_man
-00015710: 6970 756c 6174 696f 6e73 286e 6f64 652c  ipulations(node,
-00015720: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00015730: 2020 2020 2073 656c 6628 2265 6c65 6d65       self("eleme
-00015740: 6e74 206c 6f63 6b5c 6e22 290d 0a0d 0a20  nt lock\n").... 
-00015750: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
-00015760: 6f6e 616c 286c 616d 6264 6120 6e6f 6465  onal(lambda node
-00015770: 3a20 6e6f 6465 2e74 7970 6520 3d3d 2022  : node.type == "
-00015780: 6272 616e 6368 2072 6567 2229 0d0a 2020  branch reg")..  
-00015790: 2020 4074 7265 655f 7365 7061 7261 746f    @tree_separato
-000157a0: 725f 6265 666f 7265 2829 0d0a 2020 2020  r_before()..    
-000157b0: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
-000157c0: 5f28 2254 6f67 676c 6520 7669 7369 6269  _("Toggle visibi
-000157d0: 6c69 7479 206f 6620 7265 676d 6172 6b73  lity of regmarks
-000157e0: 2229 2c20 6e6f 6465 5f74 7970 653d 2262  "), node_type="b
-000157f0: 7261 6e63 6820 7265 6722 2c20 6865 6c70  ranch reg", help
-00015800: 3d22 2229 0d0a 2020 2020 6465 6620 746f  ="")..    def to
-00015810: 6767 6c65 5f76 6973 6962 696c 6974 7928  ggle_visibility(
-00015820: 6e6f 6465 2c20 2a2a 6b77 6172 6773 293a  node, **kwargs):
-00015830: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00015840: 6967 6e61 6c28 2274 6f67 676c 655f 7265  ignal("toggle_re
-00015850: 676d 6172 6b73 2229 0d0a 0d0a 2020 2020  gmarks")....    
-00015860: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
-00015870: 6c28 6c61 6d62 6461 206e 6f64 653a 2069  l(lambda node: i
-00015880: 735f 7265 676d 6172 6b28 6e6f 6465 2929  s_regmark(node))
-00015890: 0d0a 2020 2020 4074 7265 655f 7365 7061  ..    @tree_sepa
-000158a0: 7261 746f 725f 6265 666f 7265 2829 0d0a  rator_before()..
-000158b0: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-000158c0: 696f 6e28 5f28 224d 6f76 6520 6261 636b  ion(_("Move back
-000158d0: 2074 6f20 656c 656d 656e 7473 2229 2c20   to elements"), 
-000158e0: 6e6f 6465 5f74 7970 653d 656c 656d 5f67  node_type=elem_g
-000158f0: 726f 7570 5f6e 6f64 6573 2c20 6865 6c70  roup_nodes, help
-00015900: 3d22 2229 0d0a 2020 2020 6465 6620 6d6f  ="")..    def mo
-00015910: 7665 5f62 6163 6b28 6e6f 6465 2c20 2a2a  ve_back(node, **
-00015920: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00015930: 2020 2320 4472 6167 2061 6e64 2044 726f    # Drag and Dro
-00015940: 700d 0a20 2020 2020 2020 2077 6974 6820  p..        with 
-00015950: 7365 6c66 2e73 7461 7469 6328 226d 6f76  self.static("mov
-00015960: 655f 6261 636b 2229 3a0d 0a20 2020 2020  e_back"):..     
-00015970: 2020 2020 2020 2073 6967 6e61 6c5f 6e65         signal_ne
-00015980: 6564 6564 203d 2046 616c 7365 0d0a 2020  eded = False..  
-00015990: 2020 2020 2020 2020 2020 6472 6f70 5f6e            drop_n
-000159a0: 6f64 6520 3d20 7365 6c66 2e65 6c65 6d5f  ode = self.elem_
-000159b0: 6272 616e 6368 0d0a 2020 2020 2020 2020  branch..        
-000159c0: 2020 2020 6461 7461 203d 206c 6973 7428      data = list(
-000159d0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-000159e0: 6f72 2069 7465 6d20 696e 206c 6973 7428  or item in list(
-000159f0: 7365 6c66 2e72 6567 6d61 726b 7328 2929  self.regmarks())
-00015a00: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00015a10: 2020 2069 6620 6974 656d 2e73 656c 6563     if item.selec
-00015a20: 7465 643a 0d0a 2020 2020 2020 2020 2020  ted:..          
-00015a30: 2020 2020 2020 2020 2020 6461 7461 2e61            data.a
-00015a40: 7070 656e 6428 6974 656d 290d 0a20 2020  ppend(item)..   
-00015a50: 2020 2020 2020 2020 2066 6f72 2069 7465           for ite
-00015a60: 6d20 696e 2064 6174 613a 0d0a 2020 2020  m in data:..    
-00015a70: 2020 2020 2020 2020 2020 2020 6472 6f70              drop
-00015a80: 5f6e 6f64 652e 6472 6f70 2869 7465 6d29  _node.drop(item)
-00015a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015aa0: 2020 7369 676e 616c 5f6e 6565 6465 6420    signal_needed 
-00015ab0: 3d20 5472 7565 0d0a 0d0a 2020 2020 4074  = True....    @t
-00015ac0: 7265 655f 636f 6e64 6974 696f 6e61 6c28  ree_conditional(
-00015ad0: 6c61 6d62 6461 206e 6f64 653a 206e 6f74  lambda node: not
-00015ae0: 2069 735f 7265 676d 6172 6b28 6e6f 6465   is_regmark(node
-00015af0: 2929 0d0a 2020 2020 4074 7265 655f 7365  ))..    @tree_se
-00015b00: 7061 7261 746f 725f 6265 666f 7265 2829  parator_before()
-00015b10: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
-00015b20: 6174 696f 6e28 5f28 224d 6f76 6520 746f  ation(_("Move to
-00015b30: 2072 6567 6d61 726b 7322 292c 206e 6f64   regmarks"), nod
-00015b40: 655f 7479 7065 3d65 6c65 6d5f 6772 6f75  e_type=elem_grou
-00015b50: 705f 6e6f 6465 732c 2068 656c 703d 2222  p_nodes, help=""
-00015b60: 290d 0a20 2020 2064 6566 206d 6f76 655f  )..    def move_
-00015b70: 746f 5f72 6567 6d61 726b 286e 6f64 652c  to_regmark(node,
-00015b80: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00015b90: 2020 2020 2023 2044 7261 6720 616e 6420       # Drag and 
-00015ba0: 4472 6f70 0d0a 2020 2020 2020 2020 7769  Drop..        wi
-00015bb0: 7468 2073 656c 662e 7374 6174 6963 2822  th self.static("
-00015bc0: 6d6f 7665 5f74 6f5f 7265 6722 293a 0d0a  move_to_reg"):..
-00015bd0: 2020 2020 2020 2020 2020 2020 6472 6f70              drop
-00015be0: 5f6e 6f64 6520 3d20 7365 6c66 2e72 6567  _node = self.reg
-00015bf0: 5f62 7261 6e63 680d 0a20 2020 2020 2020  _branch..       
-00015c00: 2020 2020 2064 6174 6120 3d20 6c69 7374       data = list
-00015c10: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00015c20: 666f 7220 6974 656d 2069 6e20 6c69 7374  for item in list
-00015c30: 2873 656c 662e 656c 656d 735f 6e6f 6465  (self.elems_node
-00015c40: 7328 2929 3a0d 0a20 2020 2020 2020 2020  s()):..         
-00015c50: 2020 2020 2020 2069 6620 6974 656d 2e73         if item.s
-00015c60: 656c 6563 7465 643a 0d0a 2020 2020 2020  elected:..      
-00015c70: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00015c80: 7461 2e61 7070 656e 6428 6974 656d 290d  ta.append(item).
-00015c90: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00015ca0: 2069 7465 6d20 696e 2064 6174 613a 0d0a   item in data:..
-00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cc0: 2320 4e6f 2075 7365 6361 7365 2066 6f72  # No usecase for
-00015cd0: 2068 6176 696e 6720 6120 6c6f 636b 6564   having a locked
-00015ce0: 2072 6567 6d61 726b 2065 6c65 6d65 6e74   regmark element
-00015cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015d00: 2020 6966 2068 6173 6174 7472 2869 7465    if hasattr(ite
-00015d10: 6d2c 2022 6c6f 636b 2229 3a0d 0a20 2020  m, "lock"):..   
-00015d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d30: 2069 7465 6d2e 6c6f 636b 203d 2046 616c   item.lock = Fal
-00015d40: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-00015d50: 2020 2020 6472 6f70 5f6e 6f64 652e 6472      drop_node.dr
-00015d60: 6f70 2869 7465 6d29 0d0a 0d0a 2020 2020  op(item)....    
-00015d70: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
-00015d80: 6c28 6c61 6d62 6461 206e 6f64 653a 2069  l(lambda node: i
-00015d90: 735f 7265 676d 6172 6b28 6e6f 6465 2929  s_regmark(node))
-00015da0: 0d0a 2020 2020 4074 7265 655f 7365 7061  ..    @tree_sepa
-00015db0: 7261 746f 725f 6265 666f 7265 2829 0d0a  rator_before()..
-00015dc0: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-00015dd0: 696f 6e28 5f28 2243 7265 6174 6520 706c  ion(_("Create pl
-00015de0: 6163 656d 656e 7422 292c 206e 6f64 655f  acement"), node_
-00015df0: 7479 7065 3d65 6c65 6d5f 6e6f 6465 732c  type=elem_nodes,
-00015e00: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-00015e10: 6566 2072 6567 6d61 726b 5f61 735f 706c  ef regmark_as_pl
-00015e20: 6163 656d 656e 7428 6e6f 6465 2c20 2a2a  acement(node, **
-00015e30: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
-00015e40: 2020 6966 206e 6f64 6520 6973 204e 6f6e    if node is Non
-00015e50: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00015e60: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
-00015e70: 6966 2068 6173 6174 7472 286e 6f64 652c  if hasattr(node,
-00015e80: 2022 7061 7468 2229 3a0d 0a20 2020 2020   "path"):..     
-00015e90: 2020 2020 2020 2062 6220 3d20 6e6f 6465         bb = node
-00015ea0: 2e70 6174 682e 6262 6f78 2874 7261 6e73  .path.bbox(trans
-00015eb0: 666f 726d 6564 3d46 616c 7365 290d 0a20  formed=False).. 
-00015ec0: 2020 2020 2020 2065 6c69 6620 6861 7361         elif hasa
-00015ed0: 7474 7228 6e6f 6465 2c20 2273 6861 7065  ttr(node, "shape
-00015ee0: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00015ef0: 2062 6220 3d20 6e6f 6465 2e73 6861 7065   bb = node.shape
-00015f00: 2e62 626f 7828 7472 616e 7366 6f72 6d65  .bbox(transforme
-00015f10: 643d 4661 6c73 6529 0d0a 2020 2020 2020  d=False)..      
-00015f20: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00015f30: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00015f40: 2020 2020 2069 6620 6262 2069 7320 4e6f       if bb is No
-00015f50: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-00015f60: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
-00015f70: 2078 203d 2062 625b 305d 0d0a 2020 2020   x = bb[0]..    
-00015f80: 2020 2020 7920 3d20 6262 5b31 5d0d 0a20      y = bb[1].. 
-00015f90: 2020 2020 2020 2063 6f72 6e65 7220 3d20         corner = 
-00015fa0: 300d 0a20 2020 2020 2020 2074 7279 3a0d  0..        try:.
-00015fb0: 0a20 2020 2020 2020 2020 2020 2072 6f74  .            rot
-00015fc0: 6174 696f 6e20 3d20 6e6f 6465 2e6d 6174  ation = node.mat
-00015fd0: 7269 782e 726f 7461 7469 6f6e 2e61 735f  rix.rotation.as_
-00015fe0: 7261 6469 616e 730d 0a20 2020 2020 2020  radians..       
-00015ff0: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
-00016000: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
-00016010: 2020 2020 2072 6f74 6174 696f 6e20 3d20       rotation = 
-00016020: 300d 0a20 2020 2020 2020 2070 7420 3d20  0..        pt = 
-00016030: 6e6f 6465 2e6d 6174 7269 782e 706f 696e  node.matrix.poin
-00016040: 745f 696e 5f6d 6174 7269 785f 7370 6163  t_in_matrix_spac
-00016050: 6528 506f 696e 7428 6262 5b30 5d2c 2062  e(Point(bb[0], b
-00016060: 625b 315d 2929 0d0a 2020 2020 2020 2020  b[1]))..        
-00016070: 7820 3d20 7074 2e78 0d0a 2020 2020 2020  x = pt.x..      
-00016080: 2020 7920 3d20 7074 2e79 0d0a 2020 2020    y = pt.y..    
-00016090: 2020 2020 706c 6163 655f 6e6f 6465 203d      place_node =
-000160a0: 2073 656c 662e 6f70 5f62 7261 6e63 682e   self.op_branch.
-000160b0: 6164 6428 0d0a 2020 2020 2020 2020 2020  add(..          
-000160c0: 2020 7479 7065 3d22 706c 6163 6520 706f    type="place po
-000160d0: 696e 7422 2c20 783d 782c 2079 3d79 2c20  int", x=x, y=y, 
-000160e0: 636f 726e 6572 3d63 6f72 6e65 722c 2072  corner=corner, r
-000160f0: 6f74 6174 696f 6e3d 726f 7461 7469 6f6e  otation=rotation
-00016100: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-00016110: 2020 2020 2073 656c 662e 7369 676e 616c       self.signal
-00016120: 2822 7265 6672 6573 685f 7363 656e 6522  ("refresh_scene"
-00016130: 2c20 2253 6365 6e65 2229 0d0a 0d0a 2020  , "Scene")....  
-00016140: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
-00016150: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
-00016160: 2069 735f 7265 676d 6172 6b28 6e6f 6465   is_regmark(node
-00016170: 2929 0d0a 2020 2020 4074 7265 655f 7375  ))..    @tree_su
-00016180: 626d 656e 7528 5f28 2254 6f67 676c 6520  bmenu(_("Toggle 
-00016190: 4d61 676e 6574 2d4c 696e 6573 2229 290d  Magnet-Lines")).
-000161a0: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
-000161b0: 7469 6f6e 285f 2822 4172 6f75 6e64 2062  tion(_("Around b
-000161c0: 6f72 6465 7222 292c 206e 6f64 655f 7479  order"), node_ty
-000161d0: 7065 3d65 6c65 6d5f 6772 6f75 705f 6e6f  pe=elem_group_no
-000161e0: 6465 732c 2068 656c 703d 2222 290d 0a20  des, help="").. 
-000161f0: 2020 2064 6566 2072 6567 6d61 726b 5f74     def regmark_t
-00016200: 6f5f 6d61 676e 6574 5f31 286e 6f64 652c  o_magnet_1(node,
-00016210: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
-00016220: 2020 2020 2069 6620 6e6f 6465 2069 7320       if node is 
-00016230: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00016240: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
-00016250: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
-00016260: 7228 6e6f 6465 2c20 2262 6f75 6e64 7322  r(node, "bounds"
-00016270: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016280: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
-00016290: 7365 6c66 2e73 6967 6e61 6c28 226d 6167  self.signal("mag
-000162a0: 6e65 745f 6765 6e22 2c20 2822 6f75 7465  net_gen", ("oute
-000162b0: 7222 2c20 6e6f 6465 2929 0d0a 0d0a 2020  r", node))....  
-000162c0: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
-000162d0: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
-000162e0: 2069 735f 7265 676d 6172 6b28 6e6f 6465   is_regmark(node
-000162f0: 2929 0d0a 2020 2020 4074 7265 655f 7375  ))..    @tree_su
-00016300: 626d 656e 7528 5f28 2254 6f67 676c 6520  bmenu(_("Toggle 
-00016310: 4d61 676e 6574 2d4c 696e 6573 2229 290d  Magnet-Lines")).
-00016320: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
-00016330: 7469 6f6e 285f 2822 4174 2063 656e 7465  tion(_("At cente
-00016340: 7222 292c 206e 6f64 655f 7479 7065 3d65  r"), node_type=e
-00016350: 6c65 6d5f 6772 6f75 705f 6e6f 6465 732c  lem_group_nodes,
-00016360: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
-00016370: 6566 2072 6567 6d61 726b 5f74 6f5f 6d61  ef regmark_to_ma
-00016380: 676e 6574 5f32 286e 6f64 652c 202a 2a6b  gnet_2(node, **k
-00016390: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-000163a0: 2069 6620 6e6f 6465 2069 7320 4e6f 6e65   if node is None
-000163b0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000163c0: 6574 7572 6e0d 0a20 2020 2020 2020 2069  eturn..        i
-000163d0: 6620 6e6f 7420 6861 7361 7474 7228 6e6f  f not hasattr(no
-000163e0: 6465 2c20 2262 6f75 6e64 7322 293a 0d0a  de, "bounds"):..
-000163f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00016400: 726e 0d0a 2020 2020 2020 2020 7365 6c66  rn..        self
-00016410: 2e73 6967 6e61 6c28 226d 6167 6e65 745f  .signal("magnet_
-00016420: 6765 6e22 2c20 2822 6365 6e74 6572 222c  gen", ("center",
-00016430: 206e 6f64 6529 290d 0a0d 0a20 2020 2023   node))....    #
-00016440: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
-00016450: 616c 286c 616d 6264 6120 6e6f 6465 3a20  al(lambda node: 
-00016460: 6e6f 7420 6e6f 6465 2e6c 6f63 6b29 0d0a  not node.lock)..
-00016470: 2020 2020 2320 4074 7265 655f 636f 6e64      # @tree_cond
-00016480: 6974 696f 6e61 6c5f 7472 7928 6c61 6d62  itional_try(lamb
-00016490: 6461 206e 6f64 653a 206e 6f74 206e 6f64  da node: not nod
-000164a0: 652e 6c6f 636b 290d 0a20 2020 2023 2040  e.lock)..    # @
-000164b0: 7472 6565 5f6f 7065 7261 7469 6f6e 285f  tree_operation(_
-000164c0: 2822 4163 7475 616c 697a 6520 7069 7865  ("Actualize pixe
-000164d0: 6c73 2229 2c20 6e6f 6465 5f74 7970 653d  ls"), node_type=
-000164e0: 2265 6c65 6d20 696d 6167 6522 2c20 6865  "elem image", he
-000164f0: 6c70 3d22 2229 0d0a 2020 2020 2320 6465  lp="")..    # de
-00016500: 6620 696d 6167 655f 6163 7475 616c 697a  f image_actualiz
-00016510: 655f 7069 7865 6c73 286e 6f64 652c 202a  e_pixels(node, *
-00016520: 2a6b 7761 7267 7329 3a0d 0a20 2020 2023  *kwargs):..    #
-00016530: 2020 2020 2073 656c 6628 2269 6d61 6765       self("image
-00016540: 2072 6573 616d 706c 655c 6e22 290d 0a0d   resample\n")...
-00016550: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
-00016560: 7469 6f6e 616c 286c 616d 6264 6120 6e6f  tional(lambda no
-00016570: 6465 3a20 6e6f 7420 6e6f 6465 2e6c 6f63  de: not node.loc
-00016580: 6b29 0d0a 2020 2020 4074 7265 655f 7375  k)..    @tree_su
-00016590: 626d 656e 7528 5f28 225a 2d64 6570 7468  bmenu(_("Z-depth
-000165a0: 2064 6976 6964 6522 2929 0d0a 2020 2020   divide"))..    
-000165b0: 4074 7265 655f 6974 6572 6174 6528 2264  @tree_iterate("d
-000165c0: 6976 6964 6522 2c20 322c 2031 3029 0d0a  ivide", 2, 10)..
-000165d0: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-000165e0: 696f 6e28 5f28 2244 6976 6964 6520 696e  ion(_("Divide in
-000165f0: 746f 207b 6469 7669 6465 7d20 696d 6167  to {divide} imag
-00016600: 6573 2229 2c20 6e6f 6465 5f74 7970 653d  es"), node_type=
-00016610: 2265 6c65 6d20 696d 6167 6522 2c20 6865  "elem image", he
-00016620: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
-00016630: 696d 6167 655f 7a64 6570 7468 286e 6f64  image_zdepth(nod
-00016640: 652c 2064 6976 6964 653d 312c 202a 2a6b  e, divide=1, **k
-00016650: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00016660: 2069 6620 6e6f 6465 2e69 6d61 6765 2e6d   if node.image.m
-00016670: 6f64 6520 213d 2022 5247 4241 223a 0d0a  ode != "RGBA":..
-00016680: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
-00016690: 2e69 6d61 6765 203d 206e 6f64 652e 696d  .image = node.im
-000166a0: 6167 652e 636f 6e76 6572 7428 2252 4742  age.convert("RGB
-000166b0: 4122 290d 0a20 2020 2020 2020 2062 616e  A")..        ban
-000166c0: 6420 3d20 3235 3520 2f20 6469 7669 6465  d = 255 / divide
-000166d0: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
-000166e0: 696e 2072 616e 6765 2830 2c20 6469 7669  in range(0, divi
-000166f0: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
-00016700: 2020 7468 7265 7368 6f6c 645f 6d69 6e20    threshold_min 
-00016710: 3d20 6920 2a20 6261 6e64 0d0a 2020 2020  = i * band..    
-00016720: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
-00016730: 645f 6d61 7820 3d20 7468 7265 7368 6f6c  d_max = threshol
-00016740: 645f 6d69 6e20 2b20 6261 6e64 0d0a 2020  d_min + band..  
-00016750: 2020 2020 2020 2020 2020 7365 6c66 2866            self(f
-00016760: 2269 6d61 6765 2074 6872 6573 686f 6c64  "image threshold
-00016770: 207b 7468 7265 7368 6f6c 645f 6d69 6e7d   {threshold_min}
-00016780: 207b 7468 7265 7368 6f6c 645f 6d61 787d   {threshold_max}
-00016790: 5c6e 2229 0d0a 0d0a 2020 2020 4074 7265  \n")....    @tre
-000167a0: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
-000167b0: 6d62 6461 206e 6f64 653a 206e 6f64 652e  mbda node: node.
-000167c0: 6c6f 636b 290d 0a20 2020 2040 7472 6565  lock)..    @tree
-000167d0: 5f73 7562 6d65 6e75 285f 2822 496d 6167  _submenu(_("Imag
-000167e0: 6522 2929 0d0a 2020 2020 4074 7265 655f  e"))..    @tree_
-000167f0: 6f70 6572 6174 696f 6e28 5f28 2255 6e6c  operation(_("Unl
-00016800: 6f63 6b20 6d61 6e69 7075 6c61 7469 6f6e  ock manipulation
-00016810: 7322 292c 206e 6f64 655f 7479 7065 3d22  s"), node_type="
-00016820: 656c 656d 2069 6d61 6765 222c 2068 656c  elem image", hel
-00016830: 703d 2222 290d 0a20 2020 2064 6566 2069  p="")..    def i
-00016840: 6d61 6765 5f75 6e6c 6f63 6b5f 6d61 6e69  mage_unlock_mani
-00016850: 7075 6c61 7469 6f6e 7328 6e6f 6465 2c20  pulations(node, 
-00016860: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-00016870: 2020 2020 7365 6c66 2822 696d 6167 6520      self("image 
-00016880: 756e 6c6f 636b 5c6e 2229 0d0a 0d0a 2020  unlock\n")....  
-00016890: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
-000168a0: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
-000168b0: 206e 6f74 206e 6f64 652e 6c6f 636b 290d   not node.lock).
-000168c0: 0a20 2020 2040 7472 6565 5f73 7562 6d65  .    @tree_subme
-000168d0: 6e75 285f 2822 496d 6167 6522 2929 0d0a  nu(_("Image"))..
-000168e0: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
-000168f0: 696f 6e28 5f28 224c 6f63 6b20 6d61 6e69  ion(_("Lock mani
-00016900: 7075 6c61 7469 6f6e 7322 292c 206e 6f64  pulations"), nod
-00016910: 655f 7479 7065 3d22 656c 656d 2069 6d61  e_type="elem ima
-00016920: 6765 222c 2068 656c 703d 2222 290d 0a20  ge", help="").. 
-00016930: 2020 2064 6566 2069 6d61 6765 5f6c 6f63     def image_loc
-00016940: 6b5f 6d61 6e69 7075 6c61 7469 6f6e 7328  k_manipulations(
-00016950: 6e6f 6465 2c20 2a2a 6b77 6172 6773 293a  node, **kwargs):
-00016960: 0d0a 2020 2020 2020 2020 7365 6c66 2822  ..        self("
-00016970: 696d 6167 6520 6c6f 636b 5c6e 2229 0d0a  image lock\n")..
-00016980: 0d0a 2020 2020 4074 7265 655f 636f 6e64  ..    @tree_cond
-00016990: 6974 696f 6e61 6c28 6c61 6d62 6461 206e  itional(lambda n
-000169a0: 6f64 653a 206e 6f74 206e 6f64 652e 6c6f  ode: not node.lo
-000169b0: 636b 290d 0a20 2020 2040 7472 6565 5f73  ck)..    @tree_s
-000169c0: 7562 6d65 6e75 285f 2822 496d 6167 6522  ubmenu(_("Image"
-000169d0: 2929 0d0a 2020 2020 4074 7265 655f 6f70  ))..    @tree_op
-000169e0: 6572 6174 696f 6e28 5f28 2244 6974 6865  eration(_("Dithe
-000169f0: 7220 746f 2031 2062 6974 2229 2c20 6e6f  r to 1 bit"), no
-00016a00: 6465 5f74 7970 653d 2265 6c65 6d20 696d  de_type="elem im
-00016a10: 6167 6522 2c20 6865 6c70 3d22 2229 0d0a  age", help="")..
-00016a20: 2020 2020 6465 6620 696d 6167 655f 6469      def image_di
-00016a30: 7468 6572 286e 6f64 652c 202a 2a6b 7761  ther(node, **kwa
-00016a40: 7267 7329 3a0d 0a20 2020 2020 2020 2073  rgs):..        s
-00016a50: 656c 6628 2269 6d61 6765 2064 6974 6865  elf("image dithe
-00016a60: 725c 6e22 290d 0a0d 0a20 2020 2040 7472  r\n")....    @tr
-00016a70: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
-00016a80: 616d 6264 6120 6e6f 6465 3a20 6e6f 7420  ambda node: not 
-00016a90: 6e6f 6465 2e6c 6f63 6b29 0d0a 2020 2020  node.lock)..    
-00016aa0: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
-00016ab0: 2249 6d61 6765 2229 290d 0a20 2020 2040  "Image"))..    @
-00016ac0: 7472 6565 5f6f 7065 7261 7469 6f6e 285f  tree_operation(_
-00016ad0: 2822 496e 7665 7274 2069 6d61 6765 2229  ("Invert image")
-00016ae0: 2c20 6e6f 6465 5f74 7970 653d 2265 6c65  , node_type="ele
-00016af0: 6d20 696d 6167 6522 2c20 6865 6c70 3d22  m image", help="
-00016b00: 2229 0d0a 2020 2020 6465 6620 696d 6167  ")..    def imag
-00016b10: 655f 696e 7665 7274 286e 6f64 652c 202a  e_invert(node, *
-00016b20: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-00016b30: 2020 2073 656c 6628 2269 6d61 6765 2069     self("image i
-00016b40: 6e76 6572 745c 6e22 290d 0a0d 0a20 2020  nvert\n")....   
-00016b50: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
-00016b60: 616c 286c 616d 6264 6120 6e6f 6465 3a20  al(lambda node: 
-00016b70: 6e6f 7420 6e6f 6465 2e6c 6f63 6b29 0d0a  not node.lock)..
-00016b80: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
-00016b90: 7528 5f28 2249 6d61 6765 2229 290d 0a20  u(_("Image")).. 
-00016ba0: 2020 2040 7472 6565 5f6f 7065 7261 7469     @tree_operati
-00016bb0: 6f6e 285f 2822 4d69 7272 6f72 2068 6f72  on(_("Mirror hor
-00016bc0: 697a 6f6e 7461 6c22 292c 206e 6f64 655f  izontal"), node_
-00016bd0: 7479 7065 3d22 656c 656d 2069 6d61 6765  type="elem image
-00016be0: 222c 2068 656c 703d 2222 290d 0a20 2020  ", help="")..   
-00016bf0: 2064 6566 2069 6d61 6765 5f6d 6972 726f   def image_mirro
-00016c00: 7228 6e6f 6465 2c20 2a2a 6b77 6172 6773  r(node, **kwargs
-00016c10: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-00016c20: 2822 696d 6167 6520 6d69 7272 6f72 5c6e  ("image mirror\n
-00016c30: 2229 0d0a 0d0a 2020 2020 4074 7265 655f  ")....    @tree_
-00016c40: 636f 6e64 6974 696f 6e61 6c28 6c61 6d62  conditional(lamb
-00016c50: 6461 206e 6f64 653a 206e 6f74 206e 6f64  da node: not nod
-00016c60: 652e 6c6f 636b 290d 0a20 2020 2040 7472  e.lock)..    @tr
-00016c70: 6565 5f73 7562 6d65 6e75 285f 2822 496d  ee_submenu(_("Im
-00016c80: 6167 6522 2929 0d0a 2020 2020 4074 7265  age"))..    @tre
-00016c90: 655f 6f70 6572 6174 696f 6e28 5f28 2246  e_operation(_("F
-00016ca0: 6c69 7020 7665 7274 6963 616c 2229 2c20  lip vertical"), 
-00016cb0: 6e6f 6465 5f74 7970 653d 2265 6c65 6d20  node_type="elem 
-00016cc0: 696d 6167 6522 2c20 6865 6c70 3d22 2229  image", help="")
-00016cd0: 0d0a 2020 2020 6465 6620 696d 6167 655f  ..    def image_
-00016ce0: 666c 6970 286e 6f64 652c 202a 2a6b 7761  flip(node, **kwa
-00016cf0: 7267 7329 3a0d 0a20 2020 2020 2020 2073  rgs):..        s
-00016d00: 656c 6628 2269 6d61 6765 2066 6c69 705c  elf("image flip\
-00016d10: 6e22 290d 0a0d 0a20 2020 2040 7472 6565  n")....    @tree
-00016d20: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
-00016d30: 6264 6120 6e6f 6465 3a20 6e6f 7420 6e6f  bda node: not no
-00016d40: 6465 2e6c 6f63 6b29 0d0a 2020 2020 4074  de.lock)..    @t
-00016d50: 7265 655f 7375 626d 656e 7528 5f28 2249  ree_submenu(_("I
-00016d60: 6d61 6765 2229 290d 0a20 2020 2040 7472  mage"))..    @tr
-00016d70: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
-00016d80: 526f 7461 7465 2039 30c2 b020 4357 2229  Rotate 90.. CW")
-00016d90: 2c20 6e6f 6465 5f74 7970 653d 2265 6c65  , node_type="ele
-00016da0: 6d20 696d 6167 6522 2c20 6865 6c70 3d22  m image", help="
-00016db0: 2229 0d0a 2020 2020 6465 6620 696d 6167  ")..    def imag
-00016dc0: 655f 6377 286e 6f64 652c 202a 2a6b 7761  e_cw(node, **kwa
-00016dd0: 7267 7329 3a0d 0a20 2020 2020 2020 2073  rgs):..        s
-00016de0: 656c 6628 2269 6d61 6765 2063 775c 6e22  elf("image cw\n"
-00016df0: 290d 0a0d 0a20 2020 2040 7472 6565 5f63  )....    @tree_c
-00016e00: 6f6e 6469 7469 6f6e 616c 286c 616d 6264  onditional(lambd
-00016e10: 6120 6e6f 6465 3a20 6e6f 7420 6e6f 6465  a node: not node
-00016e20: 2e6c 6f63 6b29 0d0a 2020 2020 4074 7265  .lock)..    @tre
-00016e30: 655f 7375 626d 656e 7528 5f28 2249 6d61  e_submenu(_("Ima
-00016e40: 6765 2229 290d 0a20 2020 2040 7472 6565  ge"))..    @tree
-00016e50: 5f6f 7065 7261 7469 6f6e 285f 2822 526f  _operation(_("Ro
-00016e60: 7461 7465 2039 30c2 b020 4343 5722 292c  tate 90.. CCW"),
-00016e70: 206e 6f64 655f 7479 7065 3d22 656c 656d   node_type="elem
-00016e80: 2069 6d61 6765 222c 2068 656c 703d 2222   image", help=""
-00016e90: 290d 0a20 2020 2064 6566 2069 6d61 6765  )..    def image
-00016ea0: 5f63 6377 286e 6f64 652c 202a 2a6b 7761  _ccw(node, **kwa
-00016eb0: 7267 7329 3a0d 0a20 2020 2020 2020 2073  rgs):..        s
-00016ec0: 656c 6628 2269 6d61 6765 2063 6377 5c6e  elf("image ccw\n
-00016ed0: 2229 0d0a 0d0a 2020 2020 4074 7265 655f  ")....    @tree_
-00016ee0: 7375 626d 656e 7528 5f28 2249 6d61 6765  submenu(_("Image
-00016ef0: 2229 290d 0a20 2020 2040 7472 6565 5f6f  "))..    @tree_o
-00016f00: 7065 7261 7469 6f6e 280d 0a20 2020 2020  peration(..     
-00016f10: 2020 205f 2822 5361 7665 206f 7269 6769     _("Save origi
-00016f20: 6e61 6c20 696d 6167 6520 746f 206f 7574  nal image to out
-00016f30: 7075 742e 706e 6722 292c 206e 6f64 655f  put.png"), node_
-00016f40: 7479 7065 3d22 656c 656d 2069 6d61 6765  type="elem image
-00016f50: 222c 2068 656c 703d 2222 0d0a 2020 2020  ", help=""..    
-00016f60: 290d 0a20 2020 2064 6566 2069 6d61 6765  )..    def image
-00016f70: 5f73 6176 6528 6e6f 6465 2c20 2a2a 6b77  _save(node, **kw
-00016f80: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00016f90: 7365 6c66 2822 696d 6167 6520 7361 7665  self("image save
-00016fa0: 206f 7574 7075 742e 706e 675c 6e22 290d   output.png\n").
-00016fb0: 0a0d 0a20 2020 2040 7472 6565 5f73 7562  ...    @tree_sub
-00016fc0: 6d65 6e75 285f 2822 496d 6167 6522 2929  menu(_("Image"))
-00016fd0: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
-00016fe0: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
-00016ff0: 5f28 2253 6176 6520 7072 6f63 6573 7365  _("Save processe
-00017000: 6420 696d 6167 6520 746f 206f 7574 7075  d image to outpu
-00017010: 742e 706e 6722 292c 206e 6f64 655f 7479  t.png"), node_ty
-00017020: 7065 3d22 656c 656d 2069 6d61 6765 222c  pe="elem image",
-00017030: 2068 656c 703d 2222 0d0a 2020 2020 290d   help=""..    ).
-00017040: 0a20 2020 2064 6566 2069 6d61 6765 5f73  .    def image_s
-00017050: 6176 655f 7072 6f63 6573 7365 6428 6e6f  ave_processed(no
-00017060: 6465 2c20 2a2a 6b77 6172 6773 293a 0d0a  de, **kwargs):..
-00017070: 2020 2020 2020 2020 7365 6c66 2822 696d          self("im
-00017080: 6167 6520 7361 7665 206f 7574 7075 742e  age save output.
-00017090: 706e 6720 2d2d 7072 6f63 6573 7365 645c  png --processed\
-000170a0: 6e22 290d 0a0d 0a20 2020 2040 7472 6565  n")....    @tree
-000170b0: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
-000170c0: 6264 6120 6e6f 6465 3a20 6c65 6e28 6e6f  bda node: len(no
-000170d0: 6465 2e63 6869 6c64 7265 6e29 203e 2030  de.children) > 0
-000170e0: 290d 0a20 2020 2040 7472 6565 5f73 6570  )..    @tree_sep
-000170f0: 6172 6174 6f72 5f62 6566 6f72 6528 290d  arator_before().
-00017100: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
-00017110: 7469 6f6e 280d 0a20 2020 2020 2020 205f  tion(..        _
-00017120: 2822 4578 7061 6e64 2061 6c6c 2063 6869  ("Expand all chi
-00017130: 6c64 7265 6e22 292c 0d0a 2020 2020 2020  ldren"),..      
-00017140: 2020 6e6f 6465 5f74 7970 653d 280d 0a20    node_type=(.. 
-00017150: 2020 2020 2020 2020 2020 2022 6f70 2063             "op c
-00017160: 7574 222c 0d0a 2020 2020 2020 2020 2020  ut",..          
-00017170: 2020 226f 7020 7261 7374 6572 222c 0d0a    "op raster",..
-00017180: 2020 2020 2020 2020 2020 2020 226f 7020              "op 
-00017190: 696d 6167 6522 2c0d 0a20 2020 2020 2020  image",..       
-000171a0: 2020 2020 2022 6f70 2065 6e67 7261 7665       "op engrave
-000171b0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000171c0: 226f 7020 646f 7473 222c 0d0a 2020 2020  "op dots",..    
-000171d0: 2020 2020 2020 2020 226f 7020 6861 7463          "op hatc
-000171e0: 6822 2c0d 0a20 2020 2020 2020 2020 2020  h",..           
-000171f0: 2022 6272 616e 6368 2065 6c65 6d73 222c   "branch elems",
-00017200: 0d0a 2020 2020 2020 2020 2020 2020 2262  ..            "b
-00017210: 7261 6e63 6820 6f70 7322 2c0d 0a20 2020  ranch ops",..   
-00017220: 2020 2020 2020 2020 2022 6272 616e 6368           "branch
-00017230: 2072 6567 222c 0d0a 2020 2020 2020 2020   reg",..        
-00017240: 2020 2020 2267 726f 7570 222c 0d0a 2020      "group",..  
-00017250: 2020 2020 2020 2020 2020 2266 696c 6522            "file"
-00017260: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00017270: 726f 6f74 222c 0d0a 2020 2020 2020 2020  root",..        
-00017280: 292c 0d0a 2020 2020 2020 2020 6865 6c70  ),..        help
-00017290: 3d5f 2822 4578 7061 6e64 2061 6c6c 2063  =_("Expand all c
-000172a0: 6869 6c64 7265 6e20 6f66 2074 6869 7320  hildren of this 
-000172b0: 6769 7665 6e20 6e6f 6465 2e22 292c 0d0a  given node."),..
-000172c0: 2020 2020 290d 0a20 2020 2064 6566 2065      )..    def e
-000172d0: 7870 616e 645f 616c 6c5f 6368 696c 6472  xpand_all_childr
-000172e0: 656e 286e 6f64 652c 202a 2a6b 7761 7267  en(node, **kwarg
-000172f0: 7329 3a0d 0a20 2020 2020 2020 206e 6f64  s):..        nod
-00017300: 652e 6e6f 7469 6679 5f65 7870 616e 6428  e.notify_expand(
-00017310: 290d 0a0d 0a20 2020 2040 7472 6565 5f63  )....    @tree_c
-00017320: 6f6e 6469 7469 6f6e 616c 286c 616d 6264  onditional(lambd
-00017330: 6120 6e6f 6465 3a20 6c65 6e28 6e6f 6465  a node: len(node
-00017340: 2e63 6869 6c64 7265 6e29 203e 2030 290d  .children) > 0).
-00017350: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
-00017360: 7469 6f6e 280d 0a20 2020 2020 2020 205f  tion(..        _
-00017370: 2822 436f 6c6c 6170 7365 2061 6c6c 2063  ("Collapse all c
-00017380: 6869 6c64 7265 6e22 292c 0d0a 2020 2020  hildren"),..    
-00017390: 2020 2020 6e6f 6465 5f74 7970 653d 280d      node_type=(.
-000173a0: 0a20 2020 2020 2020 2020 2020 2022 6f70  .            "op
-000173b0: 2063 7574 222c 0d0a 2020 2020 2020 2020   cut",..        
-000173c0: 2020 2020 226f 7020 7261 7374 6572 222c      "op raster",
-000173d0: 0d0a 2020 2020 2020 2020 2020 2020 226f  ..            "o
-000173e0: 7020 696d 6167 6522 2c0d 0a20 2020 2020  p image",..     
-000173f0: 2020 2020 2020 2022 6f70 2065 6e67 7261         "op engra
-00017400: 7665 222c 0d0a 2020 2020 2020 2020 2020  ve",..          
-00017410: 2020 226f 7020 646f 7473 222c 0d0a 2020    "op dots",..  
-00017420: 2020 2020 2020 2020 2020 226f 7020 6861            "op ha
-00017430: 7463 6822 2c0d 0a20 2020 2020 2020 2020  tch",..         
-00017440: 2020 2022 6272 616e 6368 2065 6c65 6d73     "branch elems
-00017450: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00017460: 2262 7261 6e63 6820 6f70 7322 2c0d 0a20  "branch ops",.. 
-00017470: 2020 2020 2020 2020 2020 2022 6272 616e             "bran
-00017480: 6368 2072 6567 222c 0d0a 2020 2020 2020  ch reg",..      
-00017490: 2020 2020 2020 2267 726f 7570 222c 0d0a        "group",..
-000174a0: 2020 2020 2020 2020 2020 2020 2266 696c              "fil
-000174b0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-000174c0: 2022 726f 6f74 222c 0d0a 2020 2020 2020   "root",..      
-000174d0: 2020 292c 0d0a 2020 2020 2020 2020 6865    ),..        he
-000174e0: 6c70 3d5f 2822 436f 6c6c 6170 7365 2061  lp=_("Collapse a
-000174f0: 6c6c 2063 6869 6c64 7265 6e20 6f66 2074  ll children of t
-00017500: 6869 7320 6769 7665 6e20 6e6f 6465 2e22  his given node."
-00017510: 292c 0d0a 2020 2020 290d 0a20 2020 2064  ),..    )..    d
-00017520: 6566 2063 6f6c 6c61 7073 655f 616c 6c5f  ef collapse_all_
-00017530: 6368 696c 6472 656e 286e 6f64 652c 202a  children(node, *
-00017540: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
-00017550: 2020 206e 6f64 652e 6e6f 7469 6679 5f63     node.notify_c
-00017560: 6f6c 6c61 7073 6528 290d 0a              ollapse()..
+0000f2b0: 2020 2070 6173 730d 0a0d 0a20 2020 2040     pass....    @
+0000f2c0: 7472 6565 5f63 6f6e 6469 7469 6f6e 616c  tree_conditional
+0000f2d0: 286c 616d 6264 6120 6e6f 6465 3a20 6e6f  (lambda node: no
+0000f2e0: 6465 2e63 6f75 6e74 5f63 6869 6c64 7265  de.count_childre
+0000f2f0: 6e28 2920 3e20 3129 0d0a 2020 2020 4074  n() > 1)..    @t
+0000f300: 7265 655f 7375 626d 656e 7528 5f28 2250  ree_submenu(_("P
+0000f310: 6173 7365 7322 2929 0d0a 2020 2020 4074  asses"))..    @t
+0000f320: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
+0000f330: 2020 2020 2020 2020 5f28 2241 6464 2031          _("Add 1
+0000f340: 2070 6173 7322 292c 0d0a 2020 2020 2020   pass"),..      
+0000f350: 2020 6e6f 6465 5f74 7970 653d 2822 6f70    node_type=("op
+0000f360: 2069 6d61 6765 222c 2022 6f70 2065 6e67   image", "op eng
+0000f370: 7261 7665 222c 2022 6f70 2063 7574 222c  rave", "op cut",
+0000f380: 2022 6f70 2068 6174 6368 2229 2c0d 0a20   "op hatch"),.. 
+0000f390: 2020 2020 2020 2068 656c 703d 2222 2c0d         help="",.
+0000f3a0: 0a20 2020 2029 0d0a 2020 2020 6465 6620  .    )..    def 
+0000f3b0: 6164 645f 315f 7061 7373 286e 6f64 652c  add_1_pass(node,
+0000f3c0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+0000f3d0: 2020 2020 2061 6464 5f6e 5f70 6173 7365       add_n_passe
+0000f3e0: 7328 6e6f 6465 2c20 636f 7069 6573 3d31  s(node, copies=1
+0000f3f0: 2c20 2a2a 6b77 6172 6773 290d 0a0d 0a20  , **kwargs).... 
+0000f400: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
+0000f410: 6f6e 616c 286c 616d 6264 6120 6e6f 6465  onal(lambda node
+0000f420: 3a20 6e6f 6465 2e63 6f75 6e74 5f63 6869  : node.count_chi
+0000f430: 6c64 7265 6e28 2920 3e20 3129 0d0a 2020  ldren() > 1)..  
+0000f440: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+0000f450: 5f28 2250 6173 7365 7322 2929 0d0a 2020  _("Passes"))..  
+0000f460: 2020 4074 7265 655f 6974 6572 6174 6528    @tree_iterate(
+0000f470: 2263 6f70 6965 7322 2c20 322c 2031 3029  "copies", 2, 10)
+0000f480: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+0000f490: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
+0000f4a0: 5f28 2241 6464 207b 636f 7069 6573 7d20  _("Add {copies} 
+0000f4b0: 7061 7373 6573 2229 2c0d 0a20 2020 2020  passes"),..     
+0000f4c0: 2020 206e 6f64 655f 7479 7065 3d28 226f     node_type=("o
+0000f4d0: 7020 696d 6167 6522 2c20 226f 7020 656e  p image", "op en
+0000f4e0: 6772 6176 6522 2c20 226f 7020 6375 7422  grave", "op cut"
+0000f4f0: 2c20 226f 7020 6861 7463 6822 292c 0d0a  , "op hatch"),..
+0000f500: 2020 2020 2020 2020 6865 6c70 3d22 222c          help="",
+0000f510: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
+0000f520: 2061 6464 5f6e 5f70 6173 7365 7328 6e6f   add_n_passes(no
+0000f530: 6465 2c20 636f 7069 6573 3d31 2c20 2a2a  de, copies=1, **
+0000f540: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+0000f550: 2020 6164 645f 6e6f 6465 7320 3d20 6c69    add_nodes = li
+0000f560: 7374 286e 6f64 652e 6368 696c 6472 656e  st(node.children
+0000f570: 290d 0a0d 0a20 2020 2020 2020 2072 656d  )....        rem
+0000f580: 6f76 6564 203d 2046 616c 7365 0d0a 2020  oved = False..  
+0000f590: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000f5a0: 616e 6765 2830 2c20 6c65 6e28 6164 645f  ange(0, len(add_
+0000f5b0: 6e6f 6465 7329 293a 0d0a 2020 2020 2020  nodes)):..      
+0000f5c0: 2020 2020 2020 666f 7220 7120 696e 2072        for q in r
+0000f5d0: 616e 6765 2830 2c20 6929 3a0d 0a20 2020  ange(0, i):..   
+0000f5e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000f5f0: 6164 645f 6e6f 6465 735b 715d 2069 7320  add_nodes[q] is 
+0000f600: 6164 645f 6e6f 6465 735b 695d 3a0d 0a20  add_nodes[i]:.. 
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f620: 2020 2061 6464 5f6e 6f64 6573 5b69 5d20     add_nodes[i] 
+0000f630: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
+0000f640: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
+0000f650: 7665 6420 3d20 5472 7565 0d0a 2020 2020  ved = True..    
+0000f660: 2020 2020 6966 2072 656d 6f76 6564 3a0d      if removed:.
+0000f670: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
+0000f680: 5f6e 6f64 6573 203d 205b 6320 666f 7220  _nodes = [c for 
+0000f690: 6320 696e 2061 6464 5f6e 6f64 6573 2069  c in add_nodes i
+0000f6a0: 6620 6320 6973 206e 6f74 204e 6f6e 655d  f c is not None]
+0000f6b0: 0d0a 2020 2020 2020 2020 6164 645f 6e6f  ..        add_no
+0000f6c0: 6465 7320 2a3d 2063 6f70 6965 730d 0a20  des *= copies.. 
+0000f6d0: 2020 2020 2020 2066 6f72 206e 2069 6e20         for n in 
+0000f6e0: 6164 645f 6e6f 6465 733a 0d0a 2020 2020  add_nodes:..    
+0000f6f0: 2020 2020 2020 2020 6e6f 6465 2e61 6464          node.add
+0000f700: 5f72 6566 6572 656e 6365 286e 2e6e 6f64  _reference(n.nod
+0000f710: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
+0000f720: 2e73 6967 6e61 6c28 2272 6562 7569 6c64  .signal("rebuild
+0000f730: 5f74 7265 6522 290d 0a0d 0a20 2020 2040  _tree")....    @
+0000f740: 7472 6565 5f63 6f6e 6469 7469 6f6e 616c  tree_conditional
+0000f750: 286c 616d 6264 6120 6e6f 6465 3a20 6e6f  (lambda node: no
+0000f760: 6465 2e63 6f75 6e74 5f63 6869 6c64 7265  de.count_childre
+0000f770: 6e28 2920 3e20 3129 0d0a 2020 2020 4074  n() > 1)..    @t
+0000f780: 7265 655f 7375 626d 656e 7528 5f28 2244  ree_submenu(_("D
+0000f790: 7570 6c69 6361 7465 2065 6c65 6d65 6e74  uplicate element
+0000f7a0: 2873 2922 2929 0d0a 2020 2020 4074 7265  (s)"))..    @tre
+0000f7b0: 655f 6f70 6572 6174 696f 6e28 0d0a 2020  e_operation(..  
+0000f7c0: 2020 2020 2020 5f28 2244 7570 6c69 6361        _("Duplica
+0000f7d0: 7465 2065 6c65 6d65 6e74 7320 3120 7469  te elements 1 ti
+0000f7e0: 6d65 2229 2c0d 0a20 2020 2020 2020 206e  me"),..        n
+0000f7f0: 6f64 655f 7479 7065 3d28 226f 7020 696d  ode_type=("op im
+0000f800: 6167 6522 2c20 226f 7020 656e 6772 6176  age", "op engrav
+0000f810: 6522 2c20 226f 7020 6375 7422 292c 0d0a  e", "op cut"),..
+0000f820: 2020 2020 2020 2020 6865 6c70 3d22 222c          help="",
+0000f830: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
+0000f840: 2064 7570 5f31 5f63 6f70 7928 6e6f 6465   dup_1_copy(node
+0000f850: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+0000f860: 2020 2020 2020 6475 705f 6e5f 636f 7069        dup_n_copi
+0000f870: 6573 286e 6f64 652c 2063 6f70 6965 733d  es(node, copies=
+0000f880: 312c 202a 2a6b 7761 7267 7329 0d0a 0d0a  1, **kwargs)....
+0000f890: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
+0000f8a0: 696f 6e61 6c28 6c61 6d62 6461 206e 6f64  ional(lambda nod
+0000f8b0: 653a 206e 6f64 652e 636f 756e 745f 6368  e: node.count_ch
+0000f8c0: 696c 6472 656e 2829 203e 2031 290d 0a20  ildren() > 1).. 
+0000f8d0: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
+0000f8e0: 285f 2822 4475 706c 6963 6174 6520 656c  (_("Duplicate el
+0000f8f0: 656d 656e 7428 7329 2229 290d 0a20 2020  ement(s)"))..   
+0000f900: 2040 7472 6565 5f69 7465 7261 7465 2822   @tree_iterate("
+0000f910: 636f 7069 6573 222c 2032 2c20 3130 290d  copies", 2, 10).
+0000f920: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
+0000f930: 7469 6f6e 280d 0a20 2020 2020 2020 205f  tion(..        _
+0000f940: 2822 4475 706c 6963 6174 6520 656c 656d  ("Duplicate elem
+0000f950: 656e 7473 207b 636f 7069 6573 7d20 7469  ents {copies} ti
+0000f960: 6d65 7322 292c 0d0a 2020 2020 2020 2020  mes"),..        
+0000f970: 6e6f 6465 5f74 7970 653d 2822 6f70 2069  node_type=("op i
+0000f980: 6d61 6765 222c 2022 6f70 2065 6e67 7261  mage", "op engra
+0000f990: 7665 222c 2022 6f70 2063 7574 2229 2c0d  ve", "op cut"),.
+0000f9a0: 0a20 2020 2020 2020 2068 656c 703d 2222  .        help=""
+0000f9b0: 2c0d 0a20 2020 2029 0d0a 2020 2020 6465  ,..    )..    de
+0000f9c0: 6620 6475 705f 6e5f 636f 7069 6573 286e  f dup_n_copies(n
+0000f9d0: 6f64 652c 2063 6f70 6965 733d 312c 202a  ode, copies=1, *
+0000f9e0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+0000f9f0: 2020 2023 2043 6f64 6520 696e 2073 6572     # Code in ser
+0000fa00: 6965 732e 0d0a 2020 2020 2020 2020 2320  ies...        # 
+0000fa10: 6164 645f 6e6f 6465 7320 3d20 6c69 7374  add_nodes = list
+0000fa20: 286e 6f64 652e 6368 696c 6472 656e 290d  (node.children).
+0000fa30: 0a20 2020 2020 2020 2023 2061 6464 5f6e  .        # add_n
+0000fa40: 6f64 6573 202a 3d20 636f 7069 6573 0d0a  odes *= copies..
+0000fa50: 2020 2020 2020 2020 2320 666f 7220 6e20          # for n 
+0000fa60: 696e 2061 6464 5f6e 6f64 6573 3a0d 0a20  in add_nodes:.. 
+0000fa70: 2020 2020 2020 2023 2020 2020 206e 6f64         #     nod
+0000fa80: 652e 6164 645f 7265 6665 7265 6e63 6528  e.add_reference(
+0000fa90: 6e2e 6e6f 6465 290d 0a0d 0a20 2020 2020  n.node)....     
+0000faa0: 2020 2023 2043 6f64 6520 696e 2070 6172     # Code in par
+0000fab0: 616c 6c65 6c2e 0d0a 2020 2020 2020 2020  allel...        
+0000fac0: 6164 645f 6e6f 6465 7320 3d20 6c69 7374  add_nodes = list
+0000fad0: 286e 6f64 652e 6368 696c 6472 656e 290d  (node.children).
+0000fae0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+0000faf0: 6e20 7261 6e67 6528 6c65 6e28 6164 645f  n range(len(add_
+0000fb00: 6e6f 6465 7329 202d 2031 2c20 2d31 2c20  nodes) - 1, -1, 
+0000fb10: 2d31 293a 0d0a 2020 2020 2020 2020 2020  -1):..          
+0000fb20: 2020 6e20 3d20 6164 645f 6e6f 6465 735b    n = add_nodes[
+0000fb30: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+0000fb40: 666f 7220 6b20 696e 2072 616e 6765 2863  for k in range(c
+0000fb50: 6f70 6965 7329 3a0d 0a20 2020 2020 2020  opies):..       
+0000fb60: 2020 2020 2020 2020 206e 6f64 652e 6164           node.ad
+0000fb70: 645f 7265 6665 7265 6e63 6528 6e2e 6e6f  d_reference(n.no
+0000fb80: 6465 2c20 706f 733d 6929 0d0a 0d0a 2020  de, pos=i)....  
+0000fb90: 2020 2020 2020 7365 6c66 2e73 6967 6e61        self.signa
+0000fba0: 6c28 2272 6566 7265 7368 5f74 7265 6522  l("refresh_tree"
+0000fbb0: 290d 0a0d 0a20 2020 2040 7472 6565 5f6f  )....    @tree_o
+0000fbc0: 7065 7261 7469 6f6e 280d 0a20 2020 2020  peration(..     
+0000fbd0: 2020 205f 2822 4d61 6b65 2072 6173 7465     _("Make raste
+0000fbe0: 7220 696d 6167 6522 292c 0d0a 2020 2020  r image"),..    
+0000fbf0: 2020 2020 6e6f 6465 5f74 7970 653d 2822      node_type=("
+0000fc00: 6f70 2069 6d61 6765 222c 2022 6f70 2072  op image", "op r
+0000fc10: 6173 7465 7222 292c 0d0a 2020 2020 2020  aster"),..      
+0000fc20: 2020 6865 6c70 3d5f 2822 4372 6561 7465    help=_("Create
+0000fc30: 2061 6e20 696d 6167 6520 6672 6f6d 2074   an image from t
+0000fc40: 6865 2061 7373 6967 6e65 6420 656c 656d  he assigned elem
+0000fc50: 656e 7473 2e22 292c 0d0a 2020 2020 290d  ents."),..    ).
+0000fc60: 0a20 2020 2064 6566 206d 616b 655f 7261  .    def make_ra
+0000fc70: 7374 6572 5f69 6d61 6765 286e 6f64 652c  ster_image(node,
+0000fc80: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+0000fc90: 2020 2020 2064 6174 6120 3d20 6c69 7374       data = list
+0000fca0: 286e 6f64 652e 666c 6174 2874 7970 6573  (node.flat(types
+0000fcb0: 3d65 6c65 6d5f 7265 665f 6e6f 6465 7329  =elem_ref_nodes)
+0000fcc0: 290d 0a20 2020 2020 2020 2069 6620 6c65  )..        if le
+0000fcd0: 6e28 6461 7461 2920 3d3d 2030 3a0d 0a20  n(data) == 0:.. 
+0000fce0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000fcf0: 6e0d 0a20 2020 2020 2020 2074 7279 3a0d  n..        try:.
+0000fd00: 0a20 2020 2020 2020 2020 2020 2062 6f75  .            bou
+0000fd10: 6e64 7320 3d20 4e6f 6465 2e75 6e69 6f6e  nds = Node.union
+0000fd20: 5f62 6f75 6e64 7328 6461 7461 2c20 6174  _bounds(data, at
+0000fd30: 7472 3d22 7061 696e 745f 626f 756e 6473  tr="paint_bounds
+0000fd40: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000fd50: 7769 6474 6820 3d20 626f 756e 6473 5b32  width = bounds[2
+0000fd60: 5d20 2d20 626f 756e 6473 5b30 5d0d 0a20  ] - bounds[0].. 
+0000fd70: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+0000fd80: 7420 3d20 626f 756e 6473 5b33 5d20 2d20  t = bounds[3] - 
+0000fd90: 626f 756e 6473 5b31 5d0d 0a20 2020 2020  bounds[1]..     
+0000fda0: 2020 2065 7863 6570 7420 5479 7065 4572     except TypeEr
+0000fdb0: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+0000fdc0: 2020 7261 6973 6520 436f 6d6d 616e 6453    raise CommandS
+0000fdd0: 796e 7461 7845 7272 6f72 0d0a 2020 2020  yntaxError..    
+0000fde0: 2020 2020 6d61 6b65 5f72 6173 7465 7220      make_raster 
+0000fdf0: 3d20 7365 6c66 2e6c 6f6f 6b75 7028 2272  = self.lookup("r
+0000fe00: 656e 6465 722d 6f70 2f6d 616b 655f 7261  ender-op/make_ra
+0000fe10: 7374 6572 2229 0d0a 2020 2020 2020 2020  ster")..        
+0000fe20: 6966 206e 6f74 206d 616b 655f 7261 7374  if not make_rast
+0000fe30: 6572 3a0d 0a20 2020 2020 2020 2020 2020  er:..           
+0000fe40: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+0000fe50: 7228 224e 6f20 7265 6e64 6572 6572 2069  r("No renderer i
+0000fe60: 7320 7265 6769 7374 6572 6564 2074 6f20  s registered to 
+0000fe70: 7065 7266 6f72 6d20 7265 6e64 6572 2e22  perform render."
+0000fe80: 290d 0a0d 0a20 2020 2020 2020 2064 6f74  )....        dot
+0000fe90: 735f 7065 725f 756e 6974 7320 3d20 6e6f  s_per_units = no
+0000fea0: 6465 2e64 7069 202f 2055 4e49 5453 5f50  de.dpi / UNITS_P
+0000feb0: 4552 5f49 4e43 480d 0a20 2020 2020 2020  ER_INCH..       
+0000fec0: 206e 6577 5f77 6964 7468 203d 2077 6964   new_width = wid
+0000fed0: 7468 202a 2064 6f74 735f 7065 725f 756e  th * dots_per_un
+0000fee0: 6974 730d 0a20 2020 2020 2020 206e 6577  its..        new
+0000fef0: 5f68 6569 6768 7420 3d20 6865 6967 6874  _height = height
+0000ff00: 202a 2064 6f74 735f 7065 725f 756e 6974   * dots_per_unit
+0000ff10: 730d 0a0d 0a20 2020 2020 2020 2069 6d61  s....        ima
+0000ff20: 6765 203d 206d 616b 655f 7261 7374 6572  ge = make_raster
+0000ff30: 280d 0a20 2020 2020 2020 2020 2020 2064  (..            d
+0000ff40: 6174 612c 0d0a 2020 2020 2020 2020 2020  ata,..          
+0000ff50: 2020 626f 756e 6473 3d62 6f75 6e64 732c    bounds=bounds,
+0000ff60: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+0000ff70: 6474 683d 6e65 775f 7769 6474 682c 0d0a  dth=new_width,..
+0000ff80: 2020 2020 2020 2020 2020 2020 6865 6967              heig
+0000ff90: 6874 3d6e 6577 5f68 6569 6768 742c 0d0a  ht=new_height,..
+0000ffa0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+0000ffb0: 2020 206d 6174 7269 7820 3d20 4d61 7472     matrix = Matr
+0000ffc0: 6978 2e73 6361 6c65 2877 6964 7468 202f  ix.scale(width /
+0000ffd0: 206e 6577 5f77 6964 7468 2c20 6865 6967   new_width, heig
+0000ffe0: 6874 202f 206e 6577 5f68 6569 6768 7429  ht / new_height)
+0000fff0: 0d0a 2020 2020 2020 2020 6d61 7472 6978  ..        matrix
+00010000: 2e70 6f73 745f 7472 616e 736c 6174 6528  .post_translate(
+00010010: 626f 756e 6473 5b30 5d2c 2062 6f75 6e64  bounds[0], bound
+00010020: 735b 315d 290d 0a0d 0a20 2020 2020 2020  s[1])....       
+00010030: 2069 6d61 6765 5f6e 6f64 6520 3d20 496d   image_node = Im
+00010040: 6167 654e 6f64 6528 696d 6167 653d 696d  ageNode(image=im
+00010050: 6167 652c 206d 6174 7269 783d 6d61 7472  age, matrix=matr
+00010060: 6978 2c20 6470 693d 6e6f 6465 2e64 7069  ix, dpi=node.dpi
+00010070: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00010080: 656c 656d 5f62 7261 6e63 682e 6164 645f  elem_branch.add_
+00010090: 6e6f 6465 2869 6d61 6765 5f6e 6f64 6529  node(image_node)
+000100a0: 0d0a 2020 2020 2020 2020 6e6f 6465 2e61  ..        node.a
+000100b0: 6464 5f72 6566 6572 656e 6365 2869 6d61  dd_reference(ima
+000100c0: 6765 5f6e 6f64 6529 0d0a 2020 2020 2020  ge_node)..      
+000100d0: 2020 7365 6c66 2e73 6967 6e61 6c28 2272    self.signal("r
+000100e0: 6566 7265 7368 5f73 6365 6e65 222c 2022  efresh_scene", "
+000100f0: 5363 656e 6522 290d 0a0d 0a20 2020 2064  Scene")....    d
+00010100: 6566 2061 6464 5f61 6674 6572 5f69 6e64  ef add_after_ind
+00010110: 6578 286e 6f64 653d 4e6f 6e65 293a 0d0a  ex(node=None):..
+00010120: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00010130: 2020 2020 2020 2020 2020 6966 206e 6f64            if nod
+00010140: 6520 6973 204e 6f6e 653a 0d0a 2020 2020  e is None:..    
+00010150: 2020 2020 2020 2020 2020 2020 6e6f 6465              node
+00010160: 203d 206c 6973 7428 7365 6c66 2e6f 7073   = list(self.ops
+00010170: 2873 656c 6563 7465 643d 5472 7565 2929  (selected=True))
+00010180: 5b2d 315d 0d0a 2020 2020 2020 2020 2020  [-1]..          
+00010190: 2020 6f70 6572 6174 696f 6e73 203d 2073    operations = s
+000101a0: 656c 662e 5f74 7265 652e 6765 7428 7479  elf._tree.get(ty
+000101b0: 7065 3d22 6272 616e 6368 206f 7073 2229  pe="branch ops")
+000101c0: 2e63 6869 6c64 7265 6e0d 0a20 2020 2020  .children..     
+000101d0: 2020 2020 2020 2072 6574 7572 6e20 6f70         return op
+000101e0: 6572 6174 696f 6e73 2e69 6e64 6578 286e  erations.index(n
+000101f0: 6f64 6529 202b 2031 0d0a 2020 2020 2020  ode) + 1..      
+00010200: 2020 6578 6365 7074 2028 5661 6c75 6545    except (ValueE
+00010210: 7272 6f72 2c20 496e 6465 7845 7272 6f72  rror, IndexError
+00010220: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00010230: 7265 7475 726e 204e 6f6e 650d 0a0d 0a20  return None.... 
+00010240: 2020 2040 7472 6565 5f73 6570 6172 6174     @tree_separat
+00010250: 6f72 5f62 6566 6f72 6528 290d 0a20 2020  or_before()..   
+00010260: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
+00010270: 2822 496e 7365 7274 206f 7065 7261 7469  ("Insert operati
+00010280: 6f6e 2229 290d 0a20 2020 2040 7472 6565  on"))..    @tree
+00010290: 5f6f 7065 7261 7469 6f6e 285f 2822 4164  _operation(_("Ad
+000102a0: 6420 496d 6167 6522 292c 206e 6f64 655f  d Image"), node_
+000102b0: 7479 7065 3d6f 705f 6e6f 6465 732c 2068  type=op_nodes, h
+000102c0: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
+000102d0: 2061 6464 5f6f 7065 7261 7469 6f6e 5f69   add_operation_i
+000102e0: 6d61 6765 286e 6f64 652c 202a 2a6b 7761  mage(node, **kwa
+000102f0: 7267 7329 3a0d 0a20 2020 2020 2020 2061  rgs):..        a
+00010300: 7070 656e 645f 6f70 6572 6174 696f 6e5f  ppend_operation_
+00010310: 696d 6167 6528 6e6f 6465 2c20 706f 733d  image(node, pos=
+00010320: 6164 645f 6166 7465 725f 696e 6465 7828  add_after_index(
+00010330: 6e6f 6465 292c 202a 2a6b 7761 7267 7329  node), **kwargs)
+00010340: 0d0a 0d0a 2020 2020 4074 7265 655f 7375  ....    @tree_su
+00010350: 626d 656e 7528 5f28 2249 6e73 6572 7420  bmenu(_("Insert 
+00010360: 6f70 6572 6174 696f 6e22 2929 0d0a 2020  operation"))..  
+00010370: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
+00010380: 6e28 5f28 2241 6464 2052 6173 7465 7222  n(_("Add Raster"
+00010390: 292c 206e 6f64 655f 7479 7065 3d6f 705f  ), node_type=op_
+000103a0: 6e6f 6465 732c 2068 656c 703d 2222 290d  nodes, help="").
+000103b0: 0a20 2020 2064 6566 2061 6464 5f6f 7065  .    def add_ope
+000103c0: 7261 7469 6f6e 5f72 6173 7465 7228 6e6f  ration_raster(no
+000103d0: 6465 2c20 2a2a 6b77 6172 6773 293a 0d0a  de, **kwargs):..
+000103e0: 2020 2020 2020 2020 6170 7065 6e64 5f6f          append_o
+000103f0: 7065 7261 7469 6f6e 5f72 6173 7465 7228  peration_raster(
+00010400: 6e6f 6465 2c20 706f 733d 6164 645f 6166  node, pos=add_af
+00010410: 7465 725f 696e 6465 7828 6e6f 6465 292c  ter_index(node),
+00010420: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
+00010430: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+00010440: 5f28 2249 6e73 6572 7420 6f70 6572 6174  _("Insert operat
+00010450: 696f 6e22 2929 0d0a 2020 2020 4074 7265  ion"))..    @tre
+00010460: 655f 6f70 6572 6174 696f 6e28 5f28 2241  e_operation(_("A
+00010470: 6464 2045 6e67 7261 7665 2229 2c20 6e6f  dd Engrave"), no
+00010480: 6465 5f74 7970 653d 6f70 5f6e 6f64 6573  de_type=op_nodes
+00010490: 2c20 6865 6c70 3d22 2229 0d0a 2020 2020  , help="")..    
+000104a0: 6465 6620 6164 645f 6f70 6572 6174 696f  def add_operatio
+000104b0: 6e5f 656e 6772 6176 6528 6e6f 6465 2c20  n_engrave(node, 
+000104c0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+000104d0: 2020 2020 6170 7065 6e64 5f6f 7065 7261      append_opera
+000104e0: 7469 6f6e 5f65 6e67 7261 7665 286e 6f64  tion_engrave(nod
+000104f0: 652c 2070 6f73 3d61 6464 5f61 6674 6572  e, pos=add_after
+00010500: 5f69 6e64 6578 286e 6f64 6529 2c20 2a2a  _index(node), **
+00010510: 6b77 6172 6773 290d 0a0d 0a20 2020 2040  kwargs)....    @
+00010520: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
+00010530: 496e 7365 7274 206f 7065 7261 7469 6f6e  Insert operation
+00010540: 2229 290d 0a20 2020 2040 7472 6565 5f6f  "))..    @tree_o
+00010550: 7065 7261 7469 6f6e 285f 2822 4164 6420  peration(_("Add 
+00010560: 4375 7422 292c 206e 6f64 655f 7479 7065  Cut"), node_type
+00010570: 3d6f 705f 6e6f 6465 732c 2068 656c 703d  =op_nodes, help=
+00010580: 2222 290d 0a20 2020 2064 6566 2061 6464  "")..    def add
+00010590: 5f6f 7065 7261 7469 6f6e 5f63 7574 286e  _operation_cut(n
+000105a0: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
+000105b0: 0a20 2020 2020 2020 2061 7070 656e 645f  .        append_
+000105c0: 6f70 6572 6174 696f 6e5f 6375 7428 6e6f  operation_cut(no
+000105d0: 6465 2c20 706f 733d 6164 645f 6166 7465  de, pos=add_afte
+000105e0: 725f 696e 6465 7828 6e6f 6465 292c 202a  r_index(node), *
+000105f0: 2a6b 7761 7267 7329 0d0a 0d0a 2020 2020  *kwargs)....    
+00010600: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
+00010610: 2249 6e73 6572 7420 6f70 6572 6174 696f  "Insert operatio
+00010620: 6e22 2929 0d0a 2020 2020 4074 7265 655f  n"))..    @tree_
+00010630: 6f70 6572 6174 696f 6e28 5f28 2241 6464  operation(_("Add
+00010640: 2048 6174 6368 2229 2c20 6e6f 6465 5f74   Hatch"), node_t
+00010650: 7970 653d 6f70 5f6e 6f64 6573 2c20 6865  ype=op_nodes, he
+00010660: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+00010670: 6164 645f 6f70 6572 6174 696f 6e5f 6861  add_operation_ha
+00010680: 7463 6828 6e6f 6465 2c20 2a2a 6b77 6172  tch(node, **kwar
+00010690: 6773 293a 0d0a 2020 2020 2020 2020 6170  gs):..        ap
+000106a0: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f68  pend_operation_h
+000106b0: 6174 6368 286e 6f64 652c 2070 6f73 3d61  atch(node, pos=a
+000106c0: 6464 5f61 6674 6572 5f69 6e64 6578 286e  dd_after_index(n
+000106d0: 6f64 6529 2c20 2a2a 6b77 6172 6773 290d  ode), **kwargs).
+000106e0: 0a0d 0a20 2020 2040 7472 6565 5f73 7562  ...    @tree_sub
+000106f0: 6d65 6e75 285f 2822 496e 7365 7274 206f  menu(_("Insert o
+00010700: 7065 7261 7469 6f6e 2229 290d 0a20 2020  peration"))..   
+00010710: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+00010720: 285f 2822 4164 6420 446f 7473 2229 2c20  (_("Add Dots"), 
+00010730: 6e6f 6465 5f74 7970 653d 6f70 5f6e 6f64  node_type=op_nod
+00010740: 6573 2c20 6865 6c70 3d22 2229 0d0a 2020  es, help="")..  
+00010750: 2020 6465 6620 6164 645f 6f70 6572 6174    def add_operat
+00010760: 696f 6e5f 646f 7473 286e 6f64 652c 202a  ion_dots(node, *
+00010770: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00010780: 2020 2061 7070 656e 645f 6f70 6572 6174     append_operat
+00010790: 696f 6e5f 646f 7473 286e 6f64 652c 2070  ion_dots(node, p
+000107a0: 6f73 3d61 6464 5f61 6674 6572 5f69 6e64  os=add_after_ind
+000107b0: 6578 286e 6f64 6529 2c20 2a2a 6b77 6172  ex(node), **kwar
+000107c0: 6773 290d 0a0d 0a20 2020 2040 7472 6565  gs)....    @tree
+000107d0: 5f73 7562 6d65 6e75 285f 2822 496e 7365  _submenu(_("Inse
+000107e0: 7274 2073 7065 6369 616c 206f 7065 7261  rt special opera
+000107f0: 7469 6f6e 2873 2922 2929 0d0a 2020 2020  tion(s)"))..    
+00010800: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+00010810: 5f28 2241 6464 2048 6f6d 6522 292c 206e  _("Add Home"), n
+00010820: 6f64 655f 7479 7065 3d6f 705f 6e6f 6465  ode_type=op_node
+00010830: 732c 2068 656c 703d 2222 290d 0a20 2020  s, help="")..   
+00010840: 2064 6566 2061 6464 5f6f 7065 7261 7469   def add_operati
+00010850: 6f6e 5f68 6f6d 6528 6e6f 6465 2c20 2a2a  on_home(node, **
+00010860: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+00010870: 2020 6170 7065 6e64 5f6f 7065 7261 7469    append_operati
+00010880: 6f6e 5f68 6f6d 6528 6e6f 6465 2c20 706f  on_home(node, po
+00010890: 733d 6164 645f 6166 7465 725f 696e 6465  s=add_after_inde
+000108a0: 7828 6e6f 6465 292c 202a 2a6b 7761 7267  x(node), **kwarg
+000108b0: 7329 0d0a 0d0a 2020 2020 4074 7265 655f  s)....    @tree_
+000108c0: 7375 626d 656e 7528 5f28 2249 6e73 6572  submenu(_("Inser
+000108d0: 7420 7370 6563 6961 6c20 6f70 6572 6174  t special operat
+000108e0: 696f 6e28 7329 2229 290d 0a20 2020 2040  ion(s)"))..    @
+000108f0: 7472 6565 5f6f 7065 7261 7469 6f6e 285f  tree_operation(_
+00010900: 2822 4164 6420 5265 7475 726e 2074 6f20  ("Add Return to 
+00010910: 4f72 6967 696e 2229 2c20 6e6f 6465 5f74  Origin"), node_t
+00010920: 7970 653d 6f70 5f6e 6f64 6573 2c20 6865  ype=op_nodes, he
+00010930: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+00010940: 6164 645f 6f70 6572 6174 696f 6e5f 6f72  add_operation_or
+00010950: 6967 696e 286e 6f64 652c 202a 2a6b 7761  igin(node, **kwa
+00010960: 7267 7329 3a0d 0a20 2020 2020 2020 2061  rgs):..        a
+00010970: 7070 656e 645f 6f70 6572 6174 696f 6e5f  ppend_operation_
+00010980: 676f 746f 286e 6f64 652c 2070 6f73 3d61  goto(node, pos=a
+00010990: 6464 5f61 6674 6572 5f69 6e64 6578 286e  dd_after_index(n
+000109a0: 6f64 6529 2c20 2a2a 6b77 6172 6773 290d  ode), **kwargs).
+000109b0: 0a0d 0a20 2020 2040 7472 6565 5f73 7562  ...    @tree_sub
+000109c0: 6d65 6e75 285f 2822 496e 7365 7274 2073  menu(_("Insert s
+000109d0: 7065 6369 616c 206f 7065 7261 7469 6f6e  pecial operation
+000109e0: 2873 2922 2929 0d0a 2020 2020 4074 7265  (s)"))..    @tre
+000109f0: 655f 6f70 6572 6174 696f 6e28 5f28 2241  e_operation(_("A
+00010a00: 6464 2042 6565 7022 292c 206e 6f64 655f  dd Beep"), node_
+00010a10: 7479 7065 3d6f 705f 6e6f 6465 732c 2068  type=op_nodes, h
+00010a20: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
+00010a30: 2061 6464 5f6f 7065 7261 7469 6f6e 5f62   add_operation_b
+00010a40: 6565 7028 6e6f 6465 2c20 2a2a 6b77 6172  eep(node, **kwar
+00010a50: 6773 293a 0d0a 2020 2020 2020 2020 6170  gs):..        ap
+00010a60: 7065 6e64 5f6f 7065 7261 7469 6f6e 5f62  pend_operation_b
+00010a70: 6565 7028 6e6f 6465 2c20 706f 733d 6164  eep(node, pos=ad
+00010a80: 645f 6166 7465 725f 696e 6465 7828 6e6f  d_after_index(no
+00010a90: 6465 292c 202a 2a6b 7761 7267 7329 0d0a  de), **kwargs)..
+00010aa0: 0d0a 2020 2020 4074 7265 655f 7375 626d  ..    @tree_subm
+00010ab0: 656e 7528 5f28 2249 6e73 6572 7420 7370  enu(_("Insert sp
+00010ac0: 6563 6961 6c20 6f70 6572 6174 696f 6e28  ecial operation(
+00010ad0: 7329 2229 290d 0a20 2020 2040 7472 6565  s)"))..    @tree
+00010ae0: 5f6f 7065 7261 7469 6f6e 285f 2822 4164  _operation(_("Ad
+00010af0: 6420 496e 7465 7272 7570 7422 292c 206e  d Interrupt"), n
+00010b00: 6f64 655f 7479 7065 3d6f 705f 6e6f 6465  ode_type=op_node
+00010b10: 732c 2068 656c 703d 2222 290d 0a20 2020  s, help="")..   
+00010b20: 2064 6566 2061 6464 5f6f 7065 7261 7469   def add_operati
+00010b30: 6f6e 5f69 6e74 6572 7275 7074 286e 6f64  on_interrupt(nod
+00010b40: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+00010b50: 2020 2020 2020 2061 7070 656e 645f 6f70         append_op
+00010b60: 6572 6174 696f 6e5f 696e 7465 7272 7570  eration_interrup
+00010b70: 7428 6e6f 6465 2c20 706f 733d 6164 645f  t(node, pos=add_
+00010b80: 6166 7465 725f 696e 6465 7828 6e6f 6465  after_index(node
+00010b90: 292c 202a 2a6b 7761 7267 7329 0d0a 0d0a  ), **kwargs)....
+00010ba0: 2020 2020 4074 7265 655f 7375 626d 656e      @tree_submen
+00010bb0: 7528 5f28 2249 6e73 6572 7420 7370 6563  u(_("Insert spec
+00010bc0: 6961 6c20 6f70 6572 6174 696f 6e28 7329  ial operation(s)
+00010bd0: 2229 290d 0a20 2020 2040 7472 6565 5f70  "))..    @tree_p
+00010be0: 726f 6d70 7428 2277 6169 745f 7469 6d65  rompt("wait_time
+00010bf0: 222c 205f 2822 5761 6974 2066 6f72 2068  ", _("Wait for h
+00010c00: 6f77 206c 6f6e 6720 2869 6e20 7365 636f  ow long (in seco
+00010c10: 6e64 7329 3f22 292c 2064 6174 615f 7479  nds)?"), data_ty
+00010c20: 7065 3d66 6c6f 6174 290d 0a20 2020 2040  pe=float)..    @
+00010c30: 7472 6565 5f6f 7065 7261 7469 6f6e 285f  tree_operation(_
+00010c40: 2822 4164 6420 5761 6974 2229 2c20 6e6f  ("Add Wait"), no
+00010c50: 6465 5f74 7970 653d 6f70 5f6e 6f64 6573  de_type=op_nodes
+00010c60: 2c20 6865 6c70 3d22 2229 0d0a 2020 2020  , help="")..    
+00010c70: 6465 6620 6164 645f 6f70 6572 6174 696f  def add_operatio
+00010c80: 6e5f 7761 6974 286e 6f64 652c 2077 6169  n_wait(node, wai
+00010c90: 745f 7469 6d65 2c20 2a2a 6b77 6172 6773  t_time, **kwargs
+00010ca0: 293a 0d0a 2020 2020 2020 2020 6170 7065  ):..        appe
+00010cb0: 6e64 5f6f 7065 7261 7469 6f6e 5f77 6169  nd_operation_wai
+00010cc0: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
+00010cd0: 6e6f 6465 2c20 7761 6974 5f74 696d 653d  node, wait_time=
+00010ce0: 7761 6974 5f74 696d 652c 2070 6f73 3d61  wait_time, pos=a
+00010cf0: 6464 5f61 6674 6572 5f69 6e64 6578 286e  dd_after_index(n
+00010d00: 6f64 6529 2c20 2a2a 6b77 6172 6773 0d0a  ode), **kwargs..
+00010d10: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+00010d20: 2040 7472 6565 5f73 7562 6d65 6e75 285f   @tree_submenu(_
+00010d30: 2822 496e 7365 7274 2073 7065 6369 616c  ("Insert special
+00010d40: 206f 7065 7261 7469 6f6e 2873 2922 2929   operation(s)"))
+00010d50: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+00010d60: 6174 696f 6e28 5f28 2241 6464 204f 7574  ation(_("Add Out
+00010d70: 7075 7422 292c 206e 6f64 655f 7479 7065  put"), node_type
+00010d80: 3d6f 705f 6e6f 6465 732c 2068 656c 703d  =op_nodes, help=
+00010d90: 2222 290d 0a20 2020 2064 6566 2061 6464  "")..    def add
+00010da0: 5f6f 7065 7261 7469 6f6e 5f6f 7574 7075  _operation_outpu
+00010db0: 7428 6e6f 6465 2c20 2a2a 6b77 6172 6773  t(node, **kwargs
+00010dc0: 293a 0d0a 2020 2020 2020 2020 6170 7065  ):..        appe
+00010dd0: 6e64 5f6f 7065 7261 7469 6f6e 5f6f 7574  nd_operation_out
+00010de0: 7075 7428 6e6f 6465 2c20 706f 733d 6164  put(node, pos=ad
+00010df0: 645f 6166 7465 725f 696e 6465 7828 6e6f  d_after_index(no
+00010e00: 6465 292c 202a 2a6b 7761 7267 7329 0d0a  de), **kwargs)..
+00010e10: 0d0a 2020 2020 4074 7265 655f 7375 626d  ..    @tree_subm
+00010e20: 656e 7528 5f28 2249 6e73 6572 7420 7370  enu(_("Insert sp
+00010e30: 6563 6961 6c20 6f70 6572 6174 696f 6e28  ecial operation(
+00010e40: 7329 2229 290d 0a20 2020 2040 7472 6565  s)"))..    @tree
+00010e50: 5f6f 7065 7261 7469 6f6e 285f 2822 4164  _operation(_("Ad
+00010e60: 6420 496e 7075 7422 292c 206e 6f64 655f  d Input"), node_
+00010e70: 7479 7065 3d6f 705f 6e6f 6465 732c 2068  type=op_nodes, h
+00010e80: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
+00010e90: 2061 6464 5f6f 7065 7261 7469 6f6e 5f69   add_operation_i
+00010ea0: 6e70 7574 286e 6f64 652c 202a 2a6b 7761  nput(node, **kwa
+00010eb0: 7267 7329 3a0d 0a20 2020 2020 2020 2061  rgs):..        a
+00010ec0: 7070 656e 645f 6f70 6572 6174 696f 6e5f  ppend_operation_
+00010ed0: 696e 7075 7428 6e6f 6465 2c20 706f 733d  input(node, pos=
+00010ee0: 6164 645f 6166 7465 725f 696e 6465 7828  add_after_index(
+00010ef0: 6e6f 6465 292c 202a 2a6b 7761 7267 7329  node), **kwargs)
+00010f00: 0d0a 0d0a 2020 2020 4074 7265 655f 7375  ....    @tree_su
+00010f10: 626d 656e 7528 5f28 2249 6e73 6572 7420  bmenu(_("Insert 
+00010f20: 7370 6563 6961 6c20 6f70 6572 6174 696f  special operatio
+00010f30: 6e28 7329 2229 290d 0a20 2020 2040 7472  n(s)"))..    @tr
+00010f40: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
+00010f50: 4164 6420 486f 6d65 2f42 6565 702f 496e  Add Home/Beep/In
+00010f60: 7465 7272 7570 7422 292c 206e 6f64 655f  terrupt"), node_
+00010f70: 7479 7065 3d6f 705f 6e6f 6465 732c 2068  type=op_nodes, h
+00010f80: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
+00010f90: 2061 6464 5f6f 7065 7261 7469 6f6e 5f68   add_operation_h
+00010fa0: 6f6d 655f 6265 6570 5f69 6e74 6572 7275  ome_beep_interru
+00010fb0: 7074 286e 6f64 652c 202a 2a6b 7761 7267  pt(node, **kwarg
+00010fc0: 7329 3a0d 0a20 2020 2020 2020 2070 6f73  s):..        pos
+00010fd0: 203d 2061 6464 5f61 6674 6572 5f69 6e64   = add_after_ind
+00010fe0: 6578 286e 6f64 6529 0d0a 2020 2020 2020  ex(node)..      
+00010ff0: 2020 6170 7065 6e64 5f6f 7065 7261 7469    append_operati
+00011000: 6f6e 5f68 6f6d 6528 6e6f 6465 2c20 706f  on_home(node, po
+00011010: 733d 706f 732c 202a 2a6b 7761 7267 7329  s=pos, **kwargs)
+00011020: 0d0a 2020 2020 2020 2020 6966 2070 6f73  ..        if pos
+00011030: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00011040: 6f73 202b 3d20 310d 0a20 2020 2020 2020  os += 1..       
+00011050: 2061 7070 656e 645f 6f70 6572 6174 696f   append_operatio
+00011060: 6e5f 6265 6570 286e 6f64 652c 2070 6f73  n_beep(node, pos
+00011070: 3d70 6f73 2c20 2a2a 6b77 6172 6773 290d  =pos, **kwargs).
+00011080: 0a20 2020 2020 2020 2069 6620 706f 733a  .        if pos:
+00011090: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+000110a0: 7320 2b3d 2031 0d0a 2020 2020 2020 2020  s += 1..        
+000110b0: 6170 7065 6e64 5f6f 7065 7261 7469 6f6e  append_operation
+000110c0: 5f69 6e74 6572 7275 7074 286e 6f64 652c  _interrupt(node,
+000110d0: 2070 6f73 3d70 6f73 2c20 2a2a 6b77 6172   pos=pos, **kwar
+000110e0: 6773 290d 0a0d 0a20 2020 2040 7472 6565  gs)....    @tree
+000110f0: 5f73 7562 6d65 6e75 285f 2822 496e 7365  _submenu(_("Inse
+00011100: 7274 2073 7065 6369 616c 206f 7065 7261  rt special opera
+00011110: 7469 6f6e 2873 2922 2929 0d0a 2020 2020  tion(s)"))..    
+00011120: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+00011130: 5f28 2241 6464 204f 7269 6769 6e2f 4265  _("Add Origin/Be
+00011140: 6570 2f49 6e74 6572 7275 7074 2229 2c20  ep/Interrupt"), 
+00011150: 6e6f 6465 5f74 7970 653d 6f70 5f6e 6f64  node_type=op_nod
+00011160: 6573 2c20 6865 6c70 3d22 2229 0d0a 2020  es, help="")..  
+00011170: 2020 6465 6620 6164 645f 6f70 6572 6174    def add_operat
+00011180: 696f 6e5f 6f72 6967 696e 5f62 6565 705f  ion_origin_beep_
+00011190: 696e 7465 7272 7570 7428 6e6f 6465 2c20  interrupt(node, 
+000111a0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+000111b0: 2020 2020 706f 7320 3d20 6164 645f 6166      pos = add_af
+000111c0: 7465 725f 696e 6465 7828 6e6f 6465 290d  ter_index(node).
+000111d0: 0a20 2020 2020 2020 2061 7070 656e 645f  .        append_
+000111e0: 6f70 6572 6174 696f 6e5f 676f 746f 286e  operation_goto(n
+000111f0: 6f64 652c 2070 6f73 3d70 6f73 2c20 2a2a  ode, pos=pos, **
+00011200: 6b77 6172 6773 290d 0a20 2020 2020 2020  kwargs)..       
+00011210: 2069 6620 706f 733a 0d0a 2020 2020 2020   if pos:..      
+00011220: 2020 2020 2020 706f 7320 2b3d 2031 0d0a        pos += 1..
+00011230: 2020 2020 2020 2020 6170 7065 6e64 5f6f          append_o
+00011240: 7065 7261 7469 6f6e 5f62 6565 7028 6e6f  peration_beep(no
+00011250: 6465 2c20 706f 733d 706f 732c 202a 2a6b  de, pos=pos, **k
+00011260: 7761 7267 7329 0d0a 2020 2020 2020 2020  wargs)..        
+00011270: 6966 2070 6f73 3a0d 0a20 2020 2020 2020  if pos:..       
+00011280: 2020 2020 2070 6f73 202b 3d20 310d 0a20       pos += 1.. 
+00011290: 2020 2020 2020 2061 7070 656e 645f 6f70         append_op
+000112a0: 6572 6174 696f 6e5f 696e 7465 7272 7570  eration_interrup
+000112b0: 7428 6e6f 6465 2c20 706f 733d 706f 732c  t(node, pos=pos,
+000112c0: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
+000112d0: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
+000112e0: 6e28 5f28 2252 656c 6f61 6420 277b 6e61  n(_("Reload '{na
+000112f0: 6d65 7d27 2229 2c20 6e6f 6465 5f74 7970  me}'"), node_typ
+00011300: 653d 2266 696c 6522 2c20 6865 6c70 3d22  e="file", help="
+00011310: 2229 0d0a 2020 2020 6465 6620 7265 6c6f  ")..    def relo
+00011320: 6164 5f66 696c 6528 6e6f 6465 2c20 2a2a  ad_file(node, **
+00011330: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+00011340: 2020 6669 6c65 7061 7468 203d 206e 6f64    filepath = nod
+00011350: 652e 6669 6c65 7061 7468 0d0a 2020 2020  e.filepath..    
+00011360: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
+00011370: 7468 2e65 7869 7374 7328 6669 6c65 7061  th.exists(filepa
+00011380: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+00011390: 2020 7365 6c66 2e73 6967 6e61 6c28 0d0a    self.signal(..
+000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113b0: 2277 6172 6e69 6e67 222c 0d0a 2020 2020  "warning",..    
+000113c0: 2020 2020 2020 2020 2020 2020 5f28 2254              _("T
+000113d0: 6865 2066 696c 6520 6e6f 206c 6f6e 6765  he file no longe
+000113e0: 7220 6578 6973 7473 2122 292c 0d0a 2020  r exists!"),..  
+000113f0: 2020 2020 2020 2020 2020 2020 2020 5f28                _(
+00011400: 2246 696c 6520 646f 6573 206e 6f74 2065  "File does not e
+00011410: 7869 7374 2e22 292c 0d0a 2020 2020 2020  xist."),..      
+00011420: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00011430: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00011440: 2020 2020 206e 6f64 652e 7265 6d6f 7665       node.remove
+00011450: 5f6e 6f64 6528 290d 0a20 2020 2020 2020  _node()..       
+00011460: 2073 656c 662e 6c6f 6164 2866 696c 6570   self.load(filep
+00011470: 6174 6829 0d0a 0d0a 2020 2020 4074 7265  ath)....    @tre
+00011480: 655f 6f70 6572 6174 696f 6e28 0d0a 2020  e_operation(..  
+00011490: 2020 2020 2020 5f28 224f 7065 6e20 696e        _("Open in
+000114a0: 2053 7973 7465 6d3a 2027 7b6e 616d 657d   System: '{name}
+000114b0: 2722 292c 0d0a 2020 2020 2020 2020 6e6f  '"),..        no
+000114c0: 6465 5f74 7970 653d 2266 696c 6522 2c0d  de_type="file",.
+000114d0: 0a20 2020 2020 2020 2068 656c 703d 5f28  .        help=_(
+000114e0: 0d0a 2020 2020 2020 2020 2020 2020 224f  ..            "O
+000114f0: 7065 6e20 7468 6973 2066 696c 6520 696e  pen this file in
+00011500: 2074 6865 2073 7973 7465 6d20 6170 706c   the system appl
+00011510: 6963 6174 696f 6e20 6173 736f 6369 6174  ication associat
+00011520: 6564 2077 6974 6820 7468 6973 2074 7970  ed with this typ
+00011530: 6520 6f66 2066 696c 6522 0d0a 2020 2020  e of file"..    
+00011540: 2020 2020 292c 0d0a 2020 2020 290d 0a20      ),..    ).. 
+00011550: 2020 2064 6566 206f 7065 6e5f 7379 7374     def open_syst
+00011560: 656d 5f66 696c 6528 6e6f 6465 2c20 2a2a  em_file(node, **
+00011570: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+00011580: 2020 6669 6c65 7061 7468 203d 206e 6f64    filepath = nod
+00011590: 652e 6669 6c65 7061 7468 0d0a 2020 2020  e.filepath..    
+000115a0: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
+000115b0: 7468 2e65 7869 7374 7328 6669 6c65 7061  th.exists(filepa
+000115c0: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+000115d0: 2020 7365 6c66 2e73 6967 6e61 6c28 0d0a    self.signal(..
+000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000115f0: 2277 6172 6e69 6e67 222c 0d0a 2020 2020  "warning",..    
+00011600: 2020 2020 2020 2020 2020 2020 5f28 2254              _("T
+00011610: 6865 2066 696c 6520 6e6f 206c 6f6e 6765  he file no longe
+00011620: 7220 6578 6973 7473 2122 292c 0d0a 2020  r exists!"),..  
+00011630: 2020 2020 2020 2020 2020 2020 2020 5f28                _(
+00011640: 2246 696c 6520 646f 6573 206e 6f74 2065  "File does not e
+00011650: 7869 7374 2e22 292c 0d0a 2020 2020 2020  xist."),..      
+00011660: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00011670: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
+00011680: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
+00011690: 6420 3d20 6f73 2e70 6174 682e 7265 616c  d = os.path.real
+000116a0: 7061 7468 2866 696c 6570 6174 6829 0d0a  path(filepath)..
+000116b0: 0d0a 2020 2020 2020 2020 696d 706f 7274  ..        import
+000116c0: 2070 6c61 7466 6f72 6d0d 0a0d 0a20 2020   platform....   
+000116d0: 2020 2020 2073 7973 7465 6d20 3d20 706c       system = pl
+000116e0: 6174 666f 726d 2e73 7973 7465 6d28 290d  atform.system().
+000116f0: 0a20 2020 2020 2020 2069 6620 7379 7374  .        if syst
+00011700: 656d 203d 3d20 2244 6172 7769 6e22 3a0d  em == "Darwin":.
+00011710: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
+00011720: 6d20 6f73 2069 6d70 6f72 7420 7379 7374  m os import syst
+00011730: 656d 2061 7320 6f70 656e 5f69 6e5f 7368  em as open_in_sh
+00011740: 656c 6c0d 0a0d 0a20 2020 2020 2020 2020  ell....         
+00011750: 2020 206f 7065 6e5f 696e 5f73 6865 6c6c     open_in_shell
+00011760: 2866 226f 7065 6e20 277b 6e6f 726d 616c  (f"open '{normal
+00011770: 697a 6564 7d27 2229 0d0a 2020 2020 2020  ized}'")..      
+00011780: 2020 656c 6966 2073 7973 7465 6d20 3d3d    elif system ==
+00011790: 2022 5769 6e64 6f77 7322 3a0d 0a20 2020   "Windows":..   
+000117a0: 2020 2020 2020 2020 2066 726f 6d20 6f73           from os
+000117b0: 2069 6d70 6f72 7420 7374 6172 7466 696c   import startfil
+000117c0: 6520 6173 206f 7065 6e5f 696e 5f73 6865  e as open_in_she
+000117d0: 6c6c 0d0a 0d0a 2020 2020 2020 2020 2020  ll....          
+000117e0: 2020 6f70 656e 5f69 6e5f 7368 656c 6c28    open_in_shell(
+000117f0: 6627 227b 6e6f 726d 616c 697a 6564 7d22  f'"{normalized}"
+00011800: 2729 0d0a 2020 2020 2020 2020 656c 7365  ')..        else
+00011810: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+00011820: 726f 6d20 6f73 2069 6d70 6f72 7420 7379  rom os import sy
+00011830: 7374 656d 2061 7320 6f70 656e 5f69 6e5f  stem as open_in_
+00011840: 7368 656c 6c0d 0a0d 0a20 2020 2020 2020  shell....       
+00011850: 2020 2020 206f 7065 6e5f 696e 5f73 6865       open_in_she
+00011860: 6c6c 2866 2278 6467 2d6f 7065 6e20 277b  ll(f"xdg-open '{
+00011870: 6e6f 726d 616c 697a 6564 7d27 2229 0d0a  normalized}'")..
+00011880: 0d0a 2020 2020 6465 6620 6765 745f 7661  ..    def get_va
+00011890: 6c75 6573 2829 3a0d 0a20 2020 2020 2020  lues():..       
+000118a0: 2072 6574 7572 6e20 5b6f 2066 6f72 206f   return [o for o
+000118b0: 2069 6e20 7365 6c66 2e6f 7073 2829 2069   in self.ops() i
+000118c0: 6620 6f2e 7479 7065 2e73 7461 7274 7377  f o.type.startsw
+000118d0: 6974 6828 226f 7022 295d 0d0a 0d0a 2020  ith("op")]....  
+000118e0: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
+000118f0: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
+00011900: 206e 6f74 2069 735f 7265 676d 6172 6b28   not is_regmark(
+00011910: 6e6f 6465 2929 0d0a 2020 2020 4074 7265  node))..    @tre
+00011920: 655f 7375 626d 656e 7528 5f28 2241 7373  e_submenu(_("Ass
+00011930: 6967 6e20 4f70 6572 6174 696f 6e22 2929  ign Operation"))
+00011940: 0d0a 2020 2020 4074 7265 655f 7661 6c75  ..    @tree_valu
+00011950: 6573 2822 6f70 5f61 7373 6967 6e22 2c20  es("op_assign", 
+00011960: 7661 6c75 6573 3d67 6574 5f76 616c 7565  values=get_value
+00011970: 7329 0d0a 2020 2020 4074 7265 655f 6f70  s)..    @tree_op
+00011980: 6572 6174 696f 6e28 227b 6f70 5f61 7373  eration("{op_ass
+00011990: 6967 6e7d 222c 206e 6f64 655f 7479 7065  ign}", node_type
+000119a0: 3d65 6c65 6d5f 6e6f 6465 732c 2068 656c  =elem_nodes, hel
+000119b0: 703d 2222 290d 0a20 2020 2064 6566 206d  p="")..    def m
+000119c0: 656e 755f 6173 7369 676e 5f6f 7065 7261  enu_assign_opera
+000119d0: 7469 6f6e 7328 6e6f 6465 2c20 6f70 5f61  tions(node, op_a
+000119e0: 7373 6967 6e2c 202a 2a6b 7761 7267 7329  ssign, **kwargs)
+000119f0: 3a0d 0a20 2020 2020 2020 2069 6620 7365  :..        if se
+00011a00: 6c66 2e63 6c61 7373 6966 795f 696e 6865  lf.classify_inhe
+00011a10: 7269 745f 7374 726f 6b65 3a0d 0a20 2020  rit_stroke:..   
+00011a20: 2020 2020 2020 2020 2069 6d70 6f73 6520           impose 
+00011a30: 3d20 2274 6f5f 6f70 220d 0a20 2020 2020  = "to_op"..     
+00011a40: 2020 2020 2020 2061 7474 7269 6220 3d20         attrib = 
+00011a50: 2273 7472 6f6b 6522 0d0a 2020 2020 2020  "stroke"..      
+00011a60: 2020 2020 2020 7369 6d69 6c61 7220 3d20        similar = 
+00011a70: 5472 7565 0d0a 2020 2020 2020 2020 656c  True..        el
+00011a80: 6966 2073 656c 662e 636c 6173 7369 6679  if self.classify
+00011a90: 5f69 6e68 6572 6974 5f66 696c 6c3a 0d0a  _inherit_fill:..
+00011aa0: 2020 2020 2020 2020 2020 2020 696d 706f              impo
+00011ab0: 7365 203d 2022 746f 5f6f 7022 0d0a 2020  se = "to_op"..  
+00011ac0: 2020 2020 2020 2020 2020 6174 7472 6962            attrib
+00011ad0: 203d 2022 6669 6c6c 220d 0a20 2020 2020   = "fill"..     
+00011ae0: 2020 2020 2020 2073 696d 696c 6172 203d         similar =
+00011af0: 2054 7275 650d 0a20 2020 2020 2020 2065   True..        e
+00011b00: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00011b10: 2020 696d 706f 7365 203d 204e 6f6e 650d    impose = None.
+00011b20: 0a20 2020 2020 2020 2020 2020 2061 7474  .            att
+00011b30: 7269 6220 3d20 4e6f 6e65 0d0a 2020 2020  rib = None..    
+00011b40: 2020 2020 2020 2020 7369 6d69 6c61 7220          similar 
+00011b50: 3d20 4661 6c73 650d 0a20 2020 2020 2020  = False..       
+00011b60: 2065 7863 6c75 7369 7665 203d 2073 656c   exclusive = sel
+00011b70: 662e 636c 6173 7369 6679 5f69 6e68 6572  f.classify_inher
+00011b80: 6974 5f65 7863 6c75 7369 7665 0d0a 2020  it_exclusive..  
+00011b90: 2020 2020 2020 6461 7461 203d 206c 6973        data = lis
+00011ba0: 7428 7365 6c66 2e65 6c65 6d73 2865 6d70  t(self.elems(emp
+00011bb0: 6861 7369 7a65 643d 5472 7565 2929 0d0a  hasized=True))..
+00011bc0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00011bd0: 6967 6e5f 6f70 6572 6174 696f 6e28 0d0a  ign_operation(..
+00011be0: 2020 2020 2020 2020 2020 2020 6f70 5f61              op_a
+00011bf0: 7373 6967 6e3d 6f70 5f61 7373 6967 6e2c  ssign=op_assign,
+00011c00: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00011c10: 7461 3d64 6174 612c 0d0a 2020 2020 2020  ta=data,..      
+00011c20: 2020 2020 2020 696d 706f 7365 3d69 6d70        impose=imp
+00011c30: 6f73 652c 0d0a 2020 2020 2020 2020 2020  ose,..          
+00011c40: 2020 6174 7472 6962 3d61 7474 7269 622c    attrib=attrib,
+00011c50: 0d0a 2020 2020 2020 2020 2020 2020 7369  ..            si
+00011c60: 6d69 6c61 723d 7369 6d69 6c61 722c 0d0a  milar=similar,..
+00011c70: 2020 2020 2020 2020 2020 2020 6578 636c              excl
+00011c80: 7573 6976 653d 6578 636c 7573 6976 652c  usive=exclusive,
+00011c90: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+00011ca0: 2020 2064 6566 2065 7863 6c75 7369 7665     def exclusive
+00011cb0: 5f6d 6174 6368 286e 6f64 652c 202a 2a6b  _match(node, **k
+00011cc0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00011cd0: 2072 6574 7572 6e20 7365 6c66 2e63 6c61   return self.cla
+00011ce0: 7373 6966 795f 696e 6865 7269 745f 6578  ssify_inherit_ex
+00011cf0: 636c 7573 6976 650d 0a0d 0a20 2020 2040  clusive....    @
+00011d00: 7472 6565 5f73 6570 6172 6174 6f72 5f62  tree_separator_b
+00011d10: 6566 6f72 6528 290d 0a20 2020 2040 7472  efore()..    @tr
+00011d20: 6565 5f73 7562 6d65 6e75 285f 2822 4173  ee_submenu(_("As
+00011d30: 7369 676e 204f 7065 7261 7469 6f6e 2229  sign Operation")
+00011d40: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+00011d50: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
+00011d60: 205f 2822 5265 6d6f 7665 2061 6c6c 2061   _("Remove all a
+00011d70: 7373 6967 6e6d 656e 7473 2066 726f 6d20  ssignments from 
+00011d80: 6f70 6572 6174 696f 6e73 2229 2c0d 0a20  operations"),.. 
+00011d90: 2020 2020 2020 206e 6f64 655f 7479 7065         node_type
+00011da0: 3d65 6c65 6d5f 6772 6f75 705f 6e6f 6465  =elem_group_node
+00011db0: 732c 0d0a 2020 2020 2020 2020 6865 6c70  s,..        help
+00011dc0: 3d5f 2822 416e 7920 6578 6973 7469 6e67  =_("Any existing
+00011dd0: 2061 7373 6967 6e6d 656e 7420 6f66 2074   assignment of t
+00011de0: 6869 7320 656c 656d 656e 7420 746f 206f  his element to o
+00011df0: 7065 7261 7469 6f6e 7320 7769 6c6c 2062  perations will b
+00011e00: 6520 7265 6d6f 7665 6422 292c 0d0a 2020  e removed"),..  
+00011e10: 2020 290d 0a20 2020 2064 6566 2072 656d    )..    def rem
+00011e20: 6f76 655f 6173 7369 676e 6d65 6e74 7328  ove_assignments(
+00011e30: 7369 6e67 6c65 6e6f 6465 2c20 2a2a 6b77  singlenode, **kw
+00011e40: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00011e50: 6465 6620 7265 6d5f 6e6f 6465 2872 6e6f  def rem_node(rno
+00011e60: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
+00011e70: 2020 2320 7265 6375 7273 6976 656c 7920    # recursively 
+00011e80: 7265 6d6f 7665 2061 7373 6967 6e6d 656e  remove assignmen
+00011e90: 7473 2e2e 2e0d 0a20 2020 2020 2020 2020  ts.....         
+00011ea0: 2020 2069 6620 726e 6f64 652e 7479 7065     if rnode.type
+00011eb0: 2069 6e20 2822 6669 6c65 222c 2022 6772   in ("file", "gr
+00011ec0: 6f75 7022 293a 0d0a 2020 2020 2020 2020  oup"):..        
+00011ed0: 2020 2020 2020 2020 666f 7220 636e 6f64          for cnod
+00011ee0: 6520 696e 206c 6973 7428 726e 6f64 652e  e in list(rnode.
+00011ef0: 5f63 6869 6c64 7265 6e29 3a0d 0a20 2020  _children):..   
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f10: 2072 656d 5f6e 6f64 6528 636e 6f64 6529   rem_node(cnode)
+00011f20: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00011f30: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00011f40: 2020 2020 2066 6f72 2072 6566 2069 6e20       for ref in 
+00011f50: 6c69 7374 2872 6e6f 6465 2e72 6566 6572  list(rnode.refer
+00011f60: 656e 6365 7329 3a0d 0a20 2020 2020 2020  ences):..       
+00011f70: 2020 2020 2020 2020 2020 2020 2072 6566               ref
+00011f80: 2e72 656d 6f76 655f 6e6f 6465 2829 0d0a  .remove_node()..
+00011f90: 0d0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
+00011fa0: 656c 662e 7374 6174 6963 2822 7265 6d6f  elf.static("remo
+00011fb0: 7665 5f61 7373 6967 6e22 293a 0d0a 2020  ve_assign"):..  
+00011fc0: 2020 2020 2020 2020 2020 666f 7220 6e6f            for no
+00011fd0: 6465 2069 6e20 6c69 7374 2873 656c 662e  de in list(self.
+00011fe0: 656c 656d 7328 656d 7068 6173 697a 6564  elems(emphasized
+00011ff0: 3d54 7275 6529 293a 0d0a 2020 2020 2020  =True)):..      
+00012000: 2020 2020 2020 2020 2020 7265 6d5f 6e6f            rem_no
+00012010: 6465 286e 6f64 6529 0d0a 2020 2020 2020  de(node)..      
+00012020: 2020 7365 6c66 2e73 6967 6e61 6c28 2272    self.signal("r
+00012030: 6566 7265 7368 5f74 7265 6522 290d 0a0d  efresh_tree")...
+00012040: 0a20 2020 2040 7472 6565 5f73 6570 6172  .    @tree_separ
+00012050: 6174 6f72 5f62 6566 6f72 6528 290d 0a20  ator_before().. 
+00012060: 2020 2040 7472 6565 5f73 7562 6d65 6e75     @tree_submenu
+00012070: 285f 2822 4173 7369 676e 204f 7065 7261  (_("Assign Opera
+00012080: 7469 6f6e 2229 290d 0a20 2020 2040 7472  tion"))..    @tr
+00012090: 6565 5f63 6865 636b 2865 7863 6c75 7369  ee_check(exclusi
+000120a0: 7665 5f6d 6174 6368 290d 0a20 2020 2040  ve_match)..    @
+000120b0: 7472 6565 5f6f 7065 7261 7469 6f6e 280d  tree_operation(.
+000120c0: 0a20 2020 2020 2020 205f 2822 4578 636c  .        _("Excl
+000120d0: 7573 6976 6520 6173 7369 676e 6d65 6e74  usive assignment
+000120e0: 2229 2c0d 0a20 2020 2020 2020 206e 6f64  "),..        nod
+000120f0: 655f 7479 7065 3d65 6c65 6d5f 6e6f 6465  e_type=elem_node
+00012100: 732c 0d0a 2020 2020 2020 2020 6865 6c70  s,..        help
+00012110: 3d5f 280d 0a20 2020 2020 2020 2020 2020  =_(..           
+00012120: 2022 416e 2061 7373 6967 6e6d 656e 7420   "An assignment 
+00012130: 7769 6c6c 2072 656d 6f76 6520 616c 6c20  will remove all 
+00012140: 6f74 6865 7220 636c 6173 7369 6669 6361  other classifica
+00012150: 7469 6f6e 7320 6f66 2074 6869 7320 656c  tions of this el
+00012160: 656d 656e 7420 6966 2063 6865 636b 6564  ement if checked
+00012170: 220d 0a20 2020 2020 2020 2029 2c0d 0a20  "..        ),.. 
+00012180: 2020 2029 0d0a 2020 2020 6465 6620 7365     )..    def se
+00012190: 745f 6173 7369 676e 5f6f 7074 696f 6e5f  t_assign_option_
+000121a0: 6578 636c 7573 6976 6528 6e6f 6465 2c20  exclusive(node, 
+000121b0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+000121c0: 2020 2020 7365 6c66 2e63 6c61 7373 6966      self.classif
+000121d0: 795f 696e 6865 7269 745f 6578 636c 7573  y_inherit_exclus
+000121e0: 6976 6520 3d20 6e6f 7420 7365 6c66 2e63  ive = not self.c
+000121f0: 6c61 7373 6966 795f 696e 6865 7269 745f  lassify_inherit_
+00012200: 6578 636c 7573 6976 650d 0a0d 0a20 2020  exclusive....   
+00012210: 2064 6566 2073 7472 6f6b 655f 6d61 7463   def stroke_matc
+00012220: 6828 6e6f 6465 2c20 2a2a 6b77 6172 6773  h(node, **kwargs
+00012230: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
+00012240: 726e 2073 656c 662e 636c 6173 7369 6679  rn self.classify
+00012250: 5f69 6e68 6572 6974 5f73 7472 6f6b 650d  _inherit_stroke.
+00012260: 0a0d 0a20 2020 2040 7472 6565 5f73 6570  ...    @tree_sep
+00012270: 6172 6174 6f72 5f62 6566 6f72 6528 290d  arator_before().
+00012280: 0a20 2020 2040 7472 6565 5f73 7562 6d65  .    @tree_subme
+00012290: 6e75 285f 2822 4173 7369 676e 204f 7065  nu(_("Assign Ope
+000122a0: 7261 7469 6f6e 2229 290d 0a20 2020 2040  ration"))..    @
+000122b0: 7472 6565 5f63 6865 636b 2873 7472 6f6b  tree_check(strok
+000122c0: 655f 6d61 7463 6829 0d0a 2020 2020 4074  e_match)..    @t
+000122d0: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
+000122e0: 2020 2020 2020 2020 5f28 2249 6e68 6572          _("Inher
+000122f0: 6974 2073 7472 6f6b 6520 616e 6420 636c  it stroke and cl
+00012300: 6173 7369 6679 2073 696d 696c 6172 2229  assify similar")
+00012310: 2c0d 0a20 2020 2020 2020 206e 6f64 655f  ,..        node_
+00012320: 7479 7065 3d65 6c65 6d5f 6e6f 6465 732c  type=elem_nodes,
+00012330: 0d0a 2020 2020 2020 2020 6865 6c70 3d5f  ..        help=_
+00012340: 2822 4f70 6572 6174 696f 6e20 7769 6c6c  ("Operation will
+00012350: 2069 6e68 6572 6974 2065 6c65 6d65 6e74   inherit element
+00012360: 2073 7472 6f6b 6520 636f 6c6f 7222 292c   stroke color"),
+00012370: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
+00012380: 2073 6574 5f61 7373 6967 6e5f 6f70 7469   set_assign_opti
+00012390: 6f6e 5f73 7472 6f6b 6528 6e6f 6465 2c20  on_stroke(node, 
+000123a0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+000123b0: 2020 2020 7365 6c66 2e63 6c61 7373 6966      self.classif
+000123c0: 795f 696e 6865 7269 745f 7374 726f 6b65  y_inherit_stroke
+000123d0: 203d 206e 6f74 2073 656c 662e 636c 6173   = not self.clas
+000123e0: 7369 6679 5f69 6e68 6572 6974 5f73 7472  sify_inherit_str
+000123f0: 6f6b 650d 0a20 2020 2020 2020 2023 2050  oke..        # P
+00012400: 6f6f 7220 6d61 6e73 2072 6164 696f 0d0a  oor mans radio..
+00012410: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012420: 636c 6173 7369 6679 5f69 6e68 6572 6974  classify_inherit
+00012430: 5f73 7472 6f6b 653a 0d0a 2020 2020 2020  _stroke:..      
+00012440: 2020 2020 2020 7365 6c66 2e63 6c61 7373        self.class
+00012450: 6966 795f 696e 6865 7269 745f 6669 6c6c  ify_inherit_fill
+00012460: 203d 2046 616c 7365 0d0a 0d0a 2020 2020   = False....    
+00012470: 6465 6620 6669 6c6c 5f6d 6174 6368 286e  def fill_match(n
+00012480: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
+00012490: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000124a0: 7365 6c66 2e63 6c61 7373 6966 795f 696e  self.classify_in
+000124b0: 6865 7269 745f 6669 6c6c 0d0a 0d0a 2020  herit_fill....  
+000124c0: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+000124d0: 5f28 2241 7373 6967 6e20 4f70 6572 6174  _("Assign Operat
+000124e0: 696f 6e22 2929 0d0a 2020 2020 4074 7265  ion"))..    @tre
+000124f0: 655f 6368 6563 6b28 6669 6c6c 5f6d 6174  e_check(fill_mat
+00012500: 6368 290d 0a20 2020 2040 7472 6565 5f6f  ch)..    @tree_o
+00012510: 7065 7261 7469 6f6e 280d 0a20 2020 2020  peration(..     
+00012520: 2020 205f 2822 496e 6865 7269 7420 6669     _("Inherit fi
+00012530: 6c6c 2061 6e64 2063 6c61 7373 6966 7920  ll and classify 
+00012540: 7369 6d69 6c61 7222 292c 0d0a 2020 2020  similar"),..    
+00012550: 2020 2020 6e6f 6465 5f74 7970 653d 656c      node_type=el
+00012560: 656d 5f6e 6f64 6573 2c0d 0a20 2020 2020  em_nodes,..     
+00012570: 2020 2068 656c 703d 5f28 224f 7065 7261     help=_("Opera
+00012580: 7469 6f6e 2077 696c 6c20 696e 6865 7269  tion will inheri
+00012590: 7420 656c 656d 656e 7420 6669 6c6c 2063  t element fill c
+000125a0: 6f6c 6f72 2229 2c0d 0a20 2020 2029 0d0a  olor"),..    )..
+000125b0: 2020 2020 6465 6620 7365 745f 6173 7369      def set_assi
+000125c0: 676e 5f6f 7074 696f 6e5f 6669 6c6c 286e  gn_option_fill(n
+000125d0: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
+000125e0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+000125f0: 6173 7369 6679 5f69 6e68 6572 6974 5f66  assify_inherit_f
+00012600: 696c 6c20 3d20 6e6f 7420 7365 6c66 2e63  ill = not self.c
+00012610: 6c61 7373 6966 795f 696e 6865 7269 745f  lassify_inherit_
+00012620: 6669 6c6c 0d0a 2020 2020 2020 2020 2320  fill..        # 
+00012630: 506f 6f72 206d 616e 7320 7261 6469 6f0d  Poor mans radio.
+00012640: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00012650: 2e63 6c61 7373 6966 795f 696e 6865 7269  .classify_inheri
+00012660: 745f 6669 6c6c 3a0d 0a20 2020 2020 2020  t_fill:..       
+00012670: 2020 2020 2073 656c 662e 636c 6173 7369       self.classi
+00012680: 6679 5f69 6e68 6572 6974 5f73 7472 6f6b  fy_inherit_strok
+00012690: 6520 3d20 4661 6c73 650d 0a0d 0a20 2020  e = False....   
+000126a0: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
+000126b0: 616c 286c 616d 6264 6120 6e6f 6465 3a20  al(lambda node: 
+000126c0: 6e6f 7420 6973 5f72 6567 6d61 726b 286e  not is_regmark(n
+000126d0: 6f64 6529 290d 0a20 2020 2040 7472 6565  ode))..    @tree
+000126e0: 5f73 7562 6d65 6e75 285f 2822 4475 706c  _submenu(_("Dupl
+000126f0: 6963 6174 6520 656c 656d 656e 7428 7329  icate element(s)
+00012700: 2229 290d 0a20 2020 2040 7472 6565 5f6f  "))..    @tree_o
+00012710: 7065 7261 7469 6f6e 285f 2822 4d61 6b65  peration(_("Make
+00012720: 2031 2063 6f70 7922 292c 206e 6f64 655f   1 copy"), node_
+00012730: 7479 7065 3d65 6c65 6d5f 6772 6f75 705f  type=elem_group_
+00012740: 6e6f 6465 732c 2068 656c 703d 2222 290d  nodes, help="").
+00012750: 0a20 2020 2064 6566 2064 7570 6c69 6361  .    def duplica
+00012760: 7465 5f65 6c65 6d65 6e74 5f31 286e 6f64  te_element_1(nod
+00012770: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+00012780: 2020 2020 2020 2064 7570 6c69 6361 7465         duplicate
+00012790: 5f65 6c65 6d65 6e74 5f6e 286e 6f64 652c  _element_n(node,
+000127a0: 2063 6f70 6965 733d 312c 202a 2a6b 7761   copies=1, **kwa
+000127b0: 7267 7329 0d0a 0d0a 2020 2020 4074 7265  rgs)....    @tre
+000127c0: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
+000127d0: 6d62 6461 206e 6f64 653a 206e 6f74 2069  mbda node: not i
+000127e0: 735f 7265 676d 6172 6b28 6e6f 6465 2929  s_regmark(node))
+000127f0: 0d0a 2020 2020 4074 7265 655f 7375 626d  ..    @tree_subm
+00012800: 656e 7528 5f28 2244 7570 6c69 6361 7465  enu(_("Duplicate
+00012810: 2065 6c65 6d65 6e74 2873 2922 2929 0d0a   element(s)"))..
+00012820: 2020 2020 4074 7265 655f 6974 6572 6174      @tree_iterat
+00012830: 6528 2263 6f70 6965 7322 2c20 322c 2031  e("copies", 2, 1
+00012840: 3029 0d0a 2020 2020 4074 7265 655f 6f70  0)..    @tree_op
+00012850: 6572 6174 696f 6e28 5f28 224d 616b 6520  eration(_("Make 
+00012860: 7b63 6f70 6965 737d 2063 6f70 6965 7322  {copies} copies"
+00012870: 292c 206e 6f64 655f 7479 7065 3d65 6c65  ), node_type=ele
+00012880: 6d5f 6772 6f75 705f 6e6f 6465 732c 2068  m_group_nodes, h
+00012890: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
+000128a0: 2064 7570 6c69 6361 7465 5f65 6c65 6d65   duplicate_eleme
+000128b0: 6e74 5f6e 286e 6f64 652c 2063 6f70 6965  nt_n(node, copie
+000128c0: 732c 202a 2a6b 7761 7267 7329 3a0d 0a20  s, **kwargs):.. 
+000128d0: 2020 2020 2020 2064 6566 2063 6f70 795f         def copy_
+000128e0: 7369 6e67 6c65 5f6e 6f64 6528 6f72 676e  single_node(orgn
+000128f0: 6f64 652c 206f 7267 7061 7265 6e74 2c20  ode, orgparent, 
+00012900: 7469 6d65 732c 2064 782c 2064 7929 3a0d  times, dx, dy):.
+00012910: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+00012920: 7461 5f77 6f72 646c 6973 7420 3d20 300d  ta_wordlist = 0.
+00012930: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00012940: 206e 2069 6e20 7261 6e67 6528 7469 6d65   n in range(time
+00012950: 7329 3a0d 0a20 2020 2020 2020 2020 2020  s):..           
+00012960: 2020 2020 2064 656c 7461 5f77 6f72 646c       delta_wordl
+00012970: 6973 7420 2b3d 2031 0d0a 0d0a 2020 2020  ist += 1....    
+00012980: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+00012990: 5f6e 6f64 6520 3d20 636f 7079 286f 7267  _node = copy(org
+000129a0: 6e6f 6465 290d 0a20 2020 2020 2020 2020  node)..         
+000129b0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+000129c0: 7228 636f 7079 5f6e 6f64 652c 2022 6d61  r(copy_node, "ma
+000129d0: 7472 6978 2229 3a0d 0a20 2020 2020 2020  trix"):..       
+000129e0: 2020 2020 2020 2020 2020 2020 2063 6f70               cop
+000129f0: 795f 6e6f 6465 2e6d 6174 7269 7820 2a3d  y_node.matrix *=
+00012a00: 204d 6174 7269 782e 7472 616e 736c 6174   Matrix.translat
+00012a10: 6528 286e 202b 2031 2920 2a20 6478 2c20  e((n + 1) * dx, 
+00012a20: 286e 202b 2031 2920 2a20 6479 290d 0a20  (n + 1) * dy).. 
+00012a30: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00012a40: 6164 5f6f 7074 696f 6e61 6c20 3d20 4661  ad_optional = Fa
+00012a50: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00012a60: 2020 2020 2023 204e 6565 6420 746f 2061       # Need to a
+00012a70: 6464 2073 7472 6f6b 6520 616e 6420 6669  dd stroke and fi
+00012a80: 6c6c 2c20 6173 2063 6f70 7920 7769 6c6c  ll, as copy will
+00012a90: 2074 616b 6520 7468 650d 0a20 2020 2020   take the..     
+00012aa0: 2020 2020 2020 2020 2020 2023 2064 6566             # def
+00012ab0: 6175 6c74 2076 616c 7565 7320 666f 7220  ault values for 
+00012ac0: 7468 6573 6520 6174 7472 6962 7574 6573  these attributes
+00012ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012ae0: 2020 666f 7220 6f70 7469 6f6e 616c 2069    for optional i
+00012af0: 6e20 2822 6669 6c6c 222c 2022 7374 726f  n ("fill", "stro
+00012b00: 6b65 2229 3a0d 0a20 2020 2020 2020 2020  ke"):..         
+00012b10: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+00012b20: 7361 7474 7228 6f72 676e 6f64 652c 206f  sattr(orgnode, o
+00012b30: 7074 696f 6e61 6c29 3a0d 0a20 2020 2020  ptional):..     
+00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b50: 2020 2073 6574 6174 7472 2863 6f70 795f     setattr(copy_
+00012b60: 6e6f 6465 2c20 6f70 7469 6f6e 616c 2c20  node, optional, 
+00012b70: 6765 7461 7474 7228 6f72 676e 6f64 652c  getattr(orgnode,
+00012b80: 206f 7074 696f 6e61 6c29 290d 0a20 2020   optional))..   
+00012b90: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00012ba0: 206f 7074 696f 6e61 6c20 696e 2028 2277   optional in ("w
+00012bb0: 7866 6f6e 7422 2c20 226d 6b74 6578 7422  xfont", "mktext"
+00012bc0: 2c20 226d 6b66 6f6e 7422 2c20 226d 6b66  , "mkfont", "mkf
+00012bd0: 6f6e 7473 697a 6522 293a 0d0a 2020 2020  ontsize"):..    
+00012be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bf0: 6966 2068 6173 6174 7472 286f 7267 6e6f  if hasattr(orgno
+00012c00: 6465 2c20 6f70 7469 6f6e 616c 293a 0d0a  de, optional):..
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 2020 2020 2020 6861 645f 6f70 7469          had_opti
+00012c30: 6f6e 616c 203d 2054 7275 650d 0a20 2020  onal = True..   
+00012c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c50: 2020 2020 2073 6574 6174 7472 2863 6f70       setattr(cop
+00012c60: 795f 6e6f 6465 2c20 6f70 7469 6f6e 616c  y_node, optional
+00012c70: 2c20 6765 7461 7474 7228 6f72 676e 6f64  , getattr(orgnod
+00012c80: 652c 206f 7074 696f 6e61 6c29 290d 0a20  e, optional)).. 
+00012c90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012ca0: 6620 7365 6c66 2e63 6f70 795f 696e 6372  f self.copy_incr
+00012cb0: 6561 7365 735f 776f 7264 6c69 7374 5f72  eases_wordlist_r
+00012cc0: 6566 6572 656e 6365 7320 616e 6420 6861  eferences and ha
+00012cd0: 7361 7474 7228 6f72 676e 6f64 652c 2022  sattr(orgnode, "
+00012ce0: 7465 7874 2229 3a0d 0a20 2020 2020 2020  text"):..       
+00012cf0: 2020 2020 2020 2020 2020 2020 2063 6f70               cop
+00012d00: 795f 6e6f 6465 2e74 6578 7420 3d20 7365  y_node.text = se
+00012d10: 6c66 2e77 6f72 646c 6973 745f 6465 6c74  lf.wordlist_delt
+00012d20: 6128 6f72 676e 6f64 652e 7465 7874 2c20  a(orgnode.text, 
+00012d30: 6465 6c74 615f 776f 7264 6c69 7374 290d  delta_wordlist).
+00012d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d50: 2065 6c69 6620 7365 6c66 2e63 6f70 795f   elif self.copy_
+00012d60: 696e 6372 6561 7365 735f 776f 7264 6c69  increases_wordli
+00012d70: 7374 5f72 6566 6572 656e 6365 7320 616e  st_references an
+00012d80: 6420 6861 7361 7474 7228 652c 2022 6d6b  d hasattr(e, "mk
+00012d90: 7465 7874 2229 3a0d 0a20 2020 2020 2020  text"):..       
+00012da0: 2020 2020 2020 2020 2020 2020 2063 6f70               cop
+00012db0: 795f 6e6f 6465 2e6d 6b74 6578 7420 3d20  y_node.mktext = 
+00012dc0: 7365 6c66 2e77 6f72 646c 6973 745f 6465  self.wordlist_de
+00012dd0: 6c74 6128 652e 6d6b 7465 7874 2c20 6465  lta(e.mktext, de
+00012de0: 6c74 615f 776f 7264 6c69 7374 290d 0a20  lta_wordlist).. 
+00012df0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00012e00: 7267 7061 7265 6e74 2e61 6464 5f6e 6f64  rgparent.add_nod
+00012e10: 6528 636f 7079 5f6e 6f64 6529 0d0a 2020  e(copy_node)..  
+00012e20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012e30: 2068 6164 5f6f 7074 696f 6e61 6c3a 0d0a   had_optional:..
+00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e50: 2020 2020 666f 7220 7072 6f70 6572 7479      for property
+00012e60: 5f6f 7020 696e 2073 656c 662e 6b65 726e  _op in self.kern
+00012e70: 656c 2e6c 6f6f 6b75 705f 616c 6c28 2270  el.lookup_all("p
+00012e80: 6174 685f 7570 6461 7465 722f 2e2a 2229  ath_updater/.*")
+00012e90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012ea0: 2020 2020 2020 2020 2020 2070 726f 7065             prope
+00012eb0: 7274 795f 6f70 2873 656c 662e 6b65 726e  rty_op(self.kern
+00012ec0: 656c 2e72 6f6f 742c 2063 6f70 795f 6e6f  el.root, copy_no
+00012ed0: 6465 290d 0a0d 0a20 2020 2020 2020 2020  de)....         
+00012ee0: 2020 2020 2020 2063 6f70 795f 6e6f 6465         copy_node
+00012ef0: 732e 6170 7065 6e64 2863 6f70 795f 6e6f  s.append(copy_no
+00012f00: 6465 290d 0a0d 0a20 2020 2020 2020 2020  de)....         
+00012f10: 2020 2020 2020 2069 6620 6f72 676e 6f64         if orgnod
+00012f20: 652e 7479 7065 2069 6e20 2822 6669 6c65  e.type in ("file
+00012f30: 222c 2022 6772 6f75 7022 293a 0d0a 2020  ", "group"):..  
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f50: 2020 6e65 7770 6172 656e 7420 3d20 636f    newparent = co
+00012f60: 7079 5f6e 6f64 650d 0a20 2020 2020 2020  py_node..       
+00012f70: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00012f80: 2063 6e6f 6465 2069 6e20 6f72 676e 6f64   cnode in orgnod
+00012f90: 652e 6368 696c 6472 656e 3a0d 0a20 2020  e.children:..   
+00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fb0: 2020 2020 2063 6f70 795f 7369 6e67 6c65       copy_single
+00012fc0: 5f6e 6f64 6528 0d0a 2020 2020 2020 2020  _node(..        
+00012fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fe0: 2020 2020 636e 6f64 652c 206e 6577 7061      cnode, newpa
+00012ff0: 7265 6e74 2c20 312c 2028 6e20 2b20 3129  rent, 1, (n + 1)
+00013000: 202a 2064 782c 2028 6e20 2b20 3129 202a   * dx, (n + 1) *
+00013010: 2064 790d 0a20 2020 2020 2020 2020 2020   dy..           
+00013020: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+00013030: 0d0a 2020 2020 2020 2020 636f 7079 5f6e  ..        copy_n
+00013040: 6f64 6573 203d 206c 6973 7428 290d 0a20  odes = list().. 
+00013050: 2020 2020 2020 2064 7820 3d20 7365 6c66         dx = self
+00013060: 2e6c 656e 6774 685f 7828 2233 6d6d 2229  .length_x("3mm")
+00013070: 0d0a 2020 2020 2020 2020 6479 203d 2073  ..        dy = s
+00013080: 656c 662e 6c65 6e67 7468 5f79 2822 336d  elf.length_y("3m
+00013090: 6d22 290d 0a20 2020 2020 2020 2061 6c6c  m")..        all
+000130a0: 6461 7461 203d 206c 6973 7428 7365 6c66  data = list(self
+000130b0: 2e65 6c65 6d73 2865 6d70 6861 7369 7a65  .elems(emphasize
+000130c0: 643d 5472 7565 2929 0d0a 2020 2020 2020  d=True))..      
+000130d0: 2020 6d69 6e69 6d61 6c64 6174 6120 3d20    minimaldata = 
+000130e0: 7365 6c66 2e63 6f6e 6465 6e73 655f 656c  self.condense_el
+000130f0: 656d 656e 7473 2861 6c6c 6461 7461 2c20  ements(alldata, 
+00013100: 6578 7061 6e64 5f61 745f 656e 643d 4661  expand_at_end=Fa
+00013110: 6c73 6529 0d0a 2020 2020 2020 2020 666f  lse)..        fo
+00013120: 7220 6520 696e 206d 696e 696d 616c 6461  r e in minimalda
+00013130: 7461 3a0d 0a20 2020 2020 2020 2020 2020  ta:..           
+00013140: 2070 6172 656e 7420 3d20 652e 7061 7265   parent = e.pare
+00013150: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00013160: 636f 7079 5f73 696e 676c 655f 6e6f 6465  copy_single_node
+00013170: 2865 2c20 7061 7265 6e74 2c20 636f 7069  (e, parent, copi
+00013180: 6573 2c20 6478 2c20 6479 290d 0a0d 0a20  es, dx, dy).... 
+00013190: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000131a0: 6c61 7373 6966 795f 6e65 773a 0d0a 2020  lassify_new:..  
+000131b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000131c0: 6c61 7373 6966 7928 636f 7079 5f6e 6f64  lassify(copy_nod
+000131d0: 6573 290d 0a0d 0a20 2020 2020 2020 2073  es)....        s
+000131e0: 656c 662e 7365 745f 656d 7068 6173 6973  elf.set_emphasis
+000131f0: 284e 6f6e 6529 0d0a 0d0a 2020 2020 6465  (None)....    de
+00013200: 6620 6861 735f 776f 7264 6c69 7374 286e  f has_wordlist(n
+00013210: 6f64 6529 3a0d 0a20 2020 2020 2020 2072  ode):..        r
+00013220: 6573 756c 7420 3d20 4661 6c73 650d 0a20  esult = False.. 
+00013230: 2020 2020 2020 2074 7874 203d 2022 220d         txt = "".
+00013240: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
+00013250: 7474 7228 6e6f 6465 2c20 2274 6578 7422  ttr(node, "text"
+00013260: 2920 616e 6420 6e6f 6465 2e74 6578 7420  ) and node.text 
+00013270: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00013280: 2020 2020 2020 2020 2020 7478 7420 3d20            txt = 
+00013290: 7374 7228 6e6f 6465 2e74 6578 7429 0d0a  str(node.text)..
+000132a0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+000132b0: 7472 286e 6f64 652c 2022 6d6b 7465 7874  tr(node, "mktext
+000132c0: 2229 2061 6e64 206e 6f64 652e 6d6b 7465  ") and node.mkte
+000132d0: 7874 2069 7320 6e6f 7420 4e6f 6e65 3a0d  xt is not None:.
+000132e0: 0a20 2020 2020 2020 2020 2020 2074 7874  .            txt
+000132f0: 203d 2073 7472 286e 6f64 652e 6d6b 7465   = str(node.mkte
+00013300: 7874 290d 0a20 2020 2020 2020 2023 2056  xt)..        # V
+00013310: 6572 7920 7374 7570 6964 2c20 6275 7420  ery stupid, but 
+00013320: 676f 6f64 2065 6e6f 7567 680d 0a20 2020  good enough..   
+00013330: 2020 2020 2069 6620 227b 2220 696e 2074       if "{" in t
+00013340: 7874 2061 6e64 2022 7d22 2069 6e20 7478  xt and "}" in tx
+00013350: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00013360: 7265 7375 6c74 203d 2054 7275 650d 0a20  result = True.. 
+00013370: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00013380: 7375 6c74 0d0a 0d0a 2020 2020 4074 7265  sult....    @tre
+00013390: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
+000133a0: 6d62 6461 206e 6f64 653a 2068 6173 5f77  mbda node: has_w
+000133b0: 6f72 646c 6973 7428 6e6f 6465 2929 0d0a  ordlist(node))..
+000133c0: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
+000133d0: 696f 6e28 0d0a 2020 2020 2020 2020 5f28  ion(..        _(
+000133e0: 2249 6e63 7265 6173 6520 576f 7264 6c69  "Increase Wordli
+000133f0: 7374 2d52 6566 6572 656e 6365 2229 2c0d  st-Reference"),.
+00013400: 0a20 2020 2020 2020 206e 6f64 655f 7479  .        node_ty
+00013410: 7065 3d28 0d0a 2020 2020 2020 2020 2020  pe=(..          
+00013420: 2020 2265 6c65 6d20 7465 7874 222c 0d0a    "elem text",..
+00013430: 2020 2020 2020 2020 2020 2020 2265 6c65              "ele
+00013440: 6d20 7061 7468 222c 0d0a 2020 2020 2020  m path",..      
+00013450: 2020 292c 0d0a 2020 2020 2020 2020 6865    ),..        he
+00013460: 6c70 3d5f 2822 4164 6a75 7374 7320 7468  lp=_("Adjusts th
+00013470: 6520 7265 6665 7265 6e63 6520 7661 6c75  e reference valu
+00013480: 6520 666f 7220 6120 776f 7264 6c69 7374  e for a wordlist
+00013490: 2c20 6965 207b 6e61 6d65 7d20 746f 207b  , ie {name} to {
+000134a0: 6e61 6d65 232b 317d 2229 2c0d 0a20 2020  name#+1}"),..   
+000134b0: 2029 0d0a 2020 2020 6465 6620 776c 6973   )..    def wlis
+000134c0: 745f 706c 7573 2873 696e 676c 656e 6f64  t_plus(singlenod
+000134d0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+000134e0: 2020 2020 2020 2064 6174 6120 3d20 6c69         data = li
+000134f0: 7374 2829 0d0a 2020 2020 2020 2020 666f  st()..        fo
+00013500: 7220 6e6f 6465 2069 6e20 6c69 7374 2873  r node in list(s
+00013510: 656c 662e 656c 656d 7328 656d 7068 6173  elf.elems(emphas
+00013520: 697a 6564 3d54 7275 6529 293a 0d0a 2020  ized=True)):..  
+00013530: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00013540: 2068 6173 5f77 6f72 646c 6973 7428 6e6f   has_wordlist(no
+00013550: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
+00013560: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00013570: 2020 2020 2020 2020 2020 2020 6465 6c74              delt
+00013580: 615f 776f 7264 6c69 7374 203d 2031 0d0a  a_wordlist = 1..
+00013590: 2020 2020 2020 2020 2020 2020 6966 2068              if h
+000135a0: 6173 6174 7472 286e 6f64 652c 2022 7465  asattr(node, "te
+000135b0: 7874 2229 3a0d 0a20 2020 2020 2020 2020  xt"):..         
+000135c0: 2020 2020 2020 206e 6f64 652e 7465 7874         node.text
+000135d0: 203d 2073 656c 662e 776f 7264 6c69 7374   = self.wordlist
+000135e0: 5f64 656c 7461 286e 6f64 652e 7465 7874  _delta(node.text
+000135f0: 2c20 6465 6c74 615f 776f 7264 6c69 7374  , delta_wordlist
+00013600: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013610: 2020 206e 6f64 652e 616c 7465 7265 6428     node.altered(
+00013620: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013630: 2020 2064 6174 612e 6170 7065 6e64 286e     data.append(n
+00013640: 6f64 6529 0d0a 2020 2020 2020 2020 2020  ode)..          
+00013650: 2020 656c 6966 2068 6173 6174 7472 286e    elif hasattr(n
+00013660: 6f64 652c 2022 6d6b 7465 7874 2229 3a0d  ode, "mktext"):.
+00013670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013680: 206e 6f64 652e 6d6b 7465 7874 203d 2073   node.mktext = s
+00013690: 656c 662e 776f 7264 6c69 7374 5f64 656c  elf.wordlist_del
+000136a0: 7461 286e 6f64 652e 6d6b 7465 7874 2c20  ta(node.mktext, 
+000136b0: 6465 6c74 615f 776f 7264 6c69 7374 290d  delta_wordlist).
+000136c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000136d0: 2066 6f72 2070 726f 7065 7274 795f 6f70   for property_op
+000136e0: 2069 6e20 7365 6c66 2e6b 6572 6e65 6c2e   in self.kernel.
+000136f0: 6c6f 6f6b 7570 5f61 6c6c 2822 7061 7468  lookup_all("path
+00013700: 5f75 7064 6174 6572 2f2e 2a22 293a 0d0a  _updater/.*"):..
+00013710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013720: 2020 2020 7072 6f70 6572 7479 5f6f 7028      property_op(
+00013730: 7365 6c66 2e6b 6572 6e65 6c2e 726f 6f74  self.kernel.root
+00013740: 2c20 6e6f 6465 290d 0a20 2020 2020 2020  , node)..       
+00013750: 2020 2020 2020 2020 2064 6174 612e 6170           data.ap
+00013760: 7065 6e64 286e 6f64 6529 0d0a 2020 2020  pend(node)..    
+00013770: 2020 2020 7365 6c66 2e73 6967 6e61 6c28      self.signal(
+00013780: 2265 6c65 6d65 6e74 5f70 726f 7065 7274  "element_propert
+00013790: 795f 7570 6461 7465 222c 2064 6174 6129  y_update", data)
+000137a0: 0d0a 0d0a 2020 2020 4074 7265 655f 636f  ....    @tree_co
+000137b0: 6e64 6974 696f 6e61 6c28 6c61 6d62 6461  nditional(lambda
+000137c0: 206e 6f64 653a 2068 6173 5f77 6f72 646c   node: has_wordl
+000137d0: 6973 7428 6e6f 6465 2929 0d0a 2020 2020  ist(node))..    
+000137e0: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+000137f0: 0d0a 2020 2020 2020 2020 5f28 2244 6563  ..        _("Dec
+00013800: 7265 6173 6520 576f 7264 6c69 7374 2d52  rease Wordlist-R
+00013810: 6566 6572 656e 6365 2229 2c0d 0a20 2020  eference"),..   
+00013820: 2020 2020 206e 6f64 655f 7479 7065 3d28       node_type=(
+00013830: 0d0a 2020 2020 2020 2020 2020 2020 2265  ..            "e
+00013840: 6c65 6d20 7465 7874 222c 0d0a 2020 2020  lem text",..    
+00013850: 2020 2020 2020 2020 2265 6c65 6d20 7061          "elem pa
+00013860: 7468 222c 0d0a 2020 2020 2020 2020 292c  th",..        ),
+00013870: 0d0a 2020 2020 2020 2020 6865 6c70 3d5f  ..        help=_
+00013880: 2822 4164 6a75 7374 7320 7468 6520 7265  ("Adjusts the re
+00013890: 6665 7265 6e63 6520 7661 6c75 6520 666f  ference value fo
+000138a0: 7220 6120 776f 7264 6c69 7374 2c20 6965  r a wordlist, ie
+000138b0: 207b 6e61 6d65 232b 337d 2074 6f20 7b6e   {name#+3} to {n
+000138c0: 616d 6523 2b32 7d22 292c 0d0a 2020 2020  ame#+2}"),..    
+000138d0: 290d 0a20 2020 2064 6566 2077 6c69 7374  )..    def wlist
+000138e0: 5f6d 696e 7573 2873 696e 676c 656e 6f64  _minus(singlenod
+000138f0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+00013900: 2020 2020 2020 2064 6174 6120 3d20 6c69         data = li
+00013910: 7374 2829 0d0a 2020 2020 2020 2020 666f  st()..        fo
+00013920: 7220 6e6f 6465 2069 6e20 6c69 7374 2873  r node in list(s
+00013930: 656c 662e 656c 656d 7328 656d 7068 6173  elf.elems(emphas
+00013940: 697a 6564 3d54 7275 6529 293a 0d0a 2020  ized=True)):..  
+00013950: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00013960: 2068 6173 5f77 6f72 646c 6973 7428 6e6f   has_wordlist(no
+00013970: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
+00013980: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00013990: 2020 2020 2020 2020 2020 2020 6465 6c74              delt
+000139a0: 615f 776f 7264 6c69 7374 203d 202d 310d  a_wordlist = -1.
+000139b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000139c0: 6861 7361 7474 7228 6e6f 6465 2c20 2274  hasattr(node, "t
+000139d0: 6578 7422 293a 0d0a 2020 2020 2020 2020  ext"):..        
+000139e0: 2020 2020 2020 2020 6e6f 6465 2e74 6578          node.tex
+000139f0: 7420 3d20 7365 6c66 2e77 6f72 646c 6973  t = self.wordlis
+00013a00: 745f 6465 6c74 6128 6e6f 6465 2e74 6578  t_delta(node.tex
+00013a10: 742c 2064 656c 7461 5f77 6f72 646c 6973  t, delta_wordlis
+00013a20: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00013a30: 2020 2020 6e6f 6465 2e61 6c74 6572 6564      node.altered
+00013a40: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00013a50: 2020 2020 6461 7461 2e61 7070 656e 6428      data.append(
+00013a60: 6e6f 6465 290d 0a20 2020 2020 2020 2020  node)..         
+00013a70: 2020 2065 6c69 6620 6861 7361 7474 7228     elif hasattr(
+00013a80: 6e6f 6465 2c20 226d 6b74 6578 7422 293a  node, "mktext"):
+00013a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013aa0: 2020 6e6f 6465 2e6d 6b74 6578 7420 3d20    node.mktext = 
+00013ab0: 7365 6c66 2e77 6f72 646c 6973 745f 6465  self.wordlist_de
+00013ac0: 6c74 6128 6e6f 6465 2e6d 6b74 6578 742c  lta(node.mktext,
+00013ad0: 2064 656c 7461 5f77 6f72 646c 6973 7429   delta_wordlist)
+00013ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013af0: 2020 666f 7220 7072 6f70 6572 7479 5f6f    for property_o
+00013b00: 7020 696e 2073 656c 662e 6b65 726e 656c  p in self.kernel
+00013b10: 2e6c 6f6f 6b75 705f 616c 6c28 2270 6174  .lookup_all("pat
+00013b20: 685f 7570 6461 7465 722f 2e2a 2229 3a0d  h_updater/.*"):.
+00013b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b40: 2020 2020 2070 726f 7065 7274 795f 6f70       property_op
+00013b50: 2873 656c 662e 6b65 726e 656c 2e72 6f6f  (self.kernel.roo
+00013b60: 742c 206e 6f64 6529 0d0a 2020 2020 2020  t, node)..      
+00013b70: 2020 2020 2020 2020 2020 6461 7461 2e61            data.a
+00013b80: 7070 656e 6428 6e6f 6465 290d 0a20 2020  ppend(node)..   
+00013b90: 2020 2020 2073 656c 662e 7369 676e 616c       self.signal
+00013ba0: 2822 656c 656d 656e 745f 7072 6f70 6572  ("element_proper
+00013bb0: 7479 5f75 7064 6174 6522 2c20 6461 7461  ty_update", data
+00013bc0: 290d 0a0d 0a20 2020 2040 7472 6565 5f63  )....    @tree_c
+00013bd0: 6f6e 6469 7469 6f6e 616c 286c 616d 6264  onditional(lambd
+00013be0: 6120 6e6f 6465 3a20 6861 735f 7665 6374  a node: has_vect
+00013bf0: 6f72 697a 6528 6e6f 6465 2929 0d0a 2020  orize(node))..  
+00013c00: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+00013c10: 5f28 224f 7574 6c69 6e65 2065 6c65 6d65  _("Outline eleme
+00013c20: 6e74 2873 292e 2e2e 2229 290d 0a20 2020  nt(s)..."))..   
+00013c30: 2040 7472 6565 5f69 7465 7261 7465 2822   @tree_iterate("
+00013c40: 6f66 6673 6574 222c 2031 2c20 3130 290d  offset", 1, 10).
+00013c50: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
+00013c60: 7469 6f6e 280d 0a20 2020 2020 2020 205f  tion(..        _
+00013c70: 2822 2e2e 2e77 6974 6820 7b6f 6666 7365  ("...with {offse
+00013c80: 747d 6d6d 2064 6973 7461 6e63 6522 292c  t}mm distance"),
+00013c90: 0d0a 2020 2020 2020 2020 6e6f 6465 5f74  ..        node_t
+00013ca0: 7970 653d 656c 656d 5f6e 6f64 6573 2c0d  ype=elem_nodes,.
+00013cb0: 0a20 2020 2020 2020 2068 656c 703d 2222  .        help=""
+00013cc0: 2c0d 0a20 2020 2029 0d0a 2020 2020 6465  ,..    )..    de
+00013cd0: 6620 6d61 6b65 5f6f 7574 6c69 6e65 7328  f make_outlines(
+00013ce0: 6e6f 6465 2c20 6f66 6673 6574 3d31 2c20  node, offset=1, 
+00013cf0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+00013d00: 2020 2020 7365 6c66 2866 226f 7574 6c69      self(f"outli
+00013d10: 6e65 207b 6f66 6673 6574 7d6d 6d5c 6e22  ne {offset}mm\n"
+00013d20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00013d30: 7369 676e 616c 2822 7265 6672 6573 685f  signal("refresh_
+00013d40: 7472 6565 2229 0d0a 0d0a 2020 2020 6465  tree")....    de
+00013d50: 6620 6861 735f 7665 6374 6f72 697a 6528  f has_vectorize(
+00013d60: 6e6f 6465 293a 0d0a 2020 2020 2020 2020  node):..        
+00013d70: 7265 7375 6c74 203d 2046 616c 7365 0d0a  result = False..
+00013d80: 2020 2020 2020 2020 6d61 6b65 5f76 6563          make_vec
+00013d90: 746f 7220 3d20 7365 6c66 2e6c 6f6f 6b75  tor = self.looku
+00013da0: 7028 2272 656e 6465 722d 6f70 2f6d 616b  p("render-op/mak
+00013db0: 655f 7665 6374 6f72 2229 0d0a 2020 2020  e_vector")..    
+00013dc0: 2020 2020 6966 206d 616b 655f 7665 6374      if make_vect
+00013dd0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+00013de0: 2072 6573 756c 7420 3d20 5472 7565 0d0a   result = True..
+00013df0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00013e00: 6573 756c 740d 0a0d 0a20 2020 2040 7472  esult....    @tr
+00013e10: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
+00013e20: 616d 6264 6120 6e6f 6465 3a20 6861 735f  ambda node: has_
+00013e30: 7665 6374 6f72 697a 6528 6e6f 6465 2929  vectorize(node))
+00013e40: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+00013e50: 6174 696f 6e28 0d0a 2020 2020 2020 2020  ation(..        
+00013e60: 5f28 2254 7261 6365 2062 6974 6d61 7022  _("Trace bitmap"
+00013e70: 292c 0d0a 2020 2020 2020 2020 6e6f 6465  ),..        node
+00013e80: 5f74 7970 653d 280d 0a20 2020 2020 2020  _type=(..       
+00013e90: 2020 2020 2022 656c 656d 2074 6578 7422       "elem text"
+00013ea0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00013eb0: 656c 656d 2069 6d61 6765 222c 0d0a 2020  elem image",..  
+00013ec0: 2020 2020 2020 292c 0d0a 2020 2020 2020        ),..      
+00013ed0: 2020 6865 6c70 3d5f 2822 5665 6374 6f72    help=_("Vector
+00013ee0: 697a 6520 7468 6520 6769 7665 6e20 656c  ize the given el
+00013ef0: 656d 656e 7422 292c 0d0a 2020 2020 290d  ement"),..    ).
+00013f00: 0a20 2020 2064 6566 2074 7261 6365 5f62  .    def trace_b
+00013f10: 6974 6d61 7028 6e6f 6465 2c20 2a2a 6b77  itmap(node, **kw
+00013f20: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00013f30: 7365 6c66 2822 7665 6374 6f72 697a 655c  self("vectorize\
+00013f40: 6e22 290d 0a0d 0a20 2020 2040 7472 6565  n")....    @tree
+00013f50: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
+00013f60: 6264 6120 6e6f 6465 3a20 6e6f 7420 6973  bda node: not is
+00013f70: 5f72 6567 6d61 726b 286e 6f64 6529 290d  _regmark(node)).
+00013f80: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
+00013f90: 7469 6f6e 280d 0a20 2020 2020 2020 205f  tion(..        _
+00013fa0: 2822 436f 6e76 6572 7420 746f 2070 6174  ("Convert to pat
+00013fb0: 6822 292c 0d0a 2020 2020 2020 2020 6e6f  h"),..        no
+00013fc0: 6465 5f74 7970 653d 280d 0a20 2020 2020  de_type=(..     
+00013fd0: 2020 2020 2020 2022 656c 656d 2065 6c6c         "elem ell
+00013fe0: 6970 7365 222c 0d0a 2020 2020 2020 2020  ipse",..        
+00013ff0: 2020 2020 2265 6c65 6d20 7061 7468 222c      "elem path",
+00014000: 0d0a 2020 2020 2020 2020 2020 2020 2265  ..            "e
+00014010: 6c65 6d20 706f 6c79 6c69 6e65 222c 0d0a  lem polyline",..
+00014020: 2020 2020 2020 2020 2020 2020 2265 6c65              "ele
+00014030: 6d20 7265 6374 222c 0d0a 2020 2020 2020  m rect",..      
+00014040: 2020 2020 2020 2265 6c65 6d20 6c69 6e65        "elem line
+00014050: 222c 0d0a 2020 2020 2020 2020 292c 0d0a  ",..        ),..
+00014060: 2020 2020 2020 2020 6865 6c70 3d22 222c          help="",
+00014070: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
+00014080: 2063 6f6e 7665 7274 5f74 6f5f 7061 7468   convert_to_path
+00014090: 2873 696e 676c 656e 6f64 652c 202a 2a6b  (singlenode, **k
+000140a0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+000140b0: 2066 6f72 206e 6f64 6520 696e 206c 6973   for node in lis
+000140c0: 7428 7365 6c66 2e65 6c65 6d73 2865 6d70  t(self.elems(emp
+000140d0: 6861 7369 7a65 643d 5472 7565 2929 3a0d  hasized=True)):.
+000140e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000140f0: 6e6f 7420 6e6f 6465 206e 6f74 2069 6e20  not node not in 
+00014100: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00014110: 2020 2022 656c 656d 2065 6c6c 6970 7365     "elem ellipse
+00014120: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00014130: 2020 2020 2265 6c65 6d20 7061 7468 222c      "elem path",
+00014140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014150: 2020 2265 6c65 6d20 706f 6c79 6c69 6e65    "elem polyline
+00014160: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00014170: 2020 2020 2265 6c65 6d20 7265 6374 222c      "elem rect",
+00014180: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014190: 2020 2265 6c65 6d20 6c69 6e65 222c 0d0a    "elem line",..
+000141a0: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141c0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+000141d0: 2020 2020 2020 6f6c 6473 7475 6666 203d        oldstuff =
+000141e0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
+000141f0: 2066 6f72 2061 7474 7269 6220 696e 2028   for attrib in (
+00014200: 2273 7472 6f6b 6522 2c20 2266 696c 6c22  "stroke", "fill"
+00014210: 2c20 2273 7472 6f6b 655f 7769 6474 6822  , "stroke_width"
+00014220: 2c20 2273 7472 6f6b 655f 7363 616c 6564  , "stroke_scaled
+00014230: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
+00014240: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00014250: 6e6f 6465 2c20 6174 7472 6962 293a 0d0a  node, attrib):..
+00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014270: 2020 2020 6f6c 6476 616c 203d 2067 6574      oldval = get
+00014280: 6174 7472 286e 6f64 652c 2061 7474 7269  attr(node, attri
+00014290: 622c 204e 6f6e 6529 0d0a 2020 2020 2020  b, None)..      
+000142a0: 2020 2020 2020 2020 2020 2020 2020 6f6c                ol
+000142b0: 6473 7475 6666 2e61 7070 656e 6428 5b61  dstuff.append([a
+000142c0: 7474 7269 622c 206f 6c64 7661 6c5d 290d  ttrib, oldval]).
+000142d0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+000142e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000142f0: 2020 2070 6174 6820 3d20 6e6f 6465 2e61     path = node.a
+00014300: 735f 7061 7468 2829 0d0a 2020 2020 2020  s_path()..      
+00014310: 2020 2020 2020 2020 2020 2320 5468 6572            # Ther
+00014320: 6520 6172 6520 736f 6d65 2063 6861 6c6c  e are some chall
+00014330: 656e 6765 7320 6172 6f75 6e64 2074 6865  enges around the
+00014340: 2074 7265 6174 6d65 6e74 0d0a 2020 2020   treatment..    
+00014350: 2020 2020 2020 2020 2020 2020 2320 6f66              # of
+00014360: 2061 7263 7320 7769 7468 696e 2073 7667   arcs within svg
+00014370: 656c 656d 656e 7473 2c20 736f 206c 6574  elements, so let
+00014380: 2773 2063 6972 6375 6d76 656e 740d 0a20  's circumvent.. 
+00014390: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000143a0: 2074 6865 6d20 666f 7220 7468 6520 7469   them for the ti
+000143b0: 6d65 2062 6569 6e67 2028 756e 7469 6c20  me being (until 
+000143c0: 7265 736f 6c76 6564 290d 0a20 2020 2020  resolved)..     
+000143d0: 2020 2020 2020 2020 2020 2023 2062 7920             # by 
+000143e0: 7265 706c 6163 696e 6720 6172 6320 7365  replacing arc se
+000143f0: 676d 656e 7473 2077 6974 6820 6375 6269  gments with cubi
+00014400: 6320 6265 7a69 6572 730d 0a20 2020 2020  c beziers..     
+00014410: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00014420: 6465 2e74 7970 6520 696e 2028 2265 6c65  de.type in ("ele
+00014430: 6d20 7061 7468 222c 2022 656c 656d 2065  m path", "elem e
+00014440: 6c6c 6970 7365 2229 3a0d 0a20 2020 2020  llipse"):..     
+00014450: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00014460: 6174 682e 6170 7072 6f78 696d 6174 655f  ath.approximate_
+00014470: 6172 6373 5f77 6974 685f 6375 6269 6373  arcs_with_cubics
+00014480: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00014490: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
+000144a0: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
+000144b0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+000144c0: 2020 2020 2020 2020 2020 2020 6e65 776e              newn
+000144d0: 6f64 6520 3d20 6e6f 6465 2e72 6570 6c61  ode = node.repla
+000144e0: 6365 5f6e 6f64 6528 7061 7468 3d70 6174  ce_node(path=pat
+000144f0: 682c 2074 7970 653d 2265 6c65 6d20 7061  h, type="elem pa
+00014500: 7468 2229 0d0a 2020 2020 2020 2020 2020  th")..          
+00014510: 2020 666f 7220 6974 656d 2069 6e20 6f6c    for item in ol
+00014520: 6473 7475 6666 3a0d 0a20 2020 2020 2020  dstuff:..       
+00014530: 2020 2020 2020 2020 2073 6574 6174 7472           setattr
+00014540: 286e 6577 6e6f 6465 2c20 6974 656d 5b30  (newnode, item[0
+00014550: 5d2c 2069 7465 6d5b 315d 290d 0a20 2020  ], item[1])..   
+00014560: 2020 2020 2020 2020 206e 6577 6e6f 6465           newnode
+00014570: 2e61 6c74 6572 6564 2829 0d0a 0d0a 2020  .altered()....  
+00014580: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+00014590: 5f28 2246 6c69 7022 2929 0d0a 2020 2020  _("Flip"))..    
+000145a0: 4074 7265 655f 7365 7061 7261 746f 725f  @tree_separator_
+000145b0: 6265 666f 7265 2829 0d0a 2020 2020 4074  before()..    @t
+000145c0: 7265 655f 636f 6e64 6974 696f 6e61 6c28  ree_conditional(
+000145d0: 6c61 6d62 6461 206e 6f64 653a 206e 6f74  lambda node: not
+000145e0: 2069 735f 7265 676d 6172 6b28 6e6f 6465   is_regmark(node
+000145f0: 2929 0d0a 2020 2020 4074 7265 655f 636f  ))..    @tree_co
+00014600: 6e64 6974 696f 6e61 6c5f 7472 7928 6c61  nditional_try(la
+00014610: 6d62 6461 206e 6f64 653a 206e 6f64 652e  mbda node: node.
+00014620: 6361 6e5f 7363 616c 6529 0d0a 2020 2020  can_scale)..    
+00014630: 4074 7265 655f 6f70 6572 6174 696f 6e28  @tree_operation(
+00014640: 0d0a 2020 2020 2020 2020 5f28 2248 6f72  ..        _("Hor
+00014650: 697a 6f6e 7461 6c6c 7922 292c 0d0a 2020  izontally"),..  
+00014660: 2020 2020 2020 6e6f 6465 5f74 7970 653d        node_type=
+00014670: 656c 656d 5f67 726f 7570 5f6e 6f64 6573  elem_group_nodes
+00014680: 2c0d 0a20 2020 2020 2020 2068 656c 703d  ,..        help=
+00014690: 5f28 224d 6972 726f 7220 486f 7269 7a6f  _("Mirror Horizo
+000146a0: 6e74 616c 6c79 2229 2c0d 0a20 2020 2029  ntally"),..    )
+000146b0: 0d0a 2020 2020 6465 6620 6d69 7272 6f72  ..    def mirror
+000146c0: 5f65 6c65 6d28 6e6f 6465 2c20 2a2a 6b77  _elem(node, **kw
+000146d0: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+000146e0: 626f 756e 6473 203d 2073 656c 662e 5f65  bounds = self._e
+000146f0: 6d70 6861 7369 7a65 645f 626f 756e 6473  mphasized_bounds
+00014700: 0d0a 2020 2020 2020 2020 6966 2062 6f75  ..        if bou
+00014710: 6e64 7320 6973 204e 6f6e 653a 0d0a 2020  nds is None:..  
+00014720: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014730: 0d0a 2020 2020 2020 2020 6365 6e74 6572  ..        center
+00014740: 5f78 203d 2028 626f 756e 6473 5b32 5d20  _x = (bounds[2] 
+00014750: 2b20 626f 756e 6473 5b30 5d29 202f 2032  + bounds[0]) / 2
+00014760: 2e30 0d0a 2020 2020 2020 2020 6365 6e74  .0..        cent
+00014770: 6572 5f79 203d 2028 626f 756e 6473 5b33  er_y = (bounds[3
+00014780: 5d20 2b20 626f 756e 6473 5b31 5d29 202f  ] + bounds[1]) /
+00014790: 2032 2e30 0d0a 2020 2020 2020 2020 7365   2.0..        se
+000147a0: 6c66 2866 2273 6361 6c65 202d 3120 3120  lf(f"scale -1 1 
+000147b0: 7b63 656e 7465 725f 787d 207b 6365 6e74  {center_x} {cent
+000147c0: 6572 5f79 7d5c 6e22 290d 0a0d 0a20 2020  er_y}\n")....   
+000147d0: 2040 7472 6565 5f63 6f6e 6469 7469 6f6e   @tree_condition
+000147e0: 616c 286c 616d 6264 6120 6e6f 6465 3a20  al(lambda node: 
+000147f0: 6e6f 7420 6973 5f72 6567 6d61 726b 286e  not is_regmark(n
+00014800: 6f64 6529 290d 0a20 2020 2040 7472 6565  ode))..    @tree
+00014810: 5f73 7562 6d65 6e75 285f 2822 466c 6970  _submenu(_("Flip
+00014820: 2229 290d 0a20 2020 2040 7472 6565 5f63  "))..    @tree_c
+00014830: 6f6e 6469 7469 6f6e 616c 5f74 7279 286c  onditional_try(l
+00014840: 616d 6264 6120 6e6f 6465 3a20 6e6f 6465  ambda node: node
+00014850: 2e63 616e 5f73 6361 6c65 290d 0a20 2020  .can_scale)..   
+00014860: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+00014870: 280d 0a20 2020 2020 2020 205f 2822 5665  (..        _("Ve
+00014880: 7274 6963 616c 6c79 2229 2c0d 0a20 2020  rtically"),..   
+00014890: 2020 2020 206e 6f64 655f 7479 7065 3d65       node_type=e
+000148a0: 6c65 6d5f 6772 6f75 705f 6e6f 6465 732c  lem_group_nodes,
+000148b0: 0d0a 2020 2020 2020 2020 6865 6c70 3d5f  ..        help=_
+000148c0: 2822 466c 6970 2056 6572 7469 6361 6c6c  ("Flip Verticall
+000148d0: 7922 292c 0d0a 2020 2020 290d 0a20 2020  y"),..    )..   
+000148e0: 2064 6566 2066 6c69 705f 656c 656d 286e   def flip_elem(n
+000148f0: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
+00014900: 0a20 2020 2020 2020 2062 6f75 6e64 7320  .        bounds 
+00014910: 3d20 7365 6c66 2e5f 656d 7068 6173 697a  = self._emphasiz
+00014920: 6564 5f62 6f75 6e64 730d 0a20 2020 2020  ed_bounds..     
+00014930: 2020 2069 6620 626f 756e 6473 2069 7320     if bounds is 
+00014940: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00014950: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
+00014960: 2020 2063 656e 7465 725f 7820 3d20 2862     center_x = (b
+00014970: 6f75 6e64 735b 325d 202b 2062 6f75 6e64  ounds[2] + bound
+00014980: 735b 305d 2920 2f20 322e 300d 0a20 2020  s[0]) / 2.0..   
+00014990: 2020 2020 2063 656e 7465 725f 7920 3d20       center_y = 
+000149a0: 2862 6f75 6e64 735b 335d 202b 2062 6f75  (bounds[3] + bou
+000149b0: 6e64 735b 315d 2920 2f20 322e 300d 0a20  nds[1]) / 2.0.. 
+000149c0: 2020 2020 2020 2073 656c 6628 6622 7363         self(f"sc
+000149d0: 616c 6520 3120 2d31 207b 6365 6e74 6572  ale 1 -1 {center
+000149e0: 5f78 7d20 7b63 656e 7465 725f 797d 5c6e  _x} {center_y}\n
+000149f0: 2229 0d0a 0d0a 2020 2020 4074 7265 655f  ")....    @tree_
+00014a00: 636f 6e64 6974 696f 6e61 6c28 6c61 6d62  conditional(lamb
+00014a10: 6461 206e 6f64 653a 206e 6f74 2069 735f  da node: not is_
+00014a20: 7265 676d 6172 6b28 6e6f 6465 2929 0d0a  regmark(node))..
+00014a30: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
+00014a40: 696f 6e61 6c5f 7472 7928 6c61 6d62 6461  ional_try(lambda
+00014a50: 206e 6f64 653a 206e 6f64 652e 6361 6e5f   node: node.can_
+00014a60: 7363 616c 6529 0d0a 2020 2020 4074 7265  scale)..    @tre
+00014a70: 655f 7375 626d 656e 7528 5f28 2253 6361  e_submenu(_("Sca
+00014a80: 6c65 2229 290d 0a20 2020 2040 7472 6565  le"))..    @tree
+00014a90: 5f69 7465 7261 7465 2822 7363 616c 6522  _iterate("scale"
+00014aa0: 2c20 3235 2c20 312c 202d 3129 0d0a 2020  , 25, 1, -1)..  
+00014ab0: 2020 4074 7265 655f 6361 6c63 2822 7363    @tree_calc("sc
+00014ac0: 616c 655f 7065 7263 656e 7422 2c20 6c61  ale_percent", la
+00014ad0: 6d62 6461 2069 3a20 6622 7b28 3630 302e  mbda i: f"{(600.
+00014ae0: 3020 2f20 666c 6f61 7428 6929 293a 2e32  0 / float(i)):.2
+00014af0: 667d 2229 0d0a 2020 2020 4074 7265 655f  f}")..    @tree_
+00014b00: 6f70 6572 6174 696f 6e28 0d0a 2020 2020  operation(..    
+00014b10: 2020 2020 5f28 2253 6361 6c65 207b 7363      _("Scale {sc
+00014b20: 616c 655f 7065 7263 656e 747d 2522 292c  ale_percent}%"),
+00014b30: 0d0a 2020 2020 2020 2020 6e6f 6465 5f74  ..        node_t
+00014b40: 7970 653d 656c 656d 5f67 726f 7570 5f6e  ype=elem_group_n
+00014b50: 6f64 6573 2c0d 0a20 2020 2020 2020 2068  odes,..        h
+00014b60: 656c 703d 5f28 2253 6361 6c65 2045 6c65  elp=_("Scale Ele
+00014b70: 6d65 6e74 2229 2c0d 0a20 2020 2029 0d0a  ment"),..    )..
+00014b80: 2020 2020 6465 6620 7363 616c 655f 656c      def scale_el
+00014b90: 656d 5f61 6d6f 756e 7428 6e6f 6465 2c20  em_amount(node, 
+00014ba0: 7363 616c 652c 202a 2a6b 7761 7267 7329  scale, **kwargs)
+00014bb0: 3a0d 0a20 2020 2020 2020 2073 6361 6c65  :..        scale
+00014bc0: 203d 2036 2e30 202f 2066 6c6f 6174 2873   = 6.0 / float(s
+00014bd0: 6361 6c65 290d 0a20 2020 2020 2020 2062  cale)..        b
+00014be0: 6f75 6e64 7320 3d20 7365 6c66 2e5f 656d  ounds = self._em
+00014bf0: 7068 6173 697a 6564 5f62 6f75 6e64 730d  phasized_bounds.
+00014c00: 0a20 2020 2020 2020 2069 6620 626f 756e  .        if boun
+00014c10: 6473 2069 7320 4e6f 6e65 3a0d 0a20 2020  ds is None:..   
+00014c20: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
+00014c30: 0a20 2020 2020 2020 2063 656e 7465 725f  .        center_
+00014c40: 7820 3d20 2862 6f75 6e64 735b 325d 202b  x = (bounds[2] +
+00014c50: 2062 6f75 6e64 735b 305d 2920 2f20 322e   bounds[0]) / 2.
+00014c60: 300d 0a20 2020 2020 2020 2063 656e 7465  0..        cente
+00014c70: 725f 7920 3d20 2862 6f75 6e64 735b 335d  r_y = (bounds[3]
+00014c80: 202b 2062 6f75 6e64 735b 315d 2920 2f20   + bounds[1]) / 
+00014c90: 322e 300d 0a20 2020 2020 2020 2073 656c  2.0..        sel
+00014ca0: 6628 6622 7363 616c 6520 7b73 6361 6c65  f(f"scale {scale
+00014cb0: 7d20 7b73 6361 6c65 7d20 7b63 656e 7465  } {scale} {cente
+00014cc0: 725f 787d 207b 6365 6e74 6572 5f79 7d5c  r_x} {center_y}\
+00014cd0: 6e22 290d 0a0d 0a20 2020 2023 2040 7472  n")....    # @tr
+00014ce0: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
+00014cf0: 616d 6264 6120 6e6f 6465 3a20 6973 696e  ambda node: isin
+00014d00: 7374 616e 6365 286e 6f64 652e 6f62 6a65  stance(node.obje
+00014d10: 6374 2c20 5356 4745 6c65 6d65 6e74 2929  ct, SVGElement))
+00014d20: 0d0a 2020 2020 4074 7265 655f 636f 6e64  ..    @tree_cond
+00014d30: 6974 696f 6e61 6c28 6c61 6d62 6461 206e  itional(lambda n
+00014d40: 6f64 653a 206e 6f74 2069 735f 7265 676d  ode: not is_regm
+00014d50: 6172 6b28 6e6f 6465 2929 0d0a 2020 2020  ark(node))..    
+00014d60: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
+00014d70: 6c5f 7472 7928 6c61 6d62 6461 206e 6f64  l_try(lambda nod
+00014d80: 653a 206e 6f64 652e 6361 6e5f 726f 7461  e: node.can_rota
+00014d90: 7465 290d 0a20 2020 2040 7472 6565 5f73  te)..    @tree_s
+00014da0: 7562 6d65 6e75 285f 2822 526f 7461 7465  ubmenu(_("Rotate
+00014db0: 2229 290d 0a20 2020 2040 7472 6565 5f76  "))..    @tree_v
+00014dc0: 616c 7565 7328 0d0a 2020 2020 2020 2020  alues(..        
+00014dd0: 2261 6e67 6c65 222c 0d0a 2020 2020 2020  "angle",..      
+00014de0: 2020 280d 0a20 2020 2020 2020 2020 2020    (..           
+00014df0: 2031 3830 2c0d 0a20 2020 2020 2020 2020   180,..         
+00014e00: 2020 2031 3530 2c0d 0a20 2020 2020 2020     150,..       
+00014e10: 2020 2020 2031 3335 2c0d 0a20 2020 2020       135,..     
+00014e20: 2020 2020 2020 2031 3230 2c0d 0a20 2020         120,..   
+00014e30: 2020 2020 2020 2020 2039 302c 0d0a 2020           90,..  
+00014e40: 2020 2020 2020 2020 2020 3630 2c0d 0a20            60,.. 
+00014e50: 2020 2020 2020 2020 2020 2034 352c 0d0a             45,..
+00014e60: 2020 2020 2020 2020 2020 2020 3330 2c0d              30,.
+00014e70: 0a20 2020 2020 2020 2020 2020 2032 302c  .            20,
+00014e80: 0d0a 2020 2020 2020 2020 2020 2020 3135  ..            15
+00014e90: 2c0d 0a20 2020 2020 2020 2020 2020 2031  ,..            1
+00014ea0: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00014eb0: 352c 0d0a 2020 2020 2020 2020 2020 2020  5,..            
+00014ec0: 342c 0d0a 2020 2020 2020 2020 2020 2020  4,..            
+00014ed0: 332c 0d0a 2020 2020 2020 2020 2020 2020  3,..            
+00014ee0: 322c 0d0a 2020 2020 2020 2020 2020 2020  2,..            
+00014ef0: 312c 0d0a 2020 2020 2020 2020 2020 2020  1,..            
+00014f00: 2d31 2c0d 0a20 2020 2020 2020 2020 2020  -1,..           
+00014f10: 202d 322c 0d0a 2020 2020 2020 2020 2020   -2,..          
+00014f20: 2020 2d33 2c0d 0a20 2020 2020 2020 2020    -3,..         
+00014f30: 2020 202d 342c 0d0a 2020 2020 2020 2020     -4,..        
+00014f40: 2020 2020 2d35 2c0d 0a20 2020 2020 2020      -5,..       
+00014f50: 2020 2020 202d 3130 2c0d 0a20 2020 2020       -10,..     
+00014f60: 2020 2020 2020 202d 3135 2c0d 0a20 2020         -15,..   
+00014f70: 2020 2020 2020 2020 202d 3230 2c0d 0a20           -20,.. 
+00014f80: 2020 2020 2020 2020 2020 202d 3330 2c0d             -30,.
+00014f90: 0a20 2020 2020 2020 2020 2020 202d 3435  .            -45
+00014fa0: 2c0d 0a20 2020 2020 2020 2020 2020 202d  ,..            -
+00014fb0: 3630 2c0d 0a20 2020 2020 2020 2020 2020  60,..           
+00014fc0: 202d 3930 2c0d 0a20 2020 2020 2020 2029   -90,..        )
+00014fd0: 2c0d 0a20 2020 2029 0d0a 2020 2020 4074  ,..    )..    @t
+00014fe0: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
+00014ff0: 2252 6f74 6174 6520 7b61 6e67 6c65 7dc2  "Rotate {angle}.
+00015000: b022 292c 206e 6f64 655f 7479 7065 3d65  ."), node_type=e
+00015010: 6c65 6d5f 6772 6f75 705f 6e6f 6465 732c  lem_group_nodes,
+00015020: 2068 656c 703d 2222 290d 0a20 2020 2064   help="")..    d
+00015030: 6566 2072 6f74 6174 655f 656c 656d 5f61  ef rotate_elem_a
+00015040: 6d6f 756e 7428 6e6f 6465 2c20 616e 676c  mount(node, angl
+00015050: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+00015060: 2020 2020 2020 2074 7572 6e73 203d 2066         turns = f
+00015070: 6c6f 6174 2861 6e67 6c65 2920 2f20 3336  loat(angle) / 36
+00015080: 302e 300d 0a20 2020 2020 2020 2062 6f75  0.0..        bou
+00015090: 6e64 7320 3d20 7365 6c66 2e5f 656d 7068  nds = self._emph
+000150a0: 6173 697a 6564 5f62 6f75 6e64 730d 0a20  asized_bounds.. 
+000150b0: 2020 2020 2020 2069 6620 626f 756e 6473         if bounds
+000150c0: 2069 7320 4e6f 6e65 3a0d 0a20 2020 2020   is None:..     
+000150d0: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
+000150e0: 2020 2020 2020 2063 656e 7465 725f 7820         center_x 
+000150f0: 3d20 2862 6f75 6e64 735b 325d 202b 2062  = (bounds[2] + b
+00015100: 6f75 6e64 735b 305d 2920 2f20 322e 300d  ounds[0]) / 2.0.
+00015110: 0a20 2020 2020 2020 2063 656e 7465 725f  .        center_
+00015120: 7920 3d20 2862 6f75 6e64 735b 335d 202b  y = (bounds[3] +
+00015130: 2062 6f75 6e64 735b 315d 2920 2f20 322e   bounds[1]) / 2.
+00015140: 300d 0a20 2020 2020 2020 2073 656c 6628  0..        self(
+00015150: 6622 726f 7461 7465 207b 7475 726e 737d  f"rotate {turns}
+00015160: 7475 726e 207b 6365 6e74 6572 5f78 7d20  turn {center_x} 
+00015170: 7b63 656e 7465 725f 797d 5c6e 2229 0d0a  {center_y}\n")..
+00015180: 2020 2020 2020 2020 7365 6c66 2e73 6967          self.sig
+00015190: 6e61 6c28 2265 7874 2d6d 6f64 6966 6965  nal("ext-modifie
+000151a0: 6422 290d 0a0d 0a20 2020 2040 7472 6565  d")....    @tree
+000151b0: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
+000151c0: 6264 6120 6e6f 6465 3a20 6e6f 7420 6973  bda node: not is
+000151d0: 5f72 6567 6d61 726b 286e 6f64 6529 290d  _regmark(node)).
+000151e0: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
+000151f0: 7469 6f6e 616c 286c 616d 6264 6120 6e6f  tional(lambda no
+00015200: 6465 3a20 6861 735f 6368 616e 6765 7328  de: has_changes(
+00015210: 6e6f 6465 2929 0d0a 2020 2020 4074 7265  node))..    @tre
+00015220: 655f 636f 6e64 6974 696f 6e61 6c5f 7472  e_conditional_tr
+00015230: 7928 6c61 6d62 6461 206e 6f64 653a 206e  y(lambda node: n
+00015240: 6f64 652e 6361 6e5f 6d6f 6469 6679 290d  ode.can_modify).
+00015250: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
+00015260: 7469 6f6e 285f 2822 5265 6966 7920 5573  tion(_("Reify Us
+00015270: 6572 2043 6861 6e67 6573 2229 2c20 6e6f  er Changes"), no
+00015280: 6465 5f74 7970 653d 656c 656d 5f67 726f  de_type=elem_gro
+00015290: 7570 5f6e 6f64 6573 2c20 6865 6c70 3d22  up_nodes, help="
+000152a0: 2229 0d0a 2020 2020 6465 6620 7265 6966  ")..    def reif
+000152b0: 795f 656c 656d 5f63 6861 6e67 6573 286e  y_elem_changes(n
+000152c0: 6f64 652c 202a 2a6b 7761 7267 7329 3a0d  ode, **kwargs):.
+000152d0: 0a20 2020 2020 2020 2073 656c 6628 2272  .        self("r
+000152e0: 6569 6679 5c6e 2229 0d0a 2020 2020 2020  eify\n")..      
+000152f0: 2020 7365 6c66 2e73 6967 6e61 6c28 2265    self.signal("e
+00015300: 7874 2d6d 6f64 6966 6965 6422 290d 0a0d  xt-modified")...
+00015310: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
+00015320: 7469 6f6e 616c 286c 616d 6264 6120 6e6f  tional(lambda no
+00015330: 6465 3a20 6e6f 7420 6973 5f72 6567 6d61  de: not is_regma
+00015340: 726b 286e 6f64 6529 290d 0a20 2020 2040  rk(node))..    @
+00015350: 7472 6565 5f63 6f6e 6469 7469 6f6e 616c  tree_conditional
+00015360: 5f74 7279 286c 616d 6264 6120 6e6f 6465  _try(lambda node
+00015370: 3a20 6e6f 6465 2e63 616e 5f6d 6f64 6966  : node.can_modif
+00015380: 7929 0d0a 2020 2020 4074 7265 655f 6f70  y)..    @tree_op
+00015390: 6572 6174 696f 6e28 5f28 2242 7265 616b  eration(_("Break
+000153a0: 2053 7562 7061 7468 7322 292c 206e 6f64   Subpaths"), nod
+000153b0: 655f 7479 7065 3d22 656c 656d 2070 6174  e_type="elem pat
+000153c0: 6822 2c20 6865 6c70 3d22 2229 0d0a 2020  h", help="")..  
+000153d0: 2020 6465 6620 6272 6561 6b5f 7375 6270    def break_subp
+000153e0: 6174 685f 656c 656d 286e 6f64 652c 202a  ath_elem(node, *
+000153f0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00015400: 2020 2073 656c 6628 2265 6c65 6d65 6e74     self("element
+00015410: 2073 7562 7061 7468 5c6e 2229 0d0a 0d0a   subpath\n")....
+00015420: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
+00015430: 696f 6e61 6c28 6c61 6d62 6461 206e 6f64  ional(lambda nod
+00015440: 653a 206e 6f74 2069 735f 7265 676d 6172  e: not is_regmar
+00015450: 6b28 6e6f 6465 2929 0d0a 2020 2020 4074  k(node))..    @t
+00015460: 7265 655f 636f 6e64 6974 696f 6e61 6c28  ree_conditional(
+00015470: 6c61 6d62 6461 206e 6f64 653a 2068 6173  lambda node: has
+00015480: 5f63 6861 6e67 6573 286e 6f64 6529 290d  _changes(node)).
+00015490: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
+000154a0: 7469 6f6e 616c 5f74 7279 286c 616d 6264  tional_try(lambd
+000154b0: 6120 6e6f 6465 3a20 6e6f 6465 2e63 616e  a node: node.can
+000154c0: 5f6d 6f64 6966 7929 0d0a 2020 2020 4074  _modify)..    @t
+000154d0: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
+000154e0: 2252 6573 6574 2075 7365 7220 6368 616e  "Reset user chan
+000154f0: 6765 7322 292c 206e 6f64 655f 7479 7065  ges"), node_type
+00015500: 3d65 6c65 6d5f 6772 6f75 705f 6e6f 6465  =elem_group_node
+00015510: 732c 2068 656c 703d 2222 290d 0a20 2020  s, help="")..   
+00015520: 2064 6566 2072 6573 6574 5f75 7365 725f   def reset_user_
+00015530: 6368 616e 6765 7328 6e6f 6465 2c20 636f  changes(node, co
+00015540: 7069 6573 3d31 2c20 2a2a 6b77 6172 6773  pies=1, **kwargs
+00015550: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00015560: 2822 7265 7365 745c 6e22 290d 0a20 2020  ("reset\n")..   
+00015570: 2020 2020 2073 656c 662e 7369 676e 616c       self.signal
+00015580: 2822 6578 742d 6d6f 6469 6669 6564 2229  ("ext-modified")
+00015590: 0d0a 0d0a 2020 2020 4074 7265 655f 6f70  ....    @tree_op
+000155a0: 6572 6174 696f 6e28 0d0a 2020 2020 2020  eration(..      
+000155b0: 2020 5f28 224d 6572 6765 2069 7465 6d73    _("Merge items
+000155c0: 2229 2c0d 0a20 2020 2020 2020 206e 6f64  "),..        nod
+000155d0: 655f 7479 7065 3d22 6772 6f75 7022 2c0d  e_type="group",.
+000155e0: 0a20 2020 2020 2020 2068 656c 703d 5f28  .        help=_(
+000155f0: 224d 6572 6765 2074 6869 7320 6e6f 6465  "Merge this node
+00015600: 2773 2063 6869 6c64 7265 6e20 696e 746f  's children into
+00015610: 2031 2070 6174 682e 2229 2c0d 0a20 2020   1 path."),..   
+00015620: 2029 0d0a 2020 2020 6465 6620 6d65 7267   )..    def merg
+00015630: 655f 656c 656d 656e 7473 286e 6f64 652c  e_elements(node,
+00015640: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+00015650: 2020 2020 2073 656c 6628 2265 6c65 6d65       self("eleme
+00015660: 6e74 206d 6572 6765 5c6e 2229 0d0a 2020  nt merge\n")..  
+00015670: 2020 2020 2020 2320 4973 2074 6865 2067        # Is the g
+00015680: 726f 7570 206e 6f77 2065 6d70 7479 3f20  roup now empty? 
+00015690: 2d2d 3e20 6465 6c65 7465 0d0a 2020 2020  --> delete..    
+000156a0: 2020 2020 6966 206c 656e 286e 6f64 652e      if len(node.
+000156b0: 6368 696c 6472 656e 2920 3d3d 2030 3a0d  children) == 0:.
+000156c0: 0a20 2020 2020 2020 2020 2020 206e 6f64  .            nod
+000156d0: 652e 7265 6d6f 7665 5f6e 6f64 6528 290d  e.remove_node().
+000156e0: 0a0d 0a20 2020 2040 7472 6565 5f63 6f6e  ...    @tree_con
+000156f0: 6469 7469 6f6e 616c 286c 616d 6264 6120  ditional(lambda 
+00015700: 6e6f 6465 3a20 6e6f 6465 2e6c 6f63 6b29  node: node.lock)
+00015710: 0d0a 2020 2020 4074 7265 655f 7365 7061  ..    @tree_sepa
+00015720: 7261 746f 725f 6265 666f 7265 2829 0d0a  rator_before()..
+00015730: 2020 2020 4074 7265 655f 6f70 6572 6174      @tree_operat
+00015740: 696f 6e28 0d0a 2020 2020 2020 2020 5f28  ion(..        _(
+00015750: 2255 6e6c 6f63 6b20 656c 656d 656e 742c  "Unlock element,
+00015760: 2061 6c6c 6f77 7320 6d61 6e69 7075 6c61   allows manipula
+00015770: 7469 6f6e 2229 2c20 6e6f 6465 5f74 7970  tion"), node_typ
+00015780: 653d 656c 656d 5f6e 6f64 6573 2c20 6865  e=elem_nodes, he
+00015790: 6c70 3d22 220d 0a20 2020 2029 0d0a 2020  lp=""..    )..  
+000157a0: 2020 6465 6620 656c 656d 656e 745f 756e    def element_un
+000157b0: 6c6f 636b 5f6d 616e 6970 756c 6174 696f  lock_manipulatio
+000157c0: 6e73 286e 6f64 652c 202a 2a6b 7761 7267  ns(node, **kwarg
+000157d0: 7329 3a0d 0a20 2020 2020 2020 2073 656c  s):..        sel
+000157e0: 6628 2265 6c65 6d65 6e74 2075 6e6c 6f63  f("element unloc
+000157f0: 6b5c 6e22 290d 0a0d 0a20 2020 2040 7472  k\n")....    @tr
+00015800: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
+00015810: 616d 6264 6120 6e6f 6465 3a20 6e6f 7420  ambda node: not 
+00015820: 6e6f 6465 2e6c 6f63 6b29 0d0a 2020 2020  node.lock)..    
+00015830: 4074 7265 655f 7365 7061 7261 746f 725f  @tree_separator_
+00015840: 6265 666f 7265 2829 0d0a 2020 2020 4074  before()..    @t
+00015850: 7265 655f 6f70 6572 6174 696f 6e28 0d0a  ree_operation(..
+00015860: 2020 2020 2020 2020 5f28 224c 6f63 6b20          _("Lock 
+00015870: 656c 656d 656e 7473 2c20 7072 6576 656e  elements, preven
+00015880: 7473 206d 616e 6970 756c 6174 696f 6e73  ts manipulations
+00015890: 2229 2c20 6e6f 6465 5f74 7970 653d 656c  "), node_type=el
+000158a0: 656d 5f6e 6f64 6573 2c20 6865 6c70 3d22  em_nodes, help="
+000158b0: 220d 0a20 2020 2029 0d0a 2020 2020 6465  "..    )..    de
+000158c0: 6620 656c 656d 656e 745f 6c6f 636b 5f6d  f element_lock_m
+000158d0: 616e 6970 756c 6174 696f 6e73 286e 6f64  anipulations(nod
+000158e0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+000158f0: 2020 2020 2020 2073 656c 6628 2265 6c65         self("ele
+00015900: 6d65 6e74 206c 6f63 6b5c 6e22 290d 0a0d  ment lock\n")...
+00015910: 0a20 2020 2040 7472 6565 5f63 6f6e 6469  .    @tree_condi
+00015920: 7469 6f6e 616c 286c 616d 6264 6120 6e6f  tional(lambda no
+00015930: 6465 3a20 6e6f 6465 2e74 7970 6520 3d3d  de: node.type ==
+00015940: 2022 6272 616e 6368 2072 6567 2229 0d0a   "branch reg")..
+00015950: 2020 2020 4074 7265 655f 7365 7061 7261      @tree_separa
+00015960: 746f 725f 6265 666f 7265 2829 0d0a 2020  tor_before()..  
+00015970: 2020 4074 7265 655f 6f70 6572 6174 696f    @tree_operatio
+00015980: 6e28 5f28 2254 6f67 676c 6520 7669 7369  n(_("Toggle visi
+00015990: 6269 6c69 7479 206f 6620 7265 676d 6172  bility of regmar
+000159a0: 6b73 2229 2c20 6e6f 6465 5f74 7970 653d  ks"), node_type=
+000159b0: 2262 7261 6e63 6820 7265 6722 2c20 6865  "branch reg", he
+000159c0: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+000159d0: 746f 6767 6c65 5f76 6973 6962 696c 6974  toggle_visibilit
+000159e0: 7928 6e6f 6465 2c20 2a2a 6b77 6172 6773  y(node, **kwargs
+000159f0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00015a00: 2e73 6967 6e61 6c28 2274 6f67 676c 655f  .signal("toggle_
+00015a10: 7265 676d 6172 6b73 2229 0d0a 0d0a 2020  regmarks")....  
+00015a20: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
+00015a30: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
+00015a40: 2069 735f 7265 676d 6172 6b28 6e6f 6465   is_regmark(node
+00015a50: 2929 0d0a 2020 2020 4074 7265 655f 7365  ))..    @tree_se
+00015a60: 7061 7261 746f 725f 6265 666f 7265 2829  parator_before()
+00015a70: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+00015a80: 6174 696f 6e28 5f28 224d 6f76 6520 6261  ation(_("Move ba
+00015a90: 636b 2074 6f20 656c 656d 656e 7473 2229  ck to elements")
+00015aa0: 2c20 6e6f 6465 5f74 7970 653d 656c 656d  , node_type=elem
+00015ab0: 5f67 726f 7570 5f6e 6f64 6573 2c20 6865  _group_nodes, he
+00015ac0: 6c70 3d22 2229 0d0a 2020 2020 6465 6620  lp="")..    def 
+00015ad0: 6d6f 7665 5f62 6163 6b28 6e6f 6465 2c20  move_back(node, 
+00015ae0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+00015af0: 2020 2020 2320 4472 6167 2061 6e64 2044      # Drag and D
+00015b00: 726f 700d 0a20 2020 2020 2020 2077 6974  rop..        wit
+00015b10: 6820 7365 6c66 2e73 7461 7469 6328 226d  h self.static("m
+00015b20: 6f76 655f 6261 636b 2229 3a0d 0a20 2020  ove_back"):..   
+00015b30: 2020 2020 2020 2020 2073 6967 6e61 6c5f           signal_
+00015b40: 6e65 6564 6564 203d 2046 616c 7365 0d0a  needed = False..
+00015b50: 2020 2020 2020 2020 2020 2020 6472 6f70              drop
+00015b60: 5f6e 6f64 6520 3d20 7365 6c66 2e65 6c65  _node = self.ele
+00015b70: 6d5f 6272 616e 6368 0d0a 2020 2020 2020  m_branch..      
+00015b80: 2020 2020 2020 6461 7461 203d 206c 6973        data = lis
+00015b90: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+00015ba0: 2066 6f72 2069 7465 6d20 696e 206c 6973   for item in lis
+00015bb0: 7428 7365 6c66 2e72 6567 6d61 726b 7328  t(self.regmarks(
+00015bc0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00015bd0: 2020 2020 2069 6620 6974 656d 2e73 656c       if item.sel
+00015be0: 6563 7465 643a 0d0a 2020 2020 2020 2020  ected:..        
+00015bf0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00015c00: 2e61 7070 656e 6428 6974 656d 290d 0a20  .append(item).. 
+00015c10: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00015c20: 7465 6d20 696e 2064 6174 613a 0d0a 2020  tem in data:..  
+00015c30: 2020 2020 2020 2020 2020 2020 2020 6472                dr
+00015c40: 6f70 5f6e 6f64 652e 6472 6f70 2869 7465  op_node.drop(ite
+00015c50: 6d29 0d0a 2020 2020 2020 2020 2020 2020  m)..            
+00015c60: 2020 2020 7369 676e 616c 5f6e 6565 6465      signal_neede
+00015c70: 6420 3d20 5472 7565 0d0a 0d0a 2020 2020  d = True....    
+00015c80: 4074 7265 655f 636f 6e64 6974 696f 6e61  @tree_conditiona
+00015c90: 6c28 6c61 6d62 6461 206e 6f64 653a 206e  l(lambda node: n
+00015ca0: 6f74 2069 735f 7265 676d 6172 6b28 6e6f  ot is_regmark(no
+00015cb0: 6465 2929 0d0a 2020 2020 4074 7265 655f  de))..    @tree_
+00015cc0: 7365 7061 7261 746f 725f 6265 666f 7265  separator_before
+00015cd0: 2829 0d0a 2020 2020 4074 7265 655f 6f70  ()..    @tree_op
+00015ce0: 6572 6174 696f 6e28 5f28 224d 6f76 6520  eration(_("Move 
+00015cf0: 746f 2072 6567 6d61 726b 7322 292c 206e  to regmarks"), n
+00015d00: 6f64 655f 7479 7065 3d65 6c65 6d5f 6772  ode_type=elem_gr
+00015d10: 6f75 705f 6e6f 6465 732c 2068 656c 703d  oup_nodes, help=
+00015d20: 2222 290d 0a20 2020 2064 6566 206d 6f76  "")..    def mov
+00015d30: 655f 746f 5f72 6567 6d61 726b 286e 6f64  e_to_regmark(nod
+00015d40: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+00015d50: 2020 2020 2020 2023 2044 7261 6720 616e         # Drag an
+00015d60: 6420 4472 6f70 0d0a 2020 2020 2020 2020  d Drop..        
+00015d70: 7769 7468 2073 656c 662e 7374 6174 6963  with self.static
+00015d80: 2822 6d6f 7665 5f74 6f5f 7265 6722 293a  ("move_to_reg"):
+00015d90: 0d0a 2020 2020 2020 2020 2020 2020 6472  ..            dr
+00015da0: 6f70 5f6e 6f64 6520 3d20 7365 6c66 2e72  op_node = self.r
+00015db0: 6567 5f62 7261 6e63 680d 0a20 2020 2020  eg_branch..     
+00015dc0: 2020 2020 2020 2064 6174 6120 3d20 6c69         data = li
+00015dd0: 7374 2829 0d0a 2020 2020 2020 2020 2020  st()..          
+00015de0: 2020 666f 7220 6974 656d 2069 6e20 6c69    for item in li
+00015df0: 7374 2873 656c 662e 656c 656d 735f 6e6f  st(self.elems_no
+00015e00: 6465 7328 2929 3a0d 0a20 2020 2020 2020  des()):..       
+00015e10: 2020 2020 2020 2020 2069 6620 6974 656d           if item
+00015e20: 2e73 656c 6563 7465 643a 0d0a 2020 2020  .selected:..    
+00015e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e40: 6461 7461 2e61 7070 656e 6428 6974 656d  data.append(item
+00015e50: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00015e60: 6f72 2069 7465 6d20 696e 2064 6174 613a  or item in data:
+00015e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015e80: 2020 2320 4e6f 2075 7365 6361 7365 2066    # No usecase f
+00015e90: 6f72 2068 6176 696e 6720 6120 6c6f 636b  or having a lock
+00015ea0: 6564 2072 6567 6d61 726b 2065 6c65 6d65  ed regmark eleme
+00015eb0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
+00015ec0: 2020 2020 6966 2068 6173 6174 7472 2869      if hasattr(i
+00015ed0: 7465 6d2c 2022 6c6f 636b 2229 3a0d 0a20  tem, "lock"):.. 
+00015ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ef0: 2020 2069 7465 6d2e 6c6f 636b 203d 2046     item.lock = F
+00015f00: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00015f10: 2020 2020 2020 6472 6f70 5f6e 6f64 652e        drop_node.
+00015f20: 6472 6f70 2869 7465 6d29 0d0a 0d0a 2020  drop(item)....  
+00015f30: 2020 4074 7265 655f 636f 6e64 6974 696f    @tree_conditio
+00015f40: 6e61 6c28 6c61 6d62 6461 206e 6f64 653a  nal(lambda node:
+00015f50: 2069 735f 7265 676d 6172 6b28 6e6f 6465   is_regmark(node
+00015f60: 2929 0d0a 2020 2020 4074 7265 655f 7365  ))..    @tree_se
+00015f70: 7061 7261 746f 725f 6265 666f 7265 2829  parator_before()
+00015f80: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+00015f90: 6174 696f 6e28 5f28 2243 7265 6174 6520  ation(_("Create 
+00015fa0: 706c 6163 656d 656e 7422 292c 206e 6f64  placement"), nod
+00015fb0: 655f 7479 7065 3d65 6c65 6d5f 6e6f 6465  e_type=elem_node
+00015fc0: 732c 2068 656c 703d 2222 290d 0a20 2020  s, help="")..   
+00015fd0: 2064 6566 2072 6567 6d61 726b 5f61 735f   def regmark_as_
+00015fe0: 706c 6163 656d 656e 7428 6e6f 6465 2c20  placement(node, 
+00015ff0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+00016000: 2020 2020 6966 206e 6f64 6520 6973 204e      if node is N
+00016010: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00016020: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
+00016030: 2020 6966 2068 6173 6174 7472 286e 6f64    if hasattr(nod
+00016040: 652c 2022 7061 7468 2229 3a0d 0a20 2020  e, "path"):..   
+00016050: 2020 2020 2020 2020 2062 6220 3d20 6e6f           bb = no
+00016060: 6465 2e70 6174 682e 6262 6f78 2874 7261  de.path.bbox(tra
+00016070: 6e73 666f 726d 6564 3d46 616c 7365 290d  nsformed=False).
+00016080: 0a20 2020 2020 2020 2065 6c69 6620 6861  .        elif ha
+00016090: 7361 7474 7228 6e6f 6465 2c20 2273 6861  sattr(node, "sha
+000160a0: 7065 2229 3a0d 0a20 2020 2020 2020 2020  pe"):..         
+000160b0: 2020 2062 6220 3d20 6e6f 6465 2e73 6861     bb = node.sha
+000160c0: 7065 2e62 626f 7828 7472 616e 7366 6f72  pe.bbox(transfor
+000160d0: 6d65 643d 4661 6c73 6529 0d0a 2020 2020  med=False)..    
+000160e0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000160f0: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
+00016100: 2020 2020 2020 2069 6620 6262 2069 7320         if bb is 
+00016110: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00016120: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
+00016130: 2020 2078 203d 2062 625b 305d 0d0a 2020     x = bb[0]..  
+00016140: 2020 2020 2020 7920 3d20 6262 5b31 5d0d        y = bb[1].
+00016150: 0a20 2020 2020 2020 2063 6f72 6e65 7220  .        corner 
+00016160: 3d20 300d 0a20 2020 2020 2020 2074 7279  = 0..        try
+00016170: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00016180: 6f74 6174 696f 6e20 3d20 6e6f 6465 2e6d  otation = node.m
+00016190: 6174 7269 782e 726f 7461 7469 6f6e 2e61  atrix.rotation.a
+000161a0: 735f 7261 6469 616e 730d 0a20 2020 2020  s_radians..     
+000161b0: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
+000161c0: 7574 6545 7272 6f72 3a0d 0a20 2020 2020  uteError:..     
+000161d0: 2020 2020 2020 2072 6f74 6174 696f 6e20         rotation 
+000161e0: 3d20 300d 0a20 2020 2020 2020 2070 7420  = 0..        pt 
+000161f0: 3d20 6e6f 6465 2e6d 6174 7269 782e 706f  = node.matrix.po
+00016200: 696e 745f 696e 5f6d 6174 7269 785f 7370  int_in_matrix_sp
+00016210: 6163 6528 506f 696e 7428 6262 5b30 5d2c  ace(Point(bb[0],
+00016220: 2062 625b 315d 2929 0d0a 2020 2020 2020   bb[1]))..      
+00016230: 2020 7820 3d20 7074 2e78 0d0a 2020 2020    x = pt.x..    
+00016240: 2020 2020 7920 3d20 7074 2e79 0d0a 2020      y = pt.y..  
+00016250: 2020 2020 2020 706c 6163 655f 6e6f 6465        place_node
+00016260: 203d 2073 656c 662e 6f70 5f62 7261 6e63   = self.op_branc
+00016270: 682e 6164 6428 0d0a 2020 2020 2020 2020  h.add(..        
+00016280: 2020 2020 7479 7065 3d22 706c 6163 6520      type="place 
+00016290: 706f 696e 7422 2c20 783d 782c 2079 3d79  point", x=x, y=y
+000162a0: 2c20 636f 726e 6572 3d63 6f72 6e65 722c  , corner=corner,
+000162b0: 2072 6f74 6174 696f 6e3d 726f 7461 7469   rotation=rotati
+000162c0: 6f6e 0d0a 2020 2020 2020 2020 290d 0a20  on..        ).. 
+000162d0: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+000162e0: 616c 2822 7265 6672 6573 685f 7363 656e  al("refresh_scen
+000162f0: 6522 2c20 2253 6365 6e65 2229 0d0a 0d0a  e", "Scene")....
+00016300: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
+00016310: 696f 6e61 6c28 6c61 6d62 6461 206e 6f64  ional(lambda nod
+00016320: 653a 2069 735f 7265 676d 6172 6b28 6e6f  e: is_regmark(no
+00016330: 6465 2929 0d0a 2020 2020 4074 7265 655f  de))..    @tree_
+00016340: 7375 626d 656e 7528 5f28 2254 6f67 676c  submenu(_("Toggl
+00016350: 6520 4d61 676e 6574 2d4c 696e 6573 2229  e Magnet-Lines")
+00016360: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+00016370: 7261 7469 6f6e 285f 2822 4172 6f75 6e64  ration(_("Around
+00016380: 2062 6f72 6465 7222 292c 206e 6f64 655f   border"), node_
+00016390: 7479 7065 3d65 6c65 6d5f 6772 6f75 705f  type=elem_group_
+000163a0: 6e6f 6465 732c 2068 656c 703d 2222 290d  nodes, help="").
+000163b0: 0a20 2020 2064 6566 2072 6567 6d61 726b  .    def regmark
+000163c0: 5f74 6f5f 6d61 676e 6574 5f31 286e 6f64  _to_magnet_1(nod
+000163d0: 652c 202a 2a6b 7761 7267 7329 3a0d 0a20  e, **kwargs):.. 
+000163e0: 2020 2020 2020 2069 6620 6e6f 6465 2069         if node i
+000163f0: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00016400: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00016410: 2020 2020 2069 6620 6e6f 7420 6861 7361       if not hasa
+00016420: 7474 7228 6e6f 6465 2c20 2262 6f75 6e64  ttr(node, "bound
+00016430: 7322 293a 0d0a 2020 2020 2020 2020 2020  s"):..          
+00016440: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
+00016450: 2020 7365 6c66 2e73 6967 6e61 6c28 226d    self.signal("m
+00016460: 6167 6e65 745f 6765 6e22 2c20 2822 6f75  agnet_gen", ("ou
+00016470: 7465 7222 2c20 6e6f 6465 2929 0d0a 0d0a  ter", node))....
+00016480: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
+00016490: 696f 6e61 6c28 6c61 6d62 6461 206e 6f64  ional(lambda nod
+000164a0: 653a 2069 735f 7265 676d 6172 6b28 6e6f  e: is_regmark(no
+000164b0: 6465 2929 0d0a 2020 2020 4074 7265 655f  de))..    @tree_
+000164c0: 7375 626d 656e 7528 5f28 2254 6f67 676c  submenu(_("Toggl
+000164d0: 6520 4d61 676e 6574 2d4c 696e 6573 2229  e Magnet-Lines")
+000164e0: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+000164f0: 7261 7469 6f6e 285f 2822 4174 2063 656e  ration(_("At cen
+00016500: 7465 7222 292c 206e 6f64 655f 7479 7065  ter"), node_type
+00016510: 3d65 6c65 6d5f 6772 6f75 705f 6e6f 6465  =elem_group_node
+00016520: 732c 2068 656c 703d 2222 290d 0a20 2020  s, help="")..   
+00016530: 2064 6566 2072 6567 6d61 726b 5f74 6f5f   def regmark_to_
+00016540: 6d61 676e 6574 5f32 286e 6f64 652c 202a  magnet_2(node, *
+00016550: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00016560: 2020 2069 6620 6e6f 6465 2069 7320 4e6f     if node is No
+00016570: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00016580: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
+00016590: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
+000165a0: 6e6f 6465 2c20 2262 6f75 6e64 7322 293a  node, "bounds"):
+000165b0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000165c0: 7475 726e 0d0a 2020 2020 2020 2020 7365  turn..        se
+000165d0: 6c66 2e73 6967 6e61 6c28 226d 6167 6e65  lf.signal("magne
+000165e0: 745f 6765 6e22 2c20 2822 6365 6e74 6572  t_gen", ("center
+000165f0: 222c 206e 6f64 6529 290d 0a0d 0a20 2020  ", node))....   
+00016600: 2023 2040 7472 6565 5f63 6f6e 6469 7469   # @tree_conditi
+00016610: 6f6e 616c 286c 616d 6264 6120 6e6f 6465  onal(lambda node
+00016620: 3a20 6e6f 7420 6e6f 6465 2e6c 6f63 6b29  : not node.lock)
+00016630: 0d0a 2020 2020 2320 4074 7265 655f 636f  ..    # @tree_co
+00016640: 6e64 6974 696f 6e61 6c5f 7472 7928 6c61  nditional_try(la
+00016650: 6d62 6461 206e 6f64 653a 206e 6f74 206e  mbda node: not n
+00016660: 6f64 652e 6c6f 636b 290d 0a20 2020 2023  ode.lock)..    #
+00016670: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+00016680: 285f 2822 4163 7475 616c 697a 6520 7069  (_("Actualize pi
+00016690: 7865 6c73 2229 2c20 6e6f 6465 5f74 7970  xels"), node_typ
+000166a0: 653d 2265 6c65 6d20 696d 6167 6522 2c20  e="elem image", 
+000166b0: 6865 6c70 3d22 2229 0d0a 2020 2020 2320  help="")..    # 
+000166c0: 6465 6620 696d 6167 655f 6163 7475 616c  def image_actual
+000166d0: 697a 655f 7069 7865 6c73 286e 6f64 652c  ize_pixels(node,
+000166e0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+000166f0: 2023 2020 2020 2073 656c 6628 2269 6d61   #     self("ima
+00016700: 6765 2072 6573 616d 706c 655c 6e22 290d  ge resample\n").
+00016710: 0a0d 0a20 2020 2040 7472 6565 5f63 6f6e  ...    @tree_con
+00016720: 6469 7469 6f6e 616c 286c 616d 6264 6120  ditional(lambda 
+00016730: 6e6f 6465 3a20 6e6f 7420 6e6f 6465 2e6c  node: not node.l
+00016740: 6f63 6b29 0d0a 2020 2020 4074 7265 655f  ock)..    @tree_
+00016750: 7375 626d 656e 7528 5f28 225a 2d64 6570  submenu(_("Z-dep
+00016760: 7468 2064 6976 6964 6522 2929 0d0a 2020  th divide"))..  
+00016770: 2020 4074 7265 655f 6974 6572 6174 6528    @tree_iterate(
+00016780: 2264 6976 6964 6522 2c20 322c 2031 3029  "divide", 2, 10)
+00016790: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+000167a0: 6174 696f 6e28 5f28 2244 6976 6964 6520  ation(_("Divide 
+000167b0: 696e 746f 207b 6469 7669 6465 7d20 696d  into {divide} im
+000167c0: 6167 6573 2229 2c20 6e6f 6465 5f74 7970  ages"), node_typ
+000167d0: 653d 2265 6c65 6d20 696d 6167 6522 2c20  e="elem image", 
+000167e0: 6865 6c70 3d22 2229 0d0a 2020 2020 6465  help="")..    de
+000167f0: 6620 696d 6167 655f 7a64 6570 7468 286e  f image_zdepth(n
+00016800: 6f64 652c 2064 6976 6964 653d 312c 202a  ode, divide=1, *
+00016810: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00016820: 2020 2069 6620 6e6f 6465 2e69 6d61 6765     if node.image
+00016830: 2e6d 6f64 6520 213d 2022 5247 4241 223a  .mode != "RGBA":
+00016840: 0d0a 2020 2020 2020 2020 2020 2020 6e6f  ..            no
+00016850: 6465 2e69 6d61 6765 203d 206e 6f64 652e  de.image = node.
+00016860: 696d 6167 652e 636f 6e76 6572 7428 2252  image.convert("R
+00016870: 4742 4122 290d 0a20 2020 2020 2020 2062  GBA")..        b
+00016880: 616e 6420 3d20 3235 3520 2f20 6469 7669  and = 255 / divi
+00016890: 6465 0d0a 2020 2020 2020 2020 666f 7220  de..        for 
+000168a0: 6920 696e 2072 616e 6765 2830 2c20 6469  i in range(0, di
+000168b0: 7669 6465 293a 0d0a 2020 2020 2020 2020  vide):..        
+000168c0: 2020 2020 7468 7265 7368 6f6c 645f 6d69      threshold_mi
+000168d0: 6e20 3d20 6920 2a20 6261 6e64 0d0a 2020  n = i * band..  
+000168e0: 2020 2020 2020 2020 2020 7468 7265 7368            thresh
+000168f0: 6f6c 645f 6d61 7820 3d20 7468 7265 7368  old_max = thresh
+00016900: 6f6c 645f 6d69 6e20 2b20 6261 6e64 0d0a  old_min + band..
+00016910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016920: 2866 2269 6d61 6765 2074 6872 6573 686f  (f"image thresho
+00016930: 6c64 207b 7468 7265 7368 6f6c 645f 6d69  ld {threshold_mi
+00016940: 6e7d 207b 7468 7265 7368 6f6c 645f 6d61  n} {threshold_ma
+00016950: 787d 5c6e 2229 0d0a 0d0a 2020 2020 4074  x}\n")....    @t
+00016960: 7265 655f 636f 6e64 6974 696f 6e61 6c28  ree_conditional(
+00016970: 6c61 6d62 6461 206e 6f64 653a 206e 6f64  lambda node: nod
+00016980: 652e 6c6f 636b 290d 0a20 2020 2040 7472  e.lock)..    @tr
+00016990: 6565 5f73 7562 6d65 6e75 285f 2822 496d  ee_submenu(_("Im
+000169a0: 6167 6522 2929 0d0a 2020 2020 4074 7265  age"))..    @tre
+000169b0: 655f 6f70 6572 6174 696f 6e28 5f28 2255  e_operation(_("U
+000169c0: 6e6c 6f63 6b20 6d61 6e69 7075 6c61 7469  nlock manipulati
+000169d0: 6f6e 7322 292c 206e 6f64 655f 7479 7065  ons"), node_type
+000169e0: 3d22 656c 656d 2069 6d61 6765 222c 2068  ="elem image", h
+000169f0: 656c 703d 2222 290d 0a20 2020 2064 6566  elp="")..    def
+00016a00: 2069 6d61 6765 5f75 6e6c 6f63 6b5f 6d61   image_unlock_ma
+00016a10: 6e69 7075 6c61 7469 6f6e 7328 6e6f 6465  nipulations(node
+00016a20: 2c20 2a2a 6b77 6172 6773 293a 0d0a 2020  , **kwargs):..  
+00016a30: 2020 2020 2020 7365 6c66 2822 696d 6167        self("imag
+00016a40: 6520 756e 6c6f 636b 5c6e 2229 0d0a 0d0a  e unlock\n")....
+00016a50: 2020 2020 4074 7265 655f 636f 6e64 6974      @tree_condit
+00016a60: 696f 6e61 6c28 6c61 6d62 6461 206e 6f64  ional(lambda nod
+00016a70: 653a 206e 6f74 206e 6f64 652e 6c6f 636b  e: not node.lock
+00016a80: 290d 0a20 2020 2040 7472 6565 5f73 7562  )..    @tree_sub
+00016a90: 6d65 6e75 285f 2822 496d 6167 6522 2929  menu(_("Image"))
+00016aa0: 0d0a 2020 2020 4074 7265 655f 6f70 6572  ..    @tree_oper
+00016ab0: 6174 696f 6e28 5f28 224c 6f63 6b20 6d61  ation(_("Lock ma
+00016ac0: 6e69 7075 6c61 7469 6f6e 7322 292c 206e  nipulations"), n
+00016ad0: 6f64 655f 7479 7065 3d22 656c 656d 2069  ode_type="elem i
+00016ae0: 6d61 6765 222c 2068 656c 703d 2222 290d  mage", help="").
+00016af0: 0a20 2020 2064 6566 2069 6d61 6765 5f6c  .    def image_l
+00016b00: 6f63 6b5f 6d61 6e69 7075 6c61 7469 6f6e  ock_manipulation
+00016b10: 7328 6e6f 6465 2c20 2a2a 6b77 6172 6773  s(node, **kwargs
+00016b20: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00016b30: 2822 696d 6167 6520 6c6f 636b 5c6e 2229  ("image lock\n")
+00016b40: 0d0a 0d0a 2020 2020 4074 7265 655f 636f  ....    @tree_co
+00016b50: 6e64 6974 696f 6e61 6c28 6c61 6d62 6461  nditional(lambda
+00016b60: 206e 6f64 653a 206e 6f74 206e 6f64 652e   node: not node.
+00016b70: 6c6f 636b 290d 0a20 2020 2040 7472 6565  lock)..    @tree
+00016b80: 5f73 7562 6d65 6e75 285f 2822 496d 6167  _submenu(_("Imag
+00016b90: 6522 2929 0d0a 2020 2020 4074 7265 655f  e"))..    @tree_
+00016ba0: 6f70 6572 6174 696f 6e28 5f28 2244 6974  operation(_("Dit
+00016bb0: 6865 7220 746f 2031 2062 6974 2229 2c20  her to 1 bit"), 
+00016bc0: 6e6f 6465 5f74 7970 653d 2265 6c65 6d20  node_type="elem 
+00016bd0: 696d 6167 6522 2c20 6865 6c70 3d22 2229  image", help="")
+00016be0: 0d0a 2020 2020 6465 6620 696d 6167 655f  ..    def image_
+00016bf0: 6469 7468 6572 286e 6f64 652c 202a 2a6b  dither(node, **k
+00016c00: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00016c10: 2073 656c 6628 2269 6d61 6765 2064 6974   self("image dit
+00016c20: 6865 725c 6e22 290d 0a0d 0a20 2020 2040  her\n")....    @
+00016c30: 7472 6565 5f63 6f6e 6469 7469 6f6e 616c  tree_conditional
+00016c40: 286c 616d 6264 6120 6e6f 6465 3a20 6e6f  (lambda node: no
+00016c50: 7420 6e6f 6465 2e6c 6f63 6b29 0d0a 2020  t node.lock)..  
+00016c60: 2020 4074 7265 655f 7375 626d 656e 7528    @tree_submenu(
+00016c70: 5f28 2249 6d61 6765 2229 290d 0a20 2020  _("Image"))..   
+00016c80: 2040 7472 6565 5f6f 7065 7261 7469 6f6e   @tree_operation
+00016c90: 285f 2822 496e 7665 7274 2069 6d61 6765  (_("Invert image
+00016ca0: 2229 2c20 6e6f 6465 5f74 7970 653d 2265  "), node_type="e
+00016cb0: 6c65 6d20 696d 6167 6522 2c20 6865 6c70  lem image", help
+00016cc0: 3d22 2229 0d0a 2020 2020 6465 6620 696d  ="")..    def im
+00016cd0: 6167 655f 696e 7665 7274 286e 6f64 652c  age_invert(node,
+00016ce0: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+00016cf0: 2020 2020 2073 656c 6628 2269 6d61 6765       self("image
+00016d00: 2069 6e76 6572 745c 6e22 290d 0a0d 0a20   invert\n").... 
+00016d10: 2020 2040 7472 6565 5f63 6f6e 6469 7469     @tree_conditi
+00016d20: 6f6e 616c 286c 616d 6264 6120 6e6f 6465  onal(lambda node
+00016d30: 3a20 6e6f 7420 6e6f 6465 2e6c 6f63 6b29  : not node.lock)
+00016d40: 0d0a 2020 2020 4074 7265 655f 7375 626d  ..    @tree_subm
+00016d50: 656e 7528 5f28 2249 6d61 6765 2229 290d  enu(_("Image")).
+00016d60: 0a20 2020 2040 7472 6565 5f6f 7065 7261  .    @tree_opera
+00016d70: 7469 6f6e 285f 2822 4d69 7272 6f72 2068  tion(_("Mirror h
+00016d80: 6f72 697a 6f6e 7461 6c22 292c 206e 6f64  orizontal"), nod
+00016d90: 655f 7479 7065 3d22 656c 656d 2069 6d61  e_type="elem ima
+00016da0: 6765 222c 2068 656c 703d 2222 290d 0a20  ge", help="").. 
+00016db0: 2020 2064 6566 2069 6d61 6765 5f6d 6972     def image_mir
+00016dc0: 726f 7228 6e6f 6465 2c20 2a2a 6b77 6172  ror(node, **kwar
+00016dd0: 6773 293a 0d0a 2020 2020 2020 2020 7365  gs):..        se
+00016de0: 6c66 2822 696d 6167 6520 6d69 7272 6f72  lf("image mirror
+00016df0: 5c6e 2229 0d0a 0d0a 2020 2020 4074 7265  \n")....    @tre
+00016e00: 655f 636f 6e64 6974 696f 6e61 6c28 6c61  e_conditional(la
+00016e10: 6d62 6461 206e 6f64 653a 206e 6f74 206e  mbda node: not n
+00016e20: 6f64 652e 6c6f 636b 290d 0a20 2020 2040  ode.lock)..    @
+00016e30: 7472 6565 5f73 7562 6d65 6e75 285f 2822  tree_submenu(_("
+00016e40: 496d 6167 6522 2929 0d0a 2020 2020 4074  Image"))..    @t
+00016e50: 7265 655f 6f70 6572 6174 696f 6e28 5f28  ree_operation(_(
+00016e60: 2246 6c69 7020 7665 7274 6963 616c 2229  "Flip vertical")
+00016e70: 2c20 6e6f 6465 5f74 7970 653d 2265 6c65  , node_type="ele
+00016e80: 6d20 696d 6167 6522 2c20 6865 6c70 3d22  m image", help="
+00016e90: 2229 0d0a 2020 2020 6465 6620 696d 6167  ")..    def imag
+00016ea0: 655f 666c 6970 286e 6f64 652c 202a 2a6b  e_flip(node, **k
+00016eb0: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00016ec0: 2073 656c 6628 2269 6d61 6765 2066 6c69   self("image fli
+00016ed0: 705c 6e22 290d 0a0d 0a20 2020 2040 7472  p\n")....    @tr
+00016ee0: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
+00016ef0: 616d 6264 6120 6e6f 6465 3a20 6e6f 7420  ambda node: not 
+00016f00: 6e6f 6465 2e6c 6f63 6b29 0d0a 2020 2020  node.lock)..    
+00016f10: 4074 7265 655f 7375 626d 656e 7528 5f28  @tree_submenu(_(
+00016f20: 2249 6d61 6765 2229 290d 0a20 2020 2040  "Image"))..    @
+00016f30: 7472 6565 5f6f 7065 7261 7469 6f6e 285f  tree_operation(_
+00016f40: 2822 526f 7461 7465 2039 30c2 b020 4357  ("Rotate 90.. CW
+00016f50: 2229 2c20 6e6f 6465 5f74 7970 653d 2265  "), node_type="e
+00016f60: 6c65 6d20 696d 6167 6522 2c20 6865 6c70  lem image", help
+00016f70: 3d22 2229 0d0a 2020 2020 6465 6620 696d  ="")..    def im
+00016f80: 6167 655f 6377 286e 6f64 652c 202a 2a6b  age_cw(node, **k
+00016f90: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00016fa0: 2073 656c 6628 2269 6d61 6765 2063 775c   self("image cw\
+00016fb0: 6e22 290d 0a0d 0a20 2020 2040 7472 6565  n")....    @tree
+00016fc0: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
+00016fd0: 6264 6120 6e6f 6465 3a20 6e6f 7420 6e6f  bda node: not no
+00016fe0: 6465 2e6c 6f63 6b29 0d0a 2020 2020 4074  de.lock)..    @t
+00016ff0: 7265 655f 7375 626d 656e 7528 5f28 2249  ree_submenu(_("I
+00017000: 6d61 6765 2229 290d 0a20 2020 2040 7472  mage"))..    @tr
+00017010: 6565 5f6f 7065 7261 7469 6f6e 285f 2822  ee_operation(_("
+00017020: 526f 7461 7465 2039 30c2 b020 4343 5722  Rotate 90.. CCW"
+00017030: 292c 206e 6f64 655f 7479 7065 3d22 656c  ), node_type="el
+00017040: 656d 2069 6d61 6765 222c 2068 656c 703d  em image", help=
+00017050: 2222 290d 0a20 2020 2064 6566 2069 6d61  "")..    def ima
+00017060: 6765 5f63 6377 286e 6f64 652c 202a 2a6b  ge_ccw(node, **k
+00017070: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00017080: 2073 656c 6628 2269 6d61 6765 2063 6377   self("image ccw
+00017090: 5c6e 2229 0d0a 0d0a 2020 2020 4074 7265  \n")....    @tre
+000170a0: 655f 7375 626d 656e 7528 5f28 2249 6d61  e_submenu(_("Ima
+000170b0: 6765 2229 290d 0a20 2020 2040 7472 6565  ge"))..    @tree
+000170c0: 5f6f 7065 7261 7469 6f6e 280d 0a20 2020  _operation(..   
+000170d0: 2020 2020 205f 2822 5361 7665 206f 7269       _("Save ori
+000170e0: 6769 6e61 6c20 696d 6167 6520 746f 206f  ginal image to o
+000170f0: 7574 7075 742e 706e 6722 292c 206e 6f64  utput.png"), nod
+00017100: 655f 7479 7065 3d22 656c 656d 2069 6d61  e_type="elem ima
+00017110: 6765 222c 2068 656c 703d 2222 0d0a 2020  ge", help=""..  
+00017120: 2020 290d 0a20 2020 2064 6566 2069 6d61    )..    def ima
+00017130: 6765 5f73 6176 6528 6e6f 6465 2c20 2a2a  ge_save(node, **
+00017140: 6b77 6172 6773 293a 0d0a 2020 2020 2020  kwargs):..      
+00017150: 2020 7365 6c66 2822 696d 6167 6520 7361    self("image sa
+00017160: 7665 206f 7574 7075 742e 706e 675c 6e22  ve output.png\n"
+00017170: 290d 0a0d 0a20 2020 2040 7472 6565 5f73  )....    @tree_s
+00017180: 7562 6d65 6e75 285f 2822 496d 6167 6522  ubmenu(_("Image"
+00017190: 2929 0d0a 2020 2020 4074 7265 655f 6f70  ))..    @tree_op
+000171a0: 6572 6174 696f 6e28 0d0a 2020 2020 2020  eration(..      
+000171b0: 2020 5f28 2253 6176 6520 7072 6f63 6573    _("Save proces
+000171c0: 7365 6420 696d 6167 6520 746f 206f 7574  sed image to out
+000171d0: 7075 742e 706e 6722 292c 206e 6f64 655f  put.png"), node_
+000171e0: 7479 7065 3d22 656c 656d 2069 6d61 6765  type="elem image
+000171f0: 222c 2068 656c 703d 2222 0d0a 2020 2020  ", help=""..    
+00017200: 290d 0a20 2020 2064 6566 2069 6d61 6765  )..    def image
+00017210: 5f73 6176 655f 7072 6f63 6573 7365 6428  _save_processed(
+00017220: 6e6f 6465 2c20 2a2a 6b77 6172 6773 293a  node, **kwargs):
+00017230: 0d0a 2020 2020 2020 2020 7365 6c66 2822  ..        self("
+00017240: 696d 6167 6520 7361 7665 206f 7574 7075  image save outpu
+00017250: 742e 706e 6720 2d2d 7072 6f63 6573 7365  t.png --processe
+00017260: 645c 6e22 290d 0a0d 0a20 2020 2040 7472  d\n")....    @tr
+00017270: 6565 5f63 6f6e 6469 7469 6f6e 616c 286c  ee_conditional(l
+00017280: 616d 6264 6120 6e6f 6465 3a20 6c65 6e28  ambda node: len(
+00017290: 6e6f 6465 2e63 6869 6c64 7265 6e29 203e  node.children) >
+000172a0: 2030 290d 0a20 2020 2040 7472 6565 5f73   0)..    @tree_s
+000172b0: 6570 6172 6174 6f72 5f62 6566 6f72 6528  eparator_before(
+000172c0: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+000172d0: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
+000172e0: 205f 2822 4578 7061 6e64 2061 6c6c 2063   _("Expand all c
+000172f0: 6869 6c64 7265 6e22 292c 0d0a 2020 2020  hildren"),..    
+00017300: 2020 2020 6e6f 6465 5f74 7970 653d 280d      node_type=(.
+00017310: 0a20 2020 2020 2020 2020 2020 2022 6f70  .            "op
+00017320: 2063 7574 222c 0d0a 2020 2020 2020 2020   cut",..        
+00017330: 2020 2020 226f 7020 7261 7374 6572 222c      "op raster",
+00017340: 0d0a 2020 2020 2020 2020 2020 2020 226f  ..            "o
+00017350: 7020 696d 6167 6522 2c0d 0a20 2020 2020  p image",..     
+00017360: 2020 2020 2020 2022 6f70 2065 6e67 7261         "op engra
+00017370: 7665 222c 0d0a 2020 2020 2020 2020 2020  ve",..          
+00017380: 2020 226f 7020 646f 7473 222c 0d0a 2020    "op dots",..  
+00017390: 2020 2020 2020 2020 2020 226f 7020 6861            "op ha
+000173a0: 7463 6822 2c0d 0a20 2020 2020 2020 2020  tch",..         
+000173b0: 2020 2022 6272 616e 6368 2065 6c65 6d73     "branch elems
+000173c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000173d0: 2262 7261 6e63 6820 6f70 7322 2c0d 0a20  "branch ops",.. 
+000173e0: 2020 2020 2020 2020 2020 2022 6272 616e             "bran
+000173f0: 6368 2072 6567 222c 0d0a 2020 2020 2020  ch reg",..      
+00017400: 2020 2020 2020 2267 726f 7570 222c 0d0a        "group",..
+00017410: 2020 2020 2020 2020 2020 2020 2266 696c              "fil
+00017420: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+00017430: 2022 726f 6f74 222c 0d0a 2020 2020 2020   "root",..      
+00017440: 2020 292c 0d0a 2020 2020 2020 2020 6865    ),..        he
+00017450: 6c70 3d5f 2822 4578 7061 6e64 2061 6c6c  lp=_("Expand all
+00017460: 2063 6869 6c64 7265 6e20 6f66 2074 6869   children of thi
+00017470: 7320 6769 7665 6e20 6e6f 6465 2e22 292c  s given node."),
+00017480: 0d0a 2020 2020 290d 0a20 2020 2064 6566  ..    )..    def
+00017490: 2065 7870 616e 645f 616c 6c5f 6368 696c   expand_all_chil
+000174a0: 6472 656e 286e 6f64 652c 202a 2a6b 7761  dren(node, **kwa
+000174b0: 7267 7329 3a0d 0a20 2020 2020 2020 206e  rgs):..        n
+000174c0: 6f64 652e 6e6f 7469 6679 5f65 7870 616e  ode.notify_expan
+000174d0: 6428 290d 0a0d 0a20 2020 2040 7472 6565  d()....    @tree
+000174e0: 5f63 6f6e 6469 7469 6f6e 616c 286c 616d  _conditional(lam
+000174f0: 6264 6120 6e6f 6465 3a20 6c65 6e28 6e6f  bda node: len(no
+00017500: 6465 2e63 6869 6c64 7265 6e29 203e 2030  de.children) > 0
+00017510: 290d 0a20 2020 2040 7472 6565 5f6f 7065  )..    @tree_ope
+00017520: 7261 7469 6f6e 280d 0a20 2020 2020 2020  ration(..       
+00017530: 205f 2822 436f 6c6c 6170 7365 2061 6c6c   _("Collapse all
+00017540: 2063 6869 6c64 7265 6e22 292c 0d0a 2020   children"),..  
+00017550: 2020 2020 2020 6e6f 6465 5f74 7970 653d        node_type=
+00017560: 280d 0a20 2020 2020 2020 2020 2020 2022  (..            "
+00017570: 6f70 2063 7574 222c 0d0a 2020 2020 2020  op cut",..      
+00017580: 2020 2020 2020 226f 7020 7261 7374 6572        "op raster
+00017590: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000175a0: 226f 7020 696d 6167 6522 2c0d 0a20 2020  "op image",..   
+000175b0: 2020 2020 2020 2020 2022 6f70 2065 6e67           "op eng
+000175c0: 7261 7665 222c 0d0a 2020 2020 2020 2020  rave",..        
+000175d0: 2020 2020 226f 7020 646f 7473 222c 0d0a      "op dots",..
+000175e0: 2020 2020 2020 2020 2020 2020 226f 7020              "op 
+000175f0: 6861 7463 6822 2c0d 0a20 2020 2020 2020  hatch",..       
+00017600: 2020 2020 2022 6272 616e 6368 2065 6c65       "branch ele
+00017610: 6d73 222c 0d0a 2020 2020 2020 2020 2020  ms",..          
+00017620: 2020 2262 7261 6e63 6820 6f70 7322 2c0d    "branch ops",.
+00017630: 0a20 2020 2020 2020 2020 2020 2022 6272  .            "br
+00017640: 616e 6368 2072 6567 222c 0d0a 2020 2020  anch reg",..    
+00017650: 2020 2020 2020 2020 2267 726f 7570 222c          "group",
+00017660: 0d0a 2020 2020 2020 2020 2020 2020 2266  ..            "f
+00017670: 696c 6522 2c0d 0a20 2020 2020 2020 2020  ile",..         
+00017680: 2020 2022 726f 6f74 222c 0d0a 2020 2020     "root",..    
+00017690: 2020 2020 292c 0d0a 2020 2020 2020 2020      ),..        
+000176a0: 6865 6c70 3d5f 2822 436f 6c6c 6170 7365  help=_("Collapse
+000176b0: 2061 6c6c 2063 6869 6c64 7265 6e20 6f66   all children of
+000176c0: 2074 6869 7320 6769 7665 6e20 6e6f 6465   this given node
+000176d0: 2e22 292c 0d0a 2020 2020 290d 0a20 2020  ."),..    )..   
+000176e0: 2064 6566 2063 6f6c 6c61 7073 655f 616c   def collapse_al
+000176f0: 6c5f 6368 696c 6472 656e 286e 6f64 652c  l_children(node,
+00017700: 202a 2a6b 7761 7267 7329 3a0d 0a20 2020   **kwargs):..   
+00017710: 2020 2020 206e 6f64 652e 6e6f 7469 6679       node.notify
+00017720: 5f63 6f6c 6c61 7073 6528 290d 0a         _collapse()..
```

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/element_types.py` & `meerk40t-0.8.6000/meerk40t/core/elements/element_types.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/elements.py` & `meerk40t-0.8.6000/meerk40t/core/elements/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1466,15 +1466,15 @@
             for routine in self.kernel.lookup_all("reset_routines/.*"):
                 routine()
             self.validate_selected_area()
         if fast:
             self.signal("rebuild_tree")
         self.set_end_time("clear_all", display=True)
         self._filename = None
-        self.signal("file;loaded")
+        self.signal("file;cleared")
 
     def clear_note(self):
         self.note = None
         self.signal("note", self.note)
 
     def drag_and_drop(self, dragging_nodes, drop_node):
         data = dragging_nodes
@@ -3062,14 +3062,15 @@
     def save(self, pathname, version="default"):
         kernel = self.kernel
         for saver, save_name, sname in kernel.find("save"):
             for description, extension, mimetype, _version in saver.save_types():
                 if pathname.lower().endswith(extension) and _version == version:
                     saver.save(self, pathname, version)
                     self._filename = pathname
+                    self.signal("file;saved")
                     return True
         return False
 
     def save_types(self):
         kernel = self.kernel
         filetypes = []
         for saver, save_name, sname in kernel.find("save"):
```

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/grid.py` & `meerk40t-0.8.6000/meerk40t/core/elements/grid.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/materials.py` & `meerk40t-0.8.6000/meerk40t/core/elements/materials.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/notes.py` & `meerk40t-0.8.6000/meerk40t/core/elements/notes.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/offset.py` & `meerk40t-0.8.6000/meerk40t/core/elements/offset.py`

 * *Files 4% similar despite different names*

```diff
@@ -556,32 +556,40 @@
             helper = Point(p._segments[idx].end)
             left_end = idx
             if isinstance(segment, Arc):
                 arclinearize = linearize
                 # Arc is not working, so we always linearize
                 arclinearize = True
                 newsegment = offset_arc(segment, offset, arclinearize, interpolation)
+                if newsegment is None or len(newsegment) == 0:
+                    continue
                 left_end = idx - 1 + len(newsegment)
                 p._segments[idx] = newsegment[0]
                 for nidx in range(len(newsegment) - 1, 0, -1):  # All but the first
                     p._segments.insert(idx + 1, newsegment[nidx])
             elif isinstance(segment, QuadraticBezier):
                 newsegment = offset_quad(segment, offset, linearize, interpolation)
+                if newsegment is None or len(newsegment) == 0:
+                    continue
                 left_end = idx - 1 + len(newsegment)
                 p._segments[idx] = newsegment[0]
                 for nidx in range(len(newsegment) - 1, 0, -1):  # All but the first
                     p._segments.insert(idx + 1, newsegment[nidx])
             elif isinstance(segment, CubicBezier):
                 newsegment = offset_cubic(segment, offset, linearize, interpolation)
+                if newsegment is None or len(newsegment) == 0:
+                    continue
                 left_end = idx - 1 + len(newsegment)
                 p._segments[idx] = newsegment[0]
                 for nidx in range(len(newsegment) - 1, 0, -1):  # All but the first
                     p._segments.insert(idx + 1, newsegment[nidx])
             elif isinstance(segment, Line):
                 newsegment = offset_line(segment, offset)
+                if newsegment is None or len(newsegment) == 0:
+                    continue
                 left_end = idx - 1 + len(newsegment)
                 p._segments[idx] = newsegment[0]
                 for nidx in range(len(newsegment) - 1, 0, -1):  # All but the first
                     p._segments.insert(idx + 1, newsegment[nidx])
             stitch_segments_at_index(
                 offset, p, left_end, helper, radial=radial_connector
             )
```

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/penbox.py` & `meerk40t-0.8.6000/meerk40t/core/elements/penbox.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/placements.py` & `meerk40t-0.8.6000/meerk40t/core/elements/placements.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/render.py` & `meerk40t-0.8.6000/meerk40t/core/elements/render.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/shapes.py` & `meerk40t-0.8.6000/meerk40t/core/elements/shapes.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/trace.py` & `meerk40t-0.8.6000/meerk40t/core/elements/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,16 @@
 
 def generate_hull_shape_hull(data):
     pts = []
     for node in data:
         try:
             path = node.as_path()
             p = path.first_point
+            if p is None:
+                return None
             pts.append(p)
             for segment in path:
                 pts.append(segment.end)
             pts.append(p)
         except AttributeError:
             bounds = node.bounds
             if bounds:
@@ -445,15 +447,15 @@
         else:
             raise ValueError
         if start is None:
             # Lets take system default
             start = self.trace_start_method
         if start < 0 or start > 2:
             start = 0
-        if len(hull) == 0:
+        if hull is None or len(hull) == 0:
             channel(_("No elements bounds to trace."))
             return
 
         def run_shape(_spooler, startmethod, _hull):
             def trace_hull(startmethod=0):
                 if startmethod == 0:
                     # Immediately
```

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/tree_commands.py` & `meerk40t-0.8.6000/meerk40t/core/elements/tree_commands.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/undo_redo.py` & `meerk40t-0.8.6000/meerk40t/core/elements/undo_redo.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/elements/wordlist.py` & `meerk40t-0.8.6000/meerk40t/core/elements/wordlist.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/laserjob.py` & `meerk40t-0.8.6000/meerk40t/core/laserjob.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/logging.py` & `meerk40t-0.8.6000/meerk40t/core/logging.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/blobnode.py` & `meerk40t-0.8.6000/meerk40t/core/node/blobnode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/bootstrap.py` & `meerk40t-0.8.6000/meerk40t/core/node/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/branch_elems.py` & `meerk40t-0.8.6000/meerk40t/core/node/branch_elems.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/branch_ops.py` & `meerk40t-0.8.6000/meerk40t/core/node/branch_ops.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/branch_regmark.py` & `meerk40t-0.8.6000/meerk40t/core/node/branch_regmark.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/cutnode.py` & `meerk40t-0.8.6000/meerk40t/core/node/cutnode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_ellipse.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_ellipse.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_geomstr.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_geomstr.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_image.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_image.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_line.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_line.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_path.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_path.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_point.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_point.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_polyline.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_polyline.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_rect.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_rect.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/elem_text.py` & `meerk40t-0.8.6000/meerk40t/core/node/elem_text.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/filenode.py` & `meerk40t-0.8.6000/meerk40t/core/node/filenode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/groupnode.py` & `meerk40t-0.8.6000/meerk40t/core/node/groupnode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/lasercodenode.py` & `meerk40t-0.8.6000/meerk40t/core/node/lasercodenode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/layernode.py` & `meerk40t-0.8.6000/meerk40t/core/node/layernode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/mixins.py` & `meerk40t-0.8.6000/meerk40t/core/node/mixins.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/node.py` & `meerk40t-0.8.6000/meerk40t/core/node/node.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/nutils.py` & `meerk40t-0.8.6000/meerk40t/core/node/nutils.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/op_cut.py` & `meerk40t-0.8.6000/meerk40t/core/node/op_cut.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/op_dots.py` & `meerk40t-0.8.6000/meerk40t/core/node/op_dots.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/op_engrave.py` & `meerk40t-0.8.6000/meerk40t/core/node/op_engrave.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/op_hatch.py` & `meerk40t-0.8.6000/meerk40t/core/node/op_hatch.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/op_image.py` & `meerk40t-0.8.6000/meerk40t/core/node/op_image.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/op_raster.py` & `meerk40t-0.8.6000/meerk40t/core/node/op_raster.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/place_current.py` & `meerk40t-0.8.6000/meerk40t/core/node/place_current.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/place_point.py` & `meerk40t-0.8.6000/meerk40t/core/node/place_point.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/refnode.py` & `meerk40t-0.8.6000/meerk40t/core/node/refnode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/rootnode.py` & `meerk40t-0.8.6000/meerk40t/core/node/rootnode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/util_console.py` & `meerk40t-0.8.6000/meerk40t/core/node/util_console.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/util_goto.py` & `meerk40t-0.8.6000/meerk40t/core/node/util_goto.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/util_home.py` & `meerk40t-0.8.6000/meerk40t/core/node/util_home.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/util_input.py` & `meerk40t-0.8.6000/meerk40t/core/node/util_input.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/util_output.py` & `meerk40t-0.8.6000/meerk40t/core/node/util_output.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/node/util_wait.py` & `meerk40t-0.8.6000/meerk40t/core/node/util_wait.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/parameters.py` & `meerk40t-0.8.6000/meerk40t/core/parameters.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/planner.py` & `meerk40t-0.8.6000/meerk40t/core/planner.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/plotplanner.py` & `meerk40t-0.8.6000/meerk40t/core/plotplanner.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/space.py` & `meerk40t-0.8.6000/meerk40t/core/space.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/spoolers.py` & `meerk40t-0.8.6000/meerk40t/core/spoolers.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/svg_io.py` & `meerk40t-0.8.6000/meerk40t/core/svg_io.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/treeop.py` & `meerk40t-0.8.6000/meerk40t/core/treeop.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/undos.py` & `meerk40t-0.8.6000/meerk40t/core/undos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Undo States
 
 The undo class centralizes the undo stack and related commands. It's passed the
 rootnode of the tree and can perform marks to save the current tree states and will
 execute undo and redo operations for the tree.
 """
+import threading
 
 
 class UndoState:
     def __init__(self, state, message=None):
         self.state = state
         self.message = message
         if self.message is None:
@@ -17,14 +18,15 @@
     def __str__(self):
         return self.message
 
 
 class Undo:
     def __init__(self, tree):
         self.tree = tree
+        self._lock = threading.Lock()
         self._undo_stack = []
         self._undo_index = -1
         self.mark("init")  # Set initial tree state.
         self.message = None
 
     def __str__(self):
         return f"Undo(#{self._undo_index} in list of {len(self._undo_stack)} states)"
@@ -33,62 +35,66 @@
         """
         Marks an undo state require a backup the tree information.
 
         @param message: Optional message to be applied to the tree change.
 
         @return:
         """
-        self._undo_index += 1
-        if message is None:
-            message = self.message
-        try:
-            self._undo_stack.insert(
-                self._undo_index, UndoState(self.tree.backup_tree(), message=message)
-            )
-        except KeyError:
-            # Hit a concurrent issue.
-            pass
-        del self._undo_stack[self._undo_index + 1 :]
-        self.message = None
+        with self._lock:
+            self._undo_index += 1
+            if message is None:
+                message = self.message
+            try:
+                self._undo_stack.insert(
+                    self._undo_index,
+                    UndoState(self.tree.backup_tree(), message=message),
+                )
+            except KeyError:
+                # Hit a concurrent issue.
+                pass
+            del self._undo_stack[self._undo_index + 1 :]
+            self.message = None
 
     def undo(self):
         """
         Performs an undo operation restoring the tree state.
 
         Note: because the undo.state is used directly, the UndoState's state must be
         given a fresh copy.
         @return:
         """
-        if self._undo_index == 0:
-            # At bottom of stack.
-            return False
-        if len(self._undo_stack) == 0:
-            # Stack is entirely empty.
-            return False
-        self._undo_index -= 1
-        undo = self._undo_stack[self._undo_index]
-        self.tree.restore_tree(undo.state)
-        try:
-            undo.state = self.tree.backup_tree()  # Get unused copy
-        except KeyError:
-            pass
-        return True
+        with self._lock:
+            if self._undo_index == 0:
+                # At bottom of stack.
+                return False
+            if len(self._undo_stack) == 0:
+                # Stack is entirely empty.
+                return False
+            self._undo_index -= 1
+            undo = self._undo_stack[self._undo_index]
+            self.tree.restore_tree(undo.state)
+            try:
+                undo.state = self.tree.backup_tree()  # Get unused copy
+            except KeyError:
+                pass
+            return True
 
     def redo(self):
         """
         Performs a redo operation restoring the tree state.
         """
-        if self._undo_index >= len(self._undo_stack) - 1:
-            return False
-        self._undo_index += 1
-        redo = self._undo_stack[self._undo_index]
-        self.tree.restore_tree(redo.state)
-        try:
-            redo.state = self.tree.backup_tree()  # Get unused copy
-        except KeyError:
-            pass
-        return True
+        with self._lock:
+            if self._undo_index >= len(self._undo_stack) - 1:
+                return False
+            self._undo_index += 1
+            redo = self._undo_stack[self._undo_index]
+            self.tree.restore_tree(redo.state)
+            try:
+                redo.state = self.tree.backup_tree()  # Get unused copy
+            except KeyError:
+                pass
+            return True
 
     def undolist(self):
         for i, v in enumerate(self._undo_stack):
             q = "*" if i == self._undo_index else " "
             yield f"{q}{str(i).ljust(5)}: state {str(v)}"
```

### Comparing `meerk40t-0.8.5000/meerk40t/core/units.py` & `meerk40t-0.8.6000/meerk40t/core/units.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/view.py` & `meerk40t-0.8.6000/meerk40t/core/view.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/webhelp.py` & `meerk40t-0.8.6000/meerk40t/core/webhelp.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/core/wordlist.py` & `meerk40t-0.8.6000/meerk40t/core/wordlist.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/basedevice.py` & `meerk40t-0.8.6000/meerk40t/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/ch341/ch341.py` & `meerk40t-0.8.6000/meerk40t/device/ch341/ch341.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/ch341/ch341libusbdriver.py` & `meerk40t-0.8.6000/meerk40t/device/ch341/ch341libusbdriver.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/ch341/libusb.py` & `meerk40t-0.8.6000/meerk40t/device/ch341/libusb.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/ch341/mock.py` & `meerk40t-0.8.6000/meerk40t/device/ch341/mock.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/ch341/windll.py` & `meerk40t-0.8.6000/meerk40t/device/ch341/windll.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/dummydevice.py` & `meerk40t-0.8.6000/meerk40t/device/dummydevice.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/gui/defaultactions.py` & `meerk40t-0.8.6000/meerk40t/device/gui/defaultactions.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/gui/formatterpanel.py` & `meerk40t-0.8.6000/meerk40t/device/gui/formatterpanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/device/gui/warningpanel.py` & `meerk40t-0.8.6000/meerk40t/device/gui/warningpanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/dxf/dxf_io.py` & `meerk40t-0.8.6000/meerk40t/dxf/dxf_io.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/dxf/plugin.py` & `meerk40t-0.8.6000/meerk40t/dxf/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/external_plugins.py` & `meerk40t-0.8.6000/meerk40t/external_plugins.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/external_plugins_build.py` & `meerk40t-0.8.6000/meerk40t/external_plugins_build.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/cag.py` & `meerk40t-0.8.6000/meerk40t/extra/cag.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/embroider.py` & `meerk40t-0.8.6000/meerk40t/extra/embroider.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/ezd.py` & `meerk40t-0.8.6000/meerk40t/extra/ezd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Parser for .ezd files.
 
 These are a working type file produced by EZCad2™. They contain several pens and different settings that were used by
 the program when the file was saved. The vector objects consist of a series of laser-ready commands/shapes which refer
 to the required pen. Some modification objects like hatch and spiral work like a group containing other sub-elements
 and also contain the cached curve/path data. The image objects contain a standard 24 bit bitmap image. All elements
-are coordinated relative to the center of the working area and it is much more common to be given the center point than
+are coordinated relative to the center of the working area and, it is much more common to be given the center point than
 a specific corner. Nearly all coordinates are in mm, and denote the deviation from the center point.
 
 """
 import math
 import struct
 from io import BytesIO
 
@@ -191,25 +191,28 @@
         self.time_per_point = args[17]
         self.pulse_per_point = args[21]
         self.laser_off_tc = args[23]
         self.wobble_enable = args[26]
         self.wobble_diameter = args[27]
         self.wobble_distance = args[28]
 
-        self.add_endpoints = args[29]
-        self.add_endpoint_distance = args[30]
-        self.add_endpoint_time_per_point = args[32]
-        self.add_endpoint_point_distance = args[31]
-        self.add_endpoints_point_cycles = args[33]
-        self.opt_enable = args[40]  # Apparently crashy for older versions of ezcad.
-        self.break_angle = args[41]
-
-        self.jump_min_jump_delay2 = args[37]
-        self.jump_max_delay2 = args[38]
-        self.jump_speed_max_limit = args[39]
+        try:
+            self.add_endpoints = args[29]
+            self.add_endpoint_distance = args[30]
+            self.add_endpoint_time_per_point = args[32]
+            self.add_endpoint_point_distance = args[31]
+            self.add_endpoints_point_cycles = args[33]
+            self.opt_enable = args[40]
+            self.break_angle = args[41]
+
+            self.jump_min_jump_delay2 = args[37]
+            self.jump_max_delay2 = args[38]
+            self.jump_speed_max_limit = args[39]
+        except IndexError:
+            pass
 
 
 class EZCFile:
     """
     Parse the EZCFile given file as a stream.
     """
 
@@ -490,22 +493,29 @@
 
     def __init__(self, file):
         super().__init__(file)
         pts = []
         (count, closed) = struct.unpack("<2I", file.read(8))
         for i in range(count):
             (unk1, curve_type, unk2, unk3) = struct.unpack("<BB2H", file.read(6))
+            # Unk1 is 2 for a weird node. with t equal 0.
+            if curve_type == 0:
+                d = struct.unpack(f"<5d", file.read(40))
+                # print(d)
+                continue
             (pt_count,) = struct.unpack("<I", file.read(4))
+            # print(unk1, curve_type, unk2, unk2, pt_count)
             pts.append(
                 (
                     curve_type,
                     closed,
                     struct.unpack(f"<{pt_count * 2}d", file.read(16 * pt_count)),
                 )
             )
+
         self.points = pts
 
 
 class EZRect(EZObject):
     """
     Rectangles have optional each corner curved edges.
     """
@@ -650,28 +660,75 @@
     def __init__(self, file):
         EZObject.__init__(self, file)
         args = _parse_struct(file)
         _construct(args)
         self.distance = args[0]
 
 
+class EZExtendAxis(EZObject):
+    """
+    This is for testing on-the-fly movement.
+    """
+
+    def __init__(self, file):
+        EZObject.__init__(self, file)
+        args = _parse_struct(file)
+        _construct(args)
+        self.axis_go_zero = bool(args[0])
+        self.only_once_origin = bool(args[1])
+        self.relative = bool(args[2])
+        self.unit_type = args[3]  # Pulse (0), MM (1), Degree(2).
+        self.pulse_per_mm = args[4]
+        self.move_pulse = args[5]
+        self.max_speed = args[6]
+        self.min_speed = args[7]
+        self.acceleration_time = args[8]
+
+
 class EZText(EZObject):
     """
     Text objects.
     """
 
     def __init__(self, file):
         EZObject.__init__(self, file)
         args = _parse_struct(file)
         _interpret(args, 10, str)
         _interpret(args, 18, str)
         _interpret(args, 44, str)
+        _interpret(args, 54, str)
         _construct(args)
         self.font_angle = args[0]  # Font angle in Text.
+        self.height = args[1]  # Height in MM
+        self.text_space_setting = args[5]  # 0 auto, 1 between, 2 center
+        self.text_space = args[12]
+        self.char_space = args[13]
+        self.line_space = args[14]
+        self.font = args[18]  # Arial, JSF Font, etc
+        self.font2 = args[44]
+        self.x, self.y = args[7]
         self.text = args[10]
+        self.hatch_loop_distance = args[21]
+        self.circle_text_enable = args[48]
+        self.circle_text_diameter = args[49]
+        self.circle_text_base_angle = args[50]
+        self.circle_text_range_limit_enable = args[51]
+        self.circle_text_range_limit_angle = args[52]
+        self.save_options = args[53]  # 3 boolean values
+        self.save_filename = args[54]
+        self.circle_text_button_flags = args[85]  # 2 is first button, 1 is right to left.
+        (count,) = struct.unpack("<I", file.read(4))
+        for i in range(count):
+            (type,) = struct.unpack("<H", file.read(2))
+            # type, 7 file. 1 Text. 2 Serial
+            extradata = _parse_struct(file)
+            _construct(extradata)
+            extradata2 = _parse_struct(file)
+            _construct(extradata2)
+        (unk,) = struct.unpack("<I", file.read(4))
 
 
 class EZImage(EZObject):
     """
     Image objects consist of a lot of properties to control the encoding of the image and a 24-bit bitmap.
     """
 
@@ -786,14 +843,15 @@
     4: EZCircle,
     5: EZEllipse,
     6: EZPolygon,
     0x30: EZCombine,
     0x40: EZImage,
     0x60: EZSpiral,
     0x6000: EZEncoderDistance,
+    0x5000: EZExtendAxis,
     0x4000: EZOutput,
     0x3000: EZInput,
     0x2000: EZTimer,
     0x800: EZText,
     0x10: EZGroup,
     0x50: EZVectorFile,
     0x20: EZHatch,
```

### Comparing `meerk40t-0.8.5000/meerk40t/extra/hershey.py` & `meerk40t-0.8.6000/meerk40t/extra/hershey.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/imageactions.py` & `meerk40t-0.8.6000/meerk40t/extra/imageactions.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/inkscape.py` & `meerk40t-0.8.6000/meerk40t/extra/inkscape.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             )
             f.write("Output:\n")
             try:
                 f.write(c.stdout.decode("utf-8", errors="surrogateescape"))
             except UnicodeDecodeError:
                 pass
         result = True
-    except (FileNotFoundError, TimeoutExpired, UnicodeDecodeError) as e:
+    except (FileNotFoundError, TimeoutExpired, UnicodeDecodeError, OSError) as e:
         if f:
             f.write(f"Execution failed: {str(e)}\n")
     if f:
         f.close()
     return result, c
```

### Comparing `meerk40t-0.8.5000/meerk40t/extra/pathoptimize.py` & `meerk40t-0.8.6000/meerk40t/extra/pathoptimize.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/potrace.py` & `meerk40t-0.8.6000/meerk40t/extra/potrace.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/updater.py` & `meerk40t-0.8.6000/meerk40t/extra/updater.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/vectrace.py` & `meerk40t-0.8.6000/meerk40t/extra/vectrace.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/extra/winsleep.py` & `meerk40t-0.8.6000/meerk40t/extra/winsleep.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/fill/fills.py` & `meerk40t-0.8.6000/meerk40t/fill/fills.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,16 @@
     distance = abs(complex(transformed_vector[0], transformed_vector[1]))
 
     vm = VectorMontonizer()
     for outline in outlines:
         pts = list(map(Point, map(mx_rotate, outline)))
         vm.add_polyline(pts)
     y_min, y_max = vm.event_range()
+    if y_min is None:
+        return []
     height = y_max - y_min
     try:
         count = height / distance
     except ZeroDivisionError:
         return []
     if limit and count > limit:
         return []
```

### Comparing `meerk40t-0.8.5000/meerk40t/fill/patternfill.py` & `meerk40t-0.8.6000/meerk40t/fill/patternfill.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/fill/patterns.py` & `meerk40t-0.8.6000/meerk40t/fill/patterns.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/control.py` & `meerk40t-0.8.6000/meerk40t/grbl/control.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/controller.py` & `meerk40t-0.8.6000/meerk40t/grbl/controller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/device.py` & `meerk40t-0.8.6000/meerk40t/grbl/device.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/driver.py` & `meerk40t-0.8.6000/meerk40t/grbl/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,20 +362,19 @@
 
         @param data_type:
         @param data:
         @return:
         """
         if data_type != "grbl":
             return
-        for line in data:
-            grbl = bytes.decode(line, "utf-8")
-            for split in grbl.split("\r"):
-                g = split.strip()
-                if g:
-                    self(f"{g}{self.line_end}")
+        grbl = bytes.decode(data, "latin-1")
+        for split in grbl.split("\r"):
+            g = split.strip()
+            if g:
+                self(f"{g}{self.line_end}")
 
     def physical_home(self):
         """
         Home the laser physically (ie run into endstops).
 
         @return:
         """
```

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/emulator.py` & `meerk40t-0.8.6000/meerk40t/grbl/emulator.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/gcodejob.py` & `meerk40t-0.8.6000/meerk40t/grbl/gcodejob.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/gui/grblconfiguration.py` & `meerk40t-0.8.6000/meerk40t/grbl/gui/grblconfiguration.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/gui/grblcontroller.py` & `meerk40t-0.8.6000/meerk40t/grbl/gui/grblcontroller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/grbl/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/interpreter.py` & `meerk40t-0.8.6000/meerk40t/grbl/interpreter.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/loader.py` & `meerk40t-0.8.6000/meerk40t/grbl/loader.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/mock_connection.py` & `meerk40t-0.8.6000/meerk40t/grbl/mock_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/plugin.py` & `meerk40t-0.8.6000/meerk40t/grbl/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/serial_connection.py` & `meerk40t-0.8.6000/meerk40t/grbl/serial_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/grbl/tcp_connection.py` & `meerk40t-0.8.6000/meerk40t/grbl/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/about.py` & `meerk40t-0.8.6000/meerk40t/gui/about.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/alignment.py` & `meerk40t-0.8.6000/meerk40t/gui/alignment.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/bufferview.py` & `meerk40t-0.8.6000/meerk40t/gui/bufferview.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/busy.py` & `meerk40t-0.8.6000/meerk40t/gui/busy.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/choicepropertypanel.py` & `meerk40t-0.8.6000/meerk40t/gui/choicepropertypanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/consolepanel.py` & `meerk40t-0.8.6000/meerk40t/gui/consolepanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/devicepanel.py` & `meerk40t-0.8.6000/meerk40t/gui/devicepanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/dialogoptions.py` & `meerk40t-0.8.6000/meerk40t/gui/dialogoptions.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/executejob.py` & `meerk40t-0.8.6000/meerk40t/gui/executejob.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/fonts.py` & `meerk40t-0.8.6000/meerk40t/gui/fonts.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/guicolors.py` & `meerk40t-0.8.6000/meerk40t/gui/guicolors.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/help_assets/help_assets.py` & `meerk40t-0.8.6000/meerk40t/gui/help_assets/help_assets.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/hersheymanager.py` & `meerk40t-0.8.6000/meerk40t/gui/hersheymanager.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/icons.py` & `meerk40t-0.8.6000/meerk40t/gui/icons.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/imagesplitter.py` & `meerk40t-0.8.6000/meerk40t/gui/imagesplitter.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/keymap.py` & `meerk40t-0.8.6000/meerk40t/gui/keymap.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/laserpanel.py` & `meerk40t-0.8.6000/meerk40t/gui/laserpanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/laserrender.py` & `meerk40t-0.8.6000/meerk40t/gui/laserrender.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -90,30 +90,30 @@
     Translates all svg-text-properties to their wxfont-equivalents
     @param textnode:
     @return:
     """
     if not hasattr(textnode, "wxfont"):
         textnode.wxfont = wx.Font()
     wxfont = textnode.wxfont
+    # if the font_list is empty, then we do have a not properly initialised textnode,
+    # that needs to be resolved...
+    if textnode.font_family is None:
+        wxfont_to_svg(textnode)
 
+    svg_to_wx_family(textnode, wxfont)
+    svg_to_wx_fontstyle(textnode, wxfont)
     try:
         wxfont.SetNumericWeight(textnode.weight)  # Gets numeric weight.
     except AttributeError:
         # Running version wx4.0. No set Numeric Weight, can only set bold or normal.
         weight = textnode.weight
         wxfont.SetWeight(
             wx.FONTWEIGHT_BOLD if weight > 600 else wx.FONTWEIGHT_NORMAL
         )  # Gets numeric weight.
-    # if the font_list is empty, then we do have a not properly initialised textnode,
-    # that needs to be resolved...
-    if textnode.font_family is None:
-        wxfont_to_svg(textnode)
 
-    svg_to_wx_family(textnode, wxfont)
-    svg_to_wx_fontstyle(textnode, wxfont)
     font_size = textnode.font_size
     try:
         wxfont.SetFractionalPointSize(font_size)
     except AttributeError:
         # If we cannot set the fractional point size, we scale up to adjust to fractional levels.
         integer_font_size = int(round(font_size))
         scale = font_size / integer_font_size
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/lasertoolpanel.py` & `meerk40t-0.8.6000/meerk40t/gui/lasertoolpanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/materialtest.py` & `meerk40t-0.8.6000/meerk40t/gui/materialtest.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/mkdebug.py` & `meerk40t-0.8.6000/meerk40t/gui/mkdebug.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/mwindow.py` & `meerk40t-0.8.6000/meerk40t/gui/mwindow.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/navigationpanels.py` & `meerk40t-0.8.6000/meerk40t/gui/navigationpanels.py`

 * *Files 0% similar despite different names*

```diff
@@ -4613,883 +4613,908 @@
 00012040: 6e28 226d 6f64 6966 6965 6422 2c20 7365  n("modified", se
 00012050: 6c66 2e6f 6e5f 6d6f 6469 6669 6564 5f65  lf.on_modified_e
 00012060: 6c65 6d65 6e74 290d 0a20 2020 2020 2020  lement)..       
 00012070: 2073 656c 662e 636f 6e74 6578 742e 756e   self.context.un
 00012080: 6c69 7374 656e 2822 6275 7474 6f6e 2d72  listen("button-r
 00012090: 6570 6561 7422 2c20 7365 6c66 2e6f 6e5f  epeat", self.on_
 000120a0: 6275 7474 6f6e 5f72 6570 6561 7429 0d0a  button_repeat)..
-000120b0: 0d0a 2020 2020 6465 6620 7365 745f 7469  ..    def set_ti
-000120c0: 6d65 725f 6f70 7469 6f6e 7328 7365 6c66  mer_options(self
-000120d0: 293a 0d0a 2020 2020 2020 2020 696e 7465  ):..        inte
-000120e0: 7276 616c 203d 2073 656c 662e 636f 6e74  rval = self.cont
-000120f0: 6578 742e 6275 7474 6f6e 5f72 6570 6561  ext.button_repea
-00012100: 740d 0a20 2020 2020 2020 2069 6620 696e  t..        if in
-00012110: 7465 7276 616c 2069 7320 4e6f 6e65 3a0d  terval is None:.
-00012120: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-00012130: 6572 7661 6c20 3d20 302e 350d 0a20 2020  erval = 0.5..   
-00012140: 2020 2020 2069 6620 696e 7465 7276 616c       if interval
-00012150: 203c 2030 3a0d 0a20 2020 2020 2020 2020   < 0:..         
-00012160: 2020 2069 6e74 6572 7661 6c20 3d20 300d     interval = 0.
-00012170: 0a20 2020 2020 2020 2061 6363 656c 6572  .        acceler
-00012180: 6174 6520 3d20 7365 6c66 2e63 6f6e 7465  ate = self.conte
-00012190: 7874 2e62 7574 746f 6e5f 6163 6365 6c65  xt.button_accele
-000121a0: 7261 7465 0d0a 2020 2020 2020 2020 6966  rate..        if
-000121b0: 2061 6363 656c 6572 6174 6520 6973 204e   accelerate is N
-000121c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000121d0: 2020 6163 6365 6c65 7261 7465 203d 2054    accelerate = T
-000121e0: 7275 650d 0a20 2020 2020 2020 2073 656c  rue..        sel
-000121f0: 662e 7469 6d65 722e 696e 7465 7276 616c  f.timer.interval
-00012200: 203d 2069 6e74 6572 7661 6c0d 0a20 2020   = interval..   
-00012210: 2020 2020 2073 656c 662e 7469 6d65 722e       self.timer.
-00012220: 6163 6365 6c65 7261 7465 203d 2061 6363  accelerate = acc
-00012230: 656c 6572 6174 650d 0a0d 0a20 2020 2064  elerate....    d
-00012240: 6566 206f 6e5f 6275 7474 6f6e 5f72 6570  ef on_button_rep
-00012250: 6561 7428 7365 6c66 2c20 6f72 6967 696e  eat(self, origin
-00012260: 2c20 2a61 7267 7329 3a0d 0a20 2020 2020  , *args):..     
-00012270: 2020 2073 656c 662e 7365 745f 7469 6d65     self.set_time
-00012280: 725f 6f70 7469 6f6e 7328 290d 0a0d 0a20  r_options().... 
-00012290: 2020 2064 6566 206f 6e5f 6d6f 6469 6669     def on_modifi
-000122a0: 6564 5f65 6c65 6d65 6e74 2873 656c 662c  ed_element(self,
-000122b0: 206f 7269 6769 6e2c 202a 6172 6773 293a   origin, *args):
-000122c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-000122d0: 7064 6174 655f 6d61 7472 6978 5f74 6578  pdate_matrix_tex
-000122e0: 7428 290d 0a0d 0a20 2020 2064 6566 206f  t()....    def o
-000122f0: 6e5f 656d 7068 6173 697a 6564 5f65 6c65  n_emphasized_ele
-00012300: 6d65 6e74 735f 6368 616e 6765 6428 7365  ments_changed(se
-00012310: 6c66 2c20 6f72 6967 696e 2c20 656c 656d  lf, origin, elem
-00012320: 656e 7473 293a 0d0a 2020 2020 2020 2020  ents):..        
-00012330: 7365 6c66 2e73 656c 6563 745f 7265 6164  self.select_read
-00012340: 7928 7365 6c66 2e63 6f6e 7465 7874 2e65  y(self.context.e
-00012350: 6c65 6d65 6e74 732e 6861 735f 656d 7068  lements.has_emph
-00012360: 6173 6973 2829 290d 0a20 2020 2020 2020  asis())..       
-00012370: 2073 656c 662e 7570 6461 7465 5f6d 6174   self.update_mat
-00012380: 7269 785f 7465 7874 2829 0d0a 0d0a 2020  rix_text()....  
-00012390: 2020 6465 6620 7570 6461 7465 5f6d 6174    def update_mat
-000123a0: 7269 785f 7465 7874 2873 656c 6629 3a0d  rix_text(self):.
-000123b0: 0a20 2020 2020 2020 2066 203d 2073 656c  .        f = sel
-000123c0: 662e 636f 6e74 6578 742e 656c 656d 656e  f.context.elemen
-000123d0: 7473 2e66 6972 7374 5f65 6c65 6d65 6e74  ts.first_element
-000123e0: 2865 6d70 6861 7369 7a65 643d 5472 7565  (emphasized=True
-000123f0: 290d 0a20 2020 2020 2020 2076 203d 2066  )..        v = f
-00012400: 2069 7320 6e6f 7420 4e6f 6e65 0d0a 2020   is not None..  
-00012410: 2020 2020 2020 7365 6c66 2e74 6578 745f        self.text_
-00012420: 612e 456e 6162 6c65 2876 290d 0a20 2020  a.Enable(v)..   
-00012430: 2020 2020 2073 656c 662e 7465 7874 5f62       self.text_b
-00012440: 2e45 6e61 626c 6528 7629 0d0a 2020 2020  .Enable(v)..    
-00012450: 2020 2020 7365 6c66 2e74 6578 745f 632e      self.text_c.
-00012460: 456e 6162 6c65 2876 290d 0a20 2020 2020  Enable(v)..     
-00012470: 2020 2073 656c 662e 7465 7874 5f64 2e45     self.text_d.E
-00012480: 6e61 626c 6528 7629 0d0a 2020 2020 2020  nable(v)..      
-00012490: 2020 7365 6c66 2e74 6578 745f 652e 456e    self.text_e.En
-000124a0: 6162 6c65 2876 290d 0a20 2020 2020 2020  able(v)..       
-000124b0: 2073 656c 662e 7465 7874 5f66 2e45 6e61   self.text_f.Ena
-000124c0: 626c 6528 7629 0d0a 2020 2020 2020 2020  ble(v)..        
-000124d0: 6966 2076 3a0d 0a20 2020 2020 2020 2020  if v:..         
-000124e0: 2020 206d 6174 7269 7820 3d20 662e 6d61     matrix = f.ma
-000124f0: 7472 6978 0d0a 2020 2020 2020 2020 2020  trix..          
-00012500: 2020 2320 596f 7520 7769 6c6c 2067 6574    # You will get
-00012510: 2073 6f6d 6574 696d 6573 2073 6c69 6768   sometimes sligh
-00012520: 746c 7920 6469 6666 6572 656e 7420 6e75  tly different nu
-00012530: 6d62 6572 7320 7468 616e 2079 6f75 2077  mbers than you w
-00012540: 6f75 6c64 2065 7870 6563 7420 6475 6520  ould expect due 
-00012550: 746f 2061 7269 7468 6d65 7469 6320 6f70  to arithmetic op
-00012560: 6572 6174 696f 6e73 0d0a 2020 2020 2020  erations..      
-00012570: 2020 2020 2020 2320 7765 2077 696c 6c20        # we will 
-00012580: 7468 6572 6566 6f72 6520 2761 646a 7573  therefore 'adjus
-00012590: 7427 2074 686f 7365 2066 6967 7572 6573  t' those figures
-000125a0: 2073 6c69 6768 746c 7920 746f 2061 766f   slightly to avo
-000125b0: 6964 2063 6f6e 6675 7369 6f6e 2062 7920  id confusion by 
-000125c0: 726f 756e 6469 6e67 2074 6865 6d20 746f  rounding them to
-000125d0: 2074 6865 2073 6978 7468 2064 6563 696d   the sixth decim
-000125e0: 616c 2028 6172 6269 7472 6172 7929 0d0a  al (arbitrary)..
-000125f0: 2020 2020 2020 2020 2020 2020 2320 7468              # th
-00012600: 6174 2073 686f 756c 6420 6265 2067 6f6f  at should be goo
-00012610: 6420 656e 6f75 6768 2e2e 2e0d 0a20 2020  d enough.....   
-00012620: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00012630: 7874 5f61 2e53 6574 5661 6c75 6528 6622  xt_a.SetValue(f"
-00012640: 7b6d 6174 7269 782e 613a 2e35 667d 2229  {matrix.a:.5f}")
-00012650: 2020 2320 5363 616c 6520 580d 0a20 2020    # Scale X..   
-00012660: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00012670: 7874 5f62 2e53 6574 5661 6c75 6528 6622  xt_b.SetValue(f"
-00012680: 7b6d 6174 7269 782e 623a 2e35 667d 2229  {matrix.b:.5f}")
-00012690: 2020 2320 536b 6577 2059 0d0a 2020 2020    # Skew Y..    
-000126a0: 2020 2020 2020 2020 7365 6c66 2e74 6578          self.tex
-000126b0: 745f 632e 5365 7456 616c 7565 2866 227b  t_c.SetValue(f"{
-000126c0: 6d61 7472 6978 2e63 3a2e 3566 7d22 2920  matrix.c:.5f}") 
-000126d0: 2023 2053 6b65 7720 580d 0a20 2020 2020   # Skew X..     
-000126e0: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-000126f0: 5f64 2e53 6574 5661 6c75 6528 6622 7b6d  _d.SetValue(f"{m
-00012700: 6174 7269 782e 643a 2e35 667d 2229 2020  atrix.d:.5f}")  
-00012710: 2320 5363 616c 6520 590d 0a20 2020 2020  # Scale Y..     
-00012720: 2020 2020 2020 2023 2054 7261 6e73 6c61         # Transla
-00012730: 7465 2058 2026 2061 7265 2069 6e20 6d69  te X & are in mi
-00012740: 6c73 2c20 736f 2061 626f 7574 2030 2e30  ls, so about 0.0
-00012750: 3235 206d 6d2c 2073 6f20 3120 6469 6769  25 mm, so 1 digi
-00012760: 7420 7368 6f75 6c64 2062 6520 6d6f 7265  t should be more
-00012770: 2074 6861 6e20 656e 6f75 6768 2e2e 2e0d   than enough....
-00012780: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00012790: 656c 662e 7465 7874 5f65 2e53 6574 5661  elf.text_e.SetVa
-000127a0: 6c75 6528 6622 7b6d 6174 7269 782e 653a  lue(f"{matrix.e:
-000127b0: 2e31 667d 2229 2020 2320 5472 616e 736c  .1f}")  # Transl
-000127c0: 6174 6520 580d 0a20 2020 2020 2020 2020  ate X..         
-000127d0: 2020 2023 2073 656c 662e 7465 7874 5f66     # self.text_f
-000127e0: 2e53 6574 5661 6c75 6528 6622 7b6d 6174  .SetValue(f"{mat
-000127f0: 7269 782e 663a 2e31 667d 2229 2020 2320  rix.f:.1f}")  # 
-00012800: 5472 616e 736c 6174 6520 590d 0a20 2020  Translate Y..   
-00012810: 2020 2020 2020 2020 206c 3120 3d20 4c65           l1 = Le
-00012820: 6e67 7468 280d 0a20 2020 2020 2020 2020  ngth(..         
-00012830: 2020 2020 2020 2061 6d6f 756e 743d 6d61         amount=ma
-00012840: 7472 6978 2e65 2c20 6469 6769 7473 3d32  trix.e, digits=2
-00012850: 2c20 7072 6566 6572 7265 645f 756e 6974  , preferred_unit
-00012860: 733d 7365 6c66 2e63 6f6e 7465 7874 2e75  s=self.context.u
-00012870: 6e69 7473 5f6e 616d 650d 0a20 2020 2020  nits_name..     
-00012880: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00012890: 2020 2020 2020 6c32 203d 204c 656e 6774        l2 = Lengt
-000128a0: 6828 0d0a 2020 2020 2020 2020 2020 2020  h(..            
-000128b0: 2020 2020 616d 6f75 6e74 3d6d 6174 7269      amount=matri
-000128c0: 782e 662c 2064 6967 6974 733d 322c 2070  x.f, digits=2, p
-000128d0: 7265 6665 7272 6564 5f75 6e69 7473 3d73  referred_units=s
-000128e0: 656c 662e 636f 6e74 6578 742e 756e 6974  elf.context.unit
-000128f0: 735f 6e61 6d65 0d0a 2020 2020 2020 2020  s_name..        
-00012900: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00012910: 2020 2073 656c 662e 7465 7874 5f65 2e53     self.text_e.S
-00012920: 6574 5661 6c75 6528 6c31 2e70 7265 6665  etValue(l1.prefe
-00012930: 7272 6564 5f6c 656e 6774 6829 0d0a 2020  rred_length)..  
-00012940: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00012950: 6578 745f 662e 5365 7456 616c 7565 286c  ext_f.SetValue(l
-00012960: 322e 7072 6566 6572 7265 645f 6c65 6e67  2.preferred_leng
-00012970: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-00012980: 206d 5f65 203d 206d 6174 7269 782e 650d   m_e = matrix.e.
-00012990: 0a20 2020 2020 2020 2020 2020 206d 5f66  .            m_f
-000129a0: 203d 206d 6174 7269 782e 660d 0a20 2020   = matrix.f..   
-000129b0: 2020 2020 2020 2020 2074 7469 7031 203d           ttip1 =
-000129c0: 205f 280d 0a20 2020 2020 2020 2020 2020   _(..           
-000129d0: 2020 2020 2022 5472 616e 736c 6174 6520       "Translate 
-000129e0: 5820 2d20 6d6f 7665 7320 7468 6520 656c  X - moves the el
-000129f0: 656d 656e 7420 6279 2074 6869 7320 616d  ement by this am
-00012a00: 6f75 6e74 206f 6620 6d69 6c73 2069 6e20  ount of mils in 
-00012a10: 7468 6520 582d 6469 7265 6374 696f 6e3b  the X-direction;
-00012a20: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
-00012a30: 2020 2020 2279 6f75 206d 6179 2075 7365      "you may use
-00012a40: 2027 7265 616c 2720 6469 7374 616e 6365   'real' distance
-00012a50: 7320 7768 656e 206d 6f64 6966 7969 6e67  s when modifying
-00012a60: 2074 6869 7320 6661 6374 6f72 2c20 692e   this factor, i.
-00012a70: 652e 2032 696e 2c20 3363 6d2c 2035 306d  e. 2in, 3cm, 50m
-00012a80: 6d22 0d0a 2020 2020 2020 2020 2020 2020  m"..            
-00012a90: 290d 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00012aa0: 7469 7031 203d 2074 7469 7031 202b 2022  tip1 = ttip1 + "
-00012ab0: 5c6e 2220 2b20 5f28 2243 7572 7265 6e74  \n" + _("Current
-00012ac0: 2069 6e74 6572 6e61 6c20 7661 6c75 653a   internal value:
-00012ad0: 2022 2920 2b20 6622 7b6d 5f65 3a2e 3166   ") + f"{m_e:.1f
-00012ae0: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
-00012af0: 7474 6970 3220 3d20 5f28 0d0a 2020 2020  ttip2 = _(..    
-00012b00: 2020 2020 2020 2020 2020 2020 2254 7261              "Tra
-00012b10: 6e73 6c61 7465 2059 202d 206d 6f76 6573  nslate Y - moves
-00012b20: 2074 6865 2065 6c65 6d65 6e74 2062 7920   the element by 
-00012b30: 7468 6973 2061 6d6f 756e 7420 6f66 206d  this amount of m
-00012b40: 696c 7320 696e 2074 6865 2059 2d64 6972  ils in the Y-dir
-00012b50: 6563 7469 6f6e 3b20 220d 0a20 2020 2020  ection; "..     
-00012b60: 2020 2020 2020 2020 2020 2022 796f 7520             "you 
-00012b70: 6d61 7920 7573 6520 2772 6561 6c27 2064  may use 'real' d
-00012b80: 6973 7461 6e63 6573 2077 6865 6e20 6d6f  istances when mo
-00012b90: 6469 6679 696e 6720 7468 6973 2066 6163  difying this fac
-00012ba0: 746f 722c 2069 2e65 2e20 3269 6e2c 2033  tor, i.e. 2in, 3
-00012bb0: 636d 2c20 3530 6d6d 220d 0a20 2020 2020  cm, 50mm"..     
-00012bc0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00012bd0: 2020 2020 2020 7474 6970 3220 3d20 7474        ttip2 = tt
-00012be0: 6970 3220 2b20 225c 6e22 202b 205f 2822  ip2 + "\n" + _("
-00012bf0: 4375 7272 656e 7420 696e 7465 726e 616c  Current internal
-00012c00: 2076 616c 7565 3a20 2229 202b 2066 227b   value: ") + f"{
-00012c10: 6d5f 663a 2e31 667d 220d 0a0d 0a20 2020  m_f:.1f}"....   
-00012c20: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00012c30: 7874 5f65 2e53 6574 546f 6f6c 5469 7028  xt_e.SetToolTip(
-00012c40: 7474 6970 3129 0d0a 2020 2020 2020 2020  ttip1)..        
-00012c50: 2020 2020 7365 6c66 2e74 6578 745f 662e      self.text_f.
-00012c60: 5365 7454 6f6f 6c54 6970 2874 7469 7032  SetToolTip(ttip2
-00012c70: 290d 0a0d 0a20 2020 2064 6566 2073 656c  )....    def sel
-00012c80: 6563 745f 7265 6164 7928 7365 6c66 2c20  ect_ready(self, 
-00012c90: 7629 3a0d 0a20 2020 2020 2020 2022 2222  v):..        """
-00012ca0: 0d0a 2020 2020 2020 2020 456e 6162 6c65  ..        Enable
-00012cb0: 7320 7468 6520 7265 6c65 7661 6e74 2062  s the relevant b
-00012cc0: 7574 746f 6e73 2077 6865 6e20 7468 6572  uttons when ther
-00012cd0: 6520 6973 2061 2073 656c 6563 7469 6f6e  e is a selection
-00012ce0: 2069 6e20 7468 6520 656c 656d 656e 7473   in the elements
-00012cf0: 2e0d 0a20 2020 2020 2020 2040 7061 7261  ...        @para
-00012d00: 6d20 763a 2077 6865 7468 6572 2073 656c  m v: whether sel
-00012d10: 6563 7469 6f6e 2069 7320 6375 7272 656e  ection is curren
-00012d20: 746c 7920 6472 6167 2072 6561 6479 2e0d  tly drag ready..
-00012d30: 0a20 2020 2020 2020 2040 7265 7475 726e  .        @return
-00012d40: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00012d50: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
-00012d60: 746f 6e5f 7363 616c 655f 646f 776e 2e45  ton_scale_down.E
-00012d70: 6e61 626c 6528 7629 0d0a 2020 2020 2020  nable(v)..      
-00012d80: 2020 7365 6c66 2e62 7574 746f 6e5f 7363    self.button_sc
-00012d90: 616c 655f 7570 2e45 6e61 626c 6528 7629  ale_up.Enable(v)
-00012da0: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-00012db0: 7574 746f 6e5f 726f 7461 7465 5f63 6377  utton_rotate_ccw
-00012dc0: 2e45 6e61 626c 6528 7629 0d0a 2020 2020  .Enable(v)..    
-00012dd0: 2020 2020 7365 6c66 2e62 7574 746f 6e5f      self.button_
-00012de0: 726f 7461 7465 5f63 772e 456e 6162 6c65  rotate_cw.Enable
-00012df0: 2876 290d 0a20 2020 2020 2020 2073 656c  (v)..        sel
-00012e00: 662e 6275 7474 6f6e 5f74 7261 6e73 6c61  f.button_transla
-00012e10: 7465 5f64 6f77 6e2e 456e 6162 6c65 2876  te_down.Enable(v
-00012e20: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00012e30: 6275 7474 6f6e 5f74 7261 6e73 6c61 7465  button_translate
-00012e40: 5f75 702e 456e 6162 6c65 2876 290d 0a20  _up.Enable(v).. 
-00012e50: 2020 2020 2020 2073 656c 662e 6275 7474         self.butt
-00012e60: 6f6e 5f74 7261 6e73 6c61 7465 5f6c 6566  on_translate_lef
-00012e70: 742e 456e 6162 6c65 2876 290d 0a20 2020  t.Enable(v)..   
-00012e80: 2020 2020 2073 656c 662e 6275 7474 6f6e       self.button
-00012e90: 5f74 7261 6e73 6c61 7465 5f72 6967 6874  _translate_right
-00012ea0: 2e45 6e61 626c 6528 7629 0d0a 2020 2020  .Enable(v)..    
-00012eb0: 2020 2020 7365 6c66 2e62 7574 746f 6e5f      self.button_
-00012ec0: 7265 7365 742e 456e 6162 6c65 2876 290d  reset.Enable(v).
-00012ed0: 0a0d 0a20 2020 2064 6566 206d 6174 7269  ...    def matri
-00012ee0: 785f 7570 6461 7465 6428 7365 6c66 293a  x_updated(self):
-00012ef0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-00012f00: 6f6e 7465 7874 2e65 6c65 6d65 6e74 732e  ontext.elements.
-00012f10: 7369 676e 616c 2822 7265 6672 6573 685f  signal("refresh_
-00012f20: 7363 656e 6522 2c20 2253 6365 6e65 2229  scene", "Scene")
-00012f30: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00012f40: 7064 6174 655f 6d61 7472 6978 5f74 6578  pdate_matrix_tex
-00012f50: 7428 290d 0a0d 0a20 2020 2064 6566 205f  t()....    def _
-00012f60: 7363 616c 6528 7365 6c66 2c20 7363 616c  scale(self, scal
-00012f70: 6529 3a0d 0a20 2020 2020 2020 2073 656c  e):..        sel
-00012f80: 662e 636f 6e74 6578 7428 6622 7363 616c  f.context(f"scal
-00012f90: 6520 7b73 6361 6c65 7d20 7b73 6361 6c65  e {scale} {scale
-00012fa0: 7d20 5c6e 2229 0d0a 2020 2020 2020 2020  } \n")..        
-00012fb0: 7365 6c66 2e63 6f6e 7465 7874 2e65 6c65  self.context.ele
-00012fc0: 6d65 6e74 732e 7369 676e 616c 2822 6578  ments.signal("ex
-00012fd0: 742d 6d6f 6469 6669 6564 2229 0d0a 2020  t-modified")..  
-00012fe0: 2020 2020 2020 7365 6c66 2e6d 6174 7269        self.matri
-00012ff0: 785f 7570 6461 7465 6428 290d 0a0d 0a20  x_updated().... 
-00013000: 2020 2064 6566 205f 726f 7461 7465 2873     def _rotate(s
-00013010: 656c 662c 2061 6e67 6c65 293a 0d0a 2020  elf, angle):..  
-00013020: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00013030: 7874 2866 2272 6f74 6174 6520 7b61 6e67  xt(f"rotate {ang
-00013040: 6c65 7d64 6567 205c 6e22 290d 0a20 2020  le}deg \n")..   
-00013050: 2020 2020 2073 656c 662e 636f 6e74 6578       self.contex
-00013060: 742e 656c 656d 656e 7473 2e73 6967 6e61  t.elements.signa
-00013070: 6c28 2265 7874 2d6d 6f64 6966 6965 6422  l("ext-modified"
-00013080: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00013090: 6d61 7472 6978 5f75 7064 6174 6564 2829  matrix_updated()
-000130a0: 0d0a 0d0a 2020 2020 6465 6620 5f74 7261  ....    def _tra
-000130b0: 6e73 6c61 7465 2873 656c 662c 2064 782c  nslate(self, dx,
-000130c0: 2064 792c 2073 6361 6c65 293a 0d0a 2020   dy, scale):..  
-000130d0: 2020 2020 2020 6478 203d 2073 656c 662e        dx = self.
-000130e0: 636f 6e74 6578 742e 6465 7669 6365 2e6c  context.device.l
-000130f0: 656e 6774 6828 0d0a 2020 2020 2020 2020  ength(..        
-00013100: 2020 2020 6478 2c0d 0a20 2020 2020 2020      dx,..       
-00013110: 2020 2020 2030 2c0d 0a20 2020 2020 2020       0,..       
-00013120: 2020 2020 2073 6361 6c65 3d73 6361 6c65       scale=scale
-00013130: 2c0d 0a20 2020 2020 2020 2020 2020 206e  ,..            n
-00013140: 6577 5f75 6e69 7473 3d73 656c 662e 636f  ew_units=self.co
-00013150: 6e74 6578 742e 756e 6974 735f 6e61 6d65  ntext.units_name
-00013160: 2c0d 0a20 2020 2020 2020 2020 2020 2075  ,..            u
-00013170: 6e69 746c 6573 733d 554e 4954 535f 5045  nitless=UNITS_PE
-00013180: 525f 5049 5845 4c2c 0d0a 2020 2020 2020  R_PIXEL,..      
-00013190: 2020 290d 0a20 2020 2020 2020 2064 7920    )..        dy 
-000131a0: 3d20 7365 6c66 2e63 6f6e 7465 7874 2e64  = self.context.d
-000131b0: 6576 6963 652e 6c65 6e67 7468 280d 0a20  evice.length(.. 
-000131c0: 2020 2020 2020 2020 2020 2064 792c 0d0a             dy,..
-000131d0: 2020 2020 2020 2020 2020 2020 312c 0d0a              1,..
-000131e0: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-000131f0: 653d 7363 616c 652c 0d0a 2020 2020 2020  e=scale,..      
-00013200: 2020 2020 2020 6e65 775f 756e 6974 733d        new_units=
-00013210: 7365 6c66 2e63 6f6e 7465 7874 2e75 6e69  self.context.uni
-00013220: 7473 5f6e 616d 652c 0d0a 2020 2020 2020  ts_name,..      
-00013230: 2020 2020 2020 756e 6974 6c65 7373 3d55        unitless=U
-00013240: 4e49 5453 5f50 4552 5f50 4958 454c 2c0d  NITS_PER_PIXEL,.
-00013250: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
-00013260: 2020 2020 7365 6c66 2e63 6f6e 7465 7874      self.context
-00013270: 2866 2274 7261 6e73 6c61 7465 207b 6478  (f"translate {dx
-00013280: 7d20 7b64 797d 5c6e 2229 0d0a 2020 2020  } {dy}\n")..    
-00013290: 2020 2020 7365 6c66 2e63 6f6e 7465 7874      self.context
-000132a0: 2e65 6c65 6d65 6e74 732e 7369 676e 616c  .elements.signal
-000132b0: 2822 6578 742d 6d6f 6469 6669 6564 2229  ("ext-modified")
-000132c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
-000132d0: 6174 7269 785f 7570 6461 7465 6428 290d  atrix_updated().
-000132e0: 0a0d 0a20 2020 2064 6566 206f 6e5f 7363  ...    def on_sc
-000132f0: 616c 655f 646f 776e 5f35 3028 7365 6c66  ale_down_50(self
-00013300: 2c20 6576 656e 743d 4e6f 6e65 293a 2020  , event=None):  
-00013310: 2320 7778 476c 6164 653a 204e 6176 6967  # wxGlade: Navig
-00013320: 6174 696f 6e2e 3c65 7665 6e74 5f68 616e  ation.<event_han
-00013330: 646c 6572 3e0d 0a20 2020 2020 2020 2073  dler>..        s
-00013340: 6361 6c65 203d 2032 2e30 202f 2033 2e30  cale = 2.0 / 3.0
-00013350: 2020 2320 3636 2e36 2520 2d20 696e 7665    # 66.6% - inve
-00013360: 7273 6520 6f66 2031 3530 250d 0a20 2020  rse of 150%..   
-00013370: 2020 2020 2073 656c 662e 5f73 6361 6c65       self._scale
-00013380: 2873 6361 6c65 290d 0a0d 0a20 2020 2064  (scale)....    d
-00013390: 6566 206f 6e5f 7363 616c 655f 7570 5f35  ef on_scale_up_5
-000133a0: 3028 7365 6c66 2c20 6576 656e 743d 4e6f  0(self, event=No
-000133b0: 6e65 293a 2020 2320 7778 476c 6164 653a  ne):  # wxGlade:
-000133c0: 204e 6176 6967 6174 696f 6e2e 3c65 7665   Navigation.<eve
-000133d0: 6e74 5f68 616e 646c 6572 3e0d 0a20 2020  nt_handler>..   
-000133e0: 2020 2020 2073 6361 6c65 203d 2033 2e30       scale = 3.0
-000133f0: 202f 2032 2e30 2020 2320 3135 3025 0d0a   / 2.0  # 150%..
-00013400: 2020 2020 2020 2020 7365 6c66 2e5f 7363          self._sc
-00013410: 616c 6528 7363 616c 6529 0d0a 0d0a 2020  ale(scale)....  
-00013420: 2020 6465 6620 6f6e 5f73 6361 6c65 5f64    def on_scale_d
-00013430: 6f77 6e5f 3528 7365 6c66 2c20 6576 656e  own_5(self, even
-00013440: 743d 4e6f 6e65 293a 2020 2320 7778 476c  t=None):  # wxGl
-00013450: 6164 653a 204e 6176 6967 6174 696f 6e2e  ade: Navigation.
-00013460: 3c65 7665 6e74 5f68 616e 646c 6572 3e0d  <event_handler>.
-00013470: 0a20 2020 2020 2020 2073 6361 6c65 203d  .        scale =
-00013480: 2031 392e 3020 2f20 3230 2e30 0d0a 2020   19.0 / 20.0..  
-00013490: 2020 2020 2020 7365 6c66 2e5f 7363 616c        self._scal
-000134a0: 6528 7363 616c 6529 0d0a 0d0a 2020 2020  e(scale)....    
-000134b0: 6465 6620 6f6e 5f73 6361 6c65 5f75 705f  def on_scale_up_
-000134c0: 3528 7365 6c66 2c20 6576 656e 743d 4e6f  5(self, event=No
-000134d0: 6e65 293a 2020 2320 7778 476c 6164 653a  ne):  # wxGlade:
-000134e0: 204e 6176 6967 6174 696f 6e2e 3c65 7665   Navigation.<eve
-000134f0: 6e74 5f68 616e 646c 6572 3e0d 0a20 2020  nt_handler>..   
-00013500: 2020 2020 2073 6361 6c65 203d 2032 302e       scale = 20.
-00013510: 3020 2f20 3139 2e30 0d0a 2020 2020 2020  0 / 19.0..      
-00013520: 2020 7365 6c66 2e5f 7363 616c 6528 7363    self._scale(sc
-00013530: 616c 6529 0d0a 0d0a 2020 2020 6465 6620  ale)....    def 
-00013540: 7472 616e 735f 646f 776e 2873 656c 6629  trans_down(self)
-00013550: 3a0d 0a20 2020 2020 2020 2064 7820 3d20  :..        dx = 
-00013560: 300d 0a20 2020 2020 2020 2064 7920 3d20  0..        dy = 
-00013570: 7365 6c66 2e63 6f6e 7465 7874 2e6a 6f67  self.context.jog
-00013580: 5f61 6d6f 756e 740d 0a20 2020 2020 2020  _amount..       
-00013590: 2073 656c 662e 5f74 7261 6e73 6c61 7465   self._translate
-000135a0: 2864 782c 2064 792c 2031 290d 0a0d 0a20  (dx, dy, 1).... 
-000135b0: 2020 2064 6566 2074 7261 6e73 5f75 7028     def trans_up(
-000135c0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000135d0: 6478 203d 2030 0d0a 2020 2020 2020 2020  dx = 0..        
-000135e0: 6479 203d 2073 656c 662e 636f 6e74 6578  dy = self.contex
-000135f0: 742e 6a6f 675f 616d 6f75 6e74 0d0a 2020  t.jog_amount..  
-00013600: 2020 2020 2020 7365 6c66 2e5f 7472 616e        self._tran
-00013610: 736c 6174 6528 6478 2c20 6479 2c20 2d31  slate(dx, dy, -1
-00013620: 290d 0a0d 0a20 2020 2064 6566 2074 7261  )....    def tra
-00013630: 6e73 5f6c 6566 7428 7365 6c66 293a 0d0a  ns_left(self):..
-00013640: 2020 2020 2020 2020 6478 203d 2073 656c          dx = sel
-00013650: 662e 636f 6e74 6578 742e 6a6f 675f 616d  f.context.jog_am
-00013660: 6f75 6e74 0d0a 2020 2020 2020 2020 6479  ount..        dy
-00013670: 203d 2030 0d0a 2020 2020 2020 2020 7365   = 0..        se
-00013680: 6c66 2e5f 7472 616e 736c 6174 6528 6478  lf._translate(dx
-00013690: 2c20 6479 2c20 2d31 290d 0a0d 0a20 2020  , dy, -1)....   
-000136a0: 2064 6566 2074 7261 6e73 5f72 6967 6874   def trans_right
-000136b0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000136c0: 2064 7820 3d20 7365 6c66 2e63 6f6e 7465   dx = self.conte
-000136d0: 7874 2e6a 6f67 5f61 6d6f 756e 740d 0a20  xt.jog_amount.. 
-000136e0: 2020 2020 2020 2064 7920 3d20 300d 0a20         dy = 0.. 
-000136f0: 2020 2020 2020 2073 656c 662e 5f74 7261         self._tra
-00013700: 6e73 6c61 7465 2864 782c 2064 792c 2031  nslate(dx, dy, 1
-00013710: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
-00013720: 7472 616e 736c 6174 655f 7570 5f31 3028  translate_up_10(
-00013730: 7365 6c66 2c20 6576 656e 743d 4e6f 6e65  self, event=None
-00013740: 293a 2020 2320 7778 476c 6164 653a 204e  ):  # wxGlade: N
-00013750: 6176 6967 6174 696f 6e2e 3c65 7665 6e74  avigation.<event
-00013760: 5f68 616e 646c 6572 3e0d 0a20 2020 2020  _handler>..     
-00013770: 2020 2064 7820 3d20 300d 0a20 2020 2020     dx = 0..     
-00013780: 2020 2064 7920 3d20 7365 6c66 2e63 6f6e     dy = self.con
-00013790: 7465 7874 2e6a 6f67 5f61 6d6f 756e 7420  text.jog_amount 
-000137a0: 2a20 3130 0d0a 2020 2020 2020 2020 7365  * 10..        se
-000137b0: 6c66 2e5f 7472 616e 736c 6174 6528 6478  lf._translate(dx
-000137c0: 2c20 6479 2c20 2d31 3029 0d0a 0d0a 2020  , dy, -10)....  
-000137d0: 2020 6465 6620 6f6e 5f74 7261 6e73 6c61    def on_transla
-000137e0: 7465 5f6c 6566 745f 3130 2873 656c 662c  te_left_10(self,
-000137f0: 2065 7665 6e74 3d4e 6f6e 6529 3a20 2023   event=None):  #
-00013800: 2077 7847 6c61 6465 3a20 4e61 7669 6761   wxGlade: Naviga
-00013810: 7469 6f6e 2e3c 6576 656e 745f 6861 6e64  tion.<event_hand
-00013820: 6c65 723e 0d0a 2020 2020 2020 2020 6478  ler>..        dx
-00013830: 203d 2073 656c 662e 636f 6e74 6578 742e   = self.context.
-00013840: 6a6f 675f 616d 6f75 6e74 0d0a 2020 2020  jog_amount..    
-00013850: 2020 2020 6479 203d 2030 0d0a 2020 2020      dy = 0..    
-00013860: 2020 2020 7365 6c66 2e5f 7472 616e 736c      self._transl
-00013870: 6174 6528 6478 2c20 6479 2c20 2d31 3029  ate(dx, dy, -10)
-00013880: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f74  ....    def on_t
-00013890: 7261 6e73 6c61 7465 5f72 6967 6874 5f31  ranslate_right_1
-000138a0: 3028 7365 6c66 2c20 6576 656e 743d 4e6f  0(self, event=No
-000138b0: 6e65 293a 2020 2320 7778 476c 6164 653a  ne):  # wxGlade:
-000138c0: 204e 6176 6967 6174 696f 6e2e 3c65 7665   Navigation.<eve
-000138d0: 6e74 5f68 616e 646c 6572 3e0d 0a20 2020  nt_handler>..   
-000138e0: 2020 2020 2064 7820 3d20 7365 6c66 2e63       dx = self.c
-000138f0: 6f6e 7465 7874 2e6a 6f67 5f61 6d6f 756e  ontext.jog_amoun
-00013900: 740d 0a20 2020 2020 2020 2064 7920 3d20  t..        dy = 
-00013910: 300d 0a20 2020 2020 2020 2073 656c 662e  0..        self.
-00013920: 5f74 7261 6e73 6c61 7465 2864 782c 2064  _translate(dx, d
-00013930: 792c 2031 3029 0d0a 0d0a 2020 2020 6465  y, 10)....    de
-00013940: 6620 6f6e 5f74 7261 6e73 6c61 7465 5f64  f on_translate_d
-00013950: 6f77 6e5f 3130 2873 656c 662c 2065 7665  own_10(self, eve
-00013960: 6e74 3d4e 6f6e 6529 3a20 2023 2077 7847  nt=None):  # wxG
-00013970: 6c61 6465 3a20 4e61 7669 6761 7469 6f6e  lade: Navigation
-00013980: 2e3c 6576 656e 745f 6861 6e64 6c65 723e  .<event_handler>
-00013990: 0d0a 2020 2020 2020 2020 6478 203d 2030  ..        dx = 0
-000139a0: 0d0a 2020 2020 2020 2020 6479 203d 2073  ..        dy = s
-000139b0: 656c 662e 636f 6e74 6578 742e 6a6f 675f  elf.context.jog_
-000139c0: 616d 6f75 6e74 0d0a 2020 2020 2020 2020  amount..        
-000139d0: 7365 6c66 2e5f 7472 616e 736c 6174 6528  self._translate(
-000139e0: 6478 2c20 6479 2c20 3130 290d 0a0d 0a20  dx, dy, 10).... 
-000139f0: 2020 2064 6566 206f 6e5f 7265 7365 7428     def on_reset(
-00013a00: 7365 6c66 2c20 6576 656e 743d 4e6f 6e65  self, event=None
-00013a10: 293a 2020 2320 7778 476c 6164 653a 204e  ):  # wxGlade: N
-00013a20: 6176 6967 6174 696f 6e2e 3c65 7665 6e74  avigation.<event
-00013a30: 5f68 616e 646c 6572 3e0d 0a20 2020 2020  _handler>..     
-00013a40: 2020 2073 656c 662e 636f 6e74 6578 7428     self.context(
-00013a50: 2272 6573 6574 5c6e 2229 0d0a 2020 2020  "reset\n")..    
-00013a60: 2020 2020 7365 6c66 2e6d 6174 7269 785f      self.matrix_
-00013a70: 7570 6461 7465 6428 290d 0a0d 0a20 2020  updated()....   
-00013a80: 2064 6566 206f 6e5f 726f 7461 7465 5f63   def on_rotate_c
-00013a90: 6377 5f35 2873 656c 662c 2065 7665 6e74  cw_5(self, event
-00013aa0: 3d4e 6f6e 6529 3a20 2023 2077 7847 6c61  =None):  # wxGla
-00013ab0: 6465 3a20 4e61 7669 6761 7469 6f6e 2e3c  de: Navigation.<
-00013ac0: 6576 656e 745f 6861 6e64 6c65 723e 0d0a  event_handler>..
-00013ad0: 2020 2020 2020 2020 616e 676c 6520 3d20          angle = 
-00013ae0: 2d35 2e30 0d0a 2020 2020 2020 2020 7365  -5.0..        se
-00013af0: 6c66 2e5f 726f 7461 7465 2861 6e67 6c65  lf._rotate(angle
-00013b00: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
-00013b10: 726f 7461 7465 5f63 775f 3528 7365 6c66  rotate_cw_5(self
-00013b20: 2c20 6576 656e 743d 4e6f 6e65 293a 2020  , event=None):  
-00013b30: 2320 7778 476c 6164 653a 204e 6176 6967  # wxGlade: Navig
-00013b40: 6174 696f 6e2e 3c65 7665 6e74 5f68 616e  ation.<event_han
-00013b50: 646c 6572 3e0d 0a20 2020 2020 2020 2061  dler>..        a
-00013b60: 6e67 6c65 203d 2035 2e30 0d0a 2020 2020  ngle = 5.0..    
-00013b70: 2020 2020 7365 6c66 2e5f 726f 7461 7465      self._rotate
-00013b80: 2861 6e67 6c65 290d 0a0d 0a20 2020 2064  (angle)....    d
-00013b90: 6566 206f 6e5f 726f 7461 7465 5f63 6377  ef on_rotate_ccw
-00013ba0: 5f39 3028 7365 6c66 2c20 6576 656e 743d  _90(self, event=
-00013bb0: 4e6f 6e65 293a 2020 2320 7778 476c 6164  None):  # wxGlad
-00013bc0: 653a 204e 6176 6967 6174 696f 6e2e 3c65  e: Navigation.<e
-00013bd0: 7665 6e74 5f68 616e 646c 6572 3e0d 0a20  vent_handler>.. 
-00013be0: 2020 2020 2020 2061 6e67 6c65 203d 202d         angle = -
-00013bf0: 3930 2e30 0d0a 2020 2020 2020 2020 7365  90.0..        se
-00013c00: 6c66 2e5f 726f 7461 7465 2861 6e67 6c65  lf._rotate(angle
-00013c10: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
-00013c20: 726f 7461 7465 5f63 775f 3930 2873 656c  rotate_cw_90(sel
-00013c30: 662c 2065 7665 6e74 3d4e 6f6e 6529 3a20  f, event=None): 
-00013c40: 2023 2077 7847 6c61 6465 3a20 4e61 7669   # wxGlade: Navi
-00013c50: 6761 7469 6f6e 2e3c 6576 656e 745f 6861  gation.<event_ha
-00013c60: 6e64 6c65 723e 0d0a 2020 2020 2020 2020  ndler>..        
-00013c70: 616e 676c 6520 3d20 3930 2e30 0d0a 2020  angle = 90.0..  
-00013c80: 2020 2020 2020 7365 6c66 2e5f 726f 7461        self._rota
-00013c90: 7465 2861 6e67 6c65 290d 0a0d 0a20 2020  te(angle)....   
-00013ca0: 2040 7374 6174 6963 6d65 7468 6f64 0d0a   @staticmethod..
-00013cb0: 2020 2020 6465 6620 736b 6577 6564 5f76      def skewed_v
-00013cc0: 616c 7565 2873 7478 7429 3a0d 0a20 2020  alue(stxt):..   
-00013cd0: 2020 2020 2072 6574 7572 6e20 416e 676c       return Angl
-00013ce0: 652e 7061 7273 6528 7374 7874 292e 6173  e.parse(stxt).as
-00013cf0: 5f72 6164 6961 6e73 0d0a 0d0a 2020 2020  _radians....    
-00013d00: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
-00013d10: 2020 2064 6566 2073 6361 6c65 645f 7661     def scaled_va
-00013d20: 6c75 6528 7374 7874 293a 0d0a 2020 2020  lue(stxt):..    
-00013d30: 2020 2020 6966 2073 7478 742e 656e 6473      if stxt.ends
-00013d40: 7769 7468 2822 2522 293a 0d0a 2020 2020  with("%"):..    
-00013d50: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00013d60: 666c 6f61 7428 7374 7874 5b3a 2d31 5d29  float(stxt[:-1])
-00013d70: 202f 2031 3030 2e30 0d0a 2020 2020 2020   / 100.0..      
-00013d80: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00013d90: 2020 2020 2076 616c 7565 203d 2066 6c6f       value = flo
-00013da0: 6174 2873 7478 7429 0d0a 2020 2020 2020  at(stxt)..      
-00013db0: 2020 7265 7475 726e 2076 616c 7565 0d0a    return value..
-00013dc0: 0d0a 2020 2020 6465 6620 6f6e 5f74 6578  ..    def on_tex
-00013dd0: 745f 6d61 7472 6978 2873 656c 6629 3a0d  t_matrix(self):.
-00013de0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00013df0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
-00013e00: 5f78 203d 2073 656c 662e 7363 616c 6564  _x = self.scaled
-00013e10: 5f76 616c 7565 2873 656c 662e 7465 7874  _value(self.text
-00013e20: 5f61 2e47 6574 5661 6c75 6528 2929 0d0a  _a.GetValue())..
-00013e30: 2020 2020 2020 2020 2020 2020 736b 6577              skew
-00013e40: 5f78 203d 2073 656c 662e 736b 6577 6564  _x = self.skewed
-00013e50: 5f76 616c 7565 2873 656c 662e 7465 7874  _value(self.text
-00013e60: 5f63 2e47 6574 5661 6c75 6528 2929 0d0a  _c.GetValue())..
-00013e70: 2020 2020 2020 2020 2020 2020 7363 616c              scal
-00013e80: 655f 7920 3d20 7365 6c66 2e73 6361 6c65  e_y = self.scale
-00013e90: 645f 7661 6c75 6528 7365 6c66 2e74 6578  d_value(self.tex
-00013ea0: 745f 642e 4765 7456 616c 7565 2829 290d  t_d.GetValue()).
-00013eb0: 0a20 2020 2020 2020 2020 2020 2073 6b65  .            ske
-00013ec0: 775f 7920 3d20 7365 6c66 2e73 6b65 7765  w_y = self.skewe
-00013ed0: 645f 7661 6c75 6528 7365 6c66 2e74 6578  d_value(self.tex
-00013ee0: 745f 622e 4765 7456 616c 7565 2829 290d  t_b.GetValue()).
-00013ef0: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00013f00: 6e73 6c61 7465 5f78 203d 2066 6c6f 6174  nslate_x = float
-00013f10: 284c 656e 6774 6828 7365 6c66 2e74 6578  (Length(self.tex
-00013f20: 745f 652e 4765 7456 616c 7565 2829 2929  t_e.GetValue()))
-00013f30: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-00013f40: 616e 736c 6174 655f 7920 3d20 666c 6f61  anslate_y = floa
-00013f50: 7428 4c65 6e67 7468 2873 656c 662e 7465  t(Length(self.te
-00013f60: 7874 5f66 2e47 6574 5661 6c75 6528 2929  xt_f.GetValue())
-00013f70: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00013f80: 203d 2073 656c 662e 636f 6e74 6578 742e   = self.context.
-00013f90: 656c 656d 656e 7473 2e66 6972 7374 5f65  elements.first_e
-00013fa0: 6c65 6d65 6e74 2865 6d70 6861 7369 7a65  lement(emphasize
-00013fb0: 643d 5472 7565 290d 0a20 2020 2020 2020  d=True)..       
-00013fc0: 2020 2020 2069 6620 6620 6973 204e 6f6e       if f is Non
-00013fd0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00013fe0: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
-00013ff0: 2020 2020 2020 2020 6d61 7472 6978 203d          matrix =
-00014000: 2066 2e6d 6174 7269 780d 0a20 2020 2020   f.matrix..     
-00014010: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
-00014020: 2020 2020 2020 2020 2020 2020 2073 6361               sca
-00014030: 6c65 5f78 203d 3d20 6d61 7472 6978 2e61  le_x == matrix.a
-00014040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014050: 2020 616e 6420 736b 6577 5f79 203d 3d20    and skew_y == 
-00014060: 6d61 7472 6978 2e62 0d0a 2020 2020 2020  matrix.b..      
-00014070: 2020 2020 2020 2020 2020 616e 6420 736b            and sk
-00014080: 6577 5f78 203d 3d20 6d61 7472 6978 2e63  ew_x == matrix.c
-00014090: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000140a0: 2020 616e 6420 7363 616c 655f 7920 3d3d    and scale_y ==
-000140b0: 206d 6174 7269 782e 640d 0a20 2020 2020   matrix.d..     
-000140c0: 2020 2020 2020 2020 2020 2061 6e64 2074             and t
-000140d0: 7261 6e73 6c61 7465 5f78 203d 3d20 6d61  ranslate_x == ma
-000140e0: 7472 6978 2e65 0d0a 2020 2020 2020 2020  trix.e..        
-000140f0: 2020 2020 2020 2020 616e 6420 7472 616e          and tran
-00014100: 736c 6174 655f 7920 3d3d 206d 6174 7269  slate_y == matri
-00014110: 782e 660d 0a20 2020 2020 2020 2020 2020  x.f..           
-00014120: 2029 3a0d 0a20 2020 2020 2020 2020 2020   ):..           
-00014130: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00014140: 2020 2020 2020 2020 2023 2053 5647 2064           # SVG d
-00014150: 6566 696e 6573 2074 6865 2074 7261 6e73  efines the trans
-00014160: 666f 726d 6174 696f 6e20 4d61 7472 6978  formation Matrix
-00014170: 2061 7320 202d 204d 6174 7269 7820 7061   as  - Matrix pa
-00014180: 7261 6d65 7465 7273 2061 7265 0d0a 2020  rameters are..  
-00014190: 2020 2020 2020 2020 2020 2320 2053 6361            #  Sca
-000141a0: 6c65 2058 2020 2d20 536b 6577 2058 2020  le X  - Skew X  
-000141b0: 2d20 5472 616e 736c 6174 6520 5820 2020  - Translate X   
-000141c0: 2020 2020 2020 2020 2031 202d 2033 202d           1 - 3 -
-000141d0: 2035 0d0a 2020 2020 2020 2020 2020 2020   5..            
-000141e0: 2320 2053 6b65 7720 5920 2020 2d20 5363  #  Skew Y   - Sc
-000141f0: 616c 6520 5920 2d20 5472 616e 736c 6174  ale Y - Translat
-00014200: 6520 5920 2020 2020 2020 2020 2020 2032  e Y            2
-00014210: 202d 2034 202d 2036 0d0a 2020 2020 2020   - 4 - 6..      
-00014220: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00014230: 7874 280d 0a20 2020 2020 2020 2020 2020  xt(..           
-00014240: 2020 2020 2066 226d 6174 7269 7820 7b73       f"matrix {s
-00014250: 6361 6c65 5f78 7d20 7b73 6b65 775f 797d  cale_x} {skew_y}
-00014260: 207b 736b 6577 5f78 7d20 7b73 6361 6c65   {skew_x} {scale
-00014270: 5f79 7d20 7b74 7261 6e73 6c61 7465 5f78  _y} {translate_x
-00014280: 7d20 7b74 7261 6e73 6c61 7465 5f79 7d5c  } {translate_y}\
-00014290: 6e22 0d0a 2020 2020 2020 2020 2020 2020  n"..            
-000142a0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-000142b0: 656c 662e 636f 6e74 6578 742e 7369 676e  elf.context.sign
-000142c0: 616c 2822 7265 6672 6573 685f 7363 656e  al("refresh_scen
-000142d0: 6522 2c20 2253 6365 6e65 2229 0d0a 2020  e", "Scene")..  
-000142e0: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-000142f0: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
-00014300: 2020 2020 2020 7061 7373 0d0a 0d0a 2020        pass....  
-00014310: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
-00014320: 655f 6d61 7472 6978 5f74 6578 7428 290d  e_matrix_text().
-00014330: 0a0d 0a0d 0a63 6c61 7373 204a 6f67 4469  .....class JogDi
-00014340: 7374 616e 6365 5061 6e65 6c28 7778 2e50  stancePanel(wx.P
-00014350: 616e 656c 293a 0d0a 2020 2020 6465 6620  anel):..    def 
-00014360: 5f5f 696e 6974 5f5f 2873 656c 662c 202a  __init__(self, *
-00014370: 6172 6773 2c20 636f 6e74 6578 743d 4e6f  args, context=No
-00014380: 6e65 2c20 7061 6e65 3d46 616c 7365 2c20  ne, pane=False, 
-00014390: 2a2a 6b77 6473 293a 0d0a 2020 2020 2020  **kwds):..      
-000143a0: 2020 2320 6265 6769 6e20 7778 476c 6164    # begin wxGlad
-000143b0: 653a 204a 6f67 4469 7374 616e 6365 5061  e: JogDistancePa
-000143c0: 6e65 6c2e 5f5f 696e 6974 5f5f 0d0a 2020  nel.__init__..  
-000143d0: 2020 2020 2020 6b77 6473 5b22 7374 796c        kwds["styl
-000143e0: 6522 5d20 3d20 6b77 6473 2e67 6574 2822  e"] = kwds.get("
-000143f0: 7374 796c 6522 2c20 3029 207c 2077 782e  style", 0) | wx.
-00014400: 5441 425f 5452 4156 4552 5341 4c0d 0a20  TAB_TRAVERSAL.. 
-00014410: 2020 2020 2020 2077 782e 5061 6e65 6c2e         wx.Panel.
-00014420: 5f5f 696e 6974 5f5f 2873 656c 662c 202a  __init__(self, *
-00014430: 6172 6773 2c20 2a2a 6b77 6473 290d 0a20  args, **kwds).. 
-00014440: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00014450: 6578 7420 3d20 636f 6e74 6578 740d 0a20  ext = context.. 
-00014460: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-00014470: 5f6a 6f67 5f61 6d6f 756e 7420 3d20 5465  _jog_amount = Te
-00014480: 7874 4374 726c 280d 0a20 2020 2020 2020  xtCtrl(..       
-00014490: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-000144a0: 2020 2020 2020 2020 7778 2e49 445f 414e          wx.ID_AN
-000144b0: 592c 0d0a 2020 2020 2020 2020 2020 2020  Y,..            
-000144c0: 7374 796c 653d 7778 2e54 455f 5052 4f43  style=wx.TE_PROC
-000144d0: 4553 535f 454e 5445 522c 0d0a 2020 2020  ESS_ENTER,..    
-000144e0: 2020 2020 2020 2020 7661 6c75 653d 2231          value="1
-000144f0: 306d 6d22 2c0d 0a20 2020 2020 2020 2020  0mm",..         
-00014500: 2020 2063 6865 636b 3d22 6c65 6e67 7468     check="length
-00014510: 222c 0d0a 2020 2020 2020 2020 290d 0a20  ",..        ).. 
-00014520: 2020 2020 2020 206d 6169 6e5f 7369 7a65         main_size
-00014530: 7220 3d20 5374 6174 6963 426f 7853 697a  r = StaticBoxSiz
-00014540: 6572 2873 656c 662c 2077 782e 4944 5f41  er(self, wx.ID_A
-00014550: 4e59 2c20 5f28 224a 6f67 2044 6973 7461  NY, _("Jog Dista
-00014560: 6e63 653a 2229 2c20 7778 2e56 4552 5449  nce:"), wx.VERTI
-00014570: 4341 4c29 0d0a 2020 2020 2020 2020 6d61  CAL)..        ma
-00014580: 696e 5f73 697a 6572 2e41 6464 2873 656c  in_sizer.Add(sel
-00014590: 662e 7465 7874 5f6a 6f67 5f61 6d6f 756e  f.text_jog_amoun
-000145a0: 742c 2030 2c20 7778 2e45 5850 414e 442c  t, 0, wx.EXPAND,
-000145b0: 2030 290d 0a20 2020 2020 2020 2073 656c   0)..        sel
-000145c0: 662e 5365 7453 697a 6572 286d 6169 6e5f  f.SetSizer(main_
-000145d0: 7369 7a65 7229 0d0a 2020 2020 2020 2020  sizer)..        
-000145e0: 6d61 696e 5f73 697a 6572 2e46 6974 2873  main_sizer.Fit(s
-000145f0: 656c 6629 0d0a 2020 2020 2020 2020 7365  elf)..        se
-00014600: 6c66 2e4c 6179 6f75 7428 290d 0a0d 0a20  lf.Layout().... 
-00014610: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-00014620: 5f6a 6f67 5f61 6d6f 756e 742e 5365 7441  _jog_amount.SetA
-00014630: 6374 696f 6e52 6f75 7469 6e65 2873 656c  ctionRoutine(sel
-00014640: 662e 6f6e 5f74 6578 745f 6a6f 675f 616d  f.on_text_jog_am
-00014650: 6f75 6e74 290d 0a0d 0a20 2020 2064 6566  ount)....    def
-00014660: 2070 616e 655f 7368 6f77 2873 656c 662c   pane_show(self,
-00014670: 202a 6172 6773 293a 0d0a 2020 2020 2020   *args):..      
-00014680: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00014690: 2020 2020 6a6f 676c 656e 203d 204c 656e      joglen = Len
-000146a0: 6774 6828 0d0a 2020 2020 2020 2020 2020  gth(..          
-000146b0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-000146c0: 7874 2e6a 6f67 5f61 6d6f 756e 742c 0d0a  xt.jog_amount,..
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 6469 6769 7473 3d32 2c0d 0a20 2020 2020  digits=2,..     
-000146f0: 2020 2020 2020 2020 2020 2070 7265 6665             prefe
-00014700: 7272 6564 5f75 6e69 7473 3d73 656c 662e  rred_units=self.
-00014710: 636f 6e74 6578 742e 756e 6974 735f 6e61  context.units_na
-00014720: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-00014730: 2029 0d0a 2020 2020 2020 2020 6578 6365   )..        exce
-00014740: 7074 3a0d 0a20 2020 2020 2020 2020 2020  pt:..           
-00014750: 206a 6f67 6c65 6e20 3d20 4c65 6e67 7468   joglen = Length
-00014760: 2822 3130 6d6d 222c 2064 6967 6974 733d  ("10mm", digits=
-00014770: 322c 2070 7265 6665 7272 6564 5f75 6e69  2, preferred_uni
-00014780: 7473 3d73 656c 662e 636f 6e74 6578 742e  ts=self.context.
-00014790: 756e 6974 735f 6e61 6d65 290d 0a0d 0a20  units_name).... 
-000147a0: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-000147b0: 5f6a 6f67 5f61 6d6f 756e 742e 5365 7456  _jog_amount.SetV
-000147c0: 616c 7565 286a 6f67 6c65 6e2e 7072 6566  alue(joglen.pref
-000147d0: 6572 7265 645f 6c65 6e67 7468 290d 0a20  erred_length).. 
-000147e0: 2020 2020 2020 2073 656c 662e 4368 696c         self.Chil
-000147f0: 6472 656e 5b30 5d2e 5365 7446 6f63 7573  dren[0].SetFocus
-00014800: 2829 0d0a 0d0a 2020 2020 6465 6620 6f6e  ()....    def on
-00014810: 5f74 6578 745f 6a6f 675f 616d 6f75 6e74  _text_jog_amount
-00014820: 2873 656c 6629 3a20 2023 2077 7847 6c61  (self):  # wxGla
-00014830: 6465 3a20 4e61 7669 6761 7469 6f6e 2e3c  de: Navigation.<
-00014840: 6576 656e 745f 6861 6e64 6c65 723e 0d0a  event_handler>..
-00014850: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00014860: 2020 2020 2020 2020 2020 6a6f 6720 3d20            jog = 
-00014870: 7365 6c66 2e63 6f6e 7465 7874 2e64 6576  self.context.dev
-00014880: 6963 652e 6c65 6e67 7468 280d 0a20 2020  ice.length(..   
-00014890: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000148a0: 662e 7465 7874 5f6a 6f67 5f61 6d6f 756e  f.text_jog_amoun
-000148b0: 742e 4765 7456 616c 7565 2829 2c0d 0a20  t.GetValue(),.. 
-000148c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000148d0: 6577 5f75 6e69 7473 3d73 656c 662e 636f  ew_units=self.co
-000148e0: 6e74 6578 742e 756e 6974 735f 6e61 6d65  ntext.units_name
-000148f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014900: 2020 2075 6e69 746c 6573 733d 554e 4954     unitless=UNIT
-00014910: 535f 5045 525f 5049 5845 4c2c 0d0a 2020  S_PER_PIXEL,..  
-00014920: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
-00014930: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-00014940: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
-00014950: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00014960: 2020 2020 2073 656c 662e 636f 6e74 6578       self.contex
-00014970: 742e 6a6f 675f 616d 6f75 6e74 203d 2073  t.jog_amount = s
-00014980: 7472 286a 6f67 290d 0a20 2020 2020 2020  tr(jog)..       
-00014990: 2073 656c 662e 636f 6e74 6578 742e 7369   self.context.si
-000149a0: 676e 616c 2822 6a6f 675f 616d 6f75 6e74  gnal("jog_amount
-000149b0: 222c 2073 7472 286a 6f67 2929 0d0a 0d0a  ", str(jog))....
-000149c0: 0d0a 636c 6173 7320 4e61 7669 6761 7469  ..class Navigati
-000149d0: 6f6e 5061 6e65 6c28 7778 2e50 616e 656c  onPanel(wx.Panel
-000149e0: 293a 0d0a 2020 2020 6465 6620 5f5f 696e  ):..    def __in
-000149f0: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
-00014a00: 2c20 636f 6e74 6578 743d 4e6f 6e65 2c20  , context=None, 
-00014a10: 2a2a 6b77 6473 293a 0d0a 2020 2020 2020  **kwds):..      
-00014a20: 2020 6b77 6473 5b22 7374 796c 6522 5d20    kwds["style"] 
-00014a30: 3d20 6b77 6473 2e67 6574 2822 7374 796c  = kwds.get("styl
-00014a40: 6522 2c20 3029 207c 2077 782e 5441 425f  e", 0) | wx.TAB_
-00014a50: 5452 4156 4552 5341 4c0d 0a20 2020 2020  TRAVERSAL..     
-00014a60: 2020 2077 782e 5061 6e65 6c2e 5f5f 696e     wx.Panel.__in
-00014a70: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
-00014a80: 2c20 2a2a 6b77 6473 290d 0a20 2020 2020  , **kwds)..     
-00014a90: 2020 2073 656c 662e 636f 6e74 6578 7420     self.context 
-00014aa0: 3d20 636f 6e74 6578 740d 0a0d 0a20 2020  = context....   
-00014ab0: 2020 2020 206d 6169 6e5f 7369 7a65 7220       main_sizer 
-00014ac0: 3d20 7778 2e42 6f78 5369 7a65 7228 7778  = wx.BoxSizer(wx
-00014ad0: 2e56 4552 5449 4341 4c29 0d0a 0d0a 2020  .VERTICAL)....  
-00014ae0: 2020 2020 2020 7075 6c73 655f 616e 645f        pulse_and_
-00014af0: 6d6f 7665 5f73 697a 6572 203d 2077 782e  move_sizer = wx.
-00014b00: 426f 7853 697a 6572 2877 782e 484f 5249  BoxSizer(wx.HORI
-00014b10: 5a4f 4e54 414c 290d 0a20 2020 2020 2020  ZONTAL)..       
-00014b20: 206d 6169 6e5f 7061 6e65 6c73 5f73 697a   main_panels_siz
-00014b30: 6572 203d 2077 782e 426f 7853 697a 6572  er = wx.BoxSizer
-00014b40: 2877 782e 484f 5249 5a4f 4e54 414c 290d  (wx.HORIZONTAL).
-00014b50: 0a0d 0a20 2020 2020 2020 206a 6f67 6469  ...        jogdi
-00014b60: 7374 616e 6365 7061 6e65 6c20 3d20 4a6f  stancepanel = Jo
-00014b70: 6744 6973 7461 6e63 6550 616e 656c 2873  gDistancePanel(s
-00014b80: 656c 662c 2077 782e 4944 5f41 4e59 2c20  elf, wx.ID_ANY, 
-00014b90: 636f 6e74 6578 743d 7365 6c66 2e63 6f6e  context=self.con
-00014ba0: 7465 7874 290d 0a20 2020 2020 2020 206d  text)..        m
-00014bb0: 6169 6e5f 7369 7a65 722e 4164 6428 6a6f  ain_sizer.Add(jo
-00014bc0: 6764 6973 7461 6e63 6570 616e 656c 2c20  gdistancepanel, 
-00014bd0: 302c 2077 782e 4558 5041 4e44 2c20 3029  0, wx.EXPAND, 0)
-00014be0: 0d0a 0d0a 2020 2020 2020 2020 6e61 7669  ....        navi
-00014bf0: 6761 7469 6f6e 7061 6e65 6c20 3d20 4a6f  gationpanel = Jo
-00014c00: 6728 7365 6c66 2c20 7778 2e49 445f 414e  g(self, wx.ID_AN
-00014c10: 592c 2063 6f6e 7465 7874 3d73 656c 662e  Y, context=self.
-00014c20: 636f 6e74 6578 7429 0d0a 2020 2020 2020  context)..      
-00014c30: 2020 6d61 696e 5f70 616e 656c 735f 7369    main_panels_si
-00014c40: 7a65 722e 4164 6428 6e61 7669 6761 7469  zer.Add(navigati
-00014c50: 6f6e 7061 6e65 6c2c 2031 2c20 7778 2e45  onpanel, 1, wx.E
-00014c60: 5850 414e 442c 2030 290d 0a0d 0a20 2020  XPAND, 0)....   
-00014c70: 2020 2020 2061 6c69 676e 7061 6e65 6c20       alignpanel 
-00014c80: 3d20 4472 6167 2873 656c 662c 2077 782e  = Drag(self, wx.
-00014c90: 4944 5f41 4e59 2c20 636f 6e74 6578 743d  ID_ANY, context=
-00014ca0: 7365 6c66 2e63 6f6e 7465 7874 290d 0a20  self.context).. 
+000120b0: 0d0a 2020 2020 2320 546f 2067 6574 2075  ..    # To get u
+000120c0: 7064 6174 6573 2061 626f 7574 2074 7261  pdates about tra
+000120d0: 6e73 6c61 7469 6f6e 202f 2073 6361 6c69  nslation / scali
+000120e0: 6e67 206f 6620 7365 6c65 6374 6564 2065  ng of selected e
+000120f0: 6c65 6d65 6e74 730d 0a20 2020 2023 2077  lements..    # w
+00012100: 6520 6e65 6564 2074 6f20 6174 7461 6368  e need to attach
+00012110: 2074 6f20 736f 6d65 2073 6967 6e61 6c73   to some signals
+00012120: 2e2e 2e0d 0a20 2020 2040 7369 676e 616c  .....    @signal
+00012130: 5f6c 6973 7465 6e65 7228 2272 6566 7265  _listener("refre
+00012140: 7368 5f73 6365 6e65 2229 0d0a 2020 2020  sh_scene")..    
+00012150: 6465 6620 6f6e 5f72 6566 7265 7368 5f73  def on_refresh_s
+00012160: 6365 6e65 2873 656c 662c 206f 7269 6769  cene(self, origi
+00012170: 6e2c 2073 6365 6e65 5f6e 616d 653d 4e6f  n, scene_name=No
+00012180: 6e65 2c20 2a61 7267 7329 3a0d 0a20 2020  ne, *args):..   
+00012190: 2020 2020 2069 6620 7363 656e 655f 6e61       if scene_na
+000121a0: 6d65 203d 3d20 2253 6365 6e65 223a 0d0a  me == "Scene":..
+000121b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000121c0: 2e75 7064 6174 655f 6d61 7472 6978 5f74  .update_matrix_t
+000121d0: 6578 7428 290d 0a0d 0a20 2020 2040 7369  ext()....    @si
+000121e0: 676e 616c 5f6c 6973 7465 6e65 7228 2274  gnal_listener("t
+000121f0: 6f6f 6c5f 6d6f 6469 6669 6564 2229 0d0a  ool_modified")..
+00012200: 2020 2020 6465 6620 6f6e 5f6d 6f64 6966      def on_modif
+00012210: 6965 6428 7365 6c66 2c20 2a61 7267 7329  ied(self, *args)
+00012220: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+00012230: 7570 6461 7465 5f6d 6174 7269 785f 7465  update_matrix_te
+00012240: 7874 2829 0d0a 0d0a 2020 2020 6465 6620  xt()....    def 
+00012250: 7365 745f 7469 6d65 725f 6f70 7469 6f6e  set_timer_option
+00012260: 7328 7365 6c66 293a 0d0a 2020 2020 2020  s(self):..      
+00012270: 2020 696e 7465 7276 616c 203d 2073 656c    interval = sel
+00012280: 662e 636f 6e74 6578 742e 6275 7474 6f6e  f.context.button
+00012290: 5f72 6570 6561 740d 0a20 2020 2020 2020  _repeat..       
+000122a0: 2069 6620 696e 7465 7276 616c 2069 7320   if interval is 
+000122b0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000122c0: 2020 2069 6e74 6572 7661 6c20 3d20 302e     interval = 0.
+000122d0: 350d 0a20 2020 2020 2020 2069 6620 696e  5..        if in
+000122e0: 7465 7276 616c 203c 2030 3a0d 0a20 2020  terval < 0:..   
+000122f0: 2020 2020 2020 2020 2069 6e74 6572 7661           interva
+00012300: 6c20 3d20 300d 0a20 2020 2020 2020 2061  l = 0..        a
+00012310: 6363 656c 6572 6174 6520 3d20 7365 6c66  ccelerate = self
+00012320: 2e63 6f6e 7465 7874 2e62 7574 746f 6e5f  .context.button_
+00012330: 6163 6365 6c65 7261 7465 0d0a 2020 2020  accelerate..    
+00012340: 2020 2020 6966 2061 6363 656c 6572 6174      if accelerat
+00012350: 6520 6973 204e 6f6e 653a 0d0a 2020 2020  e is None:..    
+00012360: 2020 2020 2020 2020 6163 6365 6c65 7261          accelera
+00012370: 7465 203d 2054 7275 650d 0a20 2020 2020  te = True..     
+00012380: 2020 2073 656c 662e 7469 6d65 722e 696e     self.timer.in
+00012390: 7465 7276 616c 203d 2069 6e74 6572 7661  terval = interva
+000123a0: 6c0d 0a20 2020 2020 2020 2073 656c 662e  l..        self.
+000123b0: 7469 6d65 722e 6163 6365 6c65 7261 7465  timer.accelerate
+000123c0: 203d 2061 6363 656c 6572 6174 650d 0a0d   = accelerate...
+000123d0: 0a20 2020 2064 6566 206f 6e5f 6275 7474  .    def on_butt
+000123e0: 6f6e 5f72 6570 6561 7428 7365 6c66 2c20  on_repeat(self, 
+000123f0: 6f72 6967 696e 2c20 2a61 7267 7329 3a0d  origin, *args):.
+00012400: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00012410: 745f 7469 6d65 725f 6f70 7469 6f6e 7328  t_timer_options(
+00012420: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
+00012430: 6d6f 6469 6669 6564 5f65 6c65 6d65 6e74  modified_element
+00012440: 2873 656c 662c 206f 7269 6769 6e2c 202a  (self, origin, *
+00012450: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
+00012460: 7365 6c66 2e75 7064 6174 655f 6d61 7472  self.update_matr
+00012470: 6978 5f74 6578 7428 290d 0a0d 0a20 2020  ix_text()....   
+00012480: 2064 6566 206f 6e5f 656d 7068 6173 697a   def on_emphasiz
+00012490: 6564 5f65 6c65 6d65 6e74 735f 6368 616e  ed_elements_chan
+000124a0: 6765 6428 7365 6c66 2c20 6f72 6967 696e  ged(self, origin
+000124b0: 2c20 656c 656d 656e 7473 293a 0d0a 2020  , elements):..  
+000124c0: 2020 2020 2020 7365 6c66 2e73 656c 6563        self.selec
+000124d0: 745f 7265 6164 7928 7365 6c66 2e63 6f6e  t_ready(self.con
+000124e0: 7465 7874 2e65 6c65 6d65 6e74 732e 6861  text.elements.ha
+000124f0: 735f 656d 7068 6173 6973 2829 290d 0a20  s_emphasis()).. 
+00012500: 2020 2020 2020 2073 656c 662e 7570 6461         self.upda
+00012510: 7465 5f6d 6174 7269 785f 7465 7874 2829  te_matrix_text()
+00012520: 0d0a 0d0a 2020 2020 6465 6620 7570 6461  ....    def upda
+00012530: 7465 5f6d 6174 7269 785f 7465 7874 2873  te_matrix_text(s
+00012540: 656c 6629 3a0d 0a20 2020 2020 2020 2066  elf):..        f
+00012550: 203d 2073 656c 662e 636f 6e74 6578 742e   = self.context.
+00012560: 656c 656d 656e 7473 2e66 6972 7374 5f65  elements.first_e
+00012570: 6c65 6d65 6e74 2865 6d70 6861 7369 7a65  lement(emphasize
+00012580: 643d 5472 7565 290d 0a20 2020 2020 2020  d=True)..       
+00012590: 2076 203d 2066 2069 7320 6e6f 7420 4e6f   v = f is not No
+000125a0: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
+000125b0: 2e74 6578 745f 612e 456e 6162 6c65 2876  .text_a.Enable(v
+000125c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000125d0: 7465 7874 5f62 2e45 6e61 626c 6528 7629  text_b.Enable(v)
+000125e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+000125f0: 6578 745f 632e 456e 6162 6c65 2876 290d  ext_c.Enable(v).
+00012600: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
+00012610: 7874 5f64 2e45 6e61 626c 6528 7629 0d0a  xt_d.Enable(v)..
+00012620: 2020 2020 2020 2020 7365 6c66 2e74 6578          self.tex
+00012630: 745f 652e 456e 6162 6c65 2876 290d 0a20  t_e.Enable(v).. 
+00012640: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
+00012650: 5f66 2e45 6e61 626c 6528 7629 0d0a 2020  _f.Enable(v)..  
+00012660: 2020 2020 2020 6966 2076 3a0d 0a20 2020        if v:..   
+00012670: 2020 2020 2020 2020 206d 6174 7269 7820           matrix 
+00012680: 3d20 662e 6d61 7472 6978 0d0a 2020 2020  = f.matrix..    
+00012690: 2020 2020 2020 2020 2320 596f 7520 7769          # You wi
+000126a0: 6c6c 2067 6574 2073 6f6d 6574 696d 6573  ll get sometimes
+000126b0: 2073 6c69 6768 746c 7920 6469 6666 6572   slightly differ
+000126c0: 656e 7420 6e75 6d62 6572 7320 7468 616e  ent numbers than
+000126d0: 2079 6f75 2077 6f75 6c64 2065 7870 6563   you would expec
+000126e0: 7420 6475 6520 746f 2061 7269 7468 6d65  t due to arithme
+000126f0: 7469 6320 6f70 6572 6174 696f 6e73 0d0a  tic operations..
+00012700: 2020 2020 2020 2020 2020 2020 2320 7765              # we
+00012710: 2077 696c 6c20 7468 6572 6566 6f72 6520   will therefore 
+00012720: 2761 646a 7573 7427 2074 686f 7365 2066  'adjust' those f
+00012730: 6967 7572 6573 2073 6c69 6768 746c 7920  igures slightly 
+00012740: 746f 2061 766f 6964 2063 6f6e 6675 7369  to avoid confusi
+00012750: 6f6e 2062 7920 726f 756e 6469 6e67 2074  on by rounding t
+00012760: 6865 6d20 746f 2074 6865 2073 6978 7468  hem to the sixth
+00012770: 2064 6563 696d 616c 2028 6172 6269 7472   decimal (arbitr
+00012780: 6172 7929 0d0a 2020 2020 2020 2020 2020  ary)..          
+00012790: 2020 2320 7468 6174 2073 686f 756c 6420    # that should 
+000127a0: 6265 2067 6f6f 6420 656e 6f75 6768 2e2e  be good enough..
+000127b0: 2e0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+000127c0: 656c 662e 7465 7874 5f61 2e53 6574 5661  elf.text_a.SetVa
+000127d0: 6c75 6528 6622 7b6d 6174 7269 782e 613a  lue(f"{matrix.a:
+000127e0: 2e35 667d 2229 2020 2320 5363 616c 6520  .5f}")  # Scale 
+000127f0: 580d 0a20 2020 2020 2020 2020 2020 2073  X..            s
+00012800: 656c 662e 7465 7874 5f62 2e53 6574 5661  elf.text_b.SetVa
+00012810: 6c75 6528 6622 7b6d 6174 7269 782e 623a  lue(f"{matrix.b:
+00012820: 2e35 667d 2229 2020 2320 536b 6577 2059  .5f}")  # Skew Y
+00012830: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00012840: 6c66 2e74 6578 745f 632e 5365 7456 616c  lf.text_c.SetVal
+00012850: 7565 2866 227b 6d61 7472 6978 2e63 3a2e  ue(f"{matrix.c:.
+00012860: 3566 7d22 2920 2023 2053 6b65 7720 580d  5f}")  # Skew X.
+00012870: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00012880: 662e 7465 7874 5f64 2e53 6574 5661 6c75  f.text_d.SetValu
+00012890: 6528 6622 7b6d 6174 7269 782e 643a 2e35  e(f"{matrix.d:.5
+000128a0: 667d 2229 2020 2320 5363 616c 6520 590d  f}")  # Scale Y.
+000128b0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+000128c0: 7261 6e73 6c61 7465 2058 2026 2061 7265  ranslate X & are
+000128d0: 2069 6e20 6d69 6c73 2c20 736f 2061 626f   in mils, so abo
+000128e0: 7574 2030 2e30 3235 206d 6d2c 2073 6f20  ut 0.025 mm, so 
+000128f0: 3120 6469 6769 7420 7368 6f75 6c64 2062  1 digit should b
+00012900: 6520 6d6f 7265 2074 6861 6e20 656e 6f75  e more than enou
+00012910: 6768 2e2e 2e0d 0a20 2020 2020 2020 2020  gh.....         
+00012920: 2020 2023 2073 656c 662e 7465 7874 5f65     # self.text_e
+00012930: 2e53 6574 5661 6c75 6528 6622 7b6d 6174  .SetValue(f"{mat
+00012940: 7269 782e 653a 2e31 667d 2229 2020 2320  rix.e:.1f}")  # 
+00012950: 5472 616e 736c 6174 6520 580d 0a20 2020  Translate X..   
+00012960: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00012970: 7465 7874 5f66 2e53 6574 5661 6c75 6528  text_f.SetValue(
+00012980: 6622 7b6d 6174 7269 782e 663a 2e31 667d  f"{matrix.f:.1f}
+00012990: 2229 2020 2320 5472 616e 736c 6174 6520  ")  # Translate 
+000129a0: 590d 0a20 2020 2020 2020 2020 2020 206c  Y..            l
+000129b0: 3120 3d20 4c65 6e67 7468 280d 0a20 2020  1 = Length(..   
+000129c0: 2020 2020 2020 2020 2020 2020 2061 6d6f               amo
+000129d0: 756e 743d 6d61 7472 6978 2e65 2c20 6469  unt=matrix.e, di
+000129e0: 6769 7473 3d32 2c20 7072 6566 6572 7265  gits=2, preferre
+000129f0: 645f 756e 6974 733d 7365 6c66 2e63 6f6e  d_units=self.con
+00012a00: 7465 7874 2e75 6e69 7473 5f6e 616d 650d  text.units_name.
+00012a10: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00012a20: 2020 2020 2020 2020 2020 2020 6c32 203d              l2 =
+00012a30: 204c 656e 6774 6828 0d0a 2020 2020 2020   Length(..      
+00012a40: 2020 2020 2020 2020 2020 616d 6f75 6e74            amount
+00012a50: 3d6d 6174 7269 782e 662c 2064 6967 6974  =matrix.f, digit
+00012a60: 733d 322c 2070 7265 6665 7272 6564 5f75  s=2, preferred_u
+00012a70: 6e69 7473 3d73 656c 662e 636f 6e74 6578  nits=self.contex
+00012a80: 742e 756e 6974 735f 6e61 6d65 0d0a 2020  t.units_name..  
+00012a90: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00012aa0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00012ab0: 7874 5f65 2e53 6574 5661 6c75 6528 6c31  xt_e.SetValue(l1
+00012ac0: 2e70 7265 6665 7272 6564 5f6c 656e 6774  .preferred_lengt
+00012ad0: 6829 0d0a 2020 2020 2020 2020 2020 2020  h)..            
+00012ae0: 7365 6c66 2e74 6578 745f 662e 5365 7456  self.text_f.SetV
+00012af0: 616c 7565 286c 322e 7072 6566 6572 7265  alue(l2.preferre
+00012b00: 645f 6c65 6e67 7468 290d 0a20 2020 2020  d_length)..     
+00012b10: 2020 2020 2020 206d 5f65 203d 206d 6174         m_e = mat
+00012b20: 7269 782e 650d 0a20 2020 2020 2020 2020  rix.e..         
+00012b30: 2020 206d 5f66 203d 206d 6174 7269 782e     m_f = matrix.
+00012b40: 660d 0a20 2020 2020 2020 2020 2020 2074  f..            t
+00012b50: 7469 7031 203d 205f 280d 0a20 2020 2020  tip1 = _(..     
+00012b60: 2020 2020 2020 2020 2020 2022 5472 616e             "Tran
+00012b70: 736c 6174 6520 5820 2d20 6d6f 7665 7320  slate X - moves 
+00012b80: 7468 6520 656c 656d 656e 7420 6279 2074  the element by t
+00012b90: 6869 7320 616d 6f75 6e74 206f 6620 6d69  his amount of mi
+00012ba0: 6c73 2069 6e20 7468 6520 582d 6469 7265  ls in the X-dire
+00012bb0: 6374 696f 6e3b 2022 0d0a 2020 2020 2020  ction; "..      
+00012bc0: 2020 2020 2020 2020 2020 2279 6f75 206d            "you m
+00012bd0: 6179 2075 7365 2027 7265 616c 2720 6469  ay use 'real' di
+00012be0: 7374 616e 6365 7320 7768 656e 206d 6f64  stances when mod
+00012bf0: 6966 7969 6e67 2074 6869 7320 6661 6374  ifying this fact
+00012c00: 6f72 2c20 692e 652e 2032 696e 2c20 3363  or, i.e. 2in, 3c
+00012c10: 6d2c 2035 306d 6d22 0d0a 2020 2020 2020  m, 50mm"..      
+00012c20: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00012c30: 2020 2020 2074 7469 7031 203d 2074 7469       ttip1 = tti
+00012c40: 7031 202b 2022 5c6e 2220 2b20 5f28 2243  p1 + "\n" + _("C
+00012c50: 7572 7265 6e74 2069 6e74 6572 6e61 6c20  urrent internal 
+00012c60: 7661 6c75 653a 2022 2920 2b20 6622 7b6d  value: ") + f"{m
+00012c70: 5f65 3a2e 3166 7d22 0d0a 2020 2020 2020  _e:.1f}"..      
+00012c80: 2020 2020 2020 7474 6970 3220 3d20 5f28        ttip2 = _(
+00012c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012ca0: 2020 2254 7261 6e73 6c61 7465 2059 202d    "Translate Y -
+00012cb0: 206d 6f76 6573 2074 6865 2065 6c65 6d65   moves the eleme
+00012cc0: 6e74 2062 7920 7468 6973 2061 6d6f 756e  nt by this amoun
+00012cd0: 7420 6f66 206d 696c 7320 696e 2074 6865  t of mils in the
+00012ce0: 2059 2d64 6972 6563 7469 6f6e 3b20 220d   Y-direction; ".
+00012cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d00: 2022 796f 7520 6d61 7920 7573 6520 2772   "you may use 'r
+00012d10: 6561 6c27 2064 6973 7461 6e63 6573 2077  eal' distances w
+00012d20: 6865 6e20 6d6f 6469 6679 696e 6720 7468  hen modifying th
+00012d30: 6973 2066 6163 746f 722c 2069 2e65 2e20  is factor, i.e. 
+00012d40: 3269 6e2c 2033 636d 2c20 3530 6d6d 220d  2in, 3cm, 50mm".
+00012d50: 0a20 2020 2020 2020 2020 2020 2029 0d0a  .            )..
+00012d60: 2020 2020 2020 2020 2020 2020 7474 6970              ttip
+00012d70: 3220 3d20 7474 6970 3220 2b20 225c 6e22  2 = ttip2 + "\n"
+00012d80: 202b 205f 2822 4375 7272 656e 7420 696e   + _("Current in
+00012d90: 7465 726e 616c 2076 616c 7565 3a20 2229  ternal value: ")
+00012da0: 202b 2066 227b 6d5f 663a 2e31 667d 220d   + f"{m_f:.1f}".
+00012db0: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+00012dc0: 656c 662e 7465 7874 5f65 2e53 6574 546f  elf.text_e.SetTo
+00012dd0: 6f6c 5469 7028 7474 6970 3129 0d0a 2020  olTip(ttip1)..  
+00012de0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00012df0: 6578 745f 662e 5365 7454 6f6f 6c54 6970  ext_f.SetToolTip
+00012e00: 2874 7469 7032 290d 0a0d 0a20 2020 2064  (ttip2)....    d
+00012e10: 6566 2073 656c 6563 745f 7265 6164 7928  ef select_ready(
+00012e20: 7365 6c66 2c20 7629 3a0d 0a20 2020 2020  self, v):..     
+00012e30: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00012e40: 456e 6162 6c65 7320 7468 6520 7265 6c65  Enables the rele
+00012e50: 7661 6e74 2062 7574 746f 6e73 2077 6865  vant buttons whe
+00012e60: 6e20 7468 6572 6520 6973 2061 2073 656c  n there is a sel
+00012e70: 6563 7469 6f6e 2069 6e20 7468 6520 656c  ection in the el
+00012e80: 656d 656e 7473 2e0d 0a20 2020 2020 2020  ements...       
+00012e90: 2040 7061 7261 6d20 763a 2077 6865 7468   @param v: wheth
+00012ea0: 6572 2073 656c 6563 7469 6f6e 2069 7320  er selection is 
+00012eb0: 6375 7272 656e 746c 7920 6472 6167 2072  currently drag r
+00012ec0: 6561 6479 2e0d 0a20 2020 2020 2020 2040  eady...        @
+00012ed0: 7265 7475 726e 3a0d 0a20 2020 2020 2020  return:..       
+00012ee0: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
+00012ef0: 6c66 2e62 7574 746f 6e5f 7363 616c 655f  lf.button_scale_
+00012f00: 646f 776e 2e45 6e61 626c 6528 7629 0d0a  down.Enable(v)..
+00012f10: 2020 2020 2020 2020 7365 6c66 2e62 7574          self.but
+00012f20: 746f 6e5f 7363 616c 655f 7570 2e45 6e61  ton_scale_up.Ena
+00012f30: 626c 6528 7629 0d0a 2020 2020 2020 2020  ble(v)..        
+00012f40: 7365 6c66 2e62 7574 746f 6e5f 726f 7461  self.button_rota
+00012f50: 7465 5f63 6377 2e45 6e61 626c 6528 7629  te_ccw.Enable(v)
+00012f60: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00012f70: 7574 746f 6e5f 726f 7461 7465 5f63 772e  utton_rotate_cw.
+00012f80: 456e 6162 6c65 2876 290d 0a20 2020 2020  Enable(v)..     
+00012f90: 2020 2073 656c 662e 6275 7474 6f6e 5f74     self.button_t
+00012fa0: 7261 6e73 6c61 7465 5f64 6f77 6e2e 456e  ranslate_down.En
+00012fb0: 6162 6c65 2876 290d 0a20 2020 2020 2020  able(v)..       
+00012fc0: 2073 656c 662e 6275 7474 6f6e 5f74 7261   self.button_tra
+00012fd0: 6e73 6c61 7465 5f75 702e 456e 6162 6c65  nslate_up.Enable
+00012fe0: 2876 290d 0a20 2020 2020 2020 2073 656c  (v)..        sel
+00012ff0: 662e 6275 7474 6f6e 5f74 7261 6e73 6c61  f.button_transla
+00013000: 7465 5f6c 6566 742e 456e 6162 6c65 2876  te_left.Enable(v
+00013010: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00013020: 6275 7474 6f6e 5f74 7261 6e73 6c61 7465  button_translate
+00013030: 5f72 6967 6874 2e45 6e61 626c 6528 7629  _right.Enable(v)
+00013040: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
+00013050: 7574 746f 6e5f 7265 7365 742e 456e 6162  utton_reset.Enab
+00013060: 6c65 2876 290d 0a0d 0a20 2020 2064 6566  le(v)....    def
+00013070: 206d 6174 7269 785f 7570 6461 7465 6428   matrix_updated(
+00013080: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00013090: 7365 6c66 2e63 6f6e 7465 7874 2e65 6c65  self.context.ele
+000130a0: 6d65 6e74 732e 7369 676e 616c 2822 7265  ments.signal("re
+000130b0: 6672 6573 685f 7363 656e 6522 2c20 2253  fresh_scene", "S
+000130c0: 6365 6e65 2229 0d0a 2020 2020 2020 2020  cene")..        
+000130d0: 7365 6c66 2e75 7064 6174 655f 6d61 7472  self.update_matr
+000130e0: 6978 5f74 6578 7428 290d 0a0d 0a20 2020  ix_text()....   
+000130f0: 2064 6566 205f 7363 616c 6528 7365 6c66   def _scale(self
+00013100: 2c20 7363 616c 6529 3a0d 0a20 2020 2020  , scale):..     
+00013110: 2020 2073 656c 662e 636f 6e74 6578 7428     self.context(
+00013120: 6622 7363 616c 6520 7b73 6361 6c65 7d20  f"scale {scale} 
+00013130: 7b73 6361 6c65 7d20 5c6e 2229 0d0a 2020  {scale} \n")..  
+00013140: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00013150: 7874 2e65 6c65 6d65 6e74 732e 7369 676e  xt.elements.sign
+00013160: 616c 2822 6578 742d 6d6f 6469 6669 6564  al("ext-modified
+00013170: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
+00013180: 2e6d 6174 7269 785f 7570 6461 7465 6428  .matrix_updated(
+00013190: 290d 0a0d 0a20 2020 2064 6566 205f 726f  )....    def _ro
+000131a0: 7461 7465 2873 656c 662c 2061 6e67 6c65  tate(self, angle
+000131b0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+000131c0: 2e63 6f6e 7465 7874 2866 2272 6f74 6174  .context(f"rotat
+000131d0: 6520 7b61 6e67 6c65 7d64 6567 205c 6e22  e {angle}deg \n"
+000131e0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000131f0: 636f 6e74 6578 742e 656c 656d 656e 7473  context.elements
+00013200: 2e73 6967 6e61 6c28 2265 7874 2d6d 6f64  .signal("ext-mod
+00013210: 6966 6965 6422 290d 0a20 2020 2020 2020  ified")..       
+00013220: 2073 656c 662e 6d61 7472 6978 5f75 7064   self.matrix_upd
+00013230: 6174 6564 2829 0d0a 0d0a 2020 2020 6465  ated()....    de
+00013240: 6620 5f74 7261 6e73 6c61 7465 2873 656c  f _translate(sel
+00013250: 662c 2064 782c 2064 792c 2073 6361 6c65  f, dx, dy, scale
+00013260: 293a 0d0a 2020 2020 2020 2020 6478 203d  ):..        dx =
+00013270: 2073 656c 662e 636f 6e74 6578 742e 6465   self.context.de
+00013280: 7669 6365 2e6c 656e 6774 6828 0d0a 2020  vice.length(..  
+00013290: 2020 2020 2020 2020 2020 6478 2c0d 0a20            dx,.. 
+000132a0: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+000132b0: 2020 2020 2020 2020 2020 2073 6361 6c65             scale
+000132c0: 3d73 6361 6c65 2c0d 0a20 2020 2020 2020  =scale,..       
+000132d0: 2020 2020 206e 6577 5f75 6e69 7473 3d73       new_units=s
+000132e0: 656c 662e 636f 6e74 6578 742e 756e 6974  elf.context.unit
+000132f0: 735f 6e61 6d65 2c0d 0a20 2020 2020 2020  s_name,..       
+00013300: 2020 2020 2075 6e69 746c 6573 733d 554e       unitless=UN
+00013310: 4954 535f 5045 525f 5049 5845 4c2c 0d0a  ITS_PER_PIXEL,..
+00013320: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00013330: 2020 2064 7920 3d20 7365 6c66 2e63 6f6e     dy = self.con
+00013340: 7465 7874 2e64 6576 6963 652e 6c65 6e67  text.device.leng
+00013350: 7468 280d 0a20 2020 2020 2020 2020 2020  th(..           
+00013360: 2064 792c 0d0a 2020 2020 2020 2020 2020   dy,..          
+00013370: 2020 312c 0d0a 2020 2020 2020 2020 2020    1,..          
+00013380: 2020 7363 616c 653d 7363 616c 652c 0d0a    scale=scale,..
+00013390: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+000133a0: 756e 6974 733d 7365 6c66 2e63 6f6e 7465  units=self.conte
+000133b0: 7874 2e75 6e69 7473 5f6e 616d 652c 0d0a  xt.units_name,..
+000133c0: 2020 2020 2020 2020 2020 2020 756e 6974              unit
+000133d0: 6c65 7373 3d55 4e49 5453 5f50 4552 5f50  less=UNITS_PER_P
+000133e0: 4958 454c 2c0d 0a20 2020 2020 2020 2029  IXEL,..        )
+000133f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00013400: 6f6e 7465 7874 2866 2274 7261 6e73 6c61  ontext(f"transla
+00013410: 7465 207b 6478 7d20 7b64 797d 5c6e 2229  te {dx} {dy}\n")
+00013420: 0d0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
+00013430: 6f6e 7465 7874 2e65 6c65 6d65 6e74 732e  ontext.elements.
+00013440: 7369 676e 616c 2822 6578 742d 6d6f 6469  signal("ext-modi
+00013450: 6669 6564 2229 0d0a 2020 2020 2020 2020  fied")..        
+00013460: 7365 6c66 2e6d 6174 7269 785f 7570 6461  self.matrix_upda
+00013470: 7465 6428 290d 0a0d 0a20 2020 2064 6566  ted()....    def
+00013480: 206f 6e5f 7363 616c 655f 646f 776e 5f35   on_scale_down_5
+00013490: 3028 7365 6c66 2c20 6576 656e 743d 4e6f  0(self, event=No
+000134a0: 6e65 293a 2020 2320 7778 476c 6164 653a  ne):  # wxGlade:
+000134b0: 204e 6176 6967 6174 696f 6e2e 3c65 7665   Navigation.<eve
+000134c0: 6e74 5f68 616e 646c 6572 3e0d 0a20 2020  nt_handler>..   
+000134d0: 2020 2020 2073 6361 6c65 203d 2032 2e30       scale = 2.0
+000134e0: 202f 2033 2e30 2020 2320 3636 2e36 2520   / 3.0  # 66.6% 
+000134f0: 2d20 696e 7665 7273 6520 6f66 2031 3530  - inverse of 150
+00013500: 250d 0a20 2020 2020 2020 2073 656c 662e  %..        self.
+00013510: 5f73 6361 6c65 2873 6361 6c65 290d 0a0d  _scale(scale)...
+00013520: 0a20 2020 2064 6566 206f 6e5f 7363 616c  .    def on_scal
+00013530: 655f 7570 5f35 3028 7365 6c66 2c20 6576  e_up_50(self, ev
+00013540: 656e 743d 4e6f 6e65 293a 2020 2320 7778  ent=None):  # wx
+00013550: 476c 6164 653a 204e 6176 6967 6174 696f  Glade: Navigatio
+00013560: 6e2e 3c65 7665 6e74 5f68 616e 646c 6572  n.<event_handler
+00013570: 3e0d 0a20 2020 2020 2020 2073 6361 6c65  >..        scale
+00013580: 203d 2033 2e30 202f 2032 2e30 2020 2320   = 3.0 / 2.0  # 
+00013590: 3135 3025 0d0a 2020 2020 2020 2020 7365  150%..        se
+000135a0: 6c66 2e5f 7363 616c 6528 7363 616c 6529  lf._scale(scale)
+000135b0: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f73  ....    def on_s
+000135c0: 6361 6c65 5f64 6f77 6e5f 3528 7365 6c66  cale_down_5(self
+000135d0: 2c20 6576 656e 743d 4e6f 6e65 293a 2020  , event=None):  
+000135e0: 2320 7778 476c 6164 653a 204e 6176 6967  # wxGlade: Navig
+000135f0: 6174 696f 6e2e 3c65 7665 6e74 5f68 616e  ation.<event_han
+00013600: 646c 6572 3e0d 0a20 2020 2020 2020 2073  dler>..        s
+00013610: 6361 6c65 203d 2031 392e 3020 2f20 3230  cale = 19.0 / 20
+00013620: 2e30 0d0a 2020 2020 2020 2020 7365 6c66  .0..        self
+00013630: 2e5f 7363 616c 6528 7363 616c 6529 0d0a  ._scale(scale)..
+00013640: 0d0a 2020 2020 6465 6620 6f6e 5f73 6361  ..    def on_sca
+00013650: 6c65 5f75 705f 3528 7365 6c66 2c20 6576  le_up_5(self, ev
+00013660: 656e 743d 4e6f 6e65 293a 2020 2320 7778  ent=None):  # wx
+00013670: 476c 6164 653a 204e 6176 6967 6174 696f  Glade: Navigatio
+00013680: 6e2e 3c65 7665 6e74 5f68 616e 646c 6572  n.<event_handler
+00013690: 3e0d 0a20 2020 2020 2020 2073 6361 6c65  >..        scale
+000136a0: 203d 2032 302e 3020 2f20 3139 2e30 0d0a   = 20.0 / 19.0..
+000136b0: 2020 2020 2020 2020 7365 6c66 2e5f 7363          self._sc
+000136c0: 616c 6528 7363 616c 6529 0d0a 0d0a 2020  ale(scale)....  
+000136d0: 2020 6465 6620 7472 616e 735f 646f 776e    def trans_down
+000136e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000136f0: 2064 7820 3d20 300d 0a20 2020 2020 2020   dx = 0..       
+00013700: 2064 7920 3d20 7365 6c66 2e63 6f6e 7465   dy = self.conte
+00013710: 7874 2e6a 6f67 5f61 6d6f 756e 740d 0a20  xt.jog_amount.. 
+00013720: 2020 2020 2020 2073 656c 662e 5f74 7261         self._tra
+00013730: 6e73 6c61 7465 2864 782c 2064 792c 2031  nslate(dx, dy, 1
+00013740: 290d 0a0d 0a20 2020 2064 6566 2074 7261  )....    def tra
+00013750: 6e73 5f75 7028 7365 6c66 293a 0d0a 2020  ns_up(self):..  
+00013760: 2020 2020 2020 6478 203d 2030 0d0a 2020        dx = 0..  
+00013770: 2020 2020 2020 6479 203d 2073 656c 662e        dy = self.
+00013780: 636f 6e74 6578 742e 6a6f 675f 616d 6f75  context.jog_amou
+00013790: 6e74 0d0a 2020 2020 2020 2020 7365 6c66  nt..        self
+000137a0: 2e5f 7472 616e 736c 6174 6528 6478 2c20  ._translate(dx, 
+000137b0: 6479 2c20 2d31 290d 0a0d 0a20 2020 2064  dy, -1)....    d
+000137c0: 6566 2074 7261 6e73 5f6c 6566 7428 7365  ef trans_left(se
+000137d0: 6c66 293a 0d0a 2020 2020 2020 2020 6478  lf):..        dx
+000137e0: 203d 2073 656c 662e 636f 6e74 6578 742e   = self.context.
+000137f0: 6a6f 675f 616d 6f75 6e74 0d0a 2020 2020  jog_amount..    
+00013800: 2020 2020 6479 203d 2030 0d0a 2020 2020      dy = 0..    
+00013810: 2020 2020 7365 6c66 2e5f 7472 616e 736c      self._transl
+00013820: 6174 6528 6478 2c20 6479 2c20 2d31 290d  ate(dx, dy, -1).
+00013830: 0a0d 0a20 2020 2064 6566 2074 7261 6e73  ...    def trans
+00013840: 5f72 6967 6874 2873 656c 6629 3a0d 0a20  _right(self):.. 
+00013850: 2020 2020 2020 2064 7820 3d20 7365 6c66         dx = self
+00013860: 2e63 6f6e 7465 7874 2e6a 6f67 5f61 6d6f  .context.jog_amo
+00013870: 756e 740d 0a20 2020 2020 2020 2064 7920  unt..        dy 
+00013880: 3d20 300d 0a20 2020 2020 2020 2073 656c  = 0..        sel
+00013890: 662e 5f74 7261 6e73 6c61 7465 2864 782c  f._translate(dx,
+000138a0: 2064 792c 2031 290d 0a0d 0a20 2020 2064   dy, 1)....    d
+000138b0: 6566 206f 6e5f 7472 616e 736c 6174 655f  ef on_translate_
+000138c0: 7570 5f31 3028 7365 6c66 2c20 6576 656e  up_10(self, even
+000138d0: 743d 4e6f 6e65 293a 2020 2320 7778 476c  t=None):  # wxGl
+000138e0: 6164 653a 204e 6176 6967 6174 696f 6e2e  ade: Navigation.
+000138f0: 3c65 7665 6e74 5f68 616e 646c 6572 3e0d  <event_handler>.
+00013900: 0a20 2020 2020 2020 2064 7820 3d20 300d  .        dx = 0.
+00013910: 0a20 2020 2020 2020 2064 7920 3d20 7365  .        dy = se
+00013920: 6c66 2e63 6f6e 7465 7874 2e6a 6f67 5f61  lf.context.jog_a
+00013930: 6d6f 756e 7420 2a20 3130 0d0a 2020 2020  mount * 10..    
+00013940: 2020 2020 7365 6c66 2e5f 7472 616e 736c      self._transl
+00013950: 6174 6528 6478 2c20 6479 2c20 2d31 3029  ate(dx, dy, -10)
+00013960: 0d0a 0d0a 2020 2020 6465 6620 6f6e 5f74  ....    def on_t
+00013970: 7261 6e73 6c61 7465 5f6c 6566 745f 3130  ranslate_left_10
+00013980: 2873 656c 662c 2065 7665 6e74 3d4e 6f6e  (self, event=Non
+00013990: 6529 3a20 2023 2077 7847 6c61 6465 3a20  e):  # wxGlade: 
+000139a0: 4e61 7669 6761 7469 6f6e 2e3c 6576 656e  Navigation.<even
+000139b0: 745f 6861 6e64 6c65 723e 0d0a 2020 2020  t_handler>..    
+000139c0: 2020 2020 6478 203d 2073 656c 662e 636f      dx = self.co
+000139d0: 6e74 6578 742e 6a6f 675f 616d 6f75 6e74  ntext.jog_amount
+000139e0: 0d0a 2020 2020 2020 2020 6479 203d 2030  ..        dy = 0
+000139f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00013a00: 7472 616e 736c 6174 6528 6478 2c20 6479  translate(dx, dy
+00013a10: 2c20 2d31 3029 0d0a 0d0a 2020 2020 6465  , -10)....    de
+00013a20: 6620 6f6e 5f74 7261 6e73 6c61 7465 5f72  f on_translate_r
+00013a30: 6967 6874 5f31 3028 7365 6c66 2c20 6576  ight_10(self, ev
+00013a40: 656e 743d 4e6f 6e65 293a 2020 2320 7778  ent=None):  # wx
+00013a50: 476c 6164 653a 204e 6176 6967 6174 696f  Glade: Navigatio
+00013a60: 6e2e 3c65 7665 6e74 5f68 616e 646c 6572  n.<event_handler
+00013a70: 3e0d 0a20 2020 2020 2020 2064 7820 3d20  >..        dx = 
+00013a80: 7365 6c66 2e63 6f6e 7465 7874 2e6a 6f67  self.context.jog
+00013a90: 5f61 6d6f 756e 740d 0a20 2020 2020 2020  _amount..       
+00013aa0: 2064 7920 3d20 300d 0a20 2020 2020 2020   dy = 0..       
+00013ab0: 2073 656c 662e 5f74 7261 6e73 6c61 7465   self._translate
+00013ac0: 2864 782c 2064 792c 2031 3029 0d0a 0d0a  (dx, dy, 10)....
+00013ad0: 2020 2020 6465 6620 6f6e 5f74 7261 6e73      def on_trans
+00013ae0: 6c61 7465 5f64 6f77 6e5f 3130 2873 656c  late_down_10(sel
+00013af0: 662c 2065 7665 6e74 3d4e 6f6e 6529 3a20  f, event=None): 
+00013b00: 2023 2077 7847 6c61 6465 3a20 4e61 7669   # wxGlade: Navi
+00013b10: 6761 7469 6f6e 2e3c 6576 656e 745f 6861  gation.<event_ha
+00013b20: 6e64 6c65 723e 0d0a 2020 2020 2020 2020  ndler>..        
+00013b30: 6478 203d 2030 0d0a 2020 2020 2020 2020  dx = 0..        
+00013b40: 6479 203d 2073 656c 662e 636f 6e74 6578  dy = self.contex
+00013b50: 742e 6a6f 675f 616d 6f75 6e74 0d0a 2020  t.jog_amount..  
+00013b60: 2020 2020 2020 7365 6c66 2e5f 7472 616e        self._tran
+00013b70: 736c 6174 6528 6478 2c20 6479 2c20 3130  slate(dx, dy, 10
+00013b80: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
+00013b90: 7265 7365 7428 7365 6c66 2c20 6576 656e  reset(self, even
+00013ba0: 743d 4e6f 6e65 293a 2020 2320 7778 476c  t=None):  # wxGl
+00013bb0: 6164 653a 204e 6176 6967 6174 696f 6e2e  ade: Navigation.
+00013bc0: 3c65 7665 6e74 5f68 616e 646c 6572 3e0d  <event_handler>.
+00013bd0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00013be0: 6e74 6578 7428 2272 6573 6574 5c6e 2229  ntext("reset\n")
+00013bf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e6d  ..        self.m
+00013c00: 6174 7269 785f 7570 6461 7465 6428 290d  atrix_updated().
+00013c10: 0a0d 0a20 2020 2064 6566 206f 6e5f 726f  ...    def on_ro
+00013c20: 7461 7465 5f63 6377 5f35 2873 656c 662c  tate_ccw_5(self,
+00013c30: 2065 7665 6e74 3d4e 6f6e 6529 3a20 2023   event=None):  #
+00013c40: 2077 7847 6c61 6465 3a20 4e61 7669 6761   wxGlade: Naviga
+00013c50: 7469 6f6e 2e3c 6576 656e 745f 6861 6e64  tion.<event_hand
+00013c60: 6c65 723e 0d0a 2020 2020 2020 2020 616e  ler>..        an
+00013c70: 676c 6520 3d20 2d35 2e30 0d0a 2020 2020  gle = -5.0..    
+00013c80: 2020 2020 7365 6c66 2e5f 726f 7461 7465      self._rotate
+00013c90: 2861 6e67 6c65 290d 0a0d 0a20 2020 2064  (angle)....    d
+00013ca0: 6566 206f 6e5f 726f 7461 7465 5f63 775f  ef on_rotate_cw_
+00013cb0: 3528 7365 6c66 2c20 6576 656e 743d 4e6f  5(self, event=No
+00013cc0: 6e65 293a 2020 2320 7778 476c 6164 653a  ne):  # wxGlade:
+00013cd0: 204e 6176 6967 6174 696f 6e2e 3c65 7665   Navigation.<eve
+00013ce0: 6e74 5f68 616e 646c 6572 3e0d 0a20 2020  nt_handler>..   
+00013cf0: 2020 2020 2061 6e67 6c65 203d 2035 2e30       angle = 5.0
+00013d00: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00013d10: 726f 7461 7465 2861 6e67 6c65 290d 0a0d  rotate(angle)...
+00013d20: 0a20 2020 2064 6566 206f 6e5f 726f 7461  .    def on_rota
+00013d30: 7465 5f63 6377 5f39 3028 7365 6c66 2c20  te_ccw_90(self, 
+00013d40: 6576 656e 743d 4e6f 6e65 293a 2020 2320  event=None):  # 
+00013d50: 7778 476c 6164 653a 204e 6176 6967 6174  wxGlade: Navigat
+00013d60: 696f 6e2e 3c65 7665 6e74 5f68 616e 646c  ion.<event_handl
+00013d70: 6572 3e0d 0a20 2020 2020 2020 2061 6e67  er>..        ang
+00013d80: 6c65 203d 202d 3930 2e30 0d0a 2020 2020  le = -90.0..    
+00013d90: 2020 2020 7365 6c66 2e5f 726f 7461 7465      self._rotate
+00013da0: 2861 6e67 6c65 290d 0a0d 0a20 2020 2064  (angle)....    d
+00013db0: 6566 206f 6e5f 726f 7461 7465 5f63 775f  ef on_rotate_cw_
+00013dc0: 3930 2873 656c 662c 2065 7665 6e74 3d4e  90(self, event=N
+00013dd0: 6f6e 6529 3a20 2023 2077 7847 6c61 6465  one):  # wxGlade
+00013de0: 3a20 4e61 7669 6761 7469 6f6e 2e3c 6576  : Navigation.<ev
+00013df0: 656e 745f 6861 6e64 6c65 723e 0d0a 2020  ent_handler>..  
+00013e00: 2020 2020 2020 616e 676c 6520 3d20 3930        angle = 90
+00013e10: 2e30 0d0a 2020 2020 2020 2020 7365 6c66  .0..        self
+00013e20: 2e5f 726f 7461 7465 2861 6e67 6c65 290d  ._rotate(angle).
+00013e30: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+00013e40: 7468 6f64 0d0a 2020 2020 6465 6620 736b  thod..    def sk
+00013e50: 6577 6564 5f76 616c 7565 2873 7478 7429  ewed_value(stxt)
+00013e60: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00013e70: 6e20 416e 676c 652e 7061 7273 6528 7374  n Angle.parse(st
+00013e80: 7874 292e 6173 5f72 6164 6961 6e73 0d0a  xt).as_radians..
+00013e90: 0d0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00013ea0: 686f 640d 0a20 2020 2064 6566 2073 6361  hod..    def sca
+00013eb0: 6c65 645f 7661 6c75 6528 7374 7874 293a  led_value(stxt):
+00013ec0: 0d0a 2020 2020 2020 2020 6966 2073 7478  ..        if stx
+00013ed0: 742e 656e 6473 7769 7468 2822 2522 293a  t.endswith("%"):
+00013ee0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00013ef0: 6c75 6520 3d20 666c 6f61 7428 7374 7874  lue = float(stxt
+00013f00: 5b3a 2d31 5d29 202f 2031 3030 2e30 0d0a  [:-1]) / 100.0..
+00013f10: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00013f20: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00013f30: 203d 2066 6c6f 6174 2873 7478 7429 0d0a   = float(stxt)..
+00013f40: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00013f50: 616c 7565 0d0a 0d0a 2020 2020 6465 6620  alue....    def 
+00013f60: 6f6e 5f74 6578 745f 6d61 7472 6978 2873  on_text_matrix(s
+00013f70: 656c 6629 3a0d 0a20 2020 2020 2020 2074  elf):..        t
+00013f80: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+00013f90: 2073 6361 6c65 5f78 203d 2073 656c 662e   scale_x = self.
+00013fa0: 7363 616c 6564 5f76 616c 7565 2873 656c  scaled_value(sel
+00013fb0: 662e 7465 7874 5f61 2e47 6574 5661 6c75  f.text_a.GetValu
+00013fc0: 6528 2929 0d0a 2020 2020 2020 2020 2020  e())..          
+00013fd0: 2020 736b 6577 5f78 203d 2073 656c 662e    skew_x = self.
+00013fe0: 736b 6577 6564 5f76 616c 7565 2873 656c  skewed_value(sel
+00013ff0: 662e 7465 7874 5f63 2e47 6574 5661 6c75  f.text_c.GetValu
+00014000: 6528 2929 0d0a 2020 2020 2020 2020 2020  e())..          
+00014010: 2020 7363 616c 655f 7920 3d20 7365 6c66    scale_y = self
+00014020: 2e73 6361 6c65 645f 7661 6c75 6528 7365  .scaled_value(se
+00014030: 6c66 2e74 6578 745f 642e 4765 7456 616c  lf.text_d.GetVal
+00014040: 7565 2829 290d 0a20 2020 2020 2020 2020  ue())..         
+00014050: 2020 2073 6b65 775f 7920 3d20 7365 6c66     skew_y = self
+00014060: 2e73 6b65 7765 645f 7661 6c75 6528 7365  .skewed_value(se
+00014070: 6c66 2e74 6578 745f 622e 4765 7456 616c  lf.text_b.GetVal
+00014080: 7565 2829 290d 0a20 2020 2020 2020 2020  ue())..         
+00014090: 2020 2074 7261 6e73 6c61 7465 5f78 203d     translate_x =
+000140a0: 2066 6c6f 6174 284c 656e 6774 6828 7365   float(Length(se
+000140b0: 6c66 2e74 6578 745f 652e 4765 7456 616c  lf.text_e.GetVal
+000140c0: 7565 2829 2929 0d0a 2020 2020 2020 2020  ue()))..        
+000140d0: 2020 2020 7472 616e 736c 6174 655f 7920      translate_y 
+000140e0: 3d20 666c 6f61 7428 4c65 6e67 7468 2873  = float(Length(s
+000140f0: 656c 662e 7465 7874 5f66 2e47 6574 5661  elf.text_f.GetVa
+00014100: 6c75 6528 2929 290d 0a20 2020 2020 2020  lue()))..       
+00014110: 2020 2020 2066 203d 2073 656c 662e 636f       f = self.co
+00014120: 6e74 6578 742e 656c 656d 656e 7473 2e66  ntext.elements.f
+00014130: 6972 7374 5f65 6c65 6d65 6e74 2865 6d70  irst_element(emp
+00014140: 6861 7369 7a65 643d 5472 7565 290d 0a20  hasized=True).. 
+00014150: 2020 2020 2020 2020 2020 2069 6620 6620             if f 
+00014160: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00014170: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014180: 0d0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
+00014190: 7472 6978 203d 2066 2e6d 6174 7269 780d  trix = f.matrix.
+000141a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000141b0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+000141c0: 2020 2073 6361 6c65 5f78 203d 3d20 6d61     scale_x == ma
+000141d0: 7472 6978 2e61 0d0a 2020 2020 2020 2020  trix.a..        
+000141e0: 2020 2020 2020 2020 616e 6420 736b 6577          and skew
+000141f0: 5f79 203d 3d20 6d61 7472 6978 2e62 0d0a  _y == matrix.b..
+00014200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014210: 616e 6420 736b 6577 5f78 203d 3d20 6d61  and skew_x == ma
+00014220: 7472 6978 2e63 0d0a 2020 2020 2020 2020  trix.c..        
+00014230: 2020 2020 2020 2020 616e 6420 7363 616c          and scal
+00014240: 655f 7920 3d3d 206d 6174 7269 782e 640d  e_y == matrix.d.
+00014250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014260: 2061 6e64 2074 7261 6e73 6c61 7465 5f78   and translate_x
+00014270: 203d 3d20 6d61 7472 6978 2e65 0d0a 2020   == matrix.e..  
+00014280: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00014290: 6420 7472 616e 736c 6174 655f 7920 3d3d  d translate_y ==
+000142a0: 206d 6174 7269 782e 660d 0a20 2020 2020   matrix.f..     
+000142b0: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+000142c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000142d0: 6e0d 0a20 2020 2020 2020 2020 2020 2023  n..            #
+000142e0: 2053 5647 2064 6566 696e 6573 2074 6865   SVG defines the
+000142f0: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+00014300: 4d61 7472 6978 2061 7320 202d 204d 6174  Matrix as  - Mat
+00014310: 7269 7820 7061 7261 6d65 7465 7273 2061  rix parameters a
+00014320: 7265 0d0a 2020 2020 2020 2020 2020 2020  re..            
+00014330: 2320 2053 6361 6c65 2058 2020 2d20 536b  #  Scale X  - Sk
+00014340: 6577 2058 2020 2d20 5472 616e 736c 6174  ew X  - Translat
+00014350: 6520 5820 2020 2020 2020 2020 2020 2031  e X            1
+00014360: 202d 2033 202d 2035 0d0a 2020 2020 2020   - 3 - 5..      
+00014370: 2020 2020 2020 2320 2053 6b65 7720 5920        #  Skew Y 
+00014380: 2020 2d20 5363 616c 6520 5920 2d20 5472    - Scale Y - Tr
+00014390: 616e 736c 6174 6520 5920 2020 2020 2020  anslate Y       
+000143a0: 2020 2020 2032 202d 2034 202d 2036 0d0a       2 - 4 - 6..
+000143b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000143c0: 2e63 6f6e 7465 7874 280d 0a20 2020 2020  .context(..     
+000143d0: 2020 2020 2020 2020 2020 2066 226d 6174             f"mat
+000143e0: 7269 7820 7b73 6361 6c65 5f78 7d20 7b73  rix {scale_x} {s
+000143f0: 6b65 775f 797d 207b 736b 6577 5f78 7d20  kew_y} {skew_x} 
+00014400: 7b73 6361 6c65 5f79 7d20 7b74 7261 6e73  {scale_y} {trans
+00014410: 6c61 7465 5f78 7d20 7b74 7261 6e73 6c61  late_x} {transla
+00014420: 7465 5f79 7d5c 6e22 0d0a 2020 2020 2020  te_y}\n"..      
+00014430: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+00014440: 2020 2020 2073 656c 662e 636f 6e74 6578       self.contex
+00014450: 742e 7369 676e 616c 2822 7265 6672 6573  t.signal("refres
+00014460: 685f 7363 656e 6522 2c20 2253 6365 6e65  h_scene", "Scene
+00014470: 2229 0d0a 2020 2020 2020 2020 6578 6365  ")..        exce
+00014480: 7074 2056 616c 7565 4572 726f 723a 0d0a  pt ValueError:..
+00014490: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+000144a0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+000144b0: 2e75 7064 6174 655f 6d61 7472 6978 5f74  .update_matrix_t
+000144c0: 6578 7428 290d 0a0d 0a0d 0a63 6c61 7373  ext()......class
+000144d0: 204a 6f67 4469 7374 616e 6365 5061 6e65   JogDistancePane
+000144e0: 6c28 7778 2e50 616e 656c 293a 0d0a 2020  l(wx.Panel):..  
+000144f0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00014500: 656c 662c 202a 6172 6773 2c20 636f 6e74  elf, *args, cont
+00014510: 6578 743d 4e6f 6e65 2c20 7061 6e65 3d46  ext=None, pane=F
+00014520: 616c 7365 2c20 2a2a 6b77 6473 293a 0d0a  alse, **kwds):..
+00014530: 2020 2020 2020 2020 2320 6265 6769 6e20          # begin 
+00014540: 7778 476c 6164 653a 204a 6f67 4469 7374  wxGlade: JogDist
+00014550: 616e 6365 5061 6e65 6c2e 5f5f 696e 6974  ancePanel.__init
+00014560: 5f5f 0d0a 2020 2020 2020 2020 6b77 6473  __..        kwds
+00014570: 5b22 7374 796c 6522 5d20 3d20 6b77 6473  ["style"] = kwds
+00014580: 2e67 6574 2822 7374 796c 6522 2c20 3029  .get("style", 0)
+00014590: 207c 2077 782e 5441 425f 5452 4156 4552   | wx.TAB_TRAVER
+000145a0: 5341 4c0d 0a20 2020 2020 2020 2077 782e  SAL..        wx.
+000145b0: 5061 6e65 6c2e 5f5f 696e 6974 5f5f 2873  Panel.__init__(s
+000145c0: 656c 662c 202a 6172 6773 2c20 2a2a 6b77  elf, *args, **kw
+000145d0: 6473 290d 0a20 2020 2020 2020 2073 656c  ds)..        sel
+000145e0: 662e 636f 6e74 6578 7420 3d20 636f 6e74  f.context = cont
+000145f0: 6578 740d 0a20 2020 2020 2020 2073 656c  ext..        sel
+00014600: 662e 7465 7874 5f6a 6f67 5f61 6d6f 756e  f.text_jog_amoun
+00014610: 7420 3d20 5465 7874 4374 726c 280d 0a20  t = TextCtrl(.. 
+00014620: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00014630: 0d0a 2020 2020 2020 2020 2020 2020 7778  ..            wx
+00014640: 2e49 445f 414e 592c 0d0a 2020 2020 2020  .ID_ANY,..      
+00014650: 2020 2020 2020 7374 796c 653d 7778 2e54        style=wx.T
+00014660: 455f 5052 4f43 4553 535f 454e 5445 522c  E_PROCESS_ENTER,
+00014670: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00014680: 6c75 653d 2231 306d 6d22 2c0d 0a20 2020  lue="10mm",..   
+00014690: 2020 2020 2020 2020 2063 6865 636b 3d22           check="
+000146a0: 6c65 6e67 7468 222c 0d0a 2020 2020 2020  length",..      
+000146b0: 2020 290d 0a20 2020 2020 2020 206d 6169    )..        mai
+000146c0: 6e5f 7369 7a65 7220 3d20 5374 6174 6963  n_sizer = Static
+000146d0: 426f 7853 697a 6572 2873 656c 662c 2077  BoxSizer(self, w
+000146e0: 782e 4944 5f41 4e59 2c20 5f28 224a 6f67  x.ID_ANY, _("Jog
+000146f0: 2044 6973 7461 6e63 653a 2229 2c20 7778   Distance:"), wx
+00014700: 2e56 4552 5449 4341 4c29 0d0a 2020 2020  .VERTICAL)..    
+00014710: 2020 2020 6d61 696e 5f73 697a 6572 2e41      main_sizer.A
+00014720: 6464 2873 656c 662e 7465 7874 5f6a 6f67  dd(self.text_jog
+00014730: 5f61 6d6f 756e 742c 2030 2c20 7778 2e45  _amount, 0, wx.E
+00014740: 5850 414e 442c 2030 290d 0a20 2020 2020  XPAND, 0)..     
+00014750: 2020 2073 656c 662e 5365 7453 697a 6572     self.SetSizer
+00014760: 286d 6169 6e5f 7369 7a65 7229 0d0a 2020  (main_sizer)..  
+00014770: 2020 2020 2020 6d61 696e 5f73 697a 6572        main_sizer
+00014780: 2e46 6974 2873 656c 6629 0d0a 2020 2020  .Fit(self)..    
+00014790: 2020 2020 7365 6c66 2e4c 6179 6f75 7428      self.Layout(
+000147a0: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+000147b0: 662e 7465 7874 5f6a 6f67 5f61 6d6f 756e  f.text_jog_amoun
+000147c0: 742e 5365 7441 6374 696f 6e52 6f75 7469  t.SetActionRouti
+000147d0: 6e65 2873 656c 662e 6f6e 5f74 6578 745f  ne(self.on_text_
+000147e0: 6a6f 675f 616d 6f75 6e74 290d 0a0d 0a20  jog_amount).... 
+000147f0: 2020 2064 6566 2070 616e 655f 7368 6f77     def pane_show
+00014800: 2873 656c 662c 202a 6172 6773 293a 0d0a  (self, *args):..
+00014810: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00014820: 2020 2020 2020 2020 2020 6a6f 676c 656e            joglen
+00014830: 203d 204c 656e 6774 6828 0d0a 2020 2020   = Length(..    
+00014840: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014850: 2e63 6f6e 7465 7874 2e6a 6f67 5f61 6d6f  .context.jog_amo
+00014860: 756e 742c 0d0a 2020 2020 2020 2020 2020  unt,..          
+00014870: 2020 2020 2020 6469 6769 7473 3d32 2c0d        digits=2,.
+00014880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014890: 2070 7265 6665 7272 6564 5f75 6e69 7473   preferred_units
+000148a0: 3d73 656c 662e 636f 6e74 6578 742e 756e  =self.context.un
+000148b0: 6974 735f 6e61 6d65 2c0d 0a20 2020 2020  its_name,..     
+000148c0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000148d0: 2020 6578 6365 7074 3a0d 0a20 2020 2020    except:..     
+000148e0: 2020 2020 2020 206a 6f67 6c65 6e20 3d20         joglen = 
+000148f0: 4c65 6e67 7468 2822 3130 6d6d 222c 2064  Length("10mm", d
+00014900: 6967 6974 733d 322c 2070 7265 6665 7272  igits=2, preferr
+00014910: 6564 5f75 6e69 7473 3d73 656c 662e 636f  ed_units=self.co
+00014920: 6e74 6578 742e 756e 6974 735f 6e61 6d65  ntext.units_name
+00014930: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+00014940: 662e 7465 7874 5f6a 6f67 5f61 6d6f 756e  f.text_jog_amoun
+00014950: 742e 5365 7456 616c 7565 286a 6f67 6c65  t.SetValue(jogle
+00014960: 6e2e 7072 6566 6572 7265 645f 6c65 6e67  n.preferred_leng
+00014970: 7468 290d 0a20 2020 2020 2020 2073 656c  th)..        sel
+00014980: 662e 4368 696c 6472 656e 5b30 5d2e 5365  f.Children[0].Se
+00014990: 7446 6f63 7573 2829 0d0a 0d0a 2020 2020  tFocus()....    
+000149a0: 6465 6620 6f6e 5f74 6578 745f 6a6f 675f  def on_text_jog_
+000149b0: 616d 6f75 6e74 2873 656c 6629 3a20 2023  amount(self):  #
+000149c0: 2077 7847 6c61 6465 3a20 4e61 7669 6761   wxGlade: Naviga
+000149d0: 7469 6f6e 2e3c 6576 656e 745f 6861 6e64  tion.<event_hand
+000149e0: 6c65 723e 0d0a 2020 2020 2020 2020 7472  ler>..        tr
+000149f0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00014a00: 6a6f 6720 3d20 7365 6c66 2e63 6f6e 7465  jog = self.conte
+00014a10: 7874 2e64 6576 6963 652e 6c65 6e67 7468  xt.device.length
+00014a20: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00014a30: 2020 2073 656c 662e 7465 7874 5f6a 6f67     self.text_jog
+00014a40: 5f61 6d6f 756e 742e 4765 7456 616c 7565  _amount.GetValue
+00014a50: 2829 2c0d 0a20 2020 2020 2020 2020 2020  (),..           
+00014a60: 2020 2020 206e 6577 5f75 6e69 7473 3d73       new_units=s
+00014a70: 656c 662e 636f 6e74 6578 742e 756e 6974  elf.context.unit
+00014a80: 735f 6e61 6d65 2c0d 0a20 2020 2020 2020  s_name,..       
+00014a90: 2020 2020 2020 2020 2075 6e69 746c 6573           unitles
+00014aa0: 733d 554e 4954 535f 5045 525f 5049 5845  s=UNITS_PER_PIXE
+00014ab0: 4c2c 0d0a 2020 2020 2020 2020 2020 2020  L,..            
+00014ac0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00014ad0: 7420 5661 6c75 6545 7272 6f72 3a0d 0a20  t ValueError:.. 
+00014ae0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014af0: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+00014b00: 636f 6e74 6578 742e 6a6f 675f 616d 6f75  context.jog_amou
+00014b10: 6e74 203d 2073 7472 286a 6f67 290d 0a20  nt = str(jog).. 
+00014b20: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00014b30: 6578 742e 7369 676e 616c 2822 6a6f 675f  ext.signal("jog_
+00014b40: 616d 6f75 6e74 222c 2073 7472 286a 6f67  amount", str(jog
+00014b50: 2929 0d0a 0d0a 0d0a 636c 6173 7320 4e61  ))......class Na
+00014b60: 7669 6761 7469 6f6e 5061 6e65 6c28 7778  vigationPanel(wx
+00014b70: 2e50 616e 656c 293a 0d0a 2020 2020 6465  .Panel):..    de
+00014b80: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00014b90: 202a 6172 6773 2c20 636f 6e74 6578 743d   *args, context=
+00014ba0: 4e6f 6e65 2c20 2a2a 6b77 6473 293a 0d0a  None, **kwds):..
+00014bb0: 2020 2020 2020 2020 6b77 6473 5b22 7374          kwds["st
+00014bc0: 796c 6522 5d20 3d20 6b77 6473 2e67 6574  yle"] = kwds.get
+00014bd0: 2822 7374 796c 6522 2c20 3029 207c 2077  ("style", 0) | w
+00014be0: 782e 5441 425f 5452 4156 4552 5341 4c0d  x.TAB_TRAVERSAL.
+00014bf0: 0a20 2020 2020 2020 2077 782e 5061 6e65  .        wx.Pane
+00014c00: 6c2e 5f5f 696e 6974 5f5f 2873 656c 662c  l.__init__(self,
+00014c10: 202a 6172 6773 2c20 2a2a 6b77 6473 290d   *args, **kwds).
+00014c20: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00014c30: 6e74 6578 7420 3d20 636f 6e74 6578 740d  ntext = context.
+00014c40: 0a0d 0a20 2020 2020 2020 206d 6169 6e5f  ...        main_
+00014c50: 7369 7a65 7220 3d20 7778 2e42 6f78 5369  sizer = wx.BoxSi
+00014c60: 7a65 7228 7778 2e56 4552 5449 4341 4c29  zer(wx.VERTICAL)
+00014c70: 0d0a 0d0a 2020 2020 2020 2020 7075 6c73  ....        puls
+00014c80: 655f 616e 645f 6d6f 7665 5f73 697a 6572  e_and_move_sizer
+00014c90: 203d 2077 782e 426f 7853 697a 6572 2877   = wx.BoxSizer(w
+00014ca0: 782e 484f 5249 5a4f 4e54 414c 290d 0a20  x.HORIZONTAL).. 
 00014cb0: 2020 2020 2020 206d 6169 6e5f 7061 6e65         main_pane
-00014cc0: 6c73 5f73 697a 6572 2e41 6464 2861 6c69  ls_sizer.Add(ali
-00014cd0: 676e 7061 6e65 6c2c 2031 2c20 7778 2e45  gnpanel, 1, wx.E
-00014ce0: 5850 414e 442c 2030 290d 0a0d 0a20 2020  XPAND, 0)....   
-00014cf0: 2020 2020 2074 7261 6e73 666f 726d 7061       transformpa
-00014d00: 6e65 6c20 3d20 5472 616e 7366 6f72 6d28  nel = Transform(
-00014d10: 7365 6c66 2c20 7778 2e49 445f 414e 592c  self, wx.ID_ANY,
-00014d20: 2063 6f6e 7465 7874 3d73 656c 662e 636f   context=self.co
-00014d30: 6e74 6578 7429 0d0a 0d0a 2020 2020 2020  ntext)....      
-00014d40: 2020 6d61 696e 5f70 616e 656c 735f 7369    main_panels_si
-00014d50: 7a65 722e 4164 6428 7472 616e 7366 6f72  zer.Add(transfor
-00014d60: 6d70 616e 656c 2c20 302c 2030 2c20 3029  mpanel, 0, 0, 0)
-00014d70: 0d0a 2020 2020 2020 2020 6d61 696e 5f73  ..        main_s
-00014d80: 697a 6572 2e41 6464 286d 6169 6e5f 7061  izer.Add(main_pa
-00014d90: 6e65 6c73 5f73 697a 6572 2c20 302c 2077  nels_sizer, 0, w
-00014da0: 782e 4558 5041 4e44 2c20 3029 0d0a 0d0a  x.EXPAND, 0)....
-00014db0: 2020 2020 2020 2020 7368 6f72 745f 7075          short_pu
-00014dc0: 6c73 6520 3d20 5075 6c73 6550 616e 656c  lse = PulsePanel
-00014dd0: 2873 656c 662c 2077 782e 4944 5f41 4e59  (self, wx.ID_ANY
-00014de0: 2c20 636f 6e74 6578 743d 7365 6c66 2e63  , context=self.c
-00014df0: 6f6e 7465 7874 290d 0a20 2020 2020 2020  ontext)..       
-00014e00: 2070 756c 7365 5f61 6e64 5f6d 6f76 655f   pulse_and_move_
-00014e10: 7369 7a65 722e 4164 6428 7368 6f72 745f  sizer.Add(short_
-00014e20: 7075 6c73 652c 2031 2c20 7778 2e45 5850  pulse, 1, wx.EXP
-00014e30: 414e 442c 2030 290d 0a0d 0a20 2020 2020  AND, 0)....     
-00014e40: 2020 206d 6f76 655f 7061 6e65 6c20 3d20     move_panel = 
-00014e50: 4d6f 7665 5061 6e65 6c28 7365 6c66 2c20  MovePanel(self, 
-00014e60: 7778 2e49 445f 414e 592c 2063 6f6e 7465  wx.ID_ANY, conte
-00014e70: 7874 3d73 656c 662e 636f 6e74 6578 7429  xt=self.context)
-00014e80: 0d0a 2020 2020 2020 2020 7075 6c73 655f  ..        pulse_
-00014e90: 616e 645f 6d6f 7665 5f73 697a 6572 2e41  and_move_sizer.A
-00014ea0: 6464 286d 6f76 655f 7061 6e65 6c2c 2031  dd(move_panel, 1
-00014eb0: 2c20 7778 2e45 5850 414e 442c 2030 290d  , wx.EXPAND, 0).
-00014ec0: 0a0d 0a20 2020 2020 2020 2073 697a 655f  ...        size_
-00014ed0: 7061 6e65 6c20 3d20 506f 7369 7469 6f6e  panel = Position
-00014ee0: 5061 6e65 6c28 7365 6c66 2c20 7778 2e49  Panel(self, wx.I
-00014ef0: 445f 414e 592c 2063 6f6e 7465 7874 3d73  D_ANY, context=s
-00014f00: 656c 662e 636f 6e74 6578 742c 2073 6d61  elf.context, sma
-00014f10: 6c6c 3d54 7275 6529 0d0a 2020 2020 2020  ll=True)..      
-00014f20: 2020 7075 6c73 655f 616e 645f 6d6f 7665    pulse_and_move
-00014f30: 5f73 697a 6572 2e41 6464 2873 697a 655f  _sizer.Add(size_
-00014f40: 7061 6e65 6c2c 2031 2c20 7778 2e45 5850  panel, 1, wx.EXP
-00014f50: 414e 442c 2030 290d 0a0d 0a20 2020 2020  AND, 0)....     
-00014f60: 2020 206d 6169 6e5f 7369 7a65 722e 4164     main_sizer.Ad
-00014f70: 6428 7075 6c73 655f 616e 645f 6d6f 7665  d(pulse_and_move
-00014f80: 5f73 697a 6572 2c20 302c 2077 782e 4558  _sizer, 0, wx.EX
-00014f90: 5041 4e44 2c20 3029 0d0a 2020 2020 2020  PAND, 0)..      
-00014fa0: 2020 7365 6c66 2e53 6574 5369 7a65 7228    self.SetSizer(
-00014fb0: 6d61 696e 5f73 697a 6572 290d 0a20 2020  main_sizer)..   
-00014fc0: 2020 2020 2073 656c 662e 4c61 796f 7574       self.Layout
-00014fd0: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00014fe0: 2e70 616e 656c 7320 3d20 5b0d 0a20 2020  .panels = [..   
-00014ff0: 2020 2020 2020 2020 206a 6f67 6469 7374           jogdist
-00015000: 616e 6365 7061 6e65 6c2c 0d0a 2020 2020  ancepanel,..    
-00015010: 2020 2020 2020 2020 6e61 7669 6761 7469          navigati
-00015020: 6f6e 7061 6e65 6c2c 0d0a 2020 2020 2020  onpanel,..      
-00015030: 2020 2020 2020 616c 6967 6e70 616e 656c        alignpanel
-00015040: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
-00015050: 7261 6e73 666f 726d 7061 6e65 6c2c 0d0a  ransformpanel,..
-00015060: 2020 2020 2020 2020 2020 2020 7368 6f72              shor
-00015070: 745f 7075 6c73 652c 0d0a 2020 2020 2020  t_pulse,..      
-00015080: 2020 2020 2020 6d6f 7665 5f70 616e 656c        move_panel
-00015090: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-000150a0: 697a 655f 7061 6e65 6c2c 0d0a 2020 2020  ize_panel,..    
-000150b0: 2020 2020 5d0d 0a20 2020 2020 2020 2023      ]..        #
-000150c0: 2065 6e64 2077 7847 6c61 6465 0d0a 0d0a   end wxGlade....
-000150d0: 2020 2020 6465 6620 7061 6e65 5f73 686f      def pane_sho
-000150e0: 7728 7365 6c66 293a 0d0a 2020 2020 2020  w(self):..      
-000150f0: 2020 666f 7220 7020 696e 2073 656c 662e    for p in self.
-00015100: 7061 6e65 6c73 3a0d 0a20 2020 2020 2020  panels:..       
-00015110: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00015120: 2020 2020 2020 2020 2020 2070 2e70 616e             p.pan
-00015130: 655f 7368 6f77 2829 0d0a 2020 2020 2020  e_show()..      
-00015140: 2020 2020 2020 6578 6365 7074 2041 7474        except Att
-00015150: 7269 6275 7465 4572 726f 723a 0d0a 2020  ributeError:..  
-00015160: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00015170: 7373 0d0a 0d0a 2020 2020 6465 6620 7061  ss....    def pa
-00015180: 6e65 5f68 6964 6528 7365 6c66 293a 0d0a  ne_hide(self):..
-00015190: 2020 2020 2020 2020 666f 7220 7020 696e          for p in
-000151a0: 2073 656c 662e 7061 6e65 6c73 3a0d 0a20   self.panels:.. 
-000151b0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-000151c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000151d0: 2070 2e70 616e 655f 6869 6465 2829 0d0a   p.pane_hide()..
-000151e0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000151f0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
-00015200: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00015210: 2020 2020 7061 7373 0d0a 0d0a 0d0a 636c      pass......cl
-00015220: 6173 7320 4e61 7669 6761 7469 6f6e 284d  ass Navigation(M
-00015230: 5769 6e64 6f77 293a 0d0a 2020 2020 6465  Window):..    de
-00015240: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00015250: 202a 6172 6773 2c20 2a2a 6b77 6473 293a   *args, **kwds):
-00015260: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00015270: 292e 5f5f 696e 6974 5f5f 2835 3938 2c20  ).__init__(598, 
-00015280: 3432 392c 202a 6172 6773 2c20 2a2a 6b77  429, *args, **kw
-00015290: 6473 290d 0a0d 0a20 2020 2020 2020 2073  ds)....        s
-000152a0: 656c 662e 7061 6e65 6c20 3d20 4e61 7669  elf.panel = Navi
-000152b0: 6761 7469 6f6e 5061 6e65 6c28 7365 6c66  gationPanel(self
-000152c0: 2c20 7778 2e49 445f 414e 592c 2063 6f6e  , wx.ID_ANY, con
-000152d0: 7465 7874 3d73 656c 662e 636f 6e74 6578  text=self.contex
-000152e0: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
-000152f0: 2e61 6464 5f6d 6f64 756c 655f 6465 6c65  .add_module_dele
-00015300: 6761 7465 2873 656c 662e 7061 6e65 6c29  gate(self.panel)
-00015310: 0d0a 2020 2020 2020 2020 6963 6f6e 7369  ..        iconsi
-00015320: 7a65 203d 2067 6574 5f64 6566 6175 6c74  ze = get_default
-00015330: 5f69 636f 6e5f 7369 7a65 2829 0d0a 2020  _icon_size()..  
-00015340: 2020 2020 2020 6d69 6e77 203d 2028 3320        minw = (3 
-00015350: 2b20 3320 2b20 3329 202a 2069 636f 6e73  + 3 + 3) * icons
-00015360: 697a 6520 2b20 3135 300d 0a20 2020 2020  ize + 150..     
-00015370: 2020 206d 696e 6820 3d20 2834 202b 2031     minh = (4 + 1
-00015380: 2920 2a20 6963 6f6e 7369 7a65 202b 2031  ) * iconsize + 1
-00015390: 3730 0d0a 2020 2020 2020 2020 7375 7065  70..        supe
-000153a0: 7228 292e 5365 7453 697a 6548 696e 7473  r().SetSizeHints
-000153b0: 286d 696e 573d 6d69 6e77 2c20 6d69 6e48  (minW=minw, minH
-000153c0: 3d6d 696e 6829 0d0a 0d0a 2020 2020 2020  =minh)....      
-000153d0: 2020 5f69 636f 6e20 3d20 7778 2e4e 756c    _icon = wx.Nul
-000153e0: 6c49 636f 6e0d 0a20 2020 2020 2020 205f  lIcon..        _
-000153f0: 6963 6f6e 2e43 6f70 7946 726f 6d42 6974  icon.CopyFromBit
-00015400: 6d61 7028 6963 6f6e 7338 5f6d 6f76 655f  map(icons8_move_
-00015410: 3530 2e47 6574 4269 746d 6170 2829 290d  50.GetBitmap()).
-00015420: 0a20 2020 2020 2020 2073 656c 662e 5365  .        self.Se
-00015430: 7449 636f 6e28 5f69 636f 6e29 0d0a 2020  tIcon(_icon)..  
-00015440: 2020 2020 2020 2320 6265 6769 6e20 7778        # begin wx
-00015450: 476c 6164 653a 204e 6176 6967 6174 696f  Glade: Navigatio
-00015460: 6e2e 5f5f 7365 745f 7072 6f70 6572 7469  n.__set_properti
-00015470: 6573 0d0a 2020 2020 2020 2020 7365 6c66  es..        self
-00015480: 2e53 6574 5469 746c 6528 5f28 224e 6176  .SetTitle(_("Nav
-00015490: 6967 6174 696f 6e22 2929 0d0a 0d0a 2020  igation"))....  
-000154a0: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
-000154b0: 0a20 2020 2064 6566 2073 7562 5f72 6567  .    def sub_reg
-000154c0: 6973 7465 7228 6b65 726e 656c 293a 0d0a  ister(kernel):..
-000154d0: 0d0a 2020 2020 2020 2020 6b65 726e 656c  ..        kernel
-000154e0: 2e72 6567 6973 7465 7228 2277 7870 616e  .register("wxpan
-000154f0: 652f 4e61 7669 6761 7469 6f6e 222c 2072  e/Navigation", r
-00015500: 6567 6973 7465 725f 7061 6e65 6c5f 6e61  egister_panel_na
-00015510: 7669 6761 7469 6f6e 290d 0a20 2020 2020  vigation)..     
-00015520: 2020 206b 6572 6e65 6c2e 7265 6769 7374     kernel.regist
-00015530: 6572 280d 0a20 2020 2020 2020 2020 2020  er(..           
-00015540: 2022 6275 7474 6f6e 2f70 7265 7061 7261   "button/prepara
-00015550: 7469 6f6e 2f4e 6176 6967 6174 696f 6e22  tion/Navigation"
-00015560: 2c0d 0a20 2020 2020 2020 2020 2020 207b  ,..            {
-00015570: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015580: 2020 226c 6162 656c 223a 205f 2822 4e61    "label": _("Na
-00015590: 7669 6761 7469 6f6e 2229 2c0d 0a20 2020  vigation"),..   
-000155a0: 2020 2020 2020 2020 2020 2020 2022 6963               "ic
-000155b0: 6f6e 223a 2069 636f 6e73 385f 6d6f 7665  on": icons8_move
-000155c0: 5f35 302c 0d0a 2020 2020 2020 2020 2020  _50,..          
-000155d0: 2020 2020 2020 2274 6970 223a 205f 2822        "tip": _("
-000155e0: 4f70 656e 7320 4e61 7669 6761 7469 6f6e  Opens Navigation
-000155f0: 2057 696e 646f 7722 292c 0d0a 2020 2020   Window"),..    
-00015600: 2020 2020 2020 2020 2020 2020 2261 6374              "act
-00015610: 696f 6e22 3a20 6c61 6d62 6461 2076 3a20  ion": lambda v: 
-00015620: 6b65 726e 656c 2e63 6f6e 736f 6c65 2822  kernel.console("
-00015630: 7769 6e64 6f77 2074 6f67 676c 6520 4e61  window toggle Na
-00015640: 7669 6761 7469 6f6e 5c6e 2229 2c0d 0a20  vigation\n"),.. 
-00015650: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00015660: 7072 696f 7269 7479 223a 2031 2c0d 0a20  priority": 1,.. 
-00015670: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
-00015680: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00015690: 6465 6620 7769 6e64 6f77 5f6f 7065 6e28  def window_open(
-000156a0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000156b0: 7365 6c66 2e70 616e 656c 2e70 616e 655f  self.panel.pane_
-000156c0: 7368 6f77 2829 0d0a 0d0a 2020 2020 6465  show()....    de
-000156d0: 6620 7769 6e64 6f77 5f63 6c6f 7365 2873  f window_close(s
-000156e0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-000156f0: 656c 662e 7061 6e65 6c2e 7061 6e65 5f68  elf.panel.pane_h
-00015700: 6964 6528 290d 0a0d 0a20 2020 2040 7374  ide()....    @st
-00015710: 6174 6963 6d65 7468 6f64 0d0a 2020 2020  aticmethod..    
-00015720: 6465 6620 7375 626d 656e 7528 293a 0d0a  def submenu():..
-00015730: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-00015740: 2245 6469 7469 6e67 222c 2022 4a6f 672c  "Editing", "Jog,
-00015750: 204d 6f76 6520 616e 6420 5472 616e 7366   Move and Transf
-00015760: 6f72 6d22 290d 0a                        orm")..
+00014cc0: 6c73 5f73 697a 6572 203d 2077 782e 426f  ls_sizer = wx.Bo
+00014cd0: 7853 697a 6572 2877 782e 484f 5249 5a4f  xSizer(wx.HORIZO
+00014ce0: 4e54 414c 290d 0a0d 0a20 2020 2020 2020  NTAL)....       
+00014cf0: 206a 6f67 6469 7374 616e 6365 7061 6e65   jogdistancepane
+00014d00: 6c20 3d20 4a6f 6744 6973 7461 6e63 6550  l = JogDistanceP
+00014d10: 616e 656c 2873 656c 662c 2077 782e 4944  anel(self, wx.ID
+00014d20: 5f41 4e59 2c20 636f 6e74 6578 743d 7365  _ANY, context=se
+00014d30: 6c66 2e63 6f6e 7465 7874 290d 0a20 2020  lf.context)..   
+00014d40: 2020 2020 206d 6169 6e5f 7369 7a65 722e       main_sizer.
+00014d50: 4164 6428 6a6f 6764 6973 7461 6e63 6570  Add(jogdistancep
+00014d60: 616e 656c 2c20 302c 2077 782e 4558 5041  anel, 0, wx.EXPA
+00014d70: 4e44 2c20 3029 0d0a 0d0a 2020 2020 2020  ND, 0)....      
+00014d80: 2020 6e61 7669 6761 7469 6f6e 7061 6e65    navigationpane
+00014d90: 6c20 3d20 4a6f 6728 7365 6c66 2c20 7778  l = Jog(self, wx
+00014da0: 2e49 445f 414e 592c 2063 6f6e 7465 7874  .ID_ANY, context
+00014db0: 3d73 656c 662e 636f 6e74 6578 7429 0d0a  =self.context)..
+00014dc0: 2020 2020 2020 2020 6d61 696e 5f70 616e          main_pan
+00014dd0: 656c 735f 7369 7a65 722e 4164 6428 6e61  els_sizer.Add(na
+00014de0: 7669 6761 7469 6f6e 7061 6e65 6c2c 2031  vigationpanel, 1
+00014df0: 2c20 7778 2e45 5850 414e 442c 2030 290d  , wx.EXPAND, 0).
+00014e00: 0a0d 0a20 2020 2020 2020 2061 6c69 676e  ...        align
+00014e10: 7061 6e65 6c20 3d20 4472 6167 2873 656c  panel = Drag(sel
+00014e20: 662c 2077 782e 4944 5f41 4e59 2c20 636f  f, wx.ID_ANY, co
+00014e30: 6e74 6578 743d 7365 6c66 2e63 6f6e 7465  ntext=self.conte
+00014e40: 7874 290d 0a20 2020 2020 2020 206d 6169  xt)..        mai
+00014e50: 6e5f 7061 6e65 6c73 5f73 697a 6572 2e41  n_panels_sizer.A
+00014e60: 6464 2861 6c69 676e 7061 6e65 6c2c 2031  dd(alignpanel, 1
+00014e70: 2c20 7778 2e45 5850 414e 442c 2030 290d  , wx.EXPAND, 0).
+00014e80: 0a0d 0a20 2020 2020 2020 2074 7261 6e73  ...        trans
+00014e90: 666f 726d 7061 6e65 6c20 3d20 5472 616e  formpanel = Tran
+00014ea0: 7366 6f72 6d28 7365 6c66 2c20 7778 2e49  sform(self, wx.I
+00014eb0: 445f 414e 592c 2063 6f6e 7465 7874 3d73  D_ANY, context=s
+00014ec0: 656c 662e 636f 6e74 6578 7429 0d0a 0d0a  elf.context)....
+00014ed0: 2020 2020 2020 2020 6d61 696e 5f70 616e          main_pan
+00014ee0: 656c 735f 7369 7a65 722e 4164 6428 7472  els_sizer.Add(tr
+00014ef0: 616e 7366 6f72 6d70 616e 656c 2c20 302c  ansformpanel, 0,
+00014f00: 2030 2c20 3029 0d0a 2020 2020 2020 2020   0, 0)..        
+00014f10: 6d61 696e 5f73 697a 6572 2e41 6464 286d  main_sizer.Add(m
+00014f20: 6169 6e5f 7061 6e65 6c73 5f73 697a 6572  ain_panels_sizer
+00014f30: 2c20 302c 2077 782e 4558 5041 4e44 2c20  , 0, wx.EXPAND, 
+00014f40: 3029 0d0a 0d0a 2020 2020 2020 2020 7368  0)....        sh
+00014f50: 6f72 745f 7075 6c73 6520 3d20 5075 6c73  ort_pulse = Puls
+00014f60: 6550 616e 656c 2873 656c 662c 2077 782e  ePanel(self, wx.
+00014f70: 4944 5f41 4e59 2c20 636f 6e74 6578 743d  ID_ANY, context=
+00014f80: 7365 6c66 2e63 6f6e 7465 7874 290d 0a20  self.context).. 
+00014f90: 2020 2020 2020 2070 756c 7365 5f61 6e64         pulse_and
+00014fa0: 5f6d 6f76 655f 7369 7a65 722e 4164 6428  _move_sizer.Add(
+00014fb0: 7368 6f72 745f 7075 6c73 652c 2031 2c20  short_pulse, 1, 
+00014fc0: 7778 2e45 5850 414e 442c 2030 290d 0a0d  wx.EXPAND, 0)...
+00014fd0: 0a20 2020 2020 2020 206d 6f76 655f 7061  .        move_pa
+00014fe0: 6e65 6c20 3d20 4d6f 7665 5061 6e65 6c28  nel = MovePanel(
+00014ff0: 7365 6c66 2c20 7778 2e49 445f 414e 592c  self, wx.ID_ANY,
+00015000: 2063 6f6e 7465 7874 3d73 656c 662e 636f   context=self.co
+00015010: 6e74 6578 7429 0d0a 2020 2020 2020 2020  ntext)..        
+00015020: 7075 6c73 655f 616e 645f 6d6f 7665 5f73  pulse_and_move_s
+00015030: 697a 6572 2e41 6464 286d 6f76 655f 7061  izer.Add(move_pa
+00015040: 6e65 6c2c 2031 2c20 7778 2e45 5850 414e  nel, 1, wx.EXPAN
+00015050: 442c 2030 290d 0a0d 0a20 2020 2020 2020  D, 0)....       
+00015060: 2073 697a 655f 7061 6e65 6c20 3d20 506f   size_panel = Po
+00015070: 7369 7469 6f6e 5061 6e65 6c28 7365 6c66  sitionPanel(self
+00015080: 2c20 7778 2e49 445f 414e 592c 2063 6f6e  , wx.ID_ANY, con
+00015090: 7465 7874 3d73 656c 662e 636f 6e74 6578  text=self.contex
+000150a0: 742c 2073 6d61 6c6c 3d54 7275 6529 0d0a  t, small=True)..
+000150b0: 2020 2020 2020 2020 7075 6c73 655f 616e          pulse_an
+000150c0: 645f 6d6f 7665 5f73 697a 6572 2e41 6464  d_move_sizer.Add
+000150d0: 2873 697a 655f 7061 6e65 6c2c 2031 2c20  (size_panel, 1, 
+000150e0: 7778 2e45 5850 414e 442c 2030 290d 0a0d  wx.EXPAND, 0)...
+000150f0: 0a20 2020 2020 2020 206d 6169 6e5f 7369  .        main_si
+00015100: 7a65 722e 4164 6428 7075 6c73 655f 616e  zer.Add(pulse_an
+00015110: 645f 6d6f 7665 5f73 697a 6572 2c20 302c  d_move_sizer, 0,
+00015120: 2077 782e 4558 5041 4e44 2c20 3029 0d0a   wx.EXPAND, 0)..
+00015130: 2020 2020 2020 2020 7365 6c66 2e53 6574          self.Set
+00015140: 5369 7a65 7228 6d61 696e 5f73 697a 6572  Sizer(main_sizer
+00015150: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00015160: 4c61 796f 7574 2829 0d0a 2020 2020 2020  Layout()..      
+00015170: 2020 7365 6c66 2e70 616e 656c 7320 3d20    self.panels = 
+00015180: 5b0d 0a20 2020 2020 2020 2020 2020 206a  [..            j
+00015190: 6f67 6469 7374 616e 6365 7061 6e65 6c2c  ogdistancepanel,
+000151a0: 0d0a 2020 2020 2020 2020 2020 2020 6e61  ..            na
+000151b0: 7669 6761 7469 6f6e 7061 6e65 6c2c 0d0a  vigationpanel,..
+000151c0: 2020 2020 2020 2020 2020 2020 616c 6967              alig
+000151d0: 6e70 616e 656c 2c0d 0a20 2020 2020 2020  npanel,..       
+000151e0: 2020 2020 2074 7261 6e73 666f 726d 7061       transformpa
+000151f0: 6e65 6c2c 0d0a 2020 2020 2020 2020 2020  nel,..          
+00015200: 2020 7368 6f72 745f 7075 6c73 652c 0d0a    short_pulse,..
+00015210: 2020 2020 2020 2020 2020 2020 6d6f 7665              move
+00015220: 5f70 616e 656c 2c0d 0a20 2020 2020 2020  _panel,..       
+00015230: 2020 2020 2073 697a 655f 7061 6e65 6c2c       size_panel,
+00015240: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
+00015250: 2020 2020 2023 2065 6e64 2077 7847 6c61       # end wxGla
+00015260: 6465 0d0a 0d0a 2020 2020 6465 6620 7061  de....    def pa
+00015270: 6e65 5f73 686f 7728 7365 6c66 293a 0d0a  ne_show(self):..
+00015280: 2020 2020 2020 2020 666f 7220 7020 696e          for p in
+00015290: 2073 656c 662e 7061 6e65 6c73 3a0d 0a20   self.panels:.. 
+000152a0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
+000152b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000152c0: 2070 2e70 616e 655f 7368 6f77 2829 0d0a   p.pane_show()..
+000152d0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+000152e0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
+000152f0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00015300: 2020 2020 7061 7373 0d0a 0d0a 2020 2020      pass....    
+00015310: 6465 6620 7061 6e65 5f68 6964 6528 7365  def pane_hide(se
+00015320: 6c66 293a 0d0a 2020 2020 2020 2020 666f  lf):..        fo
+00015330: 7220 7020 696e 2073 656c 662e 7061 6e65  r p in self.pane
+00015340: 6c73 3a0d 0a20 2020 2020 2020 2020 2020  ls:..           
+00015350: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00015360: 2020 2020 2020 2070 2e70 616e 655f 6869         p.pane_hi
+00015370: 6465 2829 0d0a 2020 2020 2020 2020 2020  de()..          
+00015380: 2020 6578 6365 7074 2041 7474 7269 6275    except Attribu
+00015390: 7465 4572 726f 723a 0d0a 2020 2020 2020  teError:..      
+000153a0: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
+000153b0: 0d0a 0d0a 636c 6173 7320 4e61 7669 6761  ....class Naviga
+000153c0: 7469 6f6e 284d 5769 6e64 6f77 293a 0d0a  tion(MWindow):..
+000153d0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000153e0: 2873 656c 662c 202a 6172 6773 2c20 2a2a  (self, *args, **
+000153f0: 6b77 6473 293a 0d0a 2020 2020 2020 2020  kwds):..        
+00015400: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00015410: 2835 3938 2c20 3432 392c 202a 6172 6773  (598, 429, *args
+00015420: 2c20 2a2a 6b77 6473 290d 0a0d 0a20 2020  , **kwds)....   
+00015430: 2020 2020 2073 656c 662e 7061 6e65 6c20       self.panel 
+00015440: 3d20 4e61 7669 6761 7469 6f6e 5061 6e65  = NavigationPane
+00015450: 6c28 7365 6c66 2c20 7778 2e49 445f 414e  l(self, wx.ID_AN
+00015460: 592c 2063 6f6e 7465 7874 3d73 656c 662e  Y, context=self.
+00015470: 636f 6e74 6578 7429 0d0a 2020 2020 2020  context)..      
+00015480: 2020 7365 6c66 2e61 6464 5f6d 6f64 756c    self.add_modul
+00015490: 655f 6465 6c65 6761 7465 2873 656c 662e  e_delegate(self.
+000154a0: 7061 6e65 6c29 0d0a 2020 2020 2020 2020  panel)..        
+000154b0: 6963 6f6e 7369 7a65 203d 2067 6574 5f64  iconsize = get_d
+000154c0: 6566 6175 6c74 5f69 636f 6e5f 7369 7a65  efault_icon_size
+000154d0: 2829 0d0a 2020 2020 2020 2020 6d69 6e77  ()..        minw
+000154e0: 203d 2028 3320 2b20 3320 2b20 3329 202a   = (3 + 3 + 3) *
+000154f0: 2069 636f 6e73 697a 6520 2b20 3135 300d   iconsize + 150.
+00015500: 0a20 2020 2020 2020 206d 696e 6820 3d20  .        minh = 
+00015510: 2834 202b 2031 2920 2a20 6963 6f6e 7369  (4 + 1) * iconsi
+00015520: 7a65 202b 2031 3730 0d0a 2020 2020 2020  ze + 170..      
+00015530: 2020 7375 7065 7228 292e 5365 7453 697a    super().SetSiz
+00015540: 6548 696e 7473 286d 696e 573d 6d69 6e77  eHints(minW=minw
+00015550: 2c20 6d69 6e48 3d6d 696e 6829 0d0a 0d0a  , minH=minh)....
+00015560: 2020 2020 2020 2020 5f69 636f 6e20 3d20          _icon = 
+00015570: 7778 2e4e 756c 6c49 636f 6e0d 0a20 2020  wx.NullIcon..   
+00015580: 2020 2020 205f 6963 6f6e 2e43 6f70 7946       _icon.CopyF
+00015590: 726f 6d42 6974 6d61 7028 6963 6f6e 7338  romBitmap(icons8
+000155a0: 5f6d 6f76 655f 3530 2e47 6574 4269 746d  _move_50.GetBitm
+000155b0: 6170 2829 290d 0a20 2020 2020 2020 2073  ap())..        s
+000155c0: 656c 662e 5365 7449 636f 6e28 5f69 636f  elf.SetIcon(_ico
+000155d0: 6e29 0d0a 2020 2020 2020 2020 2320 6265  n)..        # be
+000155e0: 6769 6e20 7778 476c 6164 653a 204e 6176  gin wxGlade: Nav
+000155f0: 6967 6174 696f 6e2e 5f5f 7365 745f 7072  igation.__set_pr
+00015600: 6f70 6572 7469 6573 0d0a 2020 2020 2020  operties..      
+00015610: 2020 7365 6c66 2e53 6574 5469 746c 6528    self.SetTitle(
+00015620: 5f28 224e 6176 6967 6174 696f 6e22 2929  _("Navigation"))
+00015630: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+00015640: 6574 686f 640d 0a20 2020 2064 6566 2073  ethod..    def s
+00015650: 7562 5f72 6567 6973 7465 7228 6b65 726e  ub_register(kern
+00015660: 656c 293a 0d0a 0d0a 2020 2020 2020 2020  el):....        
+00015670: 6b65 726e 656c 2e72 6567 6973 7465 7228  kernel.register(
+00015680: 2277 7870 616e 652f 4e61 7669 6761 7469  "wxpane/Navigati
+00015690: 6f6e 222c 2072 6567 6973 7465 725f 7061  on", register_pa
+000156a0: 6e65 6c5f 6e61 7669 6761 7469 6f6e 290d  nel_navigation).
+000156b0: 0a20 2020 2020 2020 206b 6572 6e65 6c2e  .        kernel.
+000156c0: 7265 6769 7374 6572 280d 0a20 2020 2020  register(..     
+000156d0: 2020 2020 2020 2022 6275 7474 6f6e 2f70         "button/p
+000156e0: 7265 7061 7261 7469 6f6e 2f4e 6176 6967  reparation/Navig
+000156f0: 6174 696f 6e22 2c0d 0a20 2020 2020 2020  ation",..       
+00015700: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00015710: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
+00015720: 205f 2822 4e61 7669 6761 7469 6f6e 2229   _("Navigation")
+00015730: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00015740: 2020 2022 6963 6f6e 223a 2069 636f 6e73     "icon": icons
+00015750: 385f 6d6f 7665 5f35 302c 0d0a 2020 2020  8_move_50,..    
+00015760: 2020 2020 2020 2020 2020 2020 2274 6970              "tip
+00015770: 223a 205f 2822 4f70 656e 7320 4e61 7669  ": _("Opens Navi
+00015780: 6761 7469 6f6e 2057 696e 646f 7722 292c  gation Window"),
+00015790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000157a0: 2020 2261 6374 696f 6e22 3a20 6c61 6d62    "action": lamb
+000157b0: 6461 2076 3a20 6b65 726e 656c 2e63 6f6e  da v: kernel.con
+000157c0: 736f 6c65 2822 7769 6e64 6f77 2074 6f67  sole("window tog
+000157d0: 676c 6520 4e61 7669 6761 7469 6f6e 5c6e  gle Navigation\n
+000157e0: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
+000157f0: 2020 2020 2022 7072 696f 7269 7479 223a       "priority":
+00015800: 2031 2c0d 0a20 2020 2020 2020 2020 2020   1,..           
+00015810: 207d 2c0d 0a20 2020 2020 2020 2029 0d0a   },..        )..
+00015820: 0d0a 2020 2020 6465 6620 7769 6e64 6f77  ..    def window
+00015830: 5f6f 7065 6e28 7365 6c66 293a 0d0a 2020  _open(self):..  
+00015840: 2020 2020 2020 7365 6c66 2e70 616e 656c        self.panel
+00015850: 2e70 616e 655f 7368 6f77 2829 0d0a 0d0a  .pane_show()....
+00015860: 2020 2020 6465 6620 7769 6e64 6f77 5f63      def window_c
+00015870: 6c6f 7365 2873 656c 6629 3a0d 0a20 2020  lose(self):..   
+00015880: 2020 2020 2073 656c 662e 7061 6e65 6c2e       self.panel.
+00015890: 7061 6e65 5f68 6964 6528 290d 0a0d 0a20  pane_hide().... 
+000158a0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+000158b0: 0d0a 2020 2020 6465 6620 7375 626d 656e  ..    def submen
+000158c0: 7528 293a 0d0a 2020 2020 2020 2020 7265  u():..        re
+000158d0: 7475 726e 2028 2245 6469 7469 6e67 222c  turn ("Editing",
+000158e0: 2022 4a6f 672c 204d 6f76 6520 616e 6420   "Jog, Move and 
+000158f0: 5472 616e 7366 6f72 6d22 290d 0a         Transform")..
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/notes.py` & `meerk40t-0.8.6000/meerk40t/gui/notes.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/opassignment.py` & `meerk40t-0.8.6000/meerk40t/gui/opassignment.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/operation_info.py` & `meerk40t-0.8.6000/meerk40t/gui/operation_info.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/plugin.py` & `meerk40t-0.8.6000/meerk40t/gui/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/position.py` & `meerk40t-0.8.6000/meerk40t/gui/position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import wx
 from wx import aui
 
 from meerk40t.core.elements.element_types import elem_nodes
 from meerk40t.core.units import UNITS_PER_PIXEL, Length
 from meerk40t.gui.icons import icons8_compress_50
 from meerk40t.gui.wxutils import StaticBoxSizer, TextCtrl
+from meerk40t.kernel import signal_listener
 
 _ = wx.GetTranslation
 
 
 def register_panel_position(window, context):
     pane = (
         aui.AuiPaneInfo()
@@ -121,14 +122,24 @@
 
     def pane_hide(self, *args):
         self.context.unlisten("units", self.space_changed)
         self.context.unlisten("emphasized", self._update_position)
         self.context.unlisten("modified", self._update_position)
         self.context.unlisten("altered", self._update_position)
 
+    # Option 2: attach yourself to the refresh_scene and the tool_modified signals
+    @signal_listener("refresh_scene")
+    def on_refresh_scene(self, origin, scene_name=None, *args):
+        if scene_name == "Scene":
+            self.update_position(True)
+
+    @signal_listener("tool_modified")
+    def on_modified(self, *args):
+        self.update_position(True)
+
     def __set_properties(self):
         # begin wxGlade: PositionPanel.__set_properties
         self.text_h.SetToolTip(_("New height (enter to apply)"))
         self.text_w.SetToolTip(_("New width (enter to apply)"))
         self.text_x.SetToolTip(
             _("New X-coordinate of left top corner (enter to apply)")
         )
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/preferences.py` & `meerk40t-0.8.6000/meerk40t/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/attributes.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,22 +257,22 @@
         self.text_id.SetActionRoutine(self.on_text_id_change)
         self.text_label.SetActionRoutine(self.on_text_label_change)
         self.set_widgets(self.node)
 
     def on_text_id_change(self):
         try:
             self.node.id = self.text_id.GetValue()
-            self.context.elements.signal("element_property_update", self.node)
+            self.context.elements.signal("element_property_reload", self.node)
         except AttributeError:
             pass
 
     def on_text_label_change(self):
         try:
             self.node.label = self.text_label.GetValue()
-            self.context.elements.signal("element_property_update", self.node)
+            self.context.elements.signal("element_property_reload", self.node)
         except AttributeError:
             pass
 
     def pane_hide(self):
         pass
 
     def pane_show(self):
@@ -704,14 +704,22 @@
 
     def pane_hide(self):
         pass
 
     def pane_show(self):
         pass
 
+    def signal(self, signalstr, myargs):
+        # To get updates about translation / scaling of selected elements
+        if signalstr == "refresh_scene":
+            if myargs[0] == "Scene":
+                self.set_widgets(self.node)
+        elif signalstr == "tool_modified":
+            self.set_widgets(self.node)
+
     def _set_widgets_hidden(self):
         self.text_x.SetValue("")
         self.text_y.SetValue("")
         self.text_w.SetValue("")
         self.text_h.SetValue("")
         self.Hide()
 
@@ -776,14 +784,15 @@
         dx = newx - bb[0]
         dy = newy - bb[1]
         if dx != 0 or dy != 0:
             self.node.matrix.post_translate(dx, dy)
             # self.node.modified()
             self.node.translated(dx, dy)
             self.context.elements.signal("element_property_update", self.node)
+            self.context.elements.signal("refresh_scene", "Scene")
 
     def scale_it(self, was_width):
         if not self.node.can_scale:
             return
         bb = self.node.bounds
         keep_ratio = self.btn_lock_ratio.GetValue()
         try:
@@ -818,14 +827,15 @@
                 f"{Length(amount=w, preferred_units=units, digits=4).preferred_length}"
             )
             self.text_h.SetValue(
                 f"{Length(amount=h, preferred_units=units, digits=4).preferred_length}"
             )
 
             self.context.elements.signal("element_property_update", self.node)
+            self.context.elements.signal("refresh_scene", "Scene")
 
     def on_toggle_ratio(self, event):
         if self.btn_lock_ratio.GetValue():
             self.btn_lock_ratio.SetBitmap(self.bitmap_locked)
         else:
             self.btn_lock_ratio.SetBitmap(self.bitmap_unlocked)
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/blobproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/blobproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/consoleproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/consoleproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/groupproperties.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/groupproperties.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/imageproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/imageproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/inputproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/inputproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/opbranchproperties.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/opbranchproperties.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/operationpropertymain.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/operationpropertymain.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/outputproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/outputproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/pathproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/pathproperty.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,19 @@
         self.lbl_info_area.SetValue("")
         self.lbl_info_length.SetValue("")
         self.lbl_info_points.SetValue("")
         self.lbl_info_segments.SetValue("")
 
         self.Refresh()
 
+    def signal(self, signalstr, myargs):
+        for panel in self.panels:
+            if hasattr(panel, "signal"):
+                panel.signal(signalstr, myargs)
+
     def __set_properties(self):
         return
 
     def __do_layout(self):
         # begin wxGlade: PathProperty.__do_layout
         sizer_v_main = wx.BoxSizer(wx.VERTICAL)
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/placementproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/placementproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/pointproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/pointproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/propertywindow.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/propertywindow.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,14 +40,29 @@
                 if panel is page:
                     page.pane_active()
                 else:
                     panel.pane_deactive()
             except AttributeError:
                 pass
 
+    @signal_listener("refresh_scene")
+    def on_refresh_scene(self, origin, *args):
+        myargs = [i for i in args]
+        if args[0] == "Scene":
+            for p in self.panel_instances:
+                if hasattr(p, "signal"):
+                    p.signal("refresh_scene", myargs)
+
+    @signal_listener("tool_modified")
+    def on_tool_modified(self, origin, *args):
+        myargs = [i for i in args]
+        for p in self.panel_instances:
+            if hasattr(p, "signal"):
+                p.signal("tool_modified", myargs)
+
     @signal_listener("selected")
     def on_selected(self, origin, *args):
         self.Freeze()
         for p in self.panel_instances:
             try:
                 p.pane_hide()
             except AttributeError:
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/rasterwizardpanels.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/rasterwizardpanels.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/textproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/textproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/propertypanels/waitproperty.py` & `meerk40t-0.8.6000/meerk40t/gui/propertypanels/waitproperty.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scene/scene.py` & `meerk40t-0.8.6000/meerk40t/gui/scene/scene.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scene/sceneconst.py` & `meerk40t-0.8.6000/meerk40t/gui/scene/sceneconst.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scene/scenepanel.py` & `meerk40t-0.8.6000/meerk40t/gui/scene/scenepanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scene/scenespacewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scene/scenespacewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scene/widget.py` & `meerk40t-0.8.6000/meerk40t/gui/scene/widget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/affinemover.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/affinemover.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/attractionwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/attractionwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/bedwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/bedwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/elementswidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/elementswidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/gridwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/gridwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,19 @@
 
         self.set_colors()
 
     @property
     def scene_scale(self):
         matrix = self.scene.widget_root.scene_widget.matrix
         try:
-            return sqrt(abs(matrix.determinant))
+            scene_scale = sqrt(abs(matrix.determinant))
+            if scene_scale < 1e-8:
+                matrix.reset()
+                return 1.0
+            return scene_scale
         except (OverflowError, ValueError, ZeroDivisionError):
             matrix.reset()
         return 1.0
 
     ###########################
     # PEN SETUP
     ###########################
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/guidewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/guidewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/laserpathwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/laserpathwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/machineoriginwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/machineoriginwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/rectselectwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/rectselectwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/relocatewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/relocatewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/reticlewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/reticlewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/scenewidgets/selectionwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/scenewidgets/selectionwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -2601,15 +2601,15 @@
             try:
                 font = wx.Font(
                     self.font_size,
                     wx.FONTFAMILY_SWISS,
                     wx.FONTSTYLE_NORMAL,
                     wx.FONTWEIGHT_BOLD,
                 )
-            except TypeError:
+            except (TypeError, AssertionError):
                 font = wx.Font(
                     int(self.font_size),
                     wx.FONTFAMILY_SWISS,
                     wx.FONTSTYLE_NORMAL,
                     wx.FONTWEIGHT_BOLD,
                 )
             gc.SetFont(font, self.scene.colors.color_manipulation)
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/simulation.py` & `meerk40t-0.8.6000/meerk40t/gui/simulation.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/snapoptions.py` & `meerk40t-0.8.6000/meerk40t/gui/snapoptions.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/spoolerpanel.py` & `meerk40t-0.8.6000/meerk40t/gui/spoolerpanel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/infowidget.py` & `meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/infowidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/opassignwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/opassignwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/selectionwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/selectionwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/shapepropwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/shapepropwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/statusbar.py` & `meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/statusbar.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/statusbarwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/statusbarwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/statusbarwidgets/strokewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/statusbarwidgets/strokewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/circlebrush.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/circlebrush.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolcircle.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolcircle.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolcontainer.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolcontainer.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/tooldraw.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/tooldraw.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolellipse.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolellipse.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toollinetext.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toollinetext.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolmeasure.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolmeasure.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolnodeedit.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolnodeedit.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolplacement.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolplacement.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolpoint.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolpoint.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolpolygon.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolpolygon.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolpolyline.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolpolyline.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolrect.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolrect.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolrelocate.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolrelocate.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolribbon.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolribbon.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/tooltext.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/tooltext.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolvector.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolvector.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/toolwidgets/toolwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/toolwidgets/toolwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/usbconnect.py` & `meerk40t-0.8.6000/meerk40t/gui/usbconnect.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/buttonwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/buttonwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/checkboxwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/checkboxwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/cyclocycloidwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/cyclocycloidwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/handlewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/handlewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/harmonograph.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/harmonograph.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/openclosewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/openclosewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/rotationwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/rotationwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/scalewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/scalewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/seekbarwidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/seekbarwidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/utilitywidgets/togglewidget.py` & `meerk40t-0.8.6000/meerk40t/gui/utilitywidgets/togglewidget.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/wordlisteditor.py` & `meerk40t-0.8.6000/meerk40t/gui/wordlisteditor.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/wxmeerk40t.py` & `meerk40t-0.8.6000/meerk40t/gui/wxmeerk40t.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/wxmmain.py` & `meerk40t-0.8.6000/meerk40t/gui/wxmmain.py`

 * *Files 0% similar despite different names*

```diff
@@ -3286,14 +3286,16 @@
                 self.Bind(wx.EVT_MENU, language_update(i), id=m.GetId())
                 if language_code not in trans and i != 0:
                     m.Enable(False)
                 i += 1
             self.main_menubar.Append(wxglade_tmp_menu, _("Languages"))
 
     @signal_listener("file;loaded")
+    @signal_listener("file;saved")
+    @signal_listener("file;cleared")
     @signal_listener("device;renamed")
     @lookup_listener("service/device/active")
     def on_active_change(self, *args):
         self.__set_titlebar()
 
     def window_close_veto(self):
         if self.any_device_running:
@@ -3478,16 +3480,14 @@
         self.main_statusbar.SetStatusText(value, 0)
 
     @signal_listener("statusupdate")
     def on_update_statuspanel(self, origin, value=None):
         self.main_statusbar.Reposition(value)
 
     def __set_titlebar(self):
-        device_name = ""
-        device_version = ""
         label = self.context.elements.filename
         if label is None:
             label = ""
         else:
             label = " - " + label
 
         title = (
```

### Comparing `meerk40t-0.8.5000/meerk40t/gui/wxmribbon.py` & `meerk40t-0.8.6000/meerk40t/gui/wxmribbon.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/wxmscene.py` & `meerk40t-0.8.6000/meerk40t/gui/wxmscene.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/wxmtree.py` & `meerk40t-0.8.6000/meerk40t/gui/wxmtree.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/wxutils.py` & `meerk40t-0.8.6000/meerk40t/gui/wxutils.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/gui/zmatrix.py` & `meerk40t-0.8.6000/meerk40t/gui/zmatrix.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/image/imagetools.py` & `meerk40t-0.8.6000/meerk40t/image/imagetools.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/internal_plugins.py` & `meerk40t-0.8.6000/meerk40t/internal_plugins.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/channel.py` & `meerk40t-0.8.6000/meerk40t/kernel/channel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/context.py` & `meerk40t-0.8.6000/meerk40t/kernel/context.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/exceptions.py` & `meerk40t-0.8.6000/meerk40t/kernel/exceptions.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/functions.py` & `meerk40t-0.8.6000/meerk40t/kernel/functions.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/jobs.py` & `meerk40t-0.8.6000/meerk40t/kernel/jobs.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/kernel.py` & `meerk40t-0.8.6000/meerk40t/kernel/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1143,14 +1143,20 @@
             self.channel("console").unwatch(self.__print_delegate)
 
     def premain(self):
         if hasattr(self.args, "console") and self.args.console:
             self.channel("console").watch(self.__print_delegate)
             import sys
 
+            if sys.stdin is None:
+                # This may happen if we are in gui-mode of a compiled application and launch with -c. There is no
+                # stdin and consequently trying to launch with this flag will otherwise crash.
+
+                return
+
             async def aio_readline(loop):
                 while not self._shutdown:
                     print(">>", end="", flush=True)
 
                     line = await loop.run_in_executor(None, sys.stdin.readline)
                     line = line.strip()
                     if line in ("quit", "shutdown"):
```

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/lifecycles.py` & `meerk40t-0.8.6000/meerk40t/kernel/lifecycles.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/module.py` & `meerk40t-0.8.6000/meerk40t/kernel/module.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/service.py` & `meerk40t-0.8.6000/meerk40t/kernel/service.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/kernel/settings.py` & `meerk40t-0.8.6000/meerk40t/kernel/settings.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/controller.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     & : resume.
     % : fail checksum, do not resend
     ~ : begin/end realtime exception (Note, these characters would be consumed during
             the write process and should not exist in the queue)
     \x18 : quit.
 
 """
-
+import random
 import threading
 import time
 
 from meerk40t.ch341 import get_ch341_interface
 
 STATUS_BAD_STATE = 204
 STATUS_SERIAL_CORRECT_M3_FINISH = 204
@@ -691,18 +691,18 @@
         # Packet is prepared and ready to send. Open Channel.
         self.open()
 
         if len(packet) == 30:
             # We have a sendable packet.
             if not self.pre_ok:
                 self.wait_until_accepting_packets()
-            if default_checksum:
-                packet = b"\x00" + packet + bytes([onewire_crc_lookup(packet)])
-            else:
+            if not default_checksum:  #  or random.randint(0, 2) == 0:
                 packet = b"\x00" + packet + bytes([onewire_crc_lookup(packet) ^ 0xFF])
+            else:
+                packet = b"\x00" + packet + bytes([onewire_crc_lookup(packet)])
             self.connection.write(packet)
             self.pre_ok = False
 
             # Packet is sent, trying to confirm.
             status = 0
             flawless = True
             for attempts in range(500):
```

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/device.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/device.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/driver.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1195,15 +1195,15 @@
         step_amount = -abs(set_step) if self._topward else abs(set_step)
         remaining = delta - step_amount
         if (
             remaining > 0
             and self._topward
             or remaining < 0
             and not self._topward
-            or abs(remaining) > 15
+            or abs(remaining) > 5
         ):
             # Remaining value is in the wrong direction, abort and move.
             self.finished_mode()
             self._move_relative(0, remaining)
             self.raster_mode()
             remaining = 0
         if remaining:
@@ -1241,15 +1241,15 @@
         step_amount = -set_step if self._leftward else set_step
         remaining = delta - step_amount
         if (
             remaining > 0
             and self._leftward
             or remaining < 0
             and not self._leftward
-            or abs(remaining) > 15
+            or abs(remaining) > 5
         ):
             # Remaining value is in the wrong direction, abort and move.
             self.finished_mode()
             self._move_relative(remaining, 0)
             self.raster_mode()
             remaining = 0
         if remaining:
```

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhyaccelgui.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhyaccelgui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhycontrollergui.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhycontrollergui.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         sizer_controller.Add(self.button_controller_control, 0, wx.EXPAND, 0)
         sizer_controller.Add(self.text_controller_status, 0, wx.EXPAND, 0)
         sizer_main_vertical.Add(sizer_controller, 0, wx.EXPAND, 0)
         sizer_count_packets.Add(self.packet_count_text, 0, wx.EXPAND, 0)
         sizer_statistics.Add(sizer_count_packets, 1, wx.EXPAND, 0)
         sizer_count_rejected.Add(self.rejected_packet_count_text, 0, wx.EXPAND, 0)
         sizer_statistics.Add(sizer_count_rejected, 1, wx.EXPAND, 0)
-        sizer_statistics.Add(self.button_clear_stats, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        sizer_statistics.Add(self.button_clear_stats, 0, wx.EXPAND, 0)
         packet_count.Add(sizer_statistics, 1, wx.EXPAND, 0)
         packet_info.Add(self.packet_text_text, 11, wx.EXPAND, 0)
         packet_count.Add(packet_info, 0, wx.EXPAND, 0)
         byte0sizer.Add(self.text_byte_0, 0, 0, 0)
         label_1 = wx.StaticText(self, wx.ID_ANY, _("Byte 0"))
         byte0sizer.Add(label_1, 0, 0, 0)
         byte_data_status.Add(byte0sizer, 1, wx.EXPAND, 0)
```

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhydrivergui.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhydrivergui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/gui/lhyoperationproperties.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/gui/lhyoperationproperties.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/gui/tcpcontroller.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/gui/tcpcontroller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/interpreter.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/interpreter.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/laserspeed.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/laserspeed.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/loader.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/loader.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/parser.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/parser.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/plugin.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/lihuiyu/tcp_connection.py` & `meerk40t-0.8.6000/meerk40t/lihuiyu/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/main.py` & `meerk40t-0.8.6000/meerk40t/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import sys
 
 from meerk40t.external_plugins import plugin as external_plugins
 from meerk40t.internal_plugins import plugin as internal_plugins
 from meerk40t.kernel import Kernel
 
 APPLICATION_NAME = "MeerK40t"
-APPLICATION_VERSION = "0.8.5000"
+APPLICATION_VERSION = "0.8.6000"
 
 if not getattr(sys, "frozen", False):
     # If .git directory does not exist we are running from a package like pypi
     # Otherwise we are running from source
     if os.path.isdir(sys.path[0] + "/.git"):
         APPLICATION_VERSION += " git"
     elif os.path.isdir(sys.path[0] + "/.github"):
```

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/builder.py` & `meerk40t-0.8.6000/meerk40t/moshi/builder.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/controller.py` & `meerk40t-0.8.6000/meerk40t/moshi/controller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/device.py` & `meerk40t-0.8.6000/meerk40t/moshi/device.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/driver.py` & `meerk40t-0.8.6000/meerk40t/moshi/driver.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/moshi/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/gui/moshicontrollergui.py` & `meerk40t-0.8.6000/meerk40t/moshi/gui/moshicontrollergui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/gui/moshidrivergui.py` & `meerk40t-0.8.6000/meerk40t/moshi/gui/moshidrivergui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/moshi/plugin.py` & `meerk40t-0.8.6000/meerk40t/moshi/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/network/console_server.py` & `meerk40t-0.8.6000/meerk40t/network/console_server.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/network/tcp_server.py` & `meerk40t-0.8.6000/meerk40t/network/tcp_server.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/network/udp_server.py` & `meerk40t-0.8.6000/meerk40t/network/udp_server.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/controller.py` & `meerk40t-0.8.6000/meerk40t/newly/controller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/device.py` & `meerk40t-0.8.6000/meerk40t/newly/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -631,33 +631,54 @@
         @self.console_argument("file_index", type=int)
         @self.console_command(
             "move_frame",
             help=_("sends the newly move_frame command"),
             all_arguments_required=True,
         )
         def move_rect(file_index, **kwargs):
-            self.driver.connection.move_frame(file_index)
+            try:
+                self.driver.connection.move_frame(file_index)
+            except ConnectionRefusedError:
+                self.signal(
+                    "warning",
+                    _("Connection was aborted. Manual connection required."),
+                    _("Not Connected"),
+                )
 
         @self.console_argument("file_index", type=int)
         @self.console_command(
             "draw_frame",
             help=_("sends the newly draw_frame command"),
             all_arguments_required=True,
         )
         def draw_rect(file_index, **kwargs):
-            self.driver.connection.draw_frame(file_index)
+            try:
+                self.driver.connection.draw_frame(file_index)
+            except ConnectionRefusedError:
+                self.signal(
+                    "warning",
+                    _("Connection was aborted. Manual connection required."),
+                    _("Not Connected"),
+                )
 
         @self.console_argument("file_index", type=int)
         @self.console_command(
             "replay",
             help=_("sends the file replay command"),
             all_arguments_required=True,
         )
         def replay(file_index, **kwargs):
-            self.driver.connection.replay(file_index)
+            try:
+                self.driver.connection.replay(file_index)
+            except ConnectionRefusedError:
+                self.signal(
+                    "warning",
+                    _("Connection was aborted. Manual connection required."),
+                    _("Not Connected"),
+                )
 
         @self.console_command(
             "viewport_update",
             hidden=True,
             help=_("Update newly flips for movement"),
         )
         def codes_update(**kwargs):
```

### Comparing `meerk40t-0.8.5000/meerk40t/newly/driver.py` & `meerk40t-0.8.6000/meerk40t/newly/driver.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/newly/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/gui/newlyconfig.py` & `meerk40t-0.8.6000/meerk40t/newly/gui/newlyconfig.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/gui/newlycontroller.py` & `meerk40t-0.8.6000/meerk40t/newly/gui/newlycontroller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/gui/operationproperties.py` & `meerk40t-0.8.6000/meerk40t/newly/gui/operationproperties.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/mock_connection.py` & `meerk40t-0.8.6000/meerk40t/newly/mock_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/newly_params.py` & `meerk40t-0.8.6000/meerk40t/newly/newly_params.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/plugin.py` & `meerk40t-0.8.6000/meerk40t/newly/plugin.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/newly/usb_connection.py` & `meerk40t-0.8.6000/meerk40t/newly/usb_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/rotary/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/rotary/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/rotary/gui/rotarysettings.py` & `meerk40t-0.8.6000/meerk40t/rotary/gui/rotarysettings.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/rotary/rotary.py` & `meerk40t-0.8.6000/meerk40t/rotary/rotary.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/control.py` & `meerk40t-0.8.6000/meerk40t/ruida/control.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/controller.py` & `meerk40t-0.8.6000/meerk40t/ruida/controller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/device.py` & `meerk40t-0.8.6000/meerk40t/ruida/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,14 +140,36 @@
                 "tip": _("Mirror the elements on the Y-Axis"),
                 "conditional": (self, "rotary_active"),
                 "subsection": _("Mirror Output"),
             },
         ]
         self.register_choices("rotary", choices)
 
+        choices = [
+            {
+                "attr": "default_power",
+                "object": self,
+                "default": 20.0,
+                "type": float,
+                "label": _("Laser Power"),
+                "trailer": "%",
+                "tip": _("What power level do we cut at?"),
+            },
+            {
+                "attr": "default_speed",
+                "object": self,
+                "default": 40.0,
+                "type": float,
+                "trailer": "mm/s",
+                "label": _("Cut Speed"),
+                "tip": _("How fast do we cut?"),
+            },
+        ]
+        self.register_choices("ruida-global", choices)
+
         self.driver = RuidaDriver(self)
 
         self.spooler = Spooler(self, driver=self.driver)
         self.add_service_delegate(self.spooler)
         self.add_service_delegate(self.driver)
         # Tuple contains 4 value pairs: Speed Low, Speed High, Power Low, Power High, each with enabled, value
         self.setting(
```

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/driver.py` & `meerk40t-0.8.6000/meerk40t/ruida/driver.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/emulator.py` & `meerk40t-0.8.6000/meerk40t/ruida/emulator.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/gui/gui.py` & `meerk40t-0.8.6000/meerk40t/ruida/gui/gui.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/gui/ruidaconfig.py` & `meerk40t-0.8.6000/meerk40t/ruida/gui/ruidaconfig.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/gui/ruidacontroller.py` & `meerk40t-0.8.6000/meerk40t/ruida/gui/ruidacontroller.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/gui/ruidaoperationproperties.py` & `meerk40t-0.8.6000/meerk40t/ruida/gui/ruidaoperationproperties.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/loader.py` & `meerk40t-0.8.6000/meerk40t/ruida/loader.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/mock_connection.py` & `meerk40t-0.8.6000/meerk40t/ruida/mock_connection.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/plugin.py` & `meerk40t-0.8.6000/meerk40t/ruida/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Moshi Device Plugin
+Ruida Device Plugin
 
 Registers the needed classes for ruida device (or would if the ruida device could be controlled).
 """
 from meerk40t.ruida.control import RuidaControl
 from meerk40t.ruida.device import RuidaDevice
 from meerk40t.ruida.emulator import RuidaEmulator
 from meerk40t.ruida.loader import RDLoader
@@ -13,36 +13,36 @@
 def plugin(kernel, lifecycle=None):
     if lifecycle == "plugins":
         from .gui import gui
 
         return [gui.plugin]
     if lifecycle == "register":
         _ = kernel.translation
-        kernel.register("provider/device/ruida", RuidaDevice)
-        kernel.register(
-            "dev_info/ruida-beta",
-            {
-                "provider": "provider/device/ruida",
-                "friendly_name": _("K50/K60-CO2-Laser (Ruida-Controller) (INCOMPLETE)"),
-                "extended_info": _("This driver is incomplete. Use at your own risk."),
-                "priority": -1,
-                "family": _("CO2-Laser"),
-                "family_priority": 0,
-                "choices": [
-                    {
-                        "attr": "label",
-                        "default": "ruida",
-                    },
-                    {
-                        "attr": "source",
-                        "default": "co2",
-                    },
-                ],
-            },
-        )
+        # kernel.register("provider/device/ruida", RuidaDevice)
+        # kernel.register(
+        #     "dev_info/ruida-beta",
+        #     {
+        #         "provider": "provider/device/ruida",
+        #         "friendly_name": _("K50/K60-CO2-Laser (Ruida-Controller) (INCOMPLETE)"),
+        #         "extended_info": _("This driver is incomplete. Use at your own risk."),
+        #         "priority": -1,
+        #         "family": _("CO2-Laser"),
+        #         "family_priority": 0,
+        #         "choices": [
+        #             {
+        #                 "attr": "label",
+        #                 "default": "ruida",
+        #             },
+        #             {
+        #                 "attr": "source",
+        #                 "default": "co2",
+        #             },
+        #         ],
+        #     },
+        # )
         kernel.register("spoolerjob/ruida", RDJob)
         kernel.register("load/RDLoader", RDLoader)
         kernel.register("emulator/ruida", RuidaEmulator)
 
         @kernel.console_option(
             "verbose",
             "v",
@@ -77,11 +77,11 @@
                 ruidacontrol = RuidaControl(root)
                 root.device.register("ruidacontrol", ruidacontrol)
                 ruidacontrol.start(verbose=verbose)
             if quit:
                 ruidacontrol.quit()
                 root.device.unregister("ruidacontrol")
 
-    if lifecycle == "preboot":
-        suffix = "ruida"
-        for d in kernel.derivable(suffix):
-            kernel.root(f"service device start -p {d} {suffix}\n")
+    # if lifecycle == "preboot":
+    #     suffix = "ruida"
+    #     for d in kernel.derivable(suffix):
+    #         kernel.root(f"service device start -p {d} {suffix}\n")
```

### Comparing `meerk40t-0.8.5000/meerk40t/ruida/rdjob.py` & `meerk40t-0.8.6000/meerk40t/ruida/rdjob.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/svgelements.py` & `meerk40t-0.8.6000/meerk40t/svgelements.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/driver_to_path.py` & `meerk40t-0.8.6000/meerk40t/tools/driver_to_path.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/geomstr.py` & `meerk40t-0.8.6000/meerk40t/tools/geomstr.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/jhfparser.py` & `meerk40t-0.8.6000/meerk40t/tools/jhfparser.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/kerftest.py` & `meerk40t-0.8.6000/meerk40t/tools/kerftest.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/livinghinges.py` & `meerk40t-0.8.6000/meerk40t/tools/livinghinges.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/pathtools.py` & `meerk40t-0.8.6000/meerk40t/tools/pathtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -801,14 +801,16 @@
 
     def event_range(self):
         """
         Returns the range of events from the lowest to the highest in y-value.
 
         @return:
         """
+        if len(self._events) == 0:
+            return None, None
         self._sort_events()
         y_min = self._events[0][0]
         y_max = self._events[-1][0]
         return y_min, y_max
 
     def _sort_events(self):
         if not self._dirty_event_sort:
```

### Comparing `meerk40t-0.8.5000/meerk40t/tools/pointfinder.py` & `meerk40t-0.8.6000/meerk40t/tools/pointfinder.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/polybool.py` & `meerk40t-0.8.6000/meerk40t/tools/polybool.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/rasterplotter.py` & `meerk40t-0.8.6000/meerk40t/tools/rasterplotter.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/shxparser.py` & `meerk40t-0.8.6000/meerk40t/tools/shxparser.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/ttfparser.py` & `meerk40t-0.8.6000/meerk40t/tools/ttfparser.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t/tools/zinglplotter.py` & `meerk40t-0.8.6000/meerk40t/tools/zinglplotter.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/meerk40t.egg-info/PKG-INFO` & `meerk40t-0.8.6000/meerk40t.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,16 @@
 Metadata-Version: 2.1
 Name: meerk40t
-Version: 0.8.5000
+Version: 0.8.6000
 Summary: MeerK40t LaserCutter Software
 Home-page: https://github.com/meerk40t/meerk40t
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
-Description: # MeerK40t
-        MeerK40t (pronounced MeerKat) is a built-from-the-ground-up MIT licensed open-source laser cutting software.
-        
-        ## Primary Goals
-        * Provide users with high quality laser control software.
-        * Provide developers with a highly extensible platform to help further their own ideas, and provide novel work to the laser community at large.
-        
-        ## Running
-        MeerK40t is written in Python and precompiled versions are [available for download](https://github.com/meerk40t/meerk40t/releases) for Windows, Mac OSX, Linux and Raspberry Pi. Due note this sometimes will give false postitives for various viruses (especially since Meerk40t isn't signed).
-        
-        Alternatively you can run MeerK40t directly from Python. `pip install meerk40t[all]` with python installed will usually be sufficient. Then merely run `meerk40t` at the command line.
-        
-        ### GUI
-        ![meerk40t8](https://user-images.githubusercontent.com/3302478/196283699-745d0616-5e74-49b3-ba95-f4902061584b.png)
-        
-        The wxMeerK40t is the GUI and is written in wxPython. We use AUI to allow to have a very highly configurable UI. We can easily add panes and tools and there are quite a few available already.
-        
-        ### Command Line Interface
-        
-        Meerk40t has an advanced internal console system allowing access to most parts of the code with various commands. It also provides a command line interface which should allow you to automate any processes.
-        
-        ## Drivers
-        
-        Meerk40t provides a variety of drivers with an extensible framework to provide support for other new laser devices. The code was written with the myriad of possibilities for different software in mind. For example, it may be essential that GRBL be able to reset an alarm or notify the user of particular error codes. The configuration for GRBL is not the same for the configuration of other laser control drivers. With this in mind, Meerk40t can radically change how and when it works
-        
-        
-        ### Supported devices
-        *   M2-Nano
-        *   Moshiboard
-        *   GRBL
-        *   Fibre Lasers based on the JCZ controllers (still experimental)
-        *   Ruida-Emulation (Middleman between Lightburn and K40)
-        
-        ### Lihuiyu M2-Nano
-        For the Lihuiyu (stock driver), Meerk40t supports both the windows and libusb connection methods, making it compatible with Whisperer and with the original Chinese software. So MeerK40t can usually run alongside these other pieces of software interchangeably.
-        
-        ### Galvo LMC
-        
-        Meerk40t supports controlling galvo as well as gantry lasers with open source support.
-        
-        ### Moshiboard
-        
-        The support for old moshiboards makes meerk40t the only known software opensource software that controls moshiboards.
-        
-        ### GRBL
-        
-        GRBL is itself open source and the various interfaces with the board should be quite well understood.
-        
-        ## Support
-        The primary source for help and documentation is the [MeerK40t Wiki - please click here](https://github.com/meerk40t/meerk40t/wiki).
-        
-        If you have a bug, feature request, or other issue raise it here. These are likely to be resolved. Squeaky wheels get the grease.
-        https://github.com/meerk40t/meerk40t/issues
-        
-        If you need additional support, please research/ask on:
-        
-        *   [Facebook](https://www.facebook.com/groups/716000085655097/)
-        *   [Maker Forums](https://forum.makerforums.info/t/about-the-meerk40t-category/79660)
-        *   [YouTube - David Olsen's channel](https://www.youtube.com/channel/UCsAUV23O2FyKxC0HN7nkAQQ)
-        *   [YouTube - Some instruction videos](https://www.youtube.com/channel/UCMN9gGvpacxZINPZCSOecaQ)
-        *   [Discord](https://discord.gg/vkDD3HdQq6)
-        
-        ## Assisting the Project
-        
-        Open source projects live and die with their support. There are a lots of ways to help the project. There are also a lot of ways the project should help you.
-        *   Code
-        *   Provide Translations in other languages.
-        *   Design ( Good design instincts, smooth out the rough edges)
-        *   Compile/Testers
-        *   Beta testers
-        *   Make helpful support content
-        *   Make guides ("How to setup cameras?", etc)
-        *   Bounce ideas around
-        
-        
 Keywords: lasercutter,laser,vector,parser
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -97,7 +21,83 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: gui
 Provides-Extra: cam
 Provides-Extra: dxf
 Provides-Extra: camhead
+License-File: LICENSE
+
+# MeerK40t
+MeerK40t (pronounced MeerKat) is a built-from-the-ground-up MIT licensed open-source laser cutting software.
+
+## Primary Goals
+* Provide users with high quality laser control software.
+* Provide developers with a highly extensible platform to help further their own ideas, and provide novel work to the laser community at large.
+
+## Running
+MeerK40t is written in Python and precompiled versions are [available for download](https://github.com/meerk40t/meerk40t/releases) for Windows, Mac OSX, Linux and Raspberry Pi. Due note this sometimes will give false postitives for various viruses (especially since Meerk40t isn't signed).
+
+Alternatively you can run MeerK40t directly from Python. `pip install meerk40t[all]` with python installed will usually be sufficient. Then merely run `meerk40t` at the command line.
+
+### GUI
+![meerk40t8](https://user-images.githubusercontent.com/3302478/196283699-745d0616-5e74-49b3-ba95-f4902061584b.png)
+
+The wxMeerK40t is the GUI and is written in wxPython. We use AUI to allow to have a very highly configurable UI. We can easily add panes and tools and there are quite a few available already.
+
+### Command Line Interface
+
+Meerk40t has an advanced internal console system allowing access to most parts of the code with various commands. It also provides a command line interface which should allow you to automate any processes.
+
+## Drivers
+
+Meerk40t provides a variety of drivers with an extensible framework to provide support for other new laser devices. The code was written with the myriad of possibilities for different software in mind. For example, it may be essential that GRBL be able to reset an alarm or notify the user of particular error codes. The configuration for GRBL is not the same for the configuration of other laser control drivers. With this in mind, Meerk40t can radically change how and when it works
+
+
+### Supported devices
+*   M2-Nano
+*   Moshiboard
+*   GRBL
+*   Fibre Lasers based on the JCZ controllers (still experimental)
+*   Ruida-Emulation (Middleman between Lightburn and K40)
+
+### Lihuiyu M2-Nano
+For the Lihuiyu (stock driver), Meerk40t supports both the windows and libusb connection methods, making it compatible with Whisperer and with the original Chinese software. So MeerK40t can usually run alongside these other pieces of software interchangeably.
+
+### Galvo LMC
+
+Meerk40t supports controlling galvo as well as gantry lasers with open source support.
+
+### Moshiboard
+
+The support for old moshiboards makes meerk40t the only known software opensource software that controls moshiboards.
+
+### GRBL
+
+GRBL is itself open source and the various interfaces with the board should be quite well understood.
+
+## Support
+The primary source for help and documentation is the [MeerK40t Wiki - please click here](https://github.com/meerk40t/meerk40t/wiki).
+
+If you have a bug, feature request, or other issue raise it here. These are likely to be resolved. Squeaky wheels get the grease.
+https://github.com/meerk40t/meerk40t/issues
+
+If you need additional support, please research/ask on:
+
+*   [Facebook](https://www.facebook.com/groups/716000085655097/)
+*   [Maker Forums](https://forum.makerforums.info/t/about-the-meerk40t-category/79660)
+*   [YouTube - David Olsen's channel](https://www.youtube.com/channel/UCsAUV23O2FyKxC0HN7nkAQQ)
+*   [YouTube - Some instruction videos](https://www.youtube.com/channel/UCMN9gGvpacxZINPZCSOecaQ)
+*   [Discord](https://discord.gg/vkDD3HdQq6)
+
+## Assisting the Project
+
+Open source projects live and die with their support. There are a lots of ways to help the project. There are also a lot of ways the project should help you.
+*   Code
+*   Provide Translations in other languages.
+*   Design ( Good design instincts, smooth out the rough edges)
+*   Compile/Testers
+*   Beta testers
+*   Make helpful support content
+*   Make guides ("How to setup cameras?", etc)
+*   Bounce ideas around
+
```

### Comparing `meerk40t-0.8.5000/meerk40t.egg-info/SOURCES.txt` & `meerk40t-0.8.6000/meerk40t.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,16 @@
 meerk40t.egg-info/zip-safe
 meerk40t/balormk/__init__.py
 meerk40t/balormk/balor_params.py
 meerk40t/balormk/controller.py
 meerk40t/balormk/device.py
 meerk40t/balormk/driver.py
 meerk40t/balormk/elementlightjob.py
+meerk40t/balormk/livefulllightjob.py
+meerk40t/balormk/liveselectionlightjob.py
 meerk40t/balormk/mock_connection.py
 meerk40t/balormk/plugin.py
 meerk40t/balormk/usb_connection.py
 meerk40t/balormk/gui/__init__.py
 meerk40t/balormk/gui/balorconfig.py
 meerk40t/balormk/gui/balorcontroller.py
 meerk40t/balormk/gui/baloroperationproperties.py
@@ -446,14 +448,15 @@
 meerk40t/camera/plugin.py
 meerk40t/camera/gui/__init__.py
 meerk40t/camera/gui/camerapanel.py
 meerk40t/camera/gui/gui.py
 meerk40t/ch341/__init__.py
 meerk40t/ch341/libusb.py
 meerk40t/ch341/mock.py
+meerk40t/ch341/windll.py
 meerk40t/core/__init__.py
 meerk40t/core/bindalias.py
 meerk40t/core/core.py
 meerk40t/core/cutplan.py
 meerk40t/core/drivers.py
 meerk40t/core/element_commands.py
 meerk40t/core/exceptions.py
@@ -509,14 +512,15 @@
 meerk40t/core/node/blobnode.py
 meerk40t/core/node/bootstrap.py
 meerk40t/core/node/branch_elems.py
 meerk40t/core/node/branch_ops.py
 meerk40t/core/node/branch_regmark.py
 meerk40t/core/node/cutnode.py
 meerk40t/core/node/elem_ellipse.py
+meerk40t/core/node/elem_geomstr.py
 meerk40t/core/node/elem_image.py
 meerk40t/core/node/elem_line.py
 meerk40t/core/node/elem_path.py
 meerk40t/core/node/elem_point.py
 meerk40t/core/node/elem_polyline.py
 meerk40t/core/node/elem_rect.py
 meerk40t/core/node/elem_text.py
@@ -542,14 +546,20 @@
 meerk40t/core/node/util_home.py
 meerk40t/core/node/util_input.py
 meerk40t/core/node/util_output.py
 meerk40t/core/node/util_wait.py
 meerk40t/device/__init__.py
 meerk40t/device/basedevice.py
 meerk40t/device/dummydevice.py
+meerk40t/device/ch341/__init__.py
+meerk40t/device/ch341/ch341.py
+meerk40t/device/ch341/ch341libusbdriver.py
+meerk40t/device/ch341/libusb.py
+meerk40t/device/ch341/mock.py
+meerk40t/device/ch341/windll.py
 meerk40t/device/gui/__init__.py
 meerk40t/device/gui/defaultactions.py
 meerk40t/device/gui/formatterpanel.py
 meerk40t/device/gui/warningpanel.py
 meerk40t/dxf/__init__.py
 meerk40t/dxf/dxf_io.py
 meerk40t/dxf/plugin.py
```

### Comparing `meerk40t-0.8.5000/pyproject.toml` & `meerk40t-0.8.6000/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/setup.cfg` & `meerk40t-0.8.6000/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6565 726b 3430 740d 0a76 6572   = meerk40t..ver
-00000020: 7369 6f6e 203d 2030 2e38 2e35 3030 300d  sion = 0.8.5000.
+00000020: 7369 6f6e 203d 2030 2e38 2e36 3030 300d  sion = 0.8.6000.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 204d  .description = M
 00000040: 6565 724b 3430 7420 4c61 7365 7243 7574  eerK40t LaserCut
 00000050: 7465 7220 536f 6674 7761 7265 0d0a 6c6f  ter Software..lo
 00000060: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 00000070: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
 00000080: 7874 2f6d 6172 6b64 6f77 6e0d 0a6c 6f6e  xt/markdown..lon
 00000090: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

### Comparing `meerk40t-0.8.5000/setup.py` & `meerk40t-0.8.6000/setup.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/bootstrap.py` & `meerk40t-0.8.6000/test/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_core_cutcode.py` & `meerk40t-0.8.6000/test/test_core_cutcode.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_core_elements.py` & `meerk40t-0.8.6000/test/test_core_elements.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_core_plotplanner.py` & `meerk40t-0.8.6000/test/test_core_plotplanner.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_core_viewports.py` & `meerk40t-0.8.6000/test/test_core_viewports.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_drivers_grbl.py` & `meerk40t-0.8.6000/test/test_drivers_grbl.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_drivers_lihuiyu.py` & `meerk40t-0.8.6000/test/test_drivers_lihuiyu.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_element_degenerate_points.py` & `meerk40t-0.8.6000/test/test_element_degenerate_points.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_elements_classify.py` & `meerk40t-0.8.6000/test/test_elements_classify.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_elements_penbox.py` & `meerk40t-0.8.6000/test/test_elements_penbox.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_fill.py` & `meerk40t-0.8.6000/test/test_fill.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_geomstr.py` & `meerk40t-0.8.6000/test/test_geomstr.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_imagetools_actualize.py` & `meerk40t-0.8.6000/test/test_imagetools_actualize.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_imagetools_wizard.py` & `meerk40t-0.8.6000/test/test_imagetools_wizard.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_kernel.py` & `meerk40t-0.8.6000/test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_laser_speeds.py` & `meerk40t-0.8.6000/test/test_laser_speeds.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_length.py` & `meerk40t-0.8.6000/test/test_length.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_lifecycle.py` & `meerk40t-0.8.6000/test/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_operations_hatch.py` & `meerk40t-0.8.6000/test/test_operations_hatch.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_spooler.py` & `meerk40t-0.8.6000/test/test_spooler.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_wobble.py` & `meerk40t-0.8.6000/test/test_wobble.py`

 * *Files identical despite different names*

### Comparing `meerk40t-0.8.5000/test/test_zingl.py` & `meerk40t-0.8.6000/test/test_zingl.py`

 * *Files identical despite different names*

