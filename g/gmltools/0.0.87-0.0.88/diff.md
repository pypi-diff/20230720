# Comparing `tmp/gmltools-0.0.87.tar.gz` & `tmp/gmltools-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.87.tar", last modified: Thu Jul 20 07:50:40 2023, max compression
+gzip compressed data, was "gmltools-0.0.88.tar", last modified: Thu Jul 20 13:16:14 2023, max compression
```

## Comparing `gmltools-0.0.87.tar` & `gmltools-0.0.88.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.604143 gmltools-0.0.87/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.87/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.87/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-07-20 07:50:40.604143 gmltools-0.0.87/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.87/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.584047 gmltools-0.0.87/dist/
--rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.87/dist/gmltools-0.0.80.tar.gz
--rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.87/dist/gmltools-0.0.81.tar.gz
--rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.87/dist/gmltools-0.0.82.tar.gz
--rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.87/environment.txt
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.87/gmltools.yml
--rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.87/gmltools2.yml
--rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.87/gmltools3.yml
--rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.87/gmltools4.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.87/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-07-20 07:50:08.000000 gmltools-0.0.87/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 07:50:40.604143 gmltools-0.0.87/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-07-20 07:50:01.000000 gmltools-0.0.87/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.568997 gmltools-0.0.87/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.585040 gmltools-0.0.87/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.87/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.87/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.591021 gmltools-0.0.87/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.87/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    45883 2023-06-29 11:50:55.000000 gmltools-0.0.87/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.597783 gmltools-0.0.87/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.87/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.87/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.87/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.87/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   165893 2023-07-20 07:49:43.000000 gmltools-0.0.87/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7529 2023-07-20 07:31:38.000000 gmltools-0.0.87/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.87/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.599791 gmltools-0.0.87/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.87/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.87/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.87/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.603152 gmltools-0.0.87/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.87/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.87/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.87/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.87/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:50:40.590011 gmltools-0.0.87/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-07-20 07:50:40.000000 gmltools-0.0.87/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-07-20 07:50:40.000000 gmltools-0.0.87/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 07:50:40.000000 gmltools-0.0.87/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-07-20 07:50:40.000000 gmltools-0.0.87/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 07:50:40.000000 gmltools-0.0.87/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.781390 gmltools-0.0.88/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.88/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.88/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-07-20 13:16:14.780391 gmltools-0.0.88/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.88/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.666233 gmltools-0.0.88/dist/
+-rw-rw-rw-   0        0        0    78901 2023-06-14 08:50:22.000000 gmltools-0.0.88/dist/gmltools-0.0.80.tar.gz
+-rw-rw-rw-   0        0        0    78864 2023-06-14 08:54:29.000000 gmltools-0.0.88/dist/gmltools-0.0.81.tar.gz
+-rw-rw-rw-   0        0        0    79689 2023-06-26 15:34:26.000000 gmltools-0.0.88/dist/gmltools-0.0.82.tar.gz
+-rw-rw-rw-   0        0        0      483 2023-04-27 11:36:50.000000 gmltools-0.0.88/environment.txt
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.88/gmltools.yml
+-rw-rw-rw-   0        0        0    17997 2023-04-17 10:10:38.000000 gmltools-0.0.88/gmltools2.yml
+-rw-rw-rw-   0        0        0    17200 2023-04-24 08:57:47.000000 gmltools-0.0.88/gmltools3.yml
+-rw-rw-rw-   0        0        0     4638 2023-04-26 09:14:46.000000 gmltools-0.0.88/gmltools4.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.88/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-07-20 13:15:32.000000 gmltools-0.0.88/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 13:16:14.782398 gmltools-0.0.88/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-07-20 13:15:23.000000 gmltools-0.0.88/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.590344 gmltools-0.0.88/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.676234 gmltools-0.0.88/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.88/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.88/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.687891 gmltools-0.0.88/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.88/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    45961 2023-07-20 13:15:02.000000 gmltools-0.0.88/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.727800 gmltools-0.0.88/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.88/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.88/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.88/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.88/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   165893 2023-07-20 07:49:43.000000 gmltools-0.0.88/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7529 2023-07-20 07:31:38.000000 gmltools-0.0.88/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    33623 2023-07-06 11:21:54.000000 gmltools-0.0.88/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.749392 gmltools-0.0.88/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.88/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.88/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.88/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.778360 gmltools-0.0.88/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.88/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.88/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.88/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.88/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-20 13:16:14.682251 gmltools-0.0.88/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-07-20 13:16:14.000000 gmltools-0.0.88/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-07-20 13:16:14.000000 gmltools-0.0.88/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 13:16:14.000000 gmltools-0.0.88/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-07-20 13:16:14.000000 gmltools-0.0.88/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 13:16:14.000000 gmltools-0.0.88/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.87/LICENSE` & `gmltools-0.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/Models.ipynb` & `gmltools-0.0.88/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/PKG-INFO` & `gmltools-0.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.87
+Version: 0.0.88
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.87/README.md` & `gmltools-0.0.88/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/dist/gmltools-0.0.80.tar.gz` & `gmltools-0.0.88/dist/gmltools-0.0.80.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/dist/gmltools-0.0.81.tar.gz` & `gmltools-0.0.88/dist/gmltools-0.0.81.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/dist/gmltools-0.0.82.tar.gz` & `gmltools-0.0.88/dist/gmltools-0.0.82.tar.gz`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/gmltools.yml` & `gmltools-0.0.88/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/gmltools2.yml` & `gmltools-0.0.88/gmltools2.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/gmltools3.yml` & `gmltools-0.0.88/gmltools3.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/gmltools4.yml` & `gmltools-0.0.88/gmltools4.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/mltools.yml` & `gmltools-0.0.88/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/pyproject.toml` & `gmltools-0.0.88/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.87"
+version = "0.0.88"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.87/setup.py` & `gmltools-0.0.88/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.87',
+    'version': '0.0.88',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.87/src/gmltools/To_Do.txt` & `gmltools-0.0.88/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/eda/eda.py` & `gmltools-0.0.88/src/gmltools/eda/eda.py`

 * *Files 1% similar despite different names*

```diff
@@ -891,15 +891,15 @@
 
             patron= [self.df.iloc[int(i)].to_frame().T.index[0].strftime('%Y-%m-%d') for i in self.close_values]
         else:
             pass
 
         return patron
     
-    def plot_similar_pattern(self,date):
+    def plot_similar_pattern(self,date,figsize=(1200,3950),title_font_size=45,legend_size=35,annotation_font_size=40):
         """
         Plot similar pattern of a given date
         Parameters
         ----------
         date : str
             Date to plot similar pattern
         """
@@ -929,44 +929,42 @@
                 fig.update_xaxes(tickmode = 'array', tickvals = np.linspace(0,self.subsequence-1,self.subsequence), row=i+1, col=1)
             fig.update_layout(title_text=f"Patrones similares para {date} {self.df.columns.values}", title_x=0.5, height=800+height_adjuts*100)
             #x name as Hour
             fig.update_xaxes(title_text="Hour", tickfont=dict(size=24))
             fig.update_yaxes(title_text="Valor", tickfont=dict(size=24))
 
             if len(patron) ==1:
-                height=1200/1.4
-                width=3950
-            else:
-                height=1200
+                height=height/1.4
                 width=3950
+
             #tight layout automatically adjusts subplot params so that the subplot(s) fits in to the figure area
-            fig.update_layout(showlegend=True, title_x=0.5, title_y=0.999, title_font_size=45, title_font_color="black", title_font_family="Arial", title_xanchor="center", title_yanchor="top",
-                            margin=dict(t=100, b=50, l=50, r=50),legend=dict(font=dict(size=35)), height=height, width=width) 
-            fig.update_annotations(font_size=40)
+            fig.update_layout(showlegend=True, title_x=0.5, title_y=0.999, title_font_size=title_font_size, title_font_color="black", title_font_family="Arial", title_xanchor="center", title_yanchor="top",
+                            margin=dict(t=100, b=50, l=50, r=50),legend=dict(font=dict(size=legend_size)), height=height, width=width) 
+            fig.update_annotations(font_size=annotation_font_size)
             #increase size of xticks values
 
             fig.show()
         else:
             fig = go.Figure()
 
             fig.add_annotation(
                 dict(
                     x=0.5, # posición en x
                     y=0.5, # posición en y
                     showarrow=False,
                     text="No se ha podido encontrar el día más parecido", # mensaje de texto
                     xref="paper",
                     yref="paper",
-                    font=dict(size=45, color='black'), # tamaño y color del texto
+                    font=dict(size=annotation_font_size+5, color='black'), # tamaño y color del texto
                 )
             )
-            fig.update_layout(title_text=f"Patrones similares para {date} {self.df.columns.values}", title_x=0.5, height=800+height_adjuts*100, title_font_size=45)
+            fig.update_layout(title_text=f"Patrones similares para {date} {self.df.columns.values}", title_x=0.5, height=800+height_adjuts*100, title_font_size=title_font_size)
             fig.update_layout(
                 xaxis=dict(showgrid=False, zeroline=False, showticklabels=False), # esconde el eje x
                 yaxis=dict(showgrid=False, zeroline=False, showticklabels=False), # esconde el eje y
-                height=1200/1.4,
+                height=height,
 
-                width=3950)
+                width=width)
             
             fig.show()
 
         self.fig=fig
```

### Comparing `gmltools-0.0.87/src/gmltools/models/bayes.py` & `gmltools-0.0.88/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.88/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/models/dummy_model.py` & `gmltools-0.0.88/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/models/model.py` & `gmltools-0.0.88/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/models/models_info.py` & `gmltools-0.0.88/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.88/src/gmltools/models/timeseriesplit.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.88/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.88/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.88/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.88/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.88/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.87/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.88/src/gmltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.87
+Version: 0.0.88
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.87/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.88/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

