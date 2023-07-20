# Comparing `tmp/pyVIP-1.8.0.tar.gz` & `tmp/pyVIP-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyVIP-1.8.0.tar", last modified: Fri Jun 25 23:50:14 2021, max compression
+gzip compressed data, was "dist\pyVIP-1.9.0.tar", last modified: Tue Aug 31 20:49:49 2021, max compression
```

## Comparing `pyVIP-1.8.0.tar` & `pyVIP-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-06-25 23:50:14.000000 pyVIP-1.8.0/
--rw-rw-rw-   0        0        0     1062 2021-06-16 21:24:04.000000 pyVIP-1.8.0/LICENSE
--rw-rw-rw-   0        0        0       42 2021-06-16 21:24:04.000000 pyVIP-1.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0      913 2021-06-25 23:50:14.000000 pyVIP-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      322 2021-06-16 21:24:04.000000 pyVIP-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2021-06-25 23:50:14.000000 pyVIP-1.8.0/pyVIP.egg-info/
--rw-rw-rw-   0        0        0      913 2021-06-25 23:50:14.000000 pyVIP-1.8.0/pyVIP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2021-06-25 23:50:14.000000 pyVIP-1.8.0/pyVIP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-25 23:50:14.000000 pyVIP-1.8.0/pyVIP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2021-06-25 23:50:14.000000 pyVIP-1.8.0/pyVIP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-06-25 23:50:14.000000 pyVIP-1.8.0/pyVIP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      116 2021-06-16 21:24:04.000000 pyVIP-1.8.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-06-25 23:50:14.000000 pyVIP-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0      923 2021-06-16 21:24:04.000000 pyVIP-1.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-25 23:50:14.000000 pyVIP-1.8.0/virtualitics/
--rw-rw-rw-   0        0        0      338 2021-06-25 23:49:40.000000 pyVIP-1.8.0/virtualitics/__init__.py
--rw-rw-rw-   0        0        0   279794 2021-06-25 23:49:40.000000 pyVIP-1.8.0/virtualitics/api.py
--rw-rw-rw-   0        0        0     2151 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/encryption.py
--rw-rw-rw-   0        0        0     7610 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/exceptions.py
--rw-rw-rw-   0        0        0     2122 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/pkcs7.py
--rw-rw-rw-   0        0        0    41903 2021-06-25 23:49:40.000000 pyVIP-1.8.0/virtualitics/task_response_handlers.py
--rw-rw-rw-   0        0        0    17986 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/utils.py
--rw-rw-rw-   0        0        0    24922 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/vip_annotation.py
--rw-rw-rw-   0        0        0     4743 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/vip_dashboard.py
--rw-rw-rw-   0        0        0     2204 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/vip_object.py
--rw-rw-rw-   0        0        0   145295 2021-06-16 21:24:04.000000 pyVIP-1.8.0/virtualitics/vip_plot.py
--rw-rw-rw-   0        0        0     1606 2021-06-25 23:49:40.000000 pyVIP-1.8.0/virtualitics/vip_result.py
+drwxrwxrwx   0        0        0        0 2021-08-31 20:49:49.000000 pyVIP-1.9.0/
+-rw-rw-rw-   0        0        0     1062 2021-08-18 00:25:52.000000 pyVIP-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0       42 2021-08-18 00:25:52.000000 pyVIP-1.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      913 2021-08-31 20:49:49.000000 pyVIP-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2021-08-18 00:25:52.000000 pyVIP-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2021-08-31 20:49:49.000000 pyVIP-1.9.0/pyVIP.egg-info/
+-rw-rw-rw-   0        0        0      913 2021-08-31 20:49:49.000000 pyVIP-1.9.0/pyVIP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2021-08-31 20:49:49.000000 pyVIP-1.9.0/pyVIP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-31 20:49:49.000000 pyVIP-1.9.0/pyVIP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2021-08-31 20:49:49.000000 pyVIP-1.9.0/pyVIP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2021-08-31 20:49:49.000000 pyVIP-1.9.0/pyVIP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      116 2021-08-18 00:25:52.000000 pyVIP-1.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2021-08-31 20:49:49.000000 pyVIP-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      923 2021-08-18 00:25:52.000000 pyVIP-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-31 20:49:49.000000 pyVIP-1.9.0/virtualitics/
+-rw-rw-rw-   0        0        0      338 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/__init__.py
+-rw-rw-rw-   0        0        0   298911 2021-08-31 20:49:25.000000 pyVIP-1.9.0/virtualitics/api.py
+-rw-rw-rw-   0        0        0     2151 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/encryption.py
+-rw-rw-rw-   0        0        0     7610 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/exceptions.py
+-rw-rw-rw-   0        0        0     2122 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/pkcs7.py
+-rw-rw-rw-   0        0        0    45880 2021-08-27 06:50:05.000000 pyVIP-1.9.0/virtualitics/task_response_handlers.py
+-rw-rw-rw-   0        0        0    18589 2021-08-26 00:50:09.000000 pyVIP-1.9.0/virtualitics/utils.py
+-rw-rw-rw-   0        0        0    24922 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/vip_annotation.py
+-rw-rw-rw-   0        0        0     4743 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/vip_dashboard.py
+-rw-rw-rw-   0        0        0     2204 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/vip_object.py
+-rw-rw-rw-   0        0        0   178579 2021-08-25 01:50:08.000000 pyVIP-1.9.0/virtualitics/vip_plot.py
+-rw-rw-rw-   0        0        0     1606 2021-08-18 00:25:52.000000 pyVIP-1.9.0/virtualitics/vip_result.py
```

### Comparing `pyVIP-1.8.0/LICENSE` & `pyVIP-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/PKG-INFO` & `pyVIP-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVIP
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python API for VIP (Virtualitics Immersive Platform)
 Home-page: UNKNOWN
 Author: Virtualitics
 Author-email: aakash@virtualitics.com
 License: MIT LICENSE
 Description: ## pyVIP - Python API for VIP
         Virtualitics is an AI driven visual analytics tool that allows
```

### Comparing `pyVIP-1.8.0/pyVIP.egg-info/PKG-INFO` & `pyVIP-1.9.0/pyVIP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVIP
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python API for VIP (Virtualitics Immersive Platform)
 Home-page: UNKNOWN
 Author: Virtualitics
 Author-email: aakash@virtualitics.com
 License: MIT LICENSE
 Description: ## pyVIP - Python API for VIP
         Virtualitics is an AI driven visual analytics tool that allows
```

### Comparing `pyVIP-1.8.0/pyVIP.egg-info/SOURCES.txt` & `pyVIP-1.9.0/pyVIP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/setup.py` & `pyVIP-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/virtualitics/api.py` & `pyVIP-1.9.0/virtualitics/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -359,14 +359,33 @@
         # Following behavior in save_project(), append vip extension if it does not exist
         if path[-4:] != ".vip":
             path += ".vip"
 
         params = {"TaskType": "LoadProject", "Path": path}
         self._api_request(params=[params], data=None)
 
+    def load_workflow(self, path):
+        """
+        Loads VIP workflow file into software from a path local to the machine running VIP. Note that any workflow
+        currently open will be discarded. To save the workflow first, please use VIP.save_workflow().
+
+        :param path: :class:`string`
+        :return: :class:`None`
+        """
+
+        if not isinstance(path, str):
+            utils.raise_invalid_argument_exception(str(type(path)), "path", "must be a string. ")
+
+        # Following behavior in save_project(), append vip extension if it does not exist
+        if path[-5:] != ".json":
+            path += ".json"
+
+        params = {"TaskType": "LoadWorkflow", "Path": path}
+        self._api_request(params=[params], data=None)
+
     def load_data(self, data, dataset_name=None):
         """
         Loads :class:`pandas.DataFrame` into VIP. Uses column dtype to determine column type in VIP.
 
         :param data: :class:`pandas.DataFrame` object that contains the users data.
         :param dataset_name: optionally pass in a name for this dataset to show in Virtualitics
         :return: :class:`None`
@@ -579,14 +598,38 @@
         if not isinstance(overwrite, bool):
             utils.raise_invalid_argument_exception(str(type(overwrite)), "overwrite", "must be a `bool`.")
 
         params["Overwrite"] = overwrite
 
         self._api_request(params=[params], data=None)
 
+    def save_workflow(self, filename: str, overwrite=False):
+        """
+        Saves VIP workflow to the specified filepath.
+
+        :param filename: absolute path to the desired save location.
+        :param overwrite: :class:`bool` that controls whether to write over a file that may exist at the specified path.
+        :return: :class:`None`
+        """
+        try:
+            path = filename
+            if path[-5:] != ".json":
+                path += ".json"
+            params = {"TaskType": "SaveWorkflow"}
+            params["Path"] = path
+        except Exception:
+            raise exceptions.InvalidSavePathException("This is not a valid path.")
+
+        if not isinstance(overwrite, bool):
+            utils.raise_invalid_argument_exception(str(type(overwrite)), "overwrite", "must be a `bool`.")
+
+        params["Overwrite"] = overwrite
+
+        self._api_request(params=[params], data=None)
+
     def convert_column(self, column, column_type: str):
         """
         Converts column to the specified type.
 
         :param column: expects column name (:class:`str`) or a :class:`pandas.Series`
         :param column_type: {"Continuous", "Categorical"}
         :return: :class:`None`
@@ -1157,19 +1200,22 @@
         params = self._add_export_to_params(export, background, imsize, path, [params])
 
         self._api_request(params=params, data=None)
 
     def plot(self, plot_type="scatter", x=None, y=None, z=None, color=None, size=None, shape=None, transparency=None,
              halo=None, halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None,
              playback_highlight=None, arrow=None, groupby=None, x_scale=None, y_scale=None, z_scale=None,
-             size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None,
+             x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+             y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+             z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+             size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None, color_palette_id=None,
              color_normalization=None, x_normalization=None, y_normalization=None, z_normalization=None,
              size_normalization=None, transparency_normalization=None, arrow_normalization=None, export="ortho", background="white",
              imsize=(2048, 2048), path=None, save_to_local_history=True, color_bins=None, color_bin_dist=None,
-             color_inverted=None, name=None, trend_lines=None, scatter_plot_point_mode=None, line_plot_point_mode=None):
+             color_inverted=None, name=None, trend_lines=None, scatter_plot_point_mode=None, line_plot_point_mode=None, viewby=None):
         """
         Requests VIP to make the specified plot. Expects column name or :class:`pandas.Series` dimension parameters.
         Plot type is expected to be string.
 
         :param plot_type: {"scatter", "hist", "line", "maps3d", "maps2d", "ellipsoid", "surface", "convex_hull"};
             default is "scatter"
         :param x: X dimension
@@ -1189,21 +1235,37 @@
         :param playback_highlight: Optionally select a single value of the feature mapped to the Playback dimension.
             All points with this value will be shown and all other points will be hidden.
         :param arrow: Arrow dimension. Works with continuous and categorical features.
         :param groupby: Group By dimension. Works with categorical columns.
         :param x_scale: Scaling factor for X dimension. Value must be between .5 and 5.
         :param y_scale: Scaling factor for Y dimension. Value must be between .5 and 5.
         :param z_scale: Scaling factor for Z dimension. Value must be between .5 and 5.
+        :param x_range_min: Minimum visible value for the X dimension.
+        :param x_range_max: Maximum visible value for the X dimension.
+        :param x_limit_min: Minimum value displayed for the X dimension on the axis/grid box.
+        :param x_limit_max: Maximum value displayed for the X dimension on the axis/grid box.
+        :param x_limit_link: Whether limit is locked to range.
+        :param y_range_min: Minimum visible value for the Y dimension.
+        :param y_range_max: Maximum visible value for the Y dimension.
+        :param y_limit_min: Minimum value displayed for the Y dimension on the axis/grid box.
+        :param y_limit_max: Maximum value displayed for the Y dimension on the axis/grid box.
+        :param y_limit_link: Whether limit is locked to range.
+        :param z_range_min: Minimum visible value for the Z dimension.
+        :param z_range_max: Maximum visible value for the Z dimension.
+        :param z_limit_min: Minimum value displayed for the Z dimension on the axis/grid box.
+        :param z_limit_max: Maximum value displayed for the Z dimension on the axis/grid box.
+        :param z_limit_link: Whether limit is locked to range.
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "gradient", "bin", or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default but "gradient"
             can also be used.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param color_normalization: Normalization setting for color. This can only be set if the color type is set to
             "Gradient". The options are "Log10", "Softmax", "IHST"
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -1230,28 +1292,33 @@
         :param name: :class:`str` specifying the name of the plot. Default to None. A name will be automatically
             generated in VIP.
         :param trend_lines: :class:`str` specifying whether to build trend lines for the plot, and how they should be broken down.
             Options: None, Color, GroupBy, All.
             Note: Trend lines are only available for scatter plot and line plot types.
         :param scatter_plot_point_mode: :class:`str` specifies whether to show or hide points in a scatter plot visualization. (Only valid for plot_type = 'scatter_plot')
         :param line_plot_point_mode: :class:`str` specifies whether to show or hide points and lines in a line plot visualization. (Only valid for plot_type = 'line_plot')
+        :param viewby: :class:`str` specifies which viewby mode ("color" or "groupby") to use in a line plot visualization. (Only valid for plot_type = 'line_plot')
         :return: :class:`None`
         """
         plot_type = utils.case_insensitive_match(utils.PLOT_TYPE_ALIASES, plot_type, "plot_type")
         if plot_type == "SCATTER_PLOT":
             if line_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.scatter(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                                 halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                                 pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby,
-                                x_scale=x_scale, y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
+                                x_scale=x_scale, y_scale=y_scale, z_scale=z_scale, 
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
+                                size_scale=size_scale,
                                 transparency_scale=transparency_scale, halo_scale=halo_scale, arrow_scale=arrow_scale,
-                                color_type=color_type, color_normalization=color_normalization,
+                                color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                 x_normalization=x_normalization, y_normalization=y_normalization,
                                 z_normalization=z_normalization, size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, export=export, background=background, imsize=imsize, path=path,
                                 save_to_local_history=save_to_local_history, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name, trend_lines=trend_lines, scatter_plot_point_mode=scatter_plot_point_mode)
         elif plot_type == "LINE_PLOT":
@@ -1259,35 +1326,42 @@
                 raise exceptions.InvalidUsageException("'scatter_plot_point_mode' is only applicable when plot_type='scatter_plot'")
 
             return self.line(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                              halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                              pulsation_highlight=pulsation_highlight, playback=playback,
                              playback_highlight=playback_highlight, arrow=arrow, groupby=groupby,
                              x_scale=x_scale, y_scale=y_scale, z_scale=z_scale,
+                             x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                             y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                             z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                              size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                             arrow_scale=arrow_scale, color_type=color_type, x_normalization=x_normalization,
-                             y_normalization=y_normalization, z_normalization=z_normalization,
+                             arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization, 
+                             x_normalization=x_normalization, y_normalization=y_normalization, z_normalization=z_normalization,
                              size_normalization=size_normalization,
                              transparency_normalization=transparency_normalization,
                              arrow_normalization=arrow_normalization, export=export, background=background, imsize=imsize, path=path,
                              save_to_local_history=save_to_local_history, color_bins=color_bins,
-                             color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name, trend_lines=trend_lines, line_plot_point_mode=line_plot_point_mode)
+                             color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name, trend_lines=trend_lines, 
+                             line_plot_point_mode=line_plot_point_mode, viewby=viewby)
         elif plot_type == "VIOLIN_PLOT":
             if scatter_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'scatter_plot_point_mode' is only applicable when plot_type='scatter_plot'")
             if line_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.violin(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                                halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                                pulsation_highlight=pulsation_highlight, playback=playback,
                                playback_highlight=playback_highlight, arrow=arrow, groupby=groupby,
                                x_scale=x_scale, y_scale=y_scale, z_scale=z_scale,
+                               x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                               y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                               z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                               arrow_scale=arrow_scale, color_type=color_type, color_normalization=color_normalization,
+                               arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                x_normalization=x_normalization, y_normalization=y_normalization,
                                z_normalization=z_normalization, size_normalization=size_normalization,
                                transparency_normalization=transparency_normalization,
                                arrow_normalization=arrow_normalization, export=export, background=background, imsize=imsize, path=path,
                                save_to_local_history=save_to_local_history, color_bins=color_bins,
                                color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         elif plot_type == "CONVEX_HULL":
@@ -1297,16 +1371,19 @@
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.convex_hull(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                                     halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                                     pulsation_highlight=pulsation_highlight, playback=playback,
                                     playback_highlight=playback_highlight, arrow=arrow, groupby=groupby,
                                     x_scale=x_scale, y_scale=y_scale, z_scale=z_scale,
+                                    x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                    y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                    z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                     size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                    arrow_scale=arrow_scale, color_type=color_type, x_normalization=x_normalization,
+                                    arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, x_normalization=x_normalization,
                                     y_normalization=y_normalization, z_normalization=z_normalization,
                                     size_normalization=size_normalization,
                                     transparency_normalization=transparency_normalization,
                                     arrow_normalization=arrow_normalization, export=export, background=background, imsize=imsize, path=path,
                                     save_to_local_history=save_to_local_history, color_bins=color_bins,
                                     color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         elif plot_type == "CONFIDENCE_ELLIPSOID":
@@ -1316,16 +1393,19 @@
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.ellipsoid(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                                   halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                                   pulsation_highlight=pulsation_highlight, playback=playback,
                                   playback_highlight=playback_highlight, arrow=arrow, groupby=groupby,
                                   x_scale=x_scale, y_scale=y_scale, z_scale=z_scale,
+                                  x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                  y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                  z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                   size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                  arrow_scale=arrow_scale, color_type=color_type, x_normalization=x_normalization,
+                                  arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, x_normalization=x_normalization,
                                   y_normalization=y_normalization, z_normalization=z_normalization,
                                   size_normalization=size_normalization,
                                   transparency_normalization=transparency_normalization,
                                   arrow_normalization=arrow_normalization, export=export, background=background, imsize=imsize, path=path,
                                   save_to_local_history=save_to_local_history, color_bins=color_bins,
                                   color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         elif plot_type == "HISTOGRAM":
@@ -1334,49 +1414,58 @@
             if line_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.hist(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                              halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                              pulsation_highlight=pulsation_highlight, playback=playback,
                              arrow=arrow, groupby=groupby,
-                             x_scale=x_scale, y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
-                             transparency_scale=transparency_scale, halo_scale=halo_scale, arrow_scale=arrow_scale,
-                             color_type=color_type, x_normalization=x_normalization, y_normalization=y_normalization,
+                             x_scale=x_scale, y_scale=y_scale, z_scale=z_scale, 
+                             x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                             y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                             z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
+                             size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale, arrow_scale=arrow_scale,
+                             color_type=color_type, color_palette_id=color_palette_id, x_normalization=x_normalization, y_normalization=y_normalization,
                              z_normalization=z_normalization, size_normalization=size_normalization,
                              transparency_normalization=transparency_normalization,
                              arrow_normalization=arrow_normalization, export=export, background=background, imsize=imsize, path=path,
                              save_to_local_history=save_to_local_history, color_bins=color_bins,
                              color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         elif plot_type == "MAPS2D":
             if scatter_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'scatter_plot_point_mode' is only applicable when plot_type='scatter_plot'")
             if line_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.maps2d(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                                halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                                pulsation_highlight=pulsation_highlight, playback=playback, groupby=groupby,
+                               x_range_min=x_range_min, x_range_max=x_range_max,
+                               y_range_min=y_range_min, y_range_max=y_range_max,
+                               z_range_min=z_range_min, z_range_max=z_range_max, z_scale=z_scale,
                                size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                               color_type=color_type, color_normalization=color_normalization,
+                               color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                size_normalization=size_normalization,
                                transparency_normalization=transparency_normalization, export="front", background=background, imsize=imsize,
                                path=path, save_to_local_history=save_to_local_history, color_bins=color_bins,
                                color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         elif plot_type == "MAPS3D":
             if scatter_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'scatter_plot_point_mode' is only applicable when plot_type='scatter_plot'")
             if line_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.maps3d(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                                halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                                pulsation_highlight=pulsation_highlight, playback=playback,
                                playback_highlight=playback_highlight, groupby=groupby,
+                               x_range_min=x_range_min, x_range_max=x_range_max,
+                               y_range_min=y_range_min, y_range_max=y_range_max,
+                               z_range_min=z_range_min, z_range_max=z_range_max, z_scale=z_scale,
                                size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                               color_type=color_type, color_normalization=color_normalization,
+                               color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                size_normalization=size_normalization,
                                transparency_normalization=transparency_normalization, export=export, background=background, imsize=imsize,
                                path=path, save_to_local_history=save_to_local_history, color_bins=color_bins,
                                color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         elif plot_type == "SURFACE":
             if scatter_plot_point_mode is not None:
                 raise exceptions.InvalidUsageException("'scatter_plot_point_mode' is only applicable when plot_type='scatter_plot'")
@@ -1384,27 +1473,33 @@
                 raise exceptions.InvalidUsageException("'line_plot_point_mode' is only applicable when plot_type='line_plot'")
 
             return self.surface(x=x, y=y, z=z, color=color, size=size, shape=shape, transparency=transparency,
                                 halo=halo, halo_highlight=halo_highlight, pulsation=pulsation,
                                 pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby,
                                 x_scale=x_scale, y_scale=y_scale, z_scale=z_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                arrow_scale=arrow_scale, color_type=color_type, color_normalization=color_normalization,
+                                arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                 x_normalization=x_normalization, y_normalization=y_normalization,
                                 z_normalization=z_normalization, size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, export=export, background=background, imsize=imsize, path=path,
                                 save_to_local_history=save_to_local_history, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
 
     def scatter(self, x=None, y=None, z=None, color=None, size=None, shape=None, transparency=None, halo=None,
                 halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None, playback_highlight=None,
-                arrow=None, groupby=None, x_scale=None, y_scale=None, z_scale=None, size_scale=None,
-                transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None, color_normalization=None,
+                arrow=None, groupby=None, x_scale=None, y_scale=None, z_scale=None, 
+                x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+                y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+                z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+                size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None, color_palette_id=None, color_normalization=None,
                 x_normalization=None, y_normalization=None, z_normalization=None, size_normalization=None,
                 transparency_normalization=None, arrow_normalization=None, color_inverted=None, export="ortho", background="white",
                 imsize=(2048, 2048), path=None, save_to_local_history=True, color_bins=None, color_bin_dist=None,
                 name=None, trend_lines=None, scatter_plot_point_mode=None):
         """
         Generates scatter plot in VIP. Expects column name or pandas data series dimension parameters.
 
@@ -1432,14 +1527,15 @@
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "gradient", "bin", or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default but "gradient"
             can also be used.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_normalization: Normalization setting for color. This can only be set if the color type is set to
             "Gradient". The options are "Log10", "Softmax", "IHST"
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -1473,16 +1569,19 @@
         """
         # Pass dimension info
         plot = vip_plot.VipPlot(plot_type="SCATTER", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby, x_scale=x_scale,
                                 y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 transparency_scale=transparency_scale, halo_scale=halo_scale, arrow_scale=arrow_scale,
-                                color_type=color_type, color_normalization=color_normalization,
+                                color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                 x_normalization=x_normalization, y_normalization=y_normalization,
                                 z_normalization=z_normalization, size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, color_inverted=color_inverted,
                                 color_bins=color_bins, color_bin_dist=color_bin_dist, name=name, trend_lines=trend_lines, 
                                 scatter_plot_point_mode=scatter_plot_point_mode)
         params = [plot.get_params()]
@@ -1492,16 +1591,21 @@
         params = self._add_export_to_params(export, background, imsize, path, params)
         params = self._add_plot_mapping_to_params(params, save_to_local_history)
 
         return self._api_request(params=params, data=None)
 
     def hist(self, x=None, y=None, z=None, color=None, size=None, shape=None, transparency=None, halo=None,
              halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None, arrow=None, groupby=None,
-             x_scale=None, y_scale=None, z_scale=None, size_scale=None, transparency_scale=None, halo_scale=None,
-             arrow_scale=None, color_type=None, x_normalization=None, y_normalization=None, z_normalization=None,
+             x_scale=None, y_scale=None, z_scale=None, 
+             x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+             y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+             z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+             size_scale=None, transparency_scale=None, halo_scale=None,
+             arrow_scale=None, color_type=None, color_palette_id=None,
+             x_normalization=None, y_normalization=None, z_normalization=None,
              size_normalization=None, transparency_normalization=None, arrow_normalization=None, export="ortho", background="white",
              imsize=(2048, 2048), path=None, save_to_local_history=True, color_bins=None, color_bin_dist=None,
              color_inverted=False, volume_by=None, x_bins=None, y_bins=None, z_bins=None, name=None):
         """
         Generates Histogram in VIP. Expects column name or pandas data series dimension parameters.
 
         :param x: X dimension
@@ -1526,14 +1630,15 @@
         :param z_scale: Scaling factor for Z dimension. Value must be between .5 and 5.
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "bin" or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param z_normalization: Normalization setting for Z. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -1564,16 +1669,19 @@
         :return: :class:`None`
         """
         # Pass dimension info
         plot = vip_plot.VipPlot(plot_type="HISTOGRAM", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, arrow=arrow,
                                 playback=playback, groupby=groupby, x_scale=x_scale, y_scale=y_scale, z_scale=z_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 size_scale=size_scale, transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                arrow_scale=arrow_scale, color_type=color_type, x_normalization=x_normalization,
+                                arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, x_normalization=x_normalization,
                                 y_normalization=y_normalization, z_normalization=z_normalization,
                                 size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, color_inverted=color_inverted, hist_volume_by=volume_by,
                                 x_bins=x_bins, y_bins=y_bins, z_bins=z_bins, name=name)
         params = [plot.get_params()]
@@ -1584,16 +1692,19 @@
         params = self._add_plot_mapping_to_params(params, save_to_local_history)
 
         return self._api_request(params=params, data=None)
 
     def line(self, x=None, y=None, z=None, show_points=True, color=None, size=None, shape=None, transparency=None,
              halo=None, halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None,
              playback_highlight=None, arrow=None, groupby=None, x_scale=None, y_scale=None, z_scale=None,
-             size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None,
-             x_normalization=None, y_normalization=None, z_normalization=None, size_normalization=None,
+             x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+             y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+             z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+             size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None, color_palette_id=None,
+             x_normalization=None, y_normalization=None, z_normalization=None, size_normalization=None, color_normalization=None,
              transparency_normalization=None, arrow_normalization=None, export="ortho", background="white", imsize=(2048, 2048), path=None,
              save_to_local_history=True, color_bins=None, color_bin_dist=None, viewby=None, color_inverted=None,
              name=None, trend_lines=None, line_plot_point_mode=None):
         """
         Generates line plot in VIP. Expects column name or pandas data series dimension parameters.
 
         :param x: X dimension
@@ -1621,21 +1732,24 @@
         :param z_scale: Scaling factor for Z dimension. Value must be between .5 and 5.
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "bin" or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param z_normalization: Normalization setting for Z. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
+        :param color_normalization: Normalization setting for Color. This can only be set if the feature mapped to
+            this dimension is numerical and continuous, the color_type is set to "gradient" and the view-by mode is set to "groupby". The options are "Log10", "Softmax", "IHST"
         :param size_normalization: Normalization setting for Size. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param transparency_normalization: Normalization setting for Transparency.This can only be set if the feature
             mapped to this dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param arrow_normalization: Normalization setting for Arrow. This can only be set if the feature mapped to
             this dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param export: Specify whether to export a capture of the plot. Defaults to "ortho". Options are {"ortho",
@@ -1662,17 +1776,20 @@
         """
         # Pass dimension info
         plot = vip_plot.VipPlot(plot_type="LINE_PLOT", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby, x_scale=x_scale,
                                 y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                arrow_scale=arrow_scale, color_type=color_type, x_normalization=x_normalization,
-                                y_normalization=y_normalization, z_normalization=z_normalization,
+                                arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, x_normalization=x_normalization,
+                                y_normalization=y_normalization, z_normalization=z_normalization, color_normalization=color_normalization,
                                 size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization, color_inverted=color_inverted,
                                 arrow_normalization=arrow_normalization, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, name=name, show_points=show_points, viewby=viewby, 
                                 trend_lines=trend_lines, line_plot_point_mode=line_plot_point_mode)
         params = [plot.get_params()]
 
@@ -1682,15 +1799,18 @@
         params = self._add_plot_mapping_to_params(params, save_to_local_history)
 
         return self._api_request(params=params, data=None)
 
     def maps3d(self, x=None, y=None, z=None, color=None, size=None, shape=None, transparency=None, halo=None,
                halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None, playback_highlight=None,
                groupby=None, arrow=None, z_scale=None, size_scale=None, transparency_scale=None, halo_scale=None,
-               arrow_scale=None, color_type=None, z_normalization=None, color_normalization=None,
+               arrow_scale=None, color_type=None, color_palette_id=None, z_normalization=None, color_normalization=None,
+               x_range_min=None, x_range_max=None, 
+               y_range_min=None, y_range_max=None, 
+               z_range_min=None, z_range_max=None,
                size_normalization=None, transparency_normalization=None, arrow_normalization=None, export="ortho", background="white",
                imsize=(2048, 2048), path=None, save_to_local_history=True, lat_long_lines=True, country_lines=None,
                country_labels=None, globe_style="natural", heatmap_enabled=False, heatmap_intensity=None,
                heatmap_radius=None, heatmap_radius_unit=None, heatmap_feature=False, return_data=False,
                color_bins=None, color_bin_dist=None, color_inverted=None, name=None):
         """
         Generates 3D Map plot in VIP. Expects column name or pandas data series dimension parameters.
@@ -1718,14 +1838,15 @@
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "gradient", "bin", or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default but "gradient"
             can also be used.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param z_normalization: Normalization setting for Z. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param color_normalization: Normalization setting for color. This can only be set if the color type is set to
             "Gradient". The options are "Log10", "Softmax", "IHST"
         :param size_normalization: Normalization setting for Size. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -1766,15 +1887,18 @@
         """
         # Pass dimension info
         plot = vip_plot.VipPlot(plot_type="MAPS3D", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, groupby=groupby, arrow=arrow,
                                 z_scale=z_scale, size_scale=size_scale, transparency_scale=transparency_scale,
-                                halo_scale=halo_scale, arrow_scale=arrow_scale, color_type=color_type,
+                                halo_scale=halo_scale, arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id,
+                                x_range_min=x_range_min, x_range_max=x_range_max,
+                                y_range_min=y_range_min, y_range_max=y_range_max,
+                                z_range_min=z_range_min, z_range_max=z_range_max,
                                 z_normalization=z_normalization, color_normalization=color_normalization,
                                 size_normalization=size_normalization, arrow_normalization=arrow_normalization,
                                 transparency_normalization=transparency_normalization, lat_long_lines=lat_long_lines,
                                 country_lines=country_lines, country_labels=country_labels, globe_style=globe_style,
                                 heatmap_enabled=heatmap_enabled, heatmap_intensity=heatmap_intensity,
                                 heatmap_radius=heatmap_radius, heatmap_radius_unit=heatmap_radius_unit,
                                 color_bins=color_bins, color_bin_dist=color_bin_dist, color_inverted=color_inverted,
@@ -1793,16 +1917,20 @@
                                                    "been set to `True`. ")
 
         return self._api_request(params=params, data=None)
 
     def maps2d(self, x=None, y=None, z=None, color=None, size=None, shape=None, transparency=None, halo=None,
                halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None, playback_highlight=None,
                arrow=None, groupby=None, z_scale=None, size_scale=None, transparency_scale=None, halo_scale=None,
-               arrow_scale=None, color_type=None, z_normalization=None, color_normalization=None,
-               size_normalization=None, transparency_normalization=None, arrow_normalization=None, export="front", background="white",
+               arrow_scale=None, color_type=None, color_palette_id=None, z_normalization=None, color_normalization=None,
+               x_range_min=None, x_range_max=None, 
+               y_range_min=None, y_range_max=None, 
+               z_range_min=None, z_range_max=None,
+               size_normalization=None, transparency_normalization=None, arrow_normalization=None, 
+               export="front", background="white",
                imsize=(2048, 2048), path=None, save_to_local_history=True, map_provider="ArcGIS",
                map_style="Topographic", heatmap_enabled=False, heatmap_intensity=None, heatmap_radius=None,
                heatmap_radius_unit=None, heatmap_feature=False, return_data=False, color_bins=None,
                color_bin_dist=None, color_inverted=None, name=None):
         """
         Generates 2D Map plot in VIP. Expects column name or pandas data series dimension parameters.
 
@@ -1829,14 +1957,15 @@
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "gradient", "bin", or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default but "gradient"
             can also be used.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param z_normalization: Normalization setting for Z. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param color_normalization: Normalization setting for color. This can only be set if the color type is set to
             "Gradient". The options are "Log10", "Softmax", "IHST"
         :param size_normalization: Normalization setting for Size. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -1875,15 +2004,18 @@
         """
         # Pass dimension info
         plot = vip_plot.VipPlot(plot_type="MAPS2D", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, groupby=groupby, arrow=arrow,
                                 z_scale=z_scale, size_scale=size_scale, transparency_scale=transparency_scale,
-                                halo_scale=halo_scale, arrow_scale=arrow_scale, color_type=color_type,
+                                halo_scale=halo_scale, arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id,
+                                x_range_min=x_range_min, x_range_max=x_range_max,
+                                y_range_min=y_range_min, y_range_max=y_range_max,
+                                z_range_min=z_range_min, z_range_max=z_range_max,
                                 z_normalization=z_normalization, color_normalization=color_normalization,
                                 size_normalization=size_normalization, arrow_normalization=arrow_normalization,
                                 transparency_normalization=transparency_normalization, heatmap_enabled=heatmap_enabled,
                                 heatmap_intensity=heatmap_intensity, heatmap_radius=heatmap_radius,
                                 heatmap_radius_unit=heatmap_radius_unit, map_provider=map_provider,
                                 color_inverted=color_inverted, map_style=map_style, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, name=name)
@@ -1901,16 +2033,20 @@
                                                    "been set to `True`. ")
 
         return self._api_request(params=params, data=None)
 
     def ellipsoid(self, confidence=95.0, show_points=True, x=None, y=None, z=None, color=None, size=None, shape=None,
                   transparency=None, halo=None, halo_highlight=None, pulsation=None, pulsation_highlight=None,
                   playback=None, playback_highlight=None, arrow=None, groupby=None, x_scale=None, y_scale=None,
-                  z_scale=None, size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None,
-                  color_type=None, x_normalization=None, y_normalization=None, z_normalization=None,
+                  z_scale=None, 
+                  x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+                  y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+                  z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+                  size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None,
+                  color_type=None, color_palette_id=None, x_normalization=None, y_normalization=None, z_normalization=None,
                   size_normalization=None, transparency_normalization=None, arrow_normalization=None, export="ortho", background="white",
                   imsize=(2048, 2048), path=None, save_to_local_history=True, color_bins=None, color_bin_dist=None,
                   color_inverted=None, name=None):
         """
         Generates Ellipsoid plot in VIP. Expects column name or pandas data series dimension parameters.
 
         :param confidence: :class:`float` confidence probability that must be in {99.5, 99.0, 97.5, 95.0, 90.0, 80.0,
@@ -1940,14 +2076,15 @@
         :param z_scale: Scaling factor for Z dimension. Value must be between .5 and 5.
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "bin" or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param z_normalization: Normalization setting for Z. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -1976,16 +2113,19 @@
         """
         # Pass dimension info
         plot = vip_plot.VipPlot(plot_type="CONFIDENCE_ELLIPSOID", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby, x_scale=x_scale,
                                 y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                arrow_scale=arrow_scale, color_type=color_type, x_normalization=x_normalization,
+                                arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, x_normalization=x_normalization,
                                 y_normalization=y_normalization, z_normalization=z_normalization,
                                 size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, confidence=confidence, show_points=show_points,
                                 color_bins=color_bins, color_bin_dist=color_bin_dist, color_inverted=color_inverted,
                                 name=name)
         params = [plot.get_params()]
@@ -1995,17 +2135,21 @@
         params = self._add_export_to_params(export, background, imsize, path, params)
         params = self._add_plot_mapping_to_params(params, save_to_local_history)
 
         return self._api_request(params=params, data=None)
 
     def convex_hull(self, show_points=True, x=None, y=None, z=None, color=None, size=None, shape=None,
                     transparency=None, halo=None, halo_highlight=None, pulsation=None, pulsation_highlight=None,
-                    playback=None, playback_highlight=None, arrow=None, groupby=None, x_scale=None, y_scale=None,
-                    z_scale=None, size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None,
-                    color_type=None, x_normalization=None, y_normalization=None, z_normalization=None,
+                    playback=None, playback_highlight=None, arrow=None, groupby=None, 
+                    x_scale=None, y_scale=None, z_scale=None, 
+                    x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+                    y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+                    z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+                    size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None,
+                    color_type=None, color_palette_id=None, x_normalization=None, y_normalization=None, z_normalization=None,
                     size_normalization=None, transparency_normalization=None, arrow_normalization=None, export="ortho", background="white",
                     imsize=(2048, 2048), path=None, save_to_local_history=True, color_bins=None, color_bin_dist=None,
                     color_inverted=None, name=None):
         """
         Generates Convex Hull plot in VIP. Expects column name or pandas data series dimension parameters.
 
         :param show_points: Setting for how to view the convex hull. Valid options are {True, False, "show", "hide"}
@@ -2032,14 +2176,15 @@
         :param z_scale: Scaling factor for Z dimension. Value must be between .5 and 5.
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "bin" or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param z_normalization: Normalization setting for Z. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -2066,16 +2211,19 @@
         :return: :class:`None`
         """
         plot = vip_plot.VipPlot(plot_type="CONVEX_HULL", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby, x_scale=x_scale,
                                 y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                arrow_scale=arrow_scale, color_type=color_type, x_normalization=x_normalization,
+                                arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, x_normalization=x_normalization,
                                 y_normalization=y_normalization, z_normalization=z_normalization,
                                 size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, show_points=show_points, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         params = [plot.get_params()]
 
@@ -2084,16 +2232,20 @@
         params = self._add_export_to_params(export, background, imsize, path, params)
         params = self._add_plot_mapping_to_params(params, save_to_local_history)
 
         return self._api_request(params=params, data=None)
 
     def violin(self, x=None, y=None, z=None, color=None, size=None, shape=None, transparency=None, halo=None,
                halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None, playback_highlight=None,
-               arrow=None, groupby=None, x_scale=None, y_scale=None, z_scale=None, size_scale=None,
-               transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None, color_normalization=None,
+               arrow=None, groupby=None, 
+               x_scale=None, y_scale=None, z_scale=None, 
+               x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+               y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+               z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+               size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None, color_palette_id=None, color_normalization=None,
                x_normalization=None, y_normalization=None, z_normalization=None, size_normalization=None,
                transparency_normalization=None, arrow_normalization=None, export="ortho", background="white", imsize=(2048, 2048),
                path=None, save_to_local_history=True, color_bins=None, color_bin_dist=None, color_inverted=None, name=None):
         """
         Generates violin plot in VIP. Expects column name or pandas data series dimension parameters.
 
         :param x: X dimension
@@ -2120,14 +2272,15 @@
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "gradient", "bin", or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default but "gradient"
             can also be used.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param color_normalization: Normalization setting for color. This can only be set if the color type is set to
             "Gradient". The options are "Log10", "Softmax", "IHST"
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -2156,16 +2309,19 @@
         :return: :class:`None`
         """
         plot = vip_plot.VipPlot(plot_type="VIOLIN_PLOT", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby, x_scale=x_scale,
                                 y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 transparency_scale=transparency_scale, halo_scale=halo_scale,
-                                arrow_scale=arrow_scale, color_type=color_type, color_normalization=color_normalization,
+                                arrow_scale=arrow_scale, color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                 x_normalization=x_normalization, y_normalization=y_normalization,
                                 z_normalization=z_normalization, size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         params = [plot.get_params()]
 
@@ -2175,15 +2331,18 @@
         params = self._add_plot_mapping_to_params(params, save_to_local_history)
 
         return self._api_request(params=params, data=None)
 
     def surface(self, show_points=False, x=None, y=None, z=None, color=None, size=None, shape=None, transparency=None,
                 halo=None, halo_highlight=None, pulsation=None, pulsation_highlight=None, playback=None,
                 playback_highlight=None, arrow=None, groupby=None, x_scale=None, y_scale=None, z_scale=None,
-                size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None,
+                x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+                y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+                z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+                size_scale=None, transparency_scale=None, halo_scale=None, arrow_scale=None, color_type=None, color_palette_id=None,
                 color_normalization=None, x_normalization=None, y_normalization=None, z_normalization=None,
                 size_normalization=None, transparency_normalization=None, arrow_normalization=None, export="ortho", background="white",
                 imsize=(2048, 2048), path=None, save_to_local_history=True, color_bins=None, color_bin_dist=None,
                 color_inverted=None, name=None):
         """
         Generates Surface plot in VIP. Expects column name or pandas data series dimension parameters.
 
@@ -2212,14 +2371,15 @@
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param arrow_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param color_type: User can select "gradient", "bin", or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default but "gradient"
             can also be used.
+        :param color_palette_id: User can select the color palette based on the available palettes for the specified color_type.
         :param color_inverted: :class:`bool` controlling the order of colors for all color types.
         :param color_normalization: Normalization setting for color. This can only be set if the color type is set to
             "Gradient". The options are "Log10", "Softmax", "IHST"
         :param x_normalization: Normalization setting for X. This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y.This can only be set if the feature mapped to this
             dimension is numerical and continuous. The options are "Log10", "Softmax", "IHST"
@@ -2248,16 +2408,19 @@
         :return: :class:`None`
         """
         plot = vip_plot.VipPlot(plot_type="SURFACE", x=x, y=y, z=z, color=color, size=size, shape=shape,
                                 transparency=transparency, halo=halo, halo_highlight=halo_highlight,
                                 pulsation=pulsation, pulsation_highlight=pulsation_highlight, playback=playback,
                                 playback_highlight=playback_highlight, arrow=arrow, groupby=groupby, x_scale=x_scale,
                                 y_scale=y_scale, z_scale=z_scale, size_scale=size_scale,
+                                x_range_min=x_range_min, x_range_max=x_range_max, x_limit_min=x_limit_min, x_limit_max=x_limit_max, x_limit_link=x_limit_link,
+                                y_range_min=y_range_min, y_range_max=y_range_max, y_limit_min=y_limit_min, y_limit_max=y_limit_max, y_limit_link=y_limit_link,
+                                z_range_min=z_range_min, z_range_max=z_range_max, z_limit_min=z_limit_min, z_limit_max=z_limit_max, z_limit_link=z_limit_link,
                                 transparency_scale=transparency_scale, halo_scale=halo_scale, arrow_scale=arrow_scale,
-                                color_type=color_type, color_normalization=color_normalization,
+                                color_type=color_type, color_palette_id=color_palette_id, color_normalization=color_normalization,
                                 x_normalization=x_normalization, y_normalization=y_normalization,
                                 z_normalization=z_normalization, size_normalization=size_normalization,
                                 transparency_normalization=transparency_normalization,
                                 arrow_normalization=arrow_normalization, show_points=show_points, color_bins=color_bins,
                                 color_bin_dist=color_bin_dist, color_inverted=color_inverted, name=name)
         params = [plot.get_params()]
 
@@ -2418,15 +2581,15 @@
         :param exclude: List of column names to exclude in the analysis; this overrides any features listed in the
             `features` parameter.
         :param plus_minus: Include outliers that are above, below, or above and below the desired standard deviation
             mark. Defaults to both. Can be "both", "plus", or "minus"
         :param stdev: User defined standard deviation on which to classify outliers.
         :param and_or: "and" identifies data points that are outliers in all input features. "or" identifies data
             points that are outliers in any of the input features.
-        :param apply: :class:`bool` for whether to apply the result to the halo dimension.
+        :param apply: [Deprecated]:class:`bool` for whether to apply the result to the halo dimension.
         :param return_anomalies_df: Whether to return the output of the process to the notebook. Defaults to True.
         :param export: Specify whether to export a capture of the plot. Can be None/False or "ortho", "front",
             "side" or "right", "top", or "perspective"
         :param background: Specify whether to export a plot capture with a white background, or the default color
             scheme configured in VIP. Options are {"white", "default"}. White is used if the value is not specified.
         :param imsize: size of the returned dimension; [w, h]. Only used if `export` is not None. Defaults to
             (2048, 2048)
@@ -2462,24 +2625,31 @@
         if exclude is not None:
             params["Exclude"] = utils.get_features(exclude)
 
         params['ReturnData'] = return_anomalies_df
 
         params["KeepMissingValueColumns"] = keep_missing_value_columns
 
-        if isinstance(apply, bool):
-            if apply:
-                params["Apply"] = apply
-                params = [params]
-                params = self._add_export_to_params(export, background, imsize, path, params)
-                params = self._add_plot_mapping_to_params(params, save_to_local_history)
-            else:
-                params = [params]
-        else:
-            utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+        # if isinstance(apply, bool):
+        #     if apply:
+        #         params["Apply"] = apply
+        #         params = [params]
+        #         params = self._add_export_to_params(export, background, imsize, path, params)
+        #         params = self._add_plot_mapping_to_params(params, save_to_local_history)
+        #     else:
+        #         params = [params]
+        # else:
+        #     utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+        params = [params]
+        
+        if export is not None and export is not False:
+            params = self._add_export_to_params(export, background, imsize, path, params)
+
+        params = self._add_plot_mapping_to_params(params, save_to_local_history)
+
         return self._api_request(params=params, data=None)
 
     def threshold_ad(self, features=None, exclude=None, return_anomalies_df=True, threshold=1, apply=True,
                      export="ortho", background="white", imsize=(2048, 2048), path=None, save_to_local_history=True,
                      keep_missing_value_columns=True):
         """
         Alias to pca_anomaly_detection
@@ -2495,15 +2665,15 @@
         :param background: Specify whether to export a plot capture with a white background, or the default color
             scheme configured in VIP. Options are {"white", "default"}. White is used if the value is not specified.
         :param imsize: size of the returned dimension; [w, h]. Only used if `export` is not None. Defaults to
             (2048, 2048)
         :param path: Filepath to save snapshot; filepath should end with a jpg/jpeg/png/bmp extension
         :param save_to_local_history: :class:`bool`; whether to save VipPlot object to `this.local_history` list.
             Default value is True.
-        :param apply: :class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
+        :param apply: [Deprecated]:class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
             Default is True.
         :param keep_missing_value_columns: :class:`bool` for whether to keep features with more than 50% missing
             values as part of the input for pca based anomaly detection. Default is `True`.
         :return: :class:`None`
         """
         return self.pca_anomaly_detection(features, exclude, return_anomalies_df, threshold, apply, export, background, imsize,
                                           path, save_to_local_history, keep_missing_value_columns)
@@ -2525,15 +2695,15 @@
         :param background: Specify whether to export a plot capture with a white background, or the default color
             scheme configured in VIP. Options are {"white", "default"}. White is used if the value is not specified.
         :param imsize: size of the returned dimension; [w, h]. Only used if `export` is not None. Defaults to
             (2048, 2048)
         :param path: Filepath to save snapshot; filepath should end with a jpg/jpeg/png/bmp extension
         :param save_to_local_history: :class:`bool`; whether to save VipPlot object to `this.local_history` list.
             Default value is True.
-        :param apply: :class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
+        :param apply: [Deprecated]:class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
             Default is True.
         :param keep_missing_value_columns: :class:`bool` for whether to keep features with more than 50% missing
             values as part of the input for pca based anomaly detection. Default is `True`.
         :return: :class:`None`
         """
         return self.pca_anomaly_detection(features, exclude, return_anomalies_df, threshold, apply, export, background, imsize,
                                           path, save_to_local_history, keep_missing_value_columns)
@@ -2555,15 +2725,15 @@
         :param background: Specify whether to export a plot capture with a white background, or the default color
             scheme configured in VIP. Options are {"white", "default"}. White is used if the value is not specified.
         :param imsize: size of the returned dimension; [w, h]. Only used if `export` is not None. Defaults to
             (2048, 2048)
         :param path: Filepath to save snapshot; filepath should end with a jpg/jpeg/png/bmp extension
         :param save_to_local_history: :class:`bool`; whether to save VipPlot object to `this.local_history` list.
             Default value is True.
-        :param apply: :class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
+        :param apply: [Deprecated]:class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
             Default is True.
         :param keep_missing_value_columns: :class:`bool` for whether to keep features with more than 50% missing
             values as part of the input for pca based anomaly detection. Default is `True`.
         :return: :class:`None`
         """
         return self.pca_anomaly_detection(features, exclude, return_anomalies_df, threshold, apply, export, background, imsize,
                                           path, save_to_local_history, keep_missing_value_columns)
@@ -2585,15 +2755,15 @@
         :param background: Specify whether to export a plot capture with a white background, or the default color
             scheme configured in VIP. Options are {"white", "default"}. White is used if the value is not specified.
         :param imsize: size of the returned dimension; [w, h]. Only used if `export` is not None. Defaults to
             (2048, 2048)
         :param path: Filepath to save snapshot; filepath should end with a jpg/jpeg/png/bmp extension
         :param save_to_local_history: :class:`bool`; whether to save VipPlot object to `this.local_history` list.
             Default value is True.
-        :param apply: :class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
+        :param apply: [Deprecated]:class:`bool` determining whether to apply the anomaly detection result to the halo dimension.
             Default is True.
         :param keep_missing_value_columns: :class:`bool` for whether to keep features with more than 50% missing
             values as part of the input for pca based anomaly detection. Default is `True`.
         :return: :class:`None`
         """
         if not isinstance(threshold, int) and not isinstance(threshold, float):
             raise exceptions.InvalidInputTypeException("Threshold must be a number (int or float) between 0 and 100.")
@@ -2615,24 +2785,32 @@
         if features is not None:
             params["Features"] = utils.get_features(features)
         if exclude is not None:
             params["Exclude"] = utils.get_features(exclude)
 
         params["KeepMissingValueColumns"] = keep_missing_value_columns
 
-        if isinstance(apply, bool):
-            if apply:
-                params["Apply"] = apply
-                params = [params]
-                params = self._add_export_to_params(export, background, imsize, path, params)
-                params = self._add_plot_mapping_to_params(params, save_to_local_history)
-            else:
-                params = [params]
-        else:
-            utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+        # if isinstance(apply, bool):
+        #     if apply:
+        #         params["Apply"] = apply
+        #         params = [params]
+        #         params = self._add_export_to_params(export, background, imsize, path, params)
+        #         params = self._add_plot_mapping_to_params(params, save_to_local_history)
+        #     else:
+        #         params = [params]
+        # else:
+        #     utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+
+        params = [params]
+        
+        if export is not None and export is not False:
+            params = self._add_export_to_params(export, background, imsize, path, params)
+        
+        params = self._add_plot_mapping_to_params(params, save_to_local_history)
+
         return self._api_request(params=params, data=None)
 
     def pca(self, num_components, features=None, exclude=None, apply=True, return_components_df=True, export="ortho", background="white",
             imsize=(2048, 2048), path=None, save_to_local_history=True,
             keep_missing_value_columns=True):
         """
         Runs Principal Component Analysis (PCA) in VIP
@@ -2648,15 +2826,15 @@
         :param background: Specify whether to export a plot capture with a white background, or the default color
             scheme configured in VIP. Options are {"white", "default"}. White is used if the value is not specified.
         :param imsize: size of the returned dimension; [w, h]. Only used if `export` is not None. Defaults to
             (2048, 2048)
         :param path: Filepath to save snapshot; filepath should end with a jpg/jpeg/png/bmp extension
         :param save_to_local_history: :class:`bool`; whether to save VipPlot object to `this.local_history` list.
             Default value is True.
-        :param apply: :class:`bool` determining whether to apply the first 3 computed components to the spatial
+        :param apply: [Deprecated]:class:`bool` determining whether to apply the first 3 computed components to the spatial
             dimensions. Default is True.
         :param keep_missing_value_columns: :class:`bool` for whether to keep features with more than 50% missing
             values as part of the input for pca. Default is `True`.
         :return: if return_data is True, this returns a :class:`pandas.DataFrame` containing the user specified number
             of principal components. Otherwise, this returns None.
         """
         # Check num_components is a positive integer and that user inputs are formatted correctly
@@ -2680,24 +2858,32 @@
         if exclude is not None:
             params["Exclude"] = utils.get_features(exclude)
         if num_components is not None:
             params["NumComponents"] = num_components
 
         params["KeepMissingValueColumns"] = keep_missing_value_columns
 
-        if isinstance(apply, bool):
-            if apply:
-                params["Apply"] = apply
-                params = [params]
-                params = self._add_export_to_params(export, background, imsize, path, params)
-                params = self._add_plot_mapping_to_params(params, save_to_local_history)
-            else:
-                params = [params]
-        else:
-            utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+        # if isinstance(apply, bool):
+        #     if apply:
+        #         params["Apply"] = apply
+        #         params = [params]
+        #         params = self._add_export_to_params(export, background, imsize, path, params)
+        #         params = self._add_plot_mapping_to_params(params, save_to_local_history)
+        #     else:
+        #         params = [params]
+        # else:
+        #     utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+
+        params = [params]
+
+        if export is not None and export is not False:
+            params = self._add_export_to_params(export, background, imsize, path, params)
+        
+        params = self._add_plot_mapping_to_params(params, save_to_local_history)
+
         return self._api_request(params=params, data=None)
 
     def clustering(self, num_clusters=None, features=None, exclude=None, keep_missing_value_columns=True, apply=True,
                    return_clusters_df=True, export="ortho", background="white", imsize=(2048, 2048), path=None, save_to_local_history=True):
         """
         Runs K-means clustering in VIP
 
@@ -2713,15 +2899,15 @@
         :param background: Specify whether to export a plot capture with a white background, or the default color
             scheme configured in VIP. Options are {"white", "default"}. White is used if the value is not specified.
         :param imsize: size of the returned dimension; [w, h]. Only used if `export` is not None. Defaults to
             (2048, 2048)
         :param path: Filepath to save snapshot; filepath should end with a jpg/jpeg/png/bmp extension
         :param save_to_local_history: :class:`bool`; whether to save VipPlot object to `this.local_history` list.
             Default value is True.
-        :param apply: :class:`bool` determining whether to apply the clustering result to the color dimension.
+        :param apply: [Deprecated]:class:`bool` determining whether to apply the clustering result to the color dimension.
             Default is True.
         :param keep_missing_value_columns: :class:`bool` for whether to keep features with more than 50% missing
             values as part of the input for clustering. Default is `True`.
         :return: :class:`pandas.DataFrame` containing the results of the clustering. If return_data is false, this
             returns None.
         """
         # Check num_clusters is a positive integer and that user inputs are formatted correctly
@@ -2741,24 +2927,32 @@
         if features is not None:
             params["Features"] = utils.get_features(features)
         if exclude is not None:
             params["Exclude"] = utils.get_features(exclude)
 
         params["KeepMissingValueColumns"] = keep_missing_value_columns
 
-        if isinstance(apply, bool):
-            if apply:
-                params["Apply"] = apply
-                params = [params]
-                params = self._add_export_to_params(export, background, imsize, path, params)
-                params = self._add_plot_mapping_to_params(params, save_to_local_history)
-            else:
-                params = [params]
-        else:
-            utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+        # if isinstance(apply, bool):
+        #     if apply:
+        #         params["Apply"] = apply
+        #         params = [params]
+        #         params = self._add_export_to_params(export, background, imsize, path, params)
+        #         params = self._add_plot_mapping_to_params(params, save_to_local_history)
+        #     else:
+        #         params = [params]
+        # else:
+        #     utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
+
+        params = [params]
+
+        if export is not None and export is not False:
+            params = self._add_export_to_params(export, background, imsize, path, params)
+        
+        params = self._add_plot_mapping_to_params(params, save_to_local_history)
+
         return self._api_request(params=params, data=None)
 
     def network_extractor(self, node_column, associative_columns, pivot_type="mean", export="ortho", background="white",
                           imsize=(2048, 2048), path=None, save_to_local_history=True, bypass_warning=False):
         """
         Network extractor is a beta functionality (please submit feedback to "support@virtualitics.com"). With this
         method, you can extract network structures from non-network data. You must specify a column containing
@@ -2993,14 +3187,38 @@
                 params = self._add_plot_mapping_to_params(params, save_to_local_history)
             else:
                 params = [params]
         else:
             utils.raise_invalid_argument_exception(str(type(apply)), "apply", "must be a 'bool'")
         return self._api_request(params=params, data=None)
 
+    def explainable_ai(self, function, targetColumn, associativeColumns):
+        """
+        Configures and runs the Explainable AI tool in VIP.
+
+        :param function: The type of explainability function to run. Can be "IdentificationTree", "CategoryBreakdown", "RelativeEdgeDensity".
+        :param targetColumn: :class:`pandas.Series` containing values which will be treated as the target categories for explainability.
+        :param associativeColumns: [:class:`pandas.Series`] containing list of columns that will be used to as input alongside the target column.
+
+        :return: :class:`None`
+        """
+        targetColumn = utils.get_name(targetColumn)
+        associativeColumns = utils.get_features(associativeColumns)
+        netx_function = utils.case_insensitive_match(utils.EXPLAINABLE_AI_FUNCTION, function, "function")
+        if len(associativeColumns) < 1:
+            raise exceptions.InvalidUsageException("`associativeColumns` must be a list of column names. Please "
+                                                   "see documentation. ")
+
+        params = {"TaskType": "ExplainableAI"}
+        params["Target Feature"] = targetColumn
+        params["Associative Features"] = associativeColumns
+        params["ExplainableAIFunction"] = function
+        params = [params]
+        return self._api_request(params=params, data=None)
+    
     def normalize(self, norm_type="Softmax", export="ortho", background="white", imsize=(2048, 2048), path=None,
                   save_to_local_history=True):
         """
         Normalizes the axis for spatial dimensions in VIP if applicable.
 
         :param norm_type: The type of normalization to apply to the data. Can be "softmax", "log10", or "ihst"
         :param export: Specify whether to export a capture of the plot. Can be None/False or "ortho", "front",
```

### Comparing `pyVIP-1.8.0/virtualitics/encryption.py` & `pyVIP-1.9.0/virtualitics/encryption.py`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/virtualitics/exceptions.py` & `pyVIP-1.9.0/virtualitics/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/virtualitics/pkcs7.py` & `pyVIP-1.9.0/virtualitics/pkcs7.py`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/virtualitics/task_response_handlers.py` & `pyVIP-1.9.0/virtualitics/task_response_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,14 +159,16 @@
         return _create_dashboard_tile_callback(task_response, payload)
     elif task_type == "RemoveDashboardTiles":
         return _remove_dashboard_tiles_callback(task_response, payload)
     elif task_type == "CreateAnnotation":
         return _create_annotation_callback(task_response, payload)
     elif task_type == "GetAnnotations":
         return _get_annotations_callback(task_response, payload)
+    elif task_type == "ExplainableAI": 
+        return _explainable_ai_callback(task_response, payload)
 
     notes_message = ""
     if "Note" in task_response:
         note = task_response["Note"].replace('\n', '').replace('<b>', '').replace('</b>', '').strip()
         notes_message += "Note: '%s'" % note
 
     print(notes_message)
@@ -333,14 +335,19 @@
         except:
             pass
     if "ColorType" in plotSettings.keys() and plotSettings["ColorType"] is not None:
         try:
             plot.color_type = plotSettings["ColorType"]
         except:
             pass
+    if "ColorPaletteID" in plotSettings.keys() and plotSettings["ColorPaletteID"] is not None:
+        try:
+            plot.color_palette_id = plotSettings["ColorPaletteID"]
+        except:
+            pass
     if "ColorBins" in plotSettings.keys() and plotSettings["ColorBins"] is not None:
         try:
             plot.color_bins = int(plotSettings["ColorBins"])
         except:
             pass
     if "ColorBinDist" in plotSettings.keys() and plotSettings["ColorBinDist"] is not None:
         try:
@@ -478,14 +485,89 @@
         except:
             pass
     if "ScatterPlotPointMode" in plotSettings.keys() and plotSettings["ScatterPlotPointMode"] is not None:
         try:
             plot.scatter_plot_point_mode = plotSettings["ScatterPlotPointMode"]
         except:
             pass
+    if "XRangeMin" in plotSettings.keys() and plotSettings["XRangeMin"] is not None:
+        try:
+            plot.x_range_min = float(plotSettings["XRangeMin"])
+        except:
+            pass
+    if "XRangeMax" in plotSettings.keys() and plotSettings["XRangeMax"] is not None:
+        try:
+            plot.x_range_max = float(plotSettings["XRangeMax"])
+        except:
+            pass
+    if "XLimitMin" in plotSettings.keys() and plotSettings["XLimitMin"] is not None:
+        try:
+            plot.x_limit_min = float(plotSettings["XLimitMin"])
+        except:
+            pass
+    if "XLimitMax" in plotSettings.keys() and plotSettings["XLimitMax"] is not None:
+        try:
+            plot.x_limit_max = float(plotSettings["XLimitMax"])
+        except:
+            pass
+    if "XLimitLink" in plotSettings.keys() and plotSettings["XLimitLink"] is not None:
+        try:
+            plot.x_limit_link = bool(plotSettings["XLimitLink"].lower() == "true")
+        except:
+            pass
+    if "YRangeMin" in plotSettings.keys() and plotSettings["YRangeMin"] is not None:
+        try:
+            plot.y_range_min = float(plotSettings["YRangeMin"])
+        except:
+            pass
+    if "YRangeMax" in plotSettings.keys() and plotSettings["YRangeMax"] is not None:
+        try:
+            plot.y_range_max = float(plotSettings["YRangeMax"])
+        except:
+            pass
+    if "YLimitMin" in plotSettings.keys() and plotSettings["YLimitMin"] is not None:
+        try:
+            plot.y_limit_min = float(plotSettings["YLimitMin"])
+        except:
+            pass
+    if "YLimitMax" in plotSettings.keys() and plotSettings["YLimitMax"] is not None:
+        try:
+            plot.y_limit_max = float(plotSettings["YLimitMax"])
+        except:
+            pass
+    if "YLimitLink" in plotSettings.keys() and plotSettings["YLimitLink"] is not None:
+        try:
+            plot.y_limit_link = bool(plotSettings["YLimitLink"].lower() == "true")
+        except:
+            pass
+    if "ZRangeMin" in plotSettings.keys() and plotSettings["ZRangeMin"] is not None:
+        try:
+            plot.z_range_min = float(plotSettings["ZRangeMin"])
+        except:
+            pass
+    if "ZRangeMax" in plotSettings.keys() and plotSettings["ZRangeMax"] is not None:
+        try:
+            plot.z_range_max = float(plotSettings["ZRangeMax"])
+        except:
+            pass
+    if "ZLimitMin" in plotSettings.keys() and plotSettings["ZLimitMin"] is not None:
+        try:
+            plot.z_limit_min = float(plotSettings["ZLimitMin"])
+        except:
+            pass
+    if "ZLimitMax" in plotSettings.keys() and plotSettings["ZLimitMax"] is not None:
+        try:
+            plot.z_limit_max = float(plotSettings["ZLimitMax"])
+        except:
+            pass
+    if "ZLimitLink" in plotSettings.keys() and plotSettings["ZLimitLink"] is not None:
+        try:
+            plot.z_limit_link = bool(plotSettings["ZLimitLink"].lower() == "true")
+        except:
+            pass
 
     notes_message = ""
     if "Note" in task_response:
         note = task_response["Note"].replace('\n', '').replace('<b>', '').replace('</b>', '').strip()
         notes_message += "Note: '%s'" % note
 
     print(notes_message)
@@ -701,14 +783,28 @@
 
     notes_message = ""
     if "Note" in task_response:
         note = task_response["Note"].replace('\n', '').replace('<b>', '').replace('</b>', '').strip()
         notes_message += "Note: '%s'" % note
 
     print(notes_message)
+
+def _explainable_ai_callback(task_response, payload):
+    table = []
+    if "ExplainableAIReport" in task_response:
+        for insight in task_response["ExplainableAIReport"]:
+            table.append([insight["Category"], insight["Description"]])
+        display(HTML(tabulate.tabulate(table, headers=["Category", "Description"], tablefmt='html')))
+
+    notes_message = ""
+    if "Note" in task_response:
+        note = task_response["Note"].replace('\n', '').replace('<b>', '').replace('</b>', '').strip()
+        notes_message += "Note: '%s'" % note
+
+    print(notes_message)
 
 def _dataset_callback(task_response, payload):
     if "DataSetName" in task_response:
         print("Data set loaded with name: '%s'" % task_response["DataSetName"])
         return task_response["DataSetName"]
 
     return None
```

### Comparing `pyVIP-1.8.0/virtualitics/utils.py` & `pyVIP-1.9.0/virtualitics/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,17 @@
 CAMERA_ANGLE = {"default": "DEFAULT", "top": "TOP", "front": "FRONT", "side": "SIDE", "right": "SIDE"}
 CULTURE_FORMATS = {"us": "US", "eu": "EUROPE", "europe": "EUROPE"}
 PIVOT_TYPES = {"min": "Min", "max": "Max", "mean": "Mean", "median": "Median",
     "sum": "Sum", "std": "Std", "all": "All"}
 HEATMAP_RADIUS_UNITS = {"kilometers": "Kilometers", "km": "Kilometers", "miles": "Miles", "mi": "Miles",
                         "nauticalmiles": "NauticalMiles", "nm": "NauticalMiles"}
 STR_COL_DELIMETER = '\x01'
+EXPLAINABLE_AI_FUNCTION = {"identificationtree": "IdentificationTree", "id_tree" : "IdentificationTree", 
+                            "categorybreakdown": "CategoryBreakdown", "categories": "CategoryBreakdown", 
+                            "relativeedgedensity": "RelativeEdgeDensity", "edges" : "RelativeEdgeDensity"}
 
 def case_insensitive_match(d: dict, val, var_name: str):
     """
     Get case-insensitive match from d to val if it exists. Raises exception if no match found.
 
     :param d: dictionary including keys to match against
     :param val: value to match against
@@ -124,18 +127,25 @@
 
 def str_escape(s):
     """
     Escapes the input string. If input is NaN, empty string is returned.
     :param s: input string
     :returns escaped_string: escaped string bytes
     """
-    if pd.isna(s) or (s is None):
-        return b""
-    else:
-        return str(s).encode('unicode_escape')
+    tmpVal = s
+    if not pd.api.types.is_scalar(tmpVal):
+        tmpVal = "[" + ', '.join(tmpVal) + "]"
+
+    try:
+        if pd.isna(tmpVal) or (tmpVal is None):
+            return b""
+        else:
+            return str(tmpVal).encode('unicode_escape')
+    except:
+        raise exceptions.InvalidInputTypeException("Failed to escape value: " + str(s) + " of type "+ str(type(s)))
 
 
 def str_unescape(s):
     if s == b"":
         return ""
     else:
         return s.decode('unicode_escape')
```

### Comparing `pyVIP-1.8.0/virtualitics/vip_annotation.py` & `pyVIP-1.9.0/virtualitics/vip_annotation.py`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/virtualitics/vip_dashboard.py` & `pyVIP-1.9.0/virtualitics/vip_dashboard.py`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/virtualitics/vip_object.py` & `pyVIP-1.9.0/virtualitics/vip_object.py`

 * *Files identical despite different names*

### Comparing `pyVIP-1.8.0/virtualitics/vip_plot.py` & `pyVIP-1.9.0/virtualitics/vip_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,20 @@
     """
     The plot class contains all essential details of a plot in VIP.
     """
 
     def __init__(self, data_set_name=None, plot_type="scatter", x=None, y=None, z=None, color=None, size=None,
                  shape=None, transparency=None, halo=None, halo_highlight=None, pulsation=None,
                  pulsation_highlight=None, playback=None, playback_highlight=None, arrow=None, groupby=None,
-                 x_scale=None, y_scale=None, z_scale=None, size_scale=None, transparency_scale=None, halo_scale=None,
-                 arrow_scale=None, color_type=None, color_normalization=None, x_normalization=None,
+                 x_scale=None, y_scale=None, z_scale=None, 
+                 x_range_min=None, x_range_max=None, x_limit_min=None, x_limit_max=None, x_limit_link=None,
+                 y_range_min=None, y_range_max=None, y_limit_min=None, y_limit_max=None, y_limit_link=None,
+                 z_range_min=None, z_range_max=None, z_limit_min=None, z_limit_max=None, z_limit_link=None,
+                 size_scale=None, transparency_scale=None, halo_scale=None,
+                 arrow_scale=None, color_type=None, color_palette_id=None, color_normalization=None, x_normalization=None,
                  y_normalization=None, z_normalization=None, size_normalization=None, transparency_normalization=None,
                  arrow_normalization=None, show_points=None, confidence=None, map_mode=None, globe_style=None,
                  lat_long_lines=None, country_lines=None, country_labels=None, heatmap_enabled=None,
                  heatmap_intensity=None, heatmap_radius=None, heatmap_radius_unit=None, map_provider=None,
                  map_style=None, color_bins=None, color_bin_dist=None, hist_volume_by=None, viewby=None, x_bins=None,
                  y_bins=None, z_bins=None, color_inverted=None, log_level=0, name=None, trend_lines=None,
                  scatter_plot_point_mode=None, line_plot_point_mode=None, _dataset_type=None):
@@ -41,20 +45,36 @@
             All points with this value will pulsate.
         :param playback: Playback dimension. Requires user interaction to be activated; otherwise shows all.
         :param playback_highlight: Optionally select a single value of the feature mapped to the Playback dimension.
             All points with this value will be shown and all other points will be hidden.
         :param x_scale: Scaling factor for X dimension. Value must be between .5 and 5.
         :param y_scale: Scaling factor for Y dimension. Value must be between .5 and 5.
         :param z_scale: Scaling factor for Z dimension. Value must be between .5 and 5.
+        :param x_range_min: Minimum visible value for the X dimension.
+        :param x_range_max: Maximum visible value for the X dimension.
+        :param x_limit_min: Minimum value displayed for the X dimension on the axis/grid box.
+        :param x_limit_max: Maximum value displayed for the X dimension on the axis/grid box.
+        :param x_limit_link: Whether X Limits are locked to the Range.
+        :param y_range_min: Minimum visible value for the Y dimension.
+        :param y_range_max: Maximum visible value for the Y dimension.
+        :param y_limit_min: Minimum value displayed for the Y dimension on the axis/grid box.
+        :param y_limit_max: Maximum value displayed for the Y dimension on the axis/grid box.
+        :param y_limit_link: Whether Y Limits are locked to the Range.
+        :param z_range_min: Minimum visible value for the Z dimension.
+        :param z_range_max: Maximum visible value for the Z dimension.
+        :param z_limit_min: Minimum value displayed for the Z dimension on the axis/grid box.
+        :param z_limit_max: Maximum value displayed for the Z dimension on the axis/grid box.
+        :param z_limit_link: Whether Z Limits are locked to the Range.
         :param size_scale: Scaling factor for Size dimension. Value must be between .5 and 5.
         :param transparency_scale: Scaling factor for Transparency dimension. Value must be between .5 and 5.
         :param halo_scale: Scaling factor for Halo dimension. Value must be between .5 and 5.
         :param color_type: User can select "gradient", "bin", or "palette" or None (which uses VIP defaults). For
             categorical data, the only option is color "palette". For numeric data, "bin" is the default but "gradient"
             can also be used.
+        :param color_palette_id: User can select the index ofo the desired color set (color palette/color gradient sets) to configure the colors used in the plot.
         :param color_normalization: Normalization setting for color. This can only be set if the color type is set to
             "Gradient". The options are "Log10", "Softmax", "IHST"
         :param x_normalization: Normalization setting for X. This can only be set if the column mapped to the X
             dimension is numeric. The options are "Log10", "Softmax", "IHST"
         :param y_normalization: Normalization setting for Y. This can only be set if the column mapped to the Y
             dimension is numeric. The options are "Log10", "Softmax", "IHST"
         :param z_normalization: Normalization setting for Z. This can only be set if the column mapped to the Z
@@ -146,19 +166,38 @@
         self.y_scale = y_scale
         self.z_scale = z_scale
         self.size_scale = size_scale
         self.transparency_scale = transparency_scale
         self.halo_scale = halo_scale
         self.arrow_scale = arrow_scale
 
+        # Range and Limits
+        self.x_range_min = x_range_min
+        self.x_range_max = x_range_max
+        self.x_limit_min = x_limit_min
+        self.x_limit_max = x_limit_max
+        self.x_limit_link = x_limit_link
+        self.y_range_min = y_range_min
+        self.y_range_max = y_range_max
+        self.y_limit_min = y_limit_min
+        self.y_limit_max = y_limit_max
+        self.y_limit_link = y_limit_link
+        self.z_range_min = z_range_min
+        self.z_range_max = z_range_max
+        self.z_limit_min = z_limit_min
+        self.z_limit_max = z_limit_max
+        self.z_limit_link = z_limit_link
+
+
         # Color Type
         self.color_type = color_type
         self.color_bins = color_bins
         self.color_bin_dist = color_bin_dist
         self.color_inverted = color_inverted
+        self.color_palette_id = color_palette_id
 
         # Normalization
         self.x_normalization = x_normalization
         self.y_normalization = y_normalization
         self.z_normalization = z_normalization
         self.color_normalization = color_normalization
         self.size_normalization = size_normalization
@@ -243,14 +282,44 @@
         buf += "# Plot Settings: \n"
         if self.x_scale is not None:
             buf += "X Scale:\t\t{}\n".format(str(self.x_scale))
         if self.y_scale is not None:
             buf += "Y Scale:\t\t{}\n".format(str(self.y_scale))
         if self.z_scale is not None:
             buf += "Z Scale:\t\t{}\n".format(str(self.z_scale))
+        if self.x_range_min is not None:
+            buf += "X Range Min:\t\t{}\n".format(str(self.x_range_min))
+        if self.y_range_min is not None:
+            buf += "Y Range Min:\t\t{}\n".format(str(self.y_range_min))
+        if self.z_range_min is not None:
+            buf += "Z Range Min:\t\t{}\n".format(str(self.z_range_min))
+        if self.x_range_max is not None:
+            buf += "X Range Max:\t\t{}\n".format(str(self.x_range_max))
+        if self.y_range_max is not None:
+            buf += "Y Range Max:\t\t{}\n".format(str(self.y_range_max))
+        if self.z_range_max is not None:
+            buf += "Z Range Max:\t\t{}\n".format(str(self.z_range_max))
+        if self.x_limit_min is not None:
+            buf += "X Limit Min:\t\t{}\n".format(str(self.x_limit_min))
+        if self.y_limit_min is not None:
+            buf += "Y Limit Min:\t\t{}\n".format(str(self.y_limit_min))
+        if self.z_limit_min is not None:
+            buf += "Z Limit Min:\t\t{}\n".format(str(self.z_limit_min))
+        if self.x_limit_max is not None:
+            buf += "X Limit Max:\t\t{}\n".format(str(self.x_limit_max))
+        if self.y_limit_max is not None:
+            buf += "Y Limit Max:\t\t{}\n".format(str(self.y_limit_max))
+        if self.z_limit_max is not None:
+            buf += "Z Limit Max:\t\t{}\n".format(str(self.z_limit_max))
+        if self.x_limit_link is not None:
+            buf += "X Limit Link:\t\t{}\n".format(str(self.x_limit_link))
+        if self.y_limit_link is not None:
+            buf += "Y Limit Link:\t\t{}\n".format(str(self.y_limit_link))
+        if self.z_limit_link is not None:
+            buf += "Z Limit Link:\t\t{}\n".format(str(self.z_limit_link))
         if self.size_scale is not None:
             buf += "Size Scale:\t\t{}\n".format(str(self.size_scale))
         if self.transparency_scale is not None:
             buf += "Transparency Scale:\t{}\n".format(str(self.transparency_scale))
         if self.halo_scale is not None:
             buf += "Halo Scale:\t\t{}\n".format(str(self.halo_scale))
         if self.arrow_scale is not None:
@@ -259,14 +328,16 @@
             buf += "ColorType:\t\t{}\n".format(str(self.color_type))
         if self.color_bins is not None:
             buf += "Color Bin Count:\t{}\n".format(str(self.color_bins))
         if self.color_bin_dist is not None:
             buf += "Color Bin Dist:\t{}\n".format(str(self.color_bin_dist))
         if self.color_inverted is not None:
             buf += "Color Inverted:\t{}\n".format(str(self.color_inverted))
+        if self.color_palette_id is not None:
+            buf += "Color Palette Id:\t{}\n".format(str(self.color_palette_id))
         if self.x_normalization is not None:
             buf += "X Normalization:\t\t{}\n".format(str(self.x_normalization))
         if self.y_normalization is not None:
             buf += "Y Normalization:\t\t{}\n".format(str(self.y_normalization))
         if self.z_normalization is not None:
             buf += "Z Normalization:\t\t{}\n".format(str(self.z_normalization))
         if self.color_normalization is not None:
@@ -405,28 +476,60 @@
         settings = {}
         if self.x_scale is not None:
             settings["XScale"] = self.x_scale
         if self.y_scale is not None:
             settings["YScale"] = self.y_scale
         if self.z_scale is not None:
             settings["ZScale"] = self.z_scale
+        if self.x_range_min is not None:
+            settings["XRangeMin"] = self.x_range_min
+        if self.x_range_max is not None:
+            settings["XRangeMax"] = self.x_range_max
+        if self.x_limit_min is not None:
+            settings["XLimitMin"] = self.x_limit_min
+        if self.x_limit_max is not None:
+            settings["XLimitMax"] = self.x_limit_max
+        if self.x_limit_link is not None:
+            settings["XLimitLink"] = self.x_limit_link
+        if self.y_range_min is not None:
+            settings["YRangeMin"] = self.y_range_min
+        if self.y_range_max is not None:
+            settings["YRangeMax"] = self.y_range_max
+        if self.y_limit_min is not None:
+            settings["YLimitMin"] = self.y_limit_min
+        if self.y_limit_max is not None:
+            settings["YLimitMax"] = self.y_limit_max
+        if self.y_limit_link is not None:
+            settings["YLimitLink"] = self.y_limit_link
+        if self.z_range_min is not None:
+            settings["ZRangeMin"] = self.z_range_min
+        if self.z_range_max is not None:
+            settings["ZRangeMax"] = self.z_range_max
+        if self.z_limit_min is not None:
+            settings["ZLimitMin"] = self.z_limit_min
+        if self.z_limit_max is not None:
+            settings["ZLimitMax"] = self.z_limit_max
+        if self.z_limit_link is not None:
+            settings["ZLimitLink"] = self.z_limit_link
         if self.size_scale is not None:
             settings["SizeScale"] = self.size_scale
         if self.transparency_scale is not None:
             settings["TransparencyScale"] = self.transparency_scale
         if self.halo_scale is not None:
             settings["HaloScale"] = self.halo_scale
         if self.arrow_scale is not None:
             settings["ArrowScale"] = self.arrow_scale
         if self.color_type is not None:
             settings["ColorType"] = self.color_type
         if self.color_normalization is not None:
             settings["ColorNormalization"] = self.color_normalization
         if self.color_inverted is not None:
             settings["ColorInverted"] = self.color_inverted
+        if self.color_palette_id is not None:
+            settings["ColorPaletteID"] = self.color_palette_id
         if self.x_normalization is not None:
             settings["XNormalization"] = self.x_normalization
         if self.y_normalization is not None:
             settings["YNormalization"] = self.y_normalization
         if self.z_normalization is not None:
             settings["ZNormalization"] = self.z_normalization
         if self.size_normalization is not None:
@@ -1659,14 +1762,646 @@
         if self.log_level >= api.LOG_HELP_LEVEL:
             print("Attribute 'arrow_scale' is set to 'None': 'None' value implies the default scale value will "
                   "be used. ")
         self.arrow_scale = None
 
     # endregion Scaling
 
+    # region Range and Limits
+    @property
+    def x_range_min(self):
+        """
+        X Range Min setting. Must be set to :class:`float` with value between Min and Max of the column mapped to the X Dimension.
+        Default value 'None' leaves VIP to default range min value. X range min is only applicable when the X dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._x_range_min
+
+    @x_range_min.setter
+    def x_range_min(self, val):
+        """
+        X range min setting. Must be set to :class:`float` with value between Min and Max of the feature mapped on the X Dimesion. 
+        Default value 'None' leaves VIP to default range min value. X range min is only applicable when the X dimension is being used.
+
+        :param val: :class:`float` between x min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._x_range_min = None
+            return
+
+        if self.x is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "x_range_min",
+                                                   "'x_range_min' is only applicable if 'x' has been mapped.")
+        self._x_range_min = val
+
+    @x_range_min.deleter
+    def x_range_min(self):
+        """
+        Sets the X range min setting to 'None'; VIP will proceed to use the default X range min as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'x_range_min' is set to 'None': 'None' value implies the default range min value will be used.")
+        self.x_range_min = None
+
+    @property
+    def x_range_max(self):
+        """
+        X Range Max setting. Must be set to :class:`float` with value between Min and Max of the column mapped to the X Dimension.
+        Default value 'None' leaves VIP to default range max value. X range max is only applicable when the X dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._x_range_max
+
+    @x_range_max.setter
+    def x_range_max(self, val):
+        """
+        X range max setting. Must be set to :class:`float` with value between Min and Max of the feature mapped on the X Dimesion. 
+        Default value 'None' leaves VIP to default range max value. X range max is only applicable when the X dimension is being used.
+
+        :param val: :class:`float` between x min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._x_range_max = None
+            return
+
+        if self.x is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "x_range_max",
+                                                   "'x_range_max' is only applicable if 'x' has been mapped.")
+        self._x_range_max = val
+
+    @x_range_max.deleter
+    def x_range_max(self):
+        """
+        Sets the X range max setting to 'None'; VIP will proceed to use the default X range max as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'x_range_max' is set to 'None': 'None' value implies the default range max value will be used.")
+        self.x_range_max = None
+
+    @property
+    def x_limit_min(self):
+        """
+        X Limit Min setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit min value. X limit min is only applicable when the X dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._x_limit_min
+
+    @x_limit_min.setter
+    def x_limit_min(self, val):
+        """
+        X limit min setting. Must be set to :class:`float`. 
+        Default value 'None' leaves VIP to default limit min value. X limit min is only applicable when the X dimension is being used.
+
+        :param val: :class:`float`
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._x_limit_min = None
+            return
+
+        if self.x is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "x_limit_min",
+                                                   "'x_limit_min' is only applicable if 'x' has been mapped.")
+        if self.is_geospatial_plot():
+            utils.raise_invalid_argument_exception(str(type(val)), "x_limit_min",
+                                                   "'x_limit_min' is not applicable for geospatial plots. ")
+
+        self._x_limit_min = val
+
+    @x_limit_min.deleter
+    def x_limit_min(self):
+        """
+        Sets the X limit min setting to 'None'; VIP will proceed to use the default X limit min as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'x_limit_min' is set to 'None': 'None' value implies the default limit min value will be used.")
+        self.x_limit_min = None
+
+    @property
+    def x_limit_max(self):
+        """
+        X limit Max setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit max value. X limit max is only applicable when the X dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._x_limit_max
+
+    @x_limit_max.setter
+    def x_limit_max(self, val):
+        """
+        X limit max setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit max value. X limit max is only applicable when the X dimension is being used.
+
+        :param val: :class:`float` between x min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._x_limit_max = None
+            return
+
+        if self.x is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "x_limit_max",
+                                                   "'x_limit_max' is only applicable if 'x' has been mapped.")
+        if self.is_geospatial_plot():
+            utils.raise_invalid_argument_exception(str(type(val)), "x_limit_max",
+                                                   "'x_limit_max' is not applicable for geospatial plots. ")
+
+        self._x_limit_max = val
+
+    @x_limit_max.deleter
+    def x_limit_max(self):
+        """
+        Sets the X limit max setting to 'None'; VIP will proceed to use the default X limit max as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'x_max' is set to 'None': 'None' value implies the default limit max value will be used.")
+        self.x_limit_max = None
+
+    @property
+    def x_limit_link(self):
+        """
+        X limit Link setting. Must be set to :class:`bool`.
+        Default value 'None' leaves VIP to default limit link value. X limit link is only applicable when the X dimension is being used.
+
+        :return: :class:`bool`
+        """
+        return self._x_limit_link
+
+    @x_limit_link.setter
+    def x_limit_link(self, val):
+        """
+        X limit link setting. Must be set to :class:`bool`.
+        Default value 'None' leaves VIP to default limit link value. X limit link is only applicable when the X dimension is being used.
+
+        :param val: :class:`bool`
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._x_limit_link = None
+            return
+
+        if val is not None and not isinstance(val, bool):
+            utils.raise_invalid_argument_exception(str(type(val)), "x_limit_link",
+                                                    "'x_limit_link' should be a `bool` or None.")
+
+        if self.x is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "x_limit_link",
+                                                   "'x_limit_link' is only applicable if 'x' has been mapped.")
+        if self.is_geospatial_plot():
+            utils.raise_invalid_argument_exception(str(type(val)), "x_limit_link",
+                                                   "'x_limit_link' is not applicable for geospatial plots. ")
+
+        self._x_limit_link = val
+
+    @x_limit_link.deleter
+    def x_limit_link(self):
+        """
+        Sets the X limit link setting to 'None'; VIP will proceed to use the default X limit link as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'x_limit_link' is set to 'None': 'None' value implies the default limit link value will be used.")
+        self.x_limit_link = None
+
+    @property
+    def y_range_min(self):
+        """
+        Y Range Min setting. Must be set to :class:`float` with value between Min and Max of the column mapped to the Y Dimension.
+        Default value 'None' leaves VIP to default range min value. Y range min is only applicable when the X dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._y_range_min
+
+    @y_range_min.setter
+    def y_range_min(self, val):
+        """
+        Y range min setting. Must be set to :class:`float` with value between Min and Max of the feature mapped on the Y Dimesion. 
+        Default value 'None' leaves VIP to default range min value. Y range min is only applicable when the Y dimension is being used.
+
+        :param val: :class:`float` between y min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._y_range_min = None
+            return
+
+        if self.y is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "y_range_min",
+                                                   "'y_range_min' is only applicable if 'y' has been mapped.")
+
+        self._y_range_min = val
+
+    @y_range_min.deleter
+    def y_range_min(self):
+        """
+        Sets the Y range min setting to 'None'; VIP will proceed to use the default Y range min as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'y_range_min' is set to 'None': 'None' value implies the default range min value will be used.")
+        self.y_range_min = None
+
+    @property
+    def y_range_max(self):
+        """
+        Y Range Max setting. Must be set to :class:`float` with value between Min and Max of the column mapped to the Y Dimension.
+        Default value 'None' leaves VIP to default range max value. Y range max is only applicable when the Y dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._y_range_max
+
+    @y_range_max.setter
+    def y_range_max(self, val):
+        """
+        Y range max setting. Must be set to :class:`float` with value between Min and Max of the feature mapped on the Y Dimesion. 
+        Default value 'None' leaves VIP to default range max value. Y range max is only applicable when the X dimension is being used.
+
+        :param val: :class:`float` between x min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._y_range_max = None
+            return
+
+        if self.y is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "y_range_max",
+                                                   "'y_range_max' is only applicable if 'y' has been mapped.")
+
+        self._y_range_max = val
+
+    @y_range_max.deleter
+    def y_range_max(self):
+        """
+        Sets the Y range max setting to 'None'; VIP will proceed to use the default Y range max as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'y_range_max' is set to 'None': 'None' value implies the default range max value will be used.")
+        self.y_range_max = None
+
+    @property
+    def y_limit_min(self):
+        """
+        Y Limit Min setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit min value. Y limit min is only applicable when the Y dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._y_limit_min
+
+    @y_limit_min.setter
+    def y_limit_min(self, val):
+        """
+        Y limit min setting. Must be set to :class:`float`. 
+        Default value 'None' leaves VIP to default limit min value. Y limit min is only applicable when the Y dimension is being used.
+
+        :param val: :class:`float`
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._y_limit_min = None
+            return
+
+        if self.y is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "y_limit_min",
+                                                   "'y_limit_min' is only applicable if 'y' has been mapped.")
+        if self.is_geospatial_plot():
+            utils.raise_invalid_argument_exception(str(type(val)), "y_limit_min",
+                                                   "'y_limit_min' is not applicable for geospatial plots. ")
+
+        self._y_limit_min = val
+
+    @y_limit_min.deleter
+    def y_limit_min(self):
+        """
+        Sets the Y limit min setting to 'None'; VIP will proceed to use the default Y limit min as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'y_limit_min' is set to 'None': 'None' value implies the default limit min value will be used.")
+        self.y_limit_min = None
+
+    @property
+    def y_limit_max(self):
+        """
+        Y limit Max setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit max value. Y limit max is only applicable when the Y dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._y_limit_max
+
+    @y_limit_max.setter
+    def y_limit_max(self, val):
+        """
+        Y limit max setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit max value. Y limit max is only applicable when the Y dimension is being used.
+
+        :param val: :class:`float`
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._y_limit_max = None
+            return
+
+        if self.y is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "y_limit_max",
+                                                   "'y_limit_max' is only applicable if 'y' has been mapped.")
+        if self.is_geospatial_plot():
+            utils.raise_invalid_argument_exception(str(type(val)), "y_limit_max",
+                                                   "'y_limit_max' is not applicable for geospatial plots. ")
+
+        self._y_limit_max = val
+
+    @y_limit_max.deleter
+    def y_limit_max(self):
+        """
+        Sets the Y limit max setting to 'None'; VIP will proceed to use the default Y limit max as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'y_max' is set to 'None': 'None' value implies the default limit max value will be used.")
+        self.y_limit_max = None
+
+    @property
+    def y_limit_link(self):
+        """
+        Y limit Link setting. Must be set to :class:`bool`.
+        Default value 'None' leaves VIP to default limit link value. Y limit link is only applicable when the Y dimension is being used.
+
+        :return: :class:`bool`
+        """
+        return self._y_limit_link
+
+    @y_limit_link.setter
+    def y_limit_link(self, val):
+        """
+        Y limit link setting. Must be set to :class:`bool`.
+        Default value 'None' leaves VIP to default limit link value. Y limit link is only applicable when the Y dimension is being used.
+
+        :param val: :class:`bool`
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._y_limit_link = None
+            return
+
+        if val is not None and not isinstance(val, bool):
+            utils.raise_invalid_argument_exception(str(type(val)), "y_limit_link",
+                                                    "'y_limit_link' should be a `bool` or None.")
+        if self.y is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "y_limit_link",
+                                                   "'y_limit_link' is only applicable if 'y' has been mapped.")
+        if self.is_geospatial_plot():
+            utils.raise_invalid_argument_exception(str(type(val)), "y_limit_link",
+                                                   "'y_limit_link' is not applicable for geospatial plots. ")
+
+        self._y_limit_link = val
+
+    @y_limit_link.deleter
+    def y_limit_link(self):
+        """
+        Sets the Y limit link setting to 'None'; VIP will proceed to use the default Y limit link as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'y_limit_link' is set to 'None': 'None' value implies the default limit link value will be used.")
+        self.y_limit_link = None
+
+    @property
+    def z_range_min(self):
+        """
+        Z Range Min setting. Must be set to :class:`float` with value between Min and Max of the column mapped to the Z Dimension.
+        Default value 'None' leaves VIP to default range min value. Z range min is only applicable when the Z dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._z_range_min
+
+    @z_range_min.setter
+    def z_range_min(self, val):
+        """
+        Z range min setting. Must be set to :class:`float` with value between Min and Max of the feature mapped on the Z Dimesion. 
+        Default value 'None' leaves VIP to default range min value. Z range min is only applicable when the Z dimension is being used.
+
+        :param val: :class:`float` between z min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._z_range_min = None
+            return
+
+        if self.z is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "z_range_min",
+                                                   "'z_range_min' is only applicable if 'z' has been mapped.")
+
+        self._z_range_min = val
+
+    @z_range_min.deleter
+    def z_range_min(self):
+        """
+        Sets the Z range min setting to 'None'; VIP will proceed to use the default Z range min as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'z_range_min' is set to 'None': 'None' value implies the default range min value will be used.")
+        self.z_range_min = None
+
+    @property
+    def z_range_max(self):
+        """
+        Z Range Max setting. Must be set to :class:`float` with value between Min and Max of the column mapped to the Z Dimension.
+        Default value 'None' leaves VIP to default range max value. Y range max is only applicable when the Z dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._z_range_max
+
+    @z_range_max.setter
+    def z_range_max(self, val):
+        """
+        Z range max setting. Must be set to :class:`float` with value between Min and Max of the feature mapped on the Z Dimesion. 
+        Default value 'None' leaves VIP to default range max value. Z range max is only applicable when the Z dimension is being used.
+
+        :param val: :class:`float` between z min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._z_range_max = None
+            return
+
+        if self.z is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "z_range_max",
+                                                   "'z_range_max' is only applicable if 'z' has been mapped.")
+
+        self._z_range_max = val
+
+    @z_range_max.deleter
+    def z_range_max(self):
+        """
+        Sets the Z range max setting to 'None'; VIP will proceed to use the default Z range max as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'z_range_max' is set to 'None': 'None' value implies the default range max value will be used.")
+        self.z_range_max = None
+
+    @property
+    def z_limit_min(self):
+        """
+        Z Limit Min setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit min value. Z limit min is only applicable when the Z dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._z_limit_min
+
+    @z_limit_min.setter
+    def z_limit_min(self, val):
+        """
+        Z limit min setting. Must be set to :class:`float`. 
+        Default value 'None' leaves VIP to default limit min value. Z limit min is only applicable when the Z dimension is being used.
+
+        :param val: :class:`float`
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._z_limit_min = None
+            return
+
+        if self.z is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "z_limit_min",
+                                                   "'z_limit_min' is only applicable if 'z' has been mapped.")
+
+        self._z_limit_min = val
+
+    @z_limit_min.deleter
+    def z_limit_min(self):
+        """
+        Sets the Z limit min setting to 'None'; VIP will proceed to use the default Z limit min as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'z_limit_min' is set to 'None': 'None' value implies the default limit min value will be used.")
+        self.z_limit_min = None
+
+    @property
+    def z_limit_max(self):
+        """
+        Z limit Max setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit max value. Z limit max is only applicable when the Z dimension is being used.
+
+        :return: :class:`float`
+        """
+        return self._z_limit_max
+
+    @z_limit_max.setter
+    def z_limit_max(self, val):
+        """
+        Z limit max setting. Must be set to :class:`float`.
+        Default value 'None' leaves VIP to default limit max value. Z limit max is only applicable when the Z dimension is being used.
+
+        :param val: :class:`float` between z min and max
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._z_limit_max = None
+            return
+
+        if self.z is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "z_limit_max",
+                                                   "'z_limit_max' is only applicable if 'z' has been mapped.")
+
+        self._z_limit_max = val
+
+    @z_limit_max.deleter
+    def z_limit_max(self):
+        """
+        Sets the Z limit max setting to 'None'; VIP will proceed to use the default Z limit max as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'z_limit_max' is set to 'None': 'None' value implies the default limit max value will be used.")
+        self.z_limit_max = None
+
+    @property
+    def z_limit_link(self):
+        """
+        Z limit Link setting. Must be set to :class:`bool`.
+        Default value 'None' leaves VIP to default limit link value. Z limit link is only applicable when the Z dimension is being used.
+
+        :return: :class:`bool`
+        """
+        return self._z_limit_link
+
+    @z_limit_link.setter
+    def z_limit_link(self, val):
+        """
+        Z limit link setting. Must be set to :class:`bool`.
+        Default value 'None' leaves VIP to default limit link value. Z limit link is only applicable when the Z dimension is being used.
+
+        :param val: :class:`bool`
+        :return: :class:`None`
+        """
+        if (val is None):
+            self._z_limit_link = None
+            return
+
+        if val is not None and not isinstance(val, bool):
+            utils.raise_invalid_argument_exception(str(type(val)), "z_limit_link",
+                                                    "'z_limit_link' should be a `bool` or None.")
+        if self.z is None:
+            utils.raise_invalid_argument_exception(str(type(val)), "z_limit_link",
+                                                   "'z_limit_link' is only applicable if 'z' has been mapped.")
+        if self.is_geospatial_plot():
+            utils.raise_invalid_argument_exception(str(type(val)), "z_limit_link",
+                                                   "'z_limit_link' is not applicable for geospatial plots. ")
+
+        self._z_limit_link = val
+
+    @z_limit_link.deleter
+    def z_limit_link(self):
+        """
+        Sets the Z limit link setting to 'None'; VIP will proceed to use the default Z limit link as a result.
+
+        :return: :class:`None`
+        """
+        if self.log_level >= api.LOG_HELP_LEVEL:
+            print("Attribute 'z_limit_link' is set to 'None': 'None' value implies the default limit link value will be used.")
+        self.z_limit_link = None
+
+    # endregion Ranges and Limits
+
     # region Color Settings
     @property
     def color_type(self):
         """
         Color type setting. Must be set to :class:`str` and match one of the following {"gradient", "bin", "palette",
         None}. Default value 'None' leaves VIP to default color type based, which is dependent on the feature mapped
         to color. Color type setting is only applicable when the 'color' dimension has been mapped.
@@ -1877,14 +2612,59 @@
         """
         Sets color inversion state to False. VipPlots will use the default color ordering.
 
         :return: :class:`None`
         """
         self._color_inverted = False
 
+    @property
+    def color_palette_id(self):
+        """
+        Color Palette ID. Must be a :class:`int`. Default of `None` leaves the color palette id
+        as is. Value of `0-n` selects the desired color palette, based on the color_type. Color Palette ID is only applicable
+        when a feature has been mapped to 'color'
+
+        :return: :class:`None`
+        """
+        return self._color_palette_id
+
+    @color_palette_id.setter
+    def color_palette_id(self, val):
+        """
+        Color Palette ID. Must be a :class:`int`. Default of `None` leaves the color palette id
+        as is. Value of `0-n` selects the desired color palette, based on the color_type. Color Palette ID is only applicable
+        when a feature has been mapped to 'color'
+
+        :return: :class:`None`
+        """
+        if val is None:
+            self._color_palette_id = None
+            return
+
+        if type(val) is not int:
+            utils.raise_invalid_argument_exception(str(type(val)), "color_palette_id",
+                                                   "'color_palette_id' must be an integer value: [0, 1, ..., n]")
+
+        if self.color is None:
+            if self._plot_type != "HISTOGRAM":
+                utils.raise_invalid_argument_exception(str(type(val)), "color_palette_id",
+                                                   "'color_palette_id' is only applicable when 'color' dimension has "
+                                                   "been mapped or when plotting a histogram. ")
+
+        self._color_palette_id = val
+
+    @color_palette_id.deleter
+    def color_palette_id(self):
+        """
+        Sets color palette id. If not specified, VipPlots will use the default or current color palette.
+
+        :return: :class:`None`
+        """
+        self._color_palette_id = False
+
     # endregion Color Settings
 
     # region Normalization
     @property
     def x_normalization(self):
         """
         X normalization setting. Must be set to :class:`str` and match with one of the Normalization options listed
```

### Comparing `pyVIP-1.8.0/virtualitics/vip_result.py` & `pyVIP-1.9.0/virtualitics/vip_result.py`

 * *Files identical despite different names*

