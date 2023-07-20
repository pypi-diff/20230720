# Comparing `tmp/IngeoDash-0.1.0.tar.gz` & `tmp/IngeoDash-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.1.0.tar", last modified: Thu Jul 20 12:27:27 2023, max compression
+gzip compressed data, was "IngeoDash-0.1.1.tar", last modified: Thu Jul 20 19:36:39 2023, max compression
```

## Comparing `IngeoDash-0.1.0.tar` & `IngeoDash-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/IngeoDash/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 12:27:27.000000 IngeoDash-0.1.0/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:27:27.240450 IngeoDash-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 12:25:43.000000 IngeoDash-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.429639 IngeoDash-0.1.1/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/IngeoDash/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:36:39.429639 IngeoDash-0.1.1/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 19:36:39.000000 IngeoDash-0.1.1/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:36:39.433639 IngeoDash-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-20 19:34:57.000000 IngeoDash-0.1.1/setup.py
```

### Comparing `IngeoDash-0.1.0/IngeoDash/__init__.py` & `IngeoDash-0.1.1/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
```

### Comparing `IngeoDash-0.1.0/IngeoDash/__main__.py` & `IngeoDash-0.1.1/IngeoDash/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from IngeoDash.app import table_next, progress, update_row, table, table_component, table_prev
+from IngeoDash.app import table_next, progress, update_row, table, table_component, table_prev, labels_proportion
 from IngeoDash.download import download, download_component
 from IngeoDash.upload import upload, upload_component
 from IngeoDash.config import CONFIG
 from dash import dcc, Output, Input, callback, Dash, State, ctx
 import dash_bootstrap_components as dbc
 
 
@@ -49,14 +49,23 @@
 )
 def progress_callback(mem):
     mem = CONFIG(mem)
     return progress(mem)
 
 
 @callback(
+    Output(CONFIG.labels_proportion, 'children'),
+    Input(CONFIG.store, 'data')
+)
+def progress_callback(mem):
+    mem = CONFIG(mem)
+    return labels_proportion(mem)
+
+
+@callback(
     Output(CONFIG.data, 'data'),
     Input(CONFIG.data, 'active_cell'),
     State(CONFIG.store, 'data'),
     prevent_initial_call=True
 )
 def update_row_callback(table, mem):
     mem = CONFIG(mem)
```

### Comparing `IngeoDash-0.1.0/IngeoDash/annotate.py` & `IngeoDash-0.1.1/IngeoDash/annotate.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,42 +7,59 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from EvoMSA import BoW, DenseBoW
+from EvoMSA import BoW, DenseBoW, StackGeneralization
 from typing import Union
 from IngeoDash.config import Config
 from IngeoDash.config import CONFIG
+from sklearn.svm import LinearSVC
 import numpy as np
 
 
 def has_label(mem: Config, x):
     if mem.label_header in x:
         ele = x[mem.label_header]
         if ele is not None and len(f'{ele}'):
             return True
     return False
 
 
-def model(mem: Config, data: dict):
+def model(mem: Config, data: dict, select: bool=True):
     lang = mem[mem.lang]
     if lang not in CONFIG.denseBoW:
-        dense = DenseBoW(lang=lang, voc_size_exponent=15,
+        dense = DenseBoW(lang=lang, voc_size_exponent=mem.voc_size_exponent,
+                         voc_selection=mem.voc_selection,
                          n_jobs=mem.n_jobs, dataset=False)
         CONFIG.denseBoW[lang] = dense.text_representations
     dense = DenseBoW(lang=lang, key=mem.text,
                      label_key=mem.label_header,
-                     voc_size_exponent=15,
+                     voc_size_exponent=mem.voc_size_exponent,
+                     voc_selection=mem.voc_selection,
                      n_jobs=mem.n_jobs,
                      dataset=False, emoji=False, keyword=False)
     dense.text_representations_extend(CONFIG.denseBoW[lang])
-    return dense.select(D=data).fit(data)
+    if select:
+        dense.select(D=data)
+    _ = np.unique([x[mem.label_header] for x in data],
+                  return_counts=True)[1]
+    if np.any(_ < 5):
+        return dense.fit(data)
+    bow = BoW(lang=lang, key=mem.text,
+              label_key=mem.label_header,
+              voc_size_exponent=mem.voc_size_exponent,
+              voc_selection=mem.voc_selection)
+    stack = StackGeneralization(decision_function_models=[bow, dense],
+                                decision_function_name=mem.decision_function_name,
+                                estimator_class=mem.estimator_class)
+    return stack.fit(data)
+    
 
 
 def active_learning_selection(mem: Config):
     db = CONFIG.db[mem[mem.username]]
     dense = model(mem, db[mem.permanent])  
     D = db[mem.data] + db.get(mem.original, list())
     hy = dense.decision_function(D)
@@ -86,25 +103,25 @@
     db = CONFIG.db[mem[mem.username]]
     if mem.permanent in db:
         _ = np.unique([x[mem.label_header]
                        for x in db[mem.permanent]])
         if _.shape[0] > 1:
             mem[mem.labels] = tuple(_.tolist())
             return label_column_predict(mem, model=model)
-    label = mem.get(mem.labels, ('-', ))[0]
+    label = mem.get(mem.labels, (0, ))[0]
     data = db[mem.data]
     for ele in data:
         ele[mem.label_header] = ele.get(mem.label_header, label)
 
 
 def flip_label(mem: Config, k: int):
     db = CONFIG.db[mem[mem.username]]
     data = db[mem.data]
     assert k < len(data)
-    labels = mem.get(mem.labels, ('-', '+')) 
+    labels = mem.get(mem.labels, (0, 1)) 
     label = data[k][mem.label_header]
     index = (labels.index(label) + 1) % len(labels)
     data[k][mem.label_header] = labels[index]
     return data[k]
 
 
 def store(mem: Config):
```

### Comparing `IngeoDash-0.1.0/IngeoDash/app.py` & `IngeoDash-0.1.1/IngeoDash/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import flip_label, label_column, store
 from IngeoDash.config import CONFIG, Config
 from dash import dash_table, html
+from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 from dash import Patch
 import string
 import json
 import numpy as np
 
 
@@ -81,19 +82,22 @@
     buttons = dbc.ButtonGroup([dbc.Button('Previous',
                                  color='secondary',
                                  id=CONFIG.prev),
                       dbc.Button('Next', 
                                  color='primary', 
                                  id=CONFIG.next,
                                  n_clicks=0)])
-    return dbc.Stack([dbc.Progress(value=0, id=CONFIG.progress),
+    labels_proportion = dbc.Progress(id=CONFIG.labels_proportion)
+    return dbc.Stack([dbc.Progress(value=0, label='Progress',
+                                   id=CONFIG.progress,
+                                   color='info'),
+                      labels_proportion,
                       html.Div(id=CONFIG.center,
                                children=table(CONFIG)),
-                      buttons
-                      ])
+                      buttons])
 
 
 def user(mem: Config):
     try:
         username = mem[mem.username]
     except KeyError:
         for i in range(10):
@@ -130,8 +134,29 @@
     data = flip_label(mem, k=table['row'])
     patch = Patch()
     del patch[table['row']]
     patch.insert(table['row'], {k: f'{v}'for k, v in data.items()})
     return patch
 
 
-
+def labels_proportion(mem: Config):
+    if mem.username not in mem:
+        raise PreventUpdate
+    db = CONFIG.db[mem[mem.username]]
+    if mem.permanent not in db:
+        raise PreventUpdate
+    D = db[mem.permanent]
+    labels, cnt = np.unique([x[mem.label_header] for x in D], return_counts=True)
+    proportions = 100 * cnt / cnt.sum()
+    colors = ['primary', 'secondary', 'success']
+    output = []
+    for label, amount, prop, k in zip(labels, cnt, proportions,
+                                      range(len(labels))):
+        _ = dbc.Progress(value=prop, color=colors[k % len(colors)],
+                         label=f'{label} (#{amount})', bar=True)
+        output.append(_)
+    return output
+
+
+if __name__ == '__main__':
+    from IngeoDash.__main__ import test_component
+    test_component(table_component())
```

### Comparing `IngeoDash-0.1.0/IngeoDash/config.py` & `IngeoDash-0.1.1/IngeoDash/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from dataclasses import dataclass, field
+from sklearn.svm import LinearSVC
 from typing import Tuple
 from copy import deepcopy
 import json
 
 
 @dataclass
 class Config:
@@ -43,14 +44,20 @@
     text: str = 'text'
     mem: dict = field(default_factory=dict)
     prev: str='previous'
     batch_size: str='n_value'
     checklist: str='checklist'
     active_learning: str='active_learning'
     shuffle: str='shuffle'
+    labels_proportion: str='labels_proportion'
+    voc_size_exponent: int=15
+    voc_selection: str='most_common_by_type'
+    estimator_class: object=LinearSVC
+    decision_function_name: str='decision_function'
+
 
     def __getitem__(self, key):
         return self.mem[key]
     
     def __setitem__(self, key, value):
         self.mem[key] = value
```

### Comparing `IngeoDash-0.1.0/IngeoDash/download.py` & `IngeoDash-0.1.1/IngeoDash/download.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.0/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.1.1/IngeoDash/tests/test_annotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 def test_label_column():
     data = [dict() for i in range(3)]
     mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.data: data}
     db = CONFIG.db['xxx']
     label_column(mem)
     for hy in data:
-        assert '-' == hy[mem.label_header]
-    labels = ['+', '-', '-']
+        assert 0 == hy[mem.label_header]
+    labels = [1, 0, 0]
     for k, ele in zip(labels,
                       data):
         ele[mem.label_header] = k
     label_column(mem)
     for y, hy in zip(labels, data):
         assert y == hy[mem.label_header]
 
@@ -95,15 +95,15 @@
 def test_flip_label():
     data = [dict() for i in range(3)]
     mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.data: data}
     db = CONFIG.db['xxx']
     label_column(mem)
     flip_label(mem, k=1)
-    assert db[mem.data][1][mem.label_header] == '+'
+    assert db[mem.data][1][mem.label_header] == 1
 
 
 def test_store():
     data = [dict() for i in range(3)]    
     mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.data: data}
     db = CONFIG.db['xxx']
```

### Comparing `IngeoDash-0.1.0/IngeoDash/tests/test_app.py` & `IngeoDash-0.1.1/IngeoDash/tests/test_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from IngeoDash.app import mock_data, table_next, progress, user, update_row, table_component, table_prev
+from IngeoDash.app import mock_data, table_next, progress, user, update_row, table_component, table_prev, labels_proportion
+from dash.exceptions import PreventUpdate
 from IngeoDash.annotate import label_column
 from IngeoDash.config import Config
 from IngeoDash.config import CONFIG
 from EvoMSA.tests.test_base import TWEETS
 from microtc.utils import tweet_iterator
 import numpy as np
 
@@ -120,8 +121,27 @@
 def test_update_row():
     from dash import Patch
     D = mock_data()
     mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.data: D[:10]}
     label_column(mem)    
     _ = update_row(mem, dict(row=0))
-    assert isinstance(_, Patch)    
+    assert isinstance(_, Patch)
+
+
+def test_labels_proportion():
+    try:
+        labels_proportion(CONFIG)
+    except PreventUpdate:
+        pass
+    _ = {CONFIG.username: 'xxx'}
+    mem = CONFIG(_)
+    CONFIG.db['xxx'] = dict()
+    try:
+        labels_proportion(mem)
+    except PreventUpdate:
+        pass
+    CONFIG.db['xxx'].update({mem.permanent: [dict(klass=0)] * 3 + [dict(klass=1)] * 5})
+    v = np.array([3, 5])
+    v = v / v.sum() * 100
+    for ele, p in zip(labels_proportion(mem), v):
+        assert ele.value == p
```

### Comparing `IngeoDash-0.1.0/IngeoDash/tests/test_config.py` & `IngeoDash-0.1.1/IngeoDash/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                    username='username',
                    text='text',
                    mem={},
                    prev='previous',
                    batch_size='n_value',
                    checklist='checklist',
                    active_learning='active_learning',
-                   shuffle='shuffle')
+                   shuffle='shuffle',
+                   labels_proportion='labels_proportion')
     for k, v in default.items():
         assert v == getattr(conf, k)
 
 
 def test_Config_mem():
     config = Config()
```

### Comparing `IngeoDash-0.1.0/IngeoDash/tests/test_download.py` & `IngeoDash-0.1.1/IngeoDash/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.0/IngeoDash/tests/test_upload.py` & `IngeoDash-0.1.1/IngeoDash/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.0/IngeoDash/upload.py` & `IngeoDash-0.1.1/IngeoDash/upload.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.0/IngeoDash.egg-info/PKG-INFO` & `IngeoDash-0.1.1/IngeoDash.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.1.0
+Version: 0.1.1
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.1.0/LICENSE` & `IngeoDash-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.0/PKG-INFO` & `IngeoDash-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.1.0
+Version: 0.1.1
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `IngeoDash-0.1.0/README.rst` & `IngeoDash-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.1.0/setup.py` & `IngeoDash-0.1.1/setup.py`

 * *Files identical despite different names*

