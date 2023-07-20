# Comparing `tmp/DependiPy-1.0.2.tar.gz` & `tmp/DependiPy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DependiPy-1.0.2.tar", last modified: Thu Jul 20 12:13:15 2023, max compression
+gzip compressed data, was "DependiPy-1.0.8.tar", last modified: Thu Jul 20 16:58:05 2023, max compression
```

## Comparing `DependiPy-1.0.2.tar` & `DependiPy-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 12:13:15.388496 DependiPy-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-20 12:13:15.374465 DependiPy-1.0.2/DependiPy/
--rw-rw-rw-   0        0        0       72 2023-07-20 08:08:10.000000 DependiPy-1.0.2/DependiPy/__init__.py
--rw-rw-rw-   0        0        0    21802 2023-07-19 06:36:51.000000 DependiPy-1.0.2/DependiPy/archive.py
--rw-rw-rw-   0        0        0     2626 2023-07-20 08:38:43.000000 DependiPy-1.0.2/DependiPy/librarian.py
--rw-rw-rw-   0        0        0       17 2023-07-20 11:57:15.000000 DependiPy-1.0.2/DependiPy/version.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:13:15.387466 DependiPy-1.0.2/DependiPy.egg-info/
--rw-rw-rw-   0        0        0      187 2023-07-20 12:13:15.000000 DependiPy-1.0.2/DependiPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-07-20 12:13:15.000000 DependiPy-1.0.2/DependiPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 12:13:15.000000 DependiPy-1.0.2/DependiPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-20 12:13:15.000000 DependiPy-1.0.2/DependiPy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-07-20 12:13:15.000000 DependiPy-1.0.2/DependiPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-20 12:13:15.000000 DependiPy-1.0.2/DependiPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-07-20 07:58:29.000000 DependiPy-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      187 2023-07-20 12:13:15.388496 DependiPy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11582 2023-07-20 11:56:50.000000 DependiPy-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-20 12:13:15.388496 DependiPy-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-07-20 08:34:16.000000 DependiPy-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:58:05.044111 DependiPy-1.0.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:58:05.040111 DependiPy-1.0.8/DependiPy/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21373 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/archive.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/librarian.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:58:05.040111 DependiPy-1.0.8/DependiPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11507 2023-07-20 16:58:04.000000 DependiPy-1.0.8/DependiPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-20 16:58:05.000000 DependiPy-1.0.8/DependiPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-20 16:58:04.000000 DependiPy-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11507 2023-07-20 16:58:05.044111 DependiPy-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11287 2023-07-20 16:58:04.000000 DependiPy-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:58:05.044111 DependiPy-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-20 16:58:04.000000 DependiPy-1.0.8/setup.py
```

### Comparing `DependiPy-1.0.2/DependiPy/archive.py` & `DependiPy-1.0.8/DependiPy/archive.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,429 +1,429 @@
-import ast
-import pandas as pd
-import os
-import numpy as np
-from tqdm import tqdm
-import pkg_resources
-
-
-class LibMapperTools:
-
-    def __init__(self, lib_name, remove, replace_dict, exclusion, librerie_private=None, mode='lib'):
-        self.lib_name = lib_name
-        self.remove = remove
-        self.replace_dict = replace_dict
-        self.exclusion = exclusion
-        self.number_of_levels = 0
-        self.librerie_private = librerie_private
-        self.mode = mode
-
-        # lista di colonne, serve per il codice
-        self.saved_columns = ['file', 'req', 'path']
-
-    def read_files(self):
-        # vengono cergati tutti i file dentro la libreria
-        df = pd.DataFrame()
-        for (dirpath, dirnames, filenames) in os.walk(self.lib_name):
-            # vengono salvato i percorsi di ogni file
-            path = dirpath.replace("/", "").replace(".", "").replace("\\", ".")
-            # il percorso viene rotto nelle sue componenti e messo in una lista
-            levels = path.split(".")
-            # se dopo aver eliminato le cartelle da escludere rimangono delle cartelle allora si prosegue con il parsing
-            if not len(set(self.exclusion).intersection(levels)) > 0:
-                # si inizializza il dataframe temporaneo in cui si salvano le librerie di ogni file uno ad uno
-                req_temp = pd.DataFrame(columns=["level_" + str(i) for i in range(len(levels))] + self.saved_columns,
-                                        index=[i for i in range(len(filenames))])
-                # si popola il dataframe
-                req_temp.loc[:, ["level_" + str(i) for i in range(len(levels))]] = levels
-                req_temp.loc[:, 'path'] = path
-                # si legge ogni file
-                for i, file in enumerate(filenames):
-                    # filtro per i soli script python
-                    if file.split(".")[-1] == "py" and not file.startswith('test'):
-                        try:
-                            with open(dirpath + "/" + file, "r") as f:
-                                contents = f.read()
-                            # il contenuto del file viene madato alla funzione che ne estrae le librerie
-                            req = self.books_extraction(contents)
-                            req_temp.loc[req_temp.index[i], 'file'] = file
-                            req_temp.loc[req_temp.index[i], 'req'] = req
-                        except:
-                            print(file, 'impossible to read')
-                # viene popolato un dataframe comune a tutti i file
-                df = pd.concat([df, req_temp], ignore_index=True)
-                # se un file non viene considerato perche non ha il .py con il drop viene eliminata la sua riga
-                df = df.dropna(subset=['file'])
-
-        # si ottiene il numero di livelli di profondita della classe
-        number_of_levels = df.columns.difference(self.saved_columns).shape[0]
-        # si riordinano le colonne
-        df = df.loc[:, ["level_" + str(i) for i in range(number_of_levels)] + self.saved_columns]
-        self.number_of_levels = number_of_levels
-        return df
-
-    # funzione parsa il testo del codice ed estrae i nomi delle librerie usate
-    def books_extraction(self, text):
-        modules = []
-        # usando la libreria ast vengono trovati gli import
-        for node in ast.iter_child_nodes(ast.parse(text)):
-            if isinstance(node, ast.ImportFrom):
-                modules.append(node.module)
-            elif isinstance(node, ast.Import):
-                modules.append(node.names[0].name)
-
-        # se gli import erano divisi in un percorso viene preso solo il primo elemento del percorso
-        def select_first(name):
-            # se l'import era una cross reference viene tenuto tutto il percorso
-            if name.split('.')[0] == self.lib_name:
-                return name
-            # se l'import era una libreria privata viene tenuto tutto il percorso
-            elif name.split('.')[0] in self.librerie_private:
-                return name
-            # se no restituisce solo il primo termine
-            else:
-                return name.split('.')[0]
-
-        # vengono tenute le libreri in modo unico
-        librerie = list(set(list(map(select_first, modules))))
-        return librerie
-
-####################################################################################################################
-####################################################################################################################
-####################################################################################################################
-####################################################################################################################
-
-    # funzione che estrae dalla lista delle librerie quelle che appartengono alle cross referenze,
-    # quindi quelle che hanno nel nome la parola lib_name
-    def cross_reference_extraction(self, _list):
-        cross_reference_list = []
-        for _ele in _list:
-            if _ele.split(".")[0] == self.lib_name:
-                cross_reference_list.append(_ele)
-        return cross_reference_list
-
-    # funzione che fa pulizia sulle librerie nella lista che gli viene passata
-    def cleaning(self, _list):
-        elements = _list.copy()
-        if len(_list) > 0:
-            for _ele in elements:
-                # vengono rimosse le librerie legate alle cross reference
-                if _ele.split(".")[0] == self.lib_name:
-                    _list.remove(_ele)
-                # vengono rimossi i riferimenti alle librerie private
-                elif _ele.split('.')[0] in self.librerie_private and self.mode == 'lib':  # la condizione e' elif perche la lib_name potrebbe essere anche una libreria privata
-                    _list.remove(_ele)
-
-                # vengono rimosse le librerie segnate come da eliminare
-                if _ele in self.remove:
-                    _list.remove(_ele)
-
-                # vengono sostituite le librerie segnate come da sostituire
-                if _ele in self.replace_dict:
-                    _list += self.replace_dict[_ele]
-                    _list.remove(_ele)
-            return _list
-        else:
-            # viene restituito NaN se un file non ha librerie
-            return []
-
-    @staticmethod
-    def remove_unrequired(df):
-        # i file che non hanno librerie e sono __init__ vengono eliminati dalla mappatura
-        # mentre se un file non ha librerie viene cmq tenuto dentro i percorsi chiamabili
-        allowed_files = []
-        for i in range(df.shape[0]):
-            if (df.loc[df.index[i], 'req'] is pd.NA) and df.loc[df.index[i], 'file'] == "__init__.py":
-                allowed_files.append(False)
-            else:
-                allowed_files.append(True)
-
-        # per riempire la casella req dei file che non hanno librerie con una lista vuota va inserita una lista con
-        # un elemento e poi va rimosso quell'elemento
-        for i in range(df.shape[0]):
-            if df.loc[df.index[i], 'req'] is pd.NA:
-                df.loc[df.index[i], 'req'] = ['waste_list']
-                df.loc[df.index[i], 'req'].remove('waste_list')
-
-        # vengono eliminate gli script marcati come da aliminare perche senza requisiti
-        df = df.loc[allowed_files]
-        return df
-
-    @staticmethod
-    def add_path(df):
-        # viene creata una colonna con il contenuto del percorso di un file e il nome del file stesso
-        df.loc[:, 'path_file'] = df.loc[:, 'path'] + "." + df['file'].str.replace('.py', '', regex=True)
-        return df
-
-    @staticmethod
-    def cross_mapping(df, max_deep=7):  # max_deep rappresenta la profondita massima raggiungibile per una catena di cross reference
-        def cross_mapper(_cross_files, _cross_lib_temp, _max_deep):
-            # viene ridotto un contatore di sicurezza che impedisce di restare incastrati in una referenza circolare
-            _max_deep = _max_deep - 1
-            if _max_deep <= 0: return []
-            # si cicla sulle cross referenze
-            for cross_file in _cross_files:
-                # vengono aggiornate le referenze se presenti
-                if df.loc[df['path_file'] == cross_file, 'req'].shape[0] > 0:
-                    _cross_lib_temp.update(set(df.loc[df['path_file'] == cross_file, 'req'].iloc[0]))
-                # vengono aggiornate le cross referenze se presenti
-                if df.loc[df['path_file'] == cross_file, 'cross'].shape[0] > 0:
-                    chain_cross = df.loc[df['path_file'] == cross_file, 'cross'].iloc[0]
-                    # in caso di presenza di cross referenze viene chiamata ricorsivamente la funzione di mapping sulla
-                    # nuova cross reference
-                    _cross_lib_temp.update(cross_mapper(chain_cross, _cross_lib_temp, _max_deep))
-            return _cross_lib_temp
-
-        cross_lib_tot = []
-        # un file per volta vengono estratte tutti i requirements dalle cross referenze
-        files = tqdm(range(df.shape[0]), position=0, leave=True, ascii=True, unit=' files')
-        for i in files:
-            cross_files = df.iloc[i, df.columns.get_loc('cross')]
-            # origin = df.iloc[i, df.columns.get_loc('path_file')]
-            # viene chiamata la funzione che estrae le cross referenze
-            cross_lib = cross_mapper(cross_files, set([]), max_deep)
-            # i risultati vengono salvati in una lista
-            cross_lib_tot.append(list(cross_lib))
-
-        # vengono eliminate le colonne che servivano solo alle cross referenze
-        df = df.loc[:, df.columns.difference(['cross', 'path_file'])]
-
-        # variabile che verifica il numero di cross referenze
-        empty_check = 0
-        for crosses in cross_lib_tot:
-            empty_check += len(crosses)
-
-        # alle referenze di ogni file vengono aggiunte le referenze estratte con il cross mapping e vengono eliminati i duplicati
-        if empty_check > 0:
-            _list_np = df.loc[:, 'req'] + np.array(cross_lib_tot, dtype=object)
-            df.loc[:, 'req'] = _list_np.apply(set).apply(list)
-        return df
-
-    def level_explorer(self, df, level, max_levels, pre_cat, _res):
-        """
-            funzione ricorsica che mappa l'albero della libreria e verifica come ogni referenza dei file contenuti in un ramo
-            debbano essere usati se si chiede tutte le referenze di un bivio piu un alto
-        """
-
-        # un controllo impedisce un loop infinito andando a fermare la mappatura quando si raggunge la profondita massima dell'albero
-        if level >= max_levels: return _res
-        # vengono ottenuti i nomi delle cartelle di uno specifico livello
-        category1 = df.dropna(subset='level_' + str(level))['level_' + str(level)].unique()
-        # si cicla su ogni cartella
-        for cat1 in category1:
-            # viene fatta la selezione del dataframe con i soli valori corispondenti a una cartella
-            cat_df1 = df.loc[df['level_' + str(level)] == cat1, :].dropna(subset='level_' + str(level))
-            # vengono estratti tutti i requisiti di tutti i file presenti in quella cartella e sotto cartelle
-            selection1 = list(set(cat_df1.loc[:, 'req'].sum()))
-            # viene mappata la posizione nell'albero
-            level_name = pre_cat + cat1
-            # se erano presenti requisiti si prosegue
-            if len(selection1) > 0:
-                # i requisiti trovati vengono caricati in un dataframe
-                temp_pd = pd.DataFrame(columns=['path', 'req'], index=[0])
-                temp_pd.loc[temp_pd.index[0], 'req'] = selection1
-                temp_pd.loc[temp_pd.index[0], 'path'] = level_name
-                _res = pd.concat([_res, temp_pd], ignore_index=True)
-            # se sono prenenti altri livelli viene chiamata ricorsivamente la stessa funzione di mappatura
-            _res = self.level_explorer(cat_df1, level=level + 1, max_levels=max_levels, pre_cat=level_name + ".",
-                                       _res=_res)
-        return _res
-
-    def add_levels(self, df):
-        # viene usata la funzione di mappatura dei requisti per cartelle
-        res = self.level_explorer(df, 0, self.number_of_levels, "", pd.DataFrame())
-
-        # al percorso di un file viene aggiunto anche il nome del file stesso
-        df.loc[:, 'path'] = df.loc[:, 'path'] + "." + df['file'].str.replace('.py', '', regex=True)
-        # tutti i requirements vengono messi in un unico dataframe
-        res = pd.concat([res, df.loc[:, ['path', 'req']]], ignore_index=True).sort_values(by=['path'])
-        return res
-
-    def write_mapping(self, df, **kwargs):
-
-        # per poter scrivere i requisiti nel posto giusto si riporta la posizione di lavoro nel punto di partenza se in modalita script
-        if kwargs['mode'] == 'script': os.chdir(self.lib_name)
-
-        # vengono trovate tutte le librerie usate nel progetto
-        single_requirements = set([item for sublist in df['req'].tolist() for item in sublist])
-
-        distribusion_not_found, requirements_variable, requirements_versioned, _ = self.clean_from_python_packages(single_requirements)
-
-        print(f'list of distribution not found: {distribusion_not_found}')
-
-        if 'docs_only' in kwargs and kwargs.get('docs_only') == False or 'docs_only' not in kwargs:
-            # viene scritto il file dei requisiti
-            with open("requirements.txt", "w") as f:
-                for s in requirements_versioned:
-                    f.write(s + "\n")
-
-        ###############################
-        # da aggiungere la parte che costruisce la documentazione
-        if os.path.exists('docs') and os.path.exists('mkdocs.yml'):
-            for i in range(df.shape[0]):
-                if df.loc[df.index[i], f'file'] != "__init__.py":
-                    name = df.loc[df.index[i], 'path_file']
-                    with open(f"docs/{name}.md", "w") as f:
-                        f.write(f"::: {name}")
-
-            with open("mkdocs.yml", "r") as f:
-                contents_yml = f.readlines()
-
-            for i in range(len(contents_yml)):
-                contents_yml[i] = contents_yml[i].split('\n')[0]
-
-            # se sono presenti i marker per riscrivere le librerie vengono usati
-            api_is_here = True
-            try:
-                if '  - API:' in contents_yml:
-                    yml_start = contents_yml.index('  - API:') + 1
-                    yml_stop = contents_yml[yml_start:].index('') + yml_start
-                else:
-                    yml_start = contents_yml.index('nav:') + 1
-                    yml_start = contents_yml[yml_start:].index('') + yml_start
-                    yml_stop = contents_yml[yml_start:].index('') + yml_start + 1
-                    api_is_here = False
-            except:
-                raise ValueError('missing version tag in the setup.py')
-
-            #######################################################################################
-            docs = []
-            temp_to_add = None
-            for i in range(df.shape[0]):
-                if df.loc[df.index[i], f'file'] != "__init__.py":
-                    valid_col = df.loc[df.index[i], [f'level_{j}' for j in range(self.number_of_levels)]].notnull().sum() - 1
-                    chapter = df.loc[df.index[i], f'level_{valid_col}']
-                    row = f"    - {chapter}:"
-                    space = "  "*(valid_col + 1)
-                    is_to_add = space + row
-                    if is_to_add != temp_to_add:
-                        temp_to_add = is_to_add
-                        docs.append(space + row)
-                    name = df.loc[df.index[i], 'file'].split(".py")[0]
-                    docs.append(space + f"      - {name}: {df.loc[df.index[i], 'path_file']}")
-
-            #######################################################################################
-
-            # venogono aggiunte le nuove librerie alla lista da scrivere sul file
-            if api_is_here: del contents_yml[yml_start: yml_stop]
-            if not api_is_here:
-                docs.insert(0, '  - API:')
-            docs.append('')
-            contents_yml[yml_start:yml_start+1] = docs
-
-            with open("mkdocs.yml", "w") as f:
-                for s in contents_yml:
-                    f.write(str(s) + "\n")
-
-        ###############################
-        if 'docs_only' in kwargs and kwargs.get('docs_only') == False or 'docs_only' not in kwargs:
-
-            if self.mode == 'scirpt':
-                list_privat_reference = ['[' for _ in range(len(self.librerie_private))]
-
-                for ele in single_requirements:
-                    if ele != 'waste':
-                        for i, lib in enumerate(self.librerie_private):
-                            if ele.split('.')[0] == lib:
-                                list_privat_reference[i] += (ele + ',')
-
-                for i in range(len(self.librerie_private)):
-                    if len(list_privat_reference[i]) > 1:
-                        print()
-                        print(list_privat_reference[i][:-1]+']')
-                print()
-
-            if self.mode == 'lib':
-                if not os.path.exists('setup.py'):
-                    raise ValueError('missing the setup.py file mandatory for the script')
-
-                df = self.cross_mapping(df)
-                df = self.add_levels(df)
-
-                # il nome del percorso viene trasformato sostituendo i . con _ ma viene mantenuto anche il nome originale
-                df.loc[:, 'original'] = df.loc[:, 'path'].copy()
-                df.loc[:, 'path'] = df.loc[:, 'path'].str.replace(".", "_", regex=False)
-
-                with open("setup.py", "r") as f:
-                    contents = f.readlines()
-
-                for i in range(len(contents)):
-                    contents[i] = contents[i].split('\n')[0]
-
-                # controllare se ci sono gli star e end
-
-                # se sono presenti i marker per riscrivere le librerie vengono usati
-                try:
-                    vers_start = contents.index('# version go') + 1
-                    vers_stop = contents.index('# version end')
-                except:
-                    raise ValueError('missing version tag in the setup.py')
-
-                # vengono eliminate le librerie dentro i marker
-                del contents[vers_start: vers_stop]
-
-                # venogono aggiunte le nuove librerie alla lista da scrivere sul file
-                contents[vers_start:vers_start] = requirements_variable
-
-                try:
-                    start = contents.index('# start')
-                    stop = contents.index('# stop')
-                except:
-                    raise ValueError('missing version tag in the setup.py')
-
-                packets = ['' for _ in range(df.shape[0])]
-                for i in range(df.shape[0]):
-                    packets[i] += f"'{df.loc[df.index[i], 'original']}': ["
-
-                    _, _, _, eles = self.clean_from_python_packages(df.loc[df.index[i], "req"])
-
-                    j = 0
-                    for ele in eles:
-                        if ele != 'waste':
-                            if j == 0:
-                                packets[i] += f'{ele}'
-                            else:
-                                packets[i] += f', {ele}'
-                            j += 1
-                    packets[i] += '],'
-
-                packets = ['requires_dict = {'] + packets
-                packets = packets + ['}']
-
-                new_set_up = ['' for _ in range(start+len(contents)-stop+len(packets))]
-                new_set_up[:start+1] = contents[:start+1]
-                new_set_up[start+1:len(packets)+1] = packets
-                new_set_up[start+1+len(packets):] = contents[stop:]
-
-                with open("setup.py", "w") as f:
-                    for s in new_set_up:
-                        f.write(str(s) + "\n")
-
-                print(os.getcwd()+"\\setup.py")
-
-    def clean_from_python_packages(self, single_requirements):
-        # vengono matchate le librerie del progetto con le versioni da usare
-        requirements_versioned = []
-        requirements_variable = []
-        distribusion_not_found = []
-        variables = []
-        for req in single_requirements:
-            pass_card = True
-
-            # applicato un controllo se la libreira che si vuole inserire fa parte delle librerie private
-            # in quel caso non deve essere messa nel requirement.txt
-            for pl in self.librerie_private:
-                if req.startswith(pl):
-                    pass_card = False
-                    break
-
-            if pass_card:
-                req_list = self.replace_dict[req] if req in self.replace_dict else [req]
-                for req_i in req_list:
-                    try:
-                        version = pkg_resources.get_distribution(req_i).version
-                        requirements_versioned.append(f'{req_i}=={version}')
-                        requirements_variable.append(f"{req_i.replace('-', '_')} = '{req_i}=={version}'")
-                        variables.append(f"{req_i.replace('-', '_')}")
-                    except pkg_resources.DistributionNotFound:
-                        distribusion_not_found.append(req_i)
-        return distribusion_not_found, requirements_variable, requirements_versioned, variables
+import ast
+import pandas as pd
+import os
+import numpy as np
+from tqdm import tqdm
+import pkg_resources
+
+
+class LibMapperTools:
+
+    def __init__(self, lib_name, remove, replace_dict, exclusion, librerie_private=None, mode='lib'):
+        self.lib_name = lib_name
+        self.remove = remove
+        self.replace_dict = replace_dict
+        self.exclusion = exclusion
+        self.number_of_levels = 0
+        self.librerie_private = librerie_private
+        self.mode = mode
+
+        # lista di colonne, serve per il codice
+        self.saved_columns = ['file', 'req', 'path']
+
+    def read_files(self):
+        # vengono cergati tutti i file dentro la libreria
+        df = pd.DataFrame()
+        for (dirpath, dirnames, filenames) in os.walk(self.lib_name):
+            # vengono salvato i percorsi di ogni file
+            path = dirpath.replace("/", "").replace(".", "").replace("\\", ".")
+            # il percorso viene rotto nelle sue componenti e messo in una lista
+            levels = path.split(".")
+            # se dopo aver eliminato le cartelle da escludere rimangono delle cartelle allora si prosegue con il parsing
+            if not len(set(self.exclusion).intersection(levels)) > 0:
+                # si inizializza il dataframe temporaneo in cui si salvano le librerie di ogni file uno ad uno
+                req_temp = pd.DataFrame(columns=["level_" + str(i) for i in range(len(levels))] + self.saved_columns,
+                                        index=[i for i in range(len(filenames))])
+                # si popola il dataframe
+                req_temp.loc[:, ["level_" + str(i) for i in range(len(levels))]] = levels
+                req_temp.loc[:, 'path'] = path
+                # si legge ogni file
+                for i, file in enumerate(filenames):
+                    # filtro per i soli script python
+                    if file.split(".")[-1] == "py" and not file.startswith('test'):
+                        try:
+                            with open(dirpath + "/" + file, "r") as f:
+                                contents = f.read()
+                            # il contenuto del file viene madato alla funzione che ne estrae le librerie
+                            req = self.books_extraction(contents)
+                            req_temp.loc[req_temp.index[i], 'file'] = file
+                            req_temp.loc[req_temp.index[i], 'req'] = req
+                        except:
+                            print(file, 'impossible to read')
+                # viene popolato un dataframe comune a tutti i file
+                df = pd.concat([df, req_temp], ignore_index=True)
+                # se un file non viene considerato perche non ha il .py con il drop viene eliminata la sua riga
+                df = df.dropna(subset=['file'])
+
+        # si ottiene il numero di livelli di profondita della classe
+        number_of_levels = df.columns.difference(self.saved_columns).shape[0]
+        # si riordinano le colonne
+        df = df.loc[:, ["level_" + str(i) for i in range(number_of_levels)] + self.saved_columns]
+        self.number_of_levels = number_of_levels
+        return df
+
+    # funzione parsa il testo del codice ed estrae i nomi delle librerie usate
+    def books_extraction(self, text):
+        modules = []
+        # usando la libreria ast vengono trovati gli import
+        for node in ast.iter_child_nodes(ast.parse(text)):
+            if isinstance(node, ast.ImportFrom):
+                modules.append(node.module)
+            elif isinstance(node, ast.Import):
+                modules.append(node.names[0].name)
+
+        # se gli import erano divisi in un percorso viene preso solo il primo elemento del percorso
+        def select_first(name):
+            # se l'import era una cross reference viene tenuto tutto il percorso
+            if name.split('.')[0] == self.lib_name:
+                return name
+            # se l'import era una libreria privata viene tenuto tutto il percorso
+            elif name.split('.')[0] in self.librerie_private:
+                return name
+            # se no restituisce solo il primo termine
+            else:
+                return name.split('.')[0]
+
+        # vengono tenute le libreri in modo unico
+        librerie = list(set(list(map(select_first, modules))))
+        return librerie
+
+####################################################################################################################
+####################################################################################################################
+####################################################################################################################
+####################################################################################################################
+
+    # funzione che estrae dalla lista delle librerie quelle che appartengono alle cross referenze,
+    # quindi quelle che hanno nel nome la parola lib_name
+    def cross_reference_extraction(self, _list):
+        cross_reference_list = []
+        for _ele in _list:
+            if _ele.split(".")[0] == self.lib_name:
+                cross_reference_list.append(_ele)
+        return cross_reference_list
+
+    # funzione che fa pulizia sulle librerie nella lista che gli viene passata
+    def cleaning(self, _list):
+        elements = _list.copy()
+        if len(_list) > 0:
+            for _ele in elements:
+                # vengono rimosse le librerie legate alle cross reference
+                if _ele.split(".")[0] == self.lib_name:
+                    _list.remove(_ele)
+                # vengono rimossi i riferimenti alle librerie private
+                elif _ele.split('.')[0] in self.librerie_private and self.mode == 'lib':  # la condizione e' elif perche la lib_name potrebbe essere anche una libreria privata
+                    _list.remove(_ele)
+
+                # vengono rimosse le librerie segnate come da eliminare
+                if _ele in self.remove:
+                    _list.remove(_ele)
+
+                # vengono sostituite le librerie segnate come da sostituire
+                if _ele in self.replace_dict:
+                    _list += self.replace_dict[_ele]
+                    _list.remove(_ele)
+            return _list
+        else:
+            # viene restituito NaN se un file non ha librerie
+            return []
+
+    @staticmethod
+    def remove_unrequired(df):
+        # i file che non hanno librerie e sono __init__ vengono eliminati dalla mappatura
+        # mentre se un file non ha librerie viene cmq tenuto dentro i percorsi chiamabili
+        allowed_files = []
+        for i in range(df.shape[0]):
+            if (df.loc[df.index[i], 'req'] is pd.NA) and df.loc[df.index[i], 'file'] == "__init__.py":
+                allowed_files.append(False)
+            else:
+                allowed_files.append(True)
+
+        # per riempire la casella req dei file che non hanno librerie con una lista vuota va inserita una lista con
+        # un elemento e poi va rimosso quell'elemento
+        for i in range(df.shape[0]):
+            if df.loc[df.index[i], 'req'] is pd.NA:
+                df.loc[df.index[i], 'req'] = ['waste_list']
+                df.loc[df.index[i], 'req'].remove('waste_list')
+
+        # vengono eliminate gli script marcati come da aliminare perche senza requisiti
+        df = df.loc[allowed_files]
+        return df
+
+    @staticmethod
+    def add_path(df):
+        # viene creata una colonna con il contenuto del percorso di un file e il nome del file stesso
+        df.loc[:, 'path_file'] = df.loc[:, 'path'] + "." + df['file'].str.replace('.py', '', regex=True)
+        return df
+
+    @staticmethod
+    def cross_mapping(df, max_deep=7):  # max_deep rappresenta la profondita massima raggiungibile per una catena di cross reference
+        def cross_mapper(_cross_files, _cross_lib_temp, _max_deep):
+            # viene ridotto un contatore di sicurezza che impedisce di restare incastrati in una referenza circolare
+            _max_deep = _max_deep - 1
+            if _max_deep <= 0: return []
+            # si cicla sulle cross referenze
+            for cross_file in _cross_files:
+                # vengono aggiornate le referenze se presenti
+                if df.loc[df['path_file'] == cross_file, 'req'].shape[0] > 0:
+                    _cross_lib_temp.update(set(df.loc[df['path_file'] == cross_file, 'req'].iloc[0]))
+                # vengono aggiornate le cross referenze se presenti
+                if df.loc[df['path_file'] == cross_file, 'cross'].shape[0] > 0:
+                    chain_cross = df.loc[df['path_file'] == cross_file, 'cross'].iloc[0]
+                    # in caso di presenza di cross referenze viene chiamata ricorsivamente la funzione di mapping sulla
+                    # nuova cross reference
+                    _cross_lib_temp.update(cross_mapper(chain_cross, _cross_lib_temp, _max_deep))
+            return _cross_lib_temp
+
+        cross_lib_tot = []
+        # un file per volta vengono estratte tutti i requirements dalle cross referenze
+        files = tqdm(range(df.shape[0]), position=0, leave=True, ascii=True, unit=' files')
+        for i in files:
+            cross_files = df.iloc[i, df.columns.get_loc('cross')]
+            # origin = df.iloc[i, df.columns.get_loc('path_file')]
+            # viene chiamata la funzione che estrae le cross referenze
+            cross_lib = cross_mapper(cross_files, set([]), max_deep)
+            # i risultati vengono salvati in una lista
+            cross_lib_tot.append(list(cross_lib))
+
+        # vengono eliminate le colonne che servivano solo alle cross referenze
+        df = df.loc[:, df.columns.difference(['cross', 'path_file'])]
+
+        # variabile che verifica il numero di cross referenze
+        empty_check = 0
+        for crosses in cross_lib_tot:
+            empty_check += len(crosses)
+
+        # alle referenze di ogni file vengono aggiunte le referenze estratte con il cross mapping e vengono eliminati i duplicati
+        if empty_check > 0:
+            _list_np = df.loc[:, 'req'] + np.array(cross_lib_tot, dtype=object)
+            df.loc[:, 'req'] = _list_np.apply(set).apply(list)
+        return df
+
+    def level_explorer(self, df, level, max_levels, pre_cat, _res):
+        """
+            funzione ricorsica che mappa l'albero della libreria e verifica come ogni referenza dei file contenuti in un ramo
+            debbano essere usati se si chiede tutte le referenze di un bivio piu un alto
+        """
+
+        # un controllo impedisce un loop infinito andando a fermare la mappatura quando si raggunge la profondita massima dell'albero
+        if level >= max_levels: return _res
+        # vengono ottenuti i nomi delle cartelle di uno specifico livello
+        category1 = df.dropna(subset='level_' + str(level))['level_' + str(level)].unique()
+        # si cicla su ogni cartella
+        for cat1 in category1:
+            # viene fatta la selezione del dataframe con i soli valori corispondenti a una cartella
+            cat_df1 = df.loc[df['level_' + str(level)] == cat1, :].dropna(subset='level_' + str(level))
+            # vengono estratti tutti i requisiti di tutti i file presenti in quella cartella e sotto cartelle
+            selection1 = list(set(cat_df1.loc[:, 'req'].sum()))
+            # viene mappata la posizione nell'albero
+            level_name = pre_cat + cat1
+            # se erano presenti requisiti si prosegue
+            if len(selection1) > 0:
+                # i requisiti trovati vengono caricati in un dataframe
+                temp_pd = pd.DataFrame(columns=['path', 'req'], index=[0])
+                temp_pd.loc[temp_pd.index[0], 'req'] = selection1
+                temp_pd.loc[temp_pd.index[0], 'path'] = level_name
+                _res = pd.concat([_res, temp_pd], ignore_index=True)
+            # se sono prenenti altri livelli viene chiamata ricorsivamente la stessa funzione di mappatura
+            _res = self.level_explorer(cat_df1, level=level + 1, max_levels=max_levels, pre_cat=level_name + ".",
+                                       _res=_res)
+        return _res
+
+    def add_levels(self, df):
+        # viene usata la funzione di mappatura dei requisti per cartelle
+        res = self.level_explorer(df, 0, self.number_of_levels, "", pd.DataFrame())
+
+        # al percorso di un file viene aggiunto anche il nome del file stesso
+        df.loc[:, 'path'] = df.loc[:, 'path'] + "." + df['file'].str.replace('.py', '', regex=True)
+        # tutti i requirements vengono messi in un unico dataframe
+        res = pd.concat([res, df.loc[:, ['path', 'req']]], ignore_index=True).sort_values(by=['path'])
+        return res
+
+    def write_mapping(self, df, **kwargs):
+
+        # per poter scrivere i requisiti nel posto giusto si riporta la posizione di lavoro nel punto di partenza se in modalita script
+        if kwargs['mode'] == 'script': os.chdir(self.lib_name)
+
+        # vengono trovate tutte le librerie usate nel progetto
+        single_requirements = set([item for sublist in df['req'].tolist() for item in sublist])
+
+        distribusion_not_found, requirements_variable, requirements_versioned, _ = self.clean_from_python_packages(single_requirements)
+
+        print(f'list of distribution not found: {distribusion_not_found}')
+
+        if 'docs_only' in kwargs and kwargs.get('docs_only') == False or 'docs_only' not in kwargs:
+            # viene scritto il file dei requisiti
+            with open("requirements.txt", "w") as f:
+                for s in requirements_versioned:
+                    f.write(s + "\n")
+
+        ###############################
+        # da aggiungere la parte che costruisce la documentazione
+        if os.path.exists('docs') and os.path.exists('mkdocs.yml'):
+            for i in range(df.shape[0]):
+                if df.loc[df.index[i], f'file'] != "__init__.py":
+                    name = df.loc[df.index[i], 'path_file']
+                    with open(f"docs/{name}.md", "w") as f:
+                        f.write(f"::: {name}")
+
+            with open("mkdocs.yml", "r") as f:
+                contents_yml = f.readlines()
+
+            for i in range(len(contents_yml)):
+                contents_yml[i] = contents_yml[i].split('\n')[0]
+
+            # se sono presenti i marker per riscrivere le librerie vengono usati
+            api_is_here = True
+            try:
+                if '  - API:' in contents_yml:
+                    yml_start = contents_yml.index('  - API:') + 1
+                    yml_stop = contents_yml[yml_start:].index('') + yml_start
+                else:
+                    yml_start = contents_yml.index('nav:') + 1
+                    yml_start = contents_yml[yml_start:].index('') + yml_start
+                    yml_stop = contents_yml[yml_start:].index('') + yml_start + 1
+                    api_is_here = False
+            except:
+                raise ValueError('missing version tag in the setup.py')
+
+            #######################################################################################
+            docs = []
+            temp_to_add = None
+            for i in range(df.shape[0]):
+                if df.loc[df.index[i], f'file'] != "__init__.py":
+                    valid_col = df.loc[df.index[i], [f'level_{j}' for j in range(self.number_of_levels)]].notnull().sum() - 1
+                    chapter = df.loc[df.index[i], f'level_{valid_col}']
+                    row = f"    - {chapter}:"
+                    space = "  "*(valid_col + 1)
+                    is_to_add = space + row
+                    if is_to_add != temp_to_add:
+                        temp_to_add = is_to_add
+                        docs.append(space + row)
+                    name = df.loc[df.index[i], 'file'].split(".py")[0]
+                    docs.append(space + f"      - {name}: {df.loc[df.index[i], 'path_file']}")
+
+            #######################################################################################
+
+            # venogono aggiunte le nuove librerie alla lista da scrivere sul file
+            if api_is_here: del contents_yml[yml_start: yml_stop]
+            if not api_is_here:
+                docs.insert(0, '  - API:')
+            docs.append('')
+            contents_yml[yml_start:yml_start+1] = docs
+
+            with open("mkdocs.yml", "w") as f:
+                for s in contents_yml:
+                    f.write(str(s) + "\n")
+
+        ###############################
+        if 'docs_only' in kwargs and kwargs.get('docs_only') == False or 'docs_only' not in kwargs:
+
+            if self.mode == 'scirpt':
+                list_privat_reference = ['[' for _ in range(len(self.librerie_private))]
+
+                for ele in single_requirements:
+                    if ele != 'waste':
+                        for i, lib in enumerate(self.librerie_private):
+                            if ele.split('.')[0] == lib:
+                                list_privat_reference[i] += (ele + ',')
+
+                for i in range(len(self.librerie_private)):
+                    if len(list_privat_reference[i]) > 1:
+                        print()
+                        print(list_privat_reference[i][:-1]+']')
+                print()
+
+            if self.mode == 'lib':
+                if not os.path.exists('setup.py'):
+                    raise ValueError('missing the setup.py file mandatory for the script')
+
+                df = self.cross_mapping(df)
+                df = self.add_levels(df)
+
+                # il nome del percorso viene trasformato sostituendo i . con _ ma viene mantenuto anche il nome originale
+                df.loc[:, 'original'] = df.loc[:, 'path'].copy()
+                df.loc[:, 'path'] = df.loc[:, 'path'].str.replace(".", "_", regex=False)
+
+                with open("setup.py", "r") as f:
+                    contents = f.readlines()
+
+                for i in range(len(contents)):
+                    contents[i] = contents[i].split('\n')[0]
+
+                # controllare se ci sono gli star e end
+
+                # se sono presenti i marker per riscrivere le librerie vengono usati
+                try:
+                    vers_start = contents.index('# version go') + 1
+                    vers_stop = contents.index('# version end')
+                except:
+                    raise ValueError('missing version tag in the setup.py')
+
+                # vengono eliminate le librerie dentro i marker
+                del contents[vers_start: vers_stop]
+
+                # venogono aggiunte le nuove librerie alla lista da scrivere sul file
+                contents[vers_start:vers_start] = requirements_variable
+
+                try:
+                    start = contents.index('# start')
+                    stop = contents.index('# stop')
+                except:
+                    raise ValueError('missing version tag in the setup.py')
+
+                packets = ['' for _ in range(df.shape[0])]
+                for i in range(df.shape[0]):
+                    packets[i] += f"'{df.loc[df.index[i], 'original']}': ["
+
+                    _, _, _, eles = self.clean_from_python_packages(df.loc[df.index[i], "req"])
+
+                    j = 0
+                    for ele in eles:
+                        if ele != 'waste':
+                            if j == 0:
+                                packets[i] += f'{ele}'
+                            else:
+                                packets[i] += f', {ele}'
+                            j += 1
+                    packets[i] += '],'
+
+                packets = ['requires_dict = {'] + packets
+                packets = packets + ['}']
+
+                new_set_up = ['' for _ in range(start+len(contents)-stop+len(packets))]
+                new_set_up[:start+1] = contents[:start+1]
+                new_set_up[start+1:len(packets)+1] = packets
+                new_set_up[start+1+len(packets):] = contents[stop:]
+
+                with open("setup.py", "w") as f:
+                    for s in new_set_up:
+                        f.write(str(s) + "\n")
+
+                print(os.getcwd()+"\\setup.py")
+
+    def clean_from_python_packages(self, single_requirements):
+        # vengono matchate le librerie del progetto con le versioni da usare
+        requirements_versioned = []
+        requirements_variable = []
+        distribusion_not_found = []
+        variables = []
+        for req in single_requirements:
+            pass_card = True
+
+            # applicato un controllo se la libreira che si vuole inserire fa parte delle librerie private
+            # in quel caso non deve essere messa nel requirement.txt
+            for pl in self.librerie_private:
+                if req.startswith(pl):
+                    pass_card = False
+                    break
+
+            if pass_card:
+                req_list = self.replace_dict[req] if req in self.replace_dict else [req]
+                for req_i in req_list:
+                    try:
+                        version = pkg_resources.get_distribution(req_i).version
+                        requirements_versioned.append(f'{req_i}=={version}')
+                        requirements_variable.append(f"{req_i.replace('-', '_')} = '{req_i}=={version}'")
+                        variables.append(f"{req_i.replace('-', '_')}")
+                    except pkg_resources.DistributionNotFound:
+                        distribusion_not_found.append(req_i)
+        return distribusion_not_found, requirements_variable, requirements_versioned, variables
```

### Comparing `DependiPy-1.0.2/DependiPy/librarian.py` & `DependiPy-1.0.8/DependiPy/librarian.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import os
-import argparse
-from DependiPy.archive import LibMapperTools
-import json
-
-
-def main():
-
-    parser = argparse.ArgumentParser(prog='library-mapper', description="Map the requirements of a project")
-    parser.add_argument('-p', '--path',
-                        help="folder/file path, if mode lib it needs the path to the folder deeper than setup.py",
-                        required=True)
-    parser.add_argument('-m', '--mode', help="lib parser or script parser (lib,script)", required=False)
-    parser.add_argument('-c', '--config', help="config file", required=False, default='config.json')
-    parser.add_argument('-do', '--docs_only', help="generate only the documentatino", required=False, default=False)
-
-    kwargs = vars(parser.parse_args())
-
-    try:
-        with open(kwargs['config']) as json_file:
-            config = json.load(json_file)
-    except:
-        config = {}
-
-    librerie_private = config.get('private_lib', [])
-    print("privat libraries: ", librerie_private)
-    # nome delle cartelle da non considerare per la mappatura
-    exclusion = config.get('exclude_folder', [])
-    # lista di librerie aggiuntive che non si vuole inseire nei requirements se fossero presenti
-    remove = config.get('exclude_lib', [])
-    # dizionario per sostituire alcuni nomi se serve
-    replace_dict = config.get('replace_lib', {})
-
-    # percorso della libreria
-    path = kwargs['path']
-    os.chdir(path)
-    os.chdir('..')
-    # nome della cartella che contiene la libreria, rappresenta il livello 0
-    lib_name = os.path.normpath(path).split('\\')
-    if lib_name[-1] == '':
-        lib_name = lib_name[-2]
-    else:
-        lib_name = lib_name[-1]
-
-    # se trovo il file setup.py e non ho un mode dagli argomenti passati allora imposto mode come lib
-    mode = 'lib' if os.path.exists('setup.py') else 'script'
-    mode = kwargs['mode'] if kwargs['mode'] is not None else mode
-
-    lmt = LibMapperTools(lib_name=lib_name, remove=remove, replace_dict=replace_dict, exclusion=exclusion,
-                         librerie_private=librerie_private, mode=mode)
-
-    requirements_pd = lmt.read_files()
-
-    requirements_pd = lmt.add_path(requirements_pd)
-
-    # applico la funzione che estrae le cross reference e la applico alla colonna delle librerie
-    requirements_pd.loc[:, 'cross'] = requirements_pd.loc[:, 'req'].apply(lmt.cross_reference_extraction)
-
-    requirements_pd.loc[:, 'req'] = requirements_pd.loc[:, 'req'].apply(lmt.cleaning)
-
-    lmt.write_mapping(requirements_pd, **kwargs)
-
-
-if __name__ == '__main__':
-
+import os
+import argparse
+from DependiPy.archive import LibMapperTools
+import json
+
+
+def main():
+
+    parser = argparse.ArgumentParser(prog='library-mapper', description="Map the requirements of a project")
+    parser.add_argument('-p', '--path',
+                        help="folder/file path, if mode lib it needs the path to the folder deeper than setup.py",
+                        required=True)
+    parser.add_argument('-m', '--mode', help="lib parser or script parser (lib,script)", required=False)
+    parser.add_argument('-c', '--config', help="config file", required=False, default='config.json')
+    parser.add_argument('-do', '--docs_only', help="generate only the documentatino", required=False, default=False)
+
+    kwargs = vars(parser.parse_args())
+
+    try:
+        with open(kwargs['config']) as json_file:
+            config = json.load(json_file)
+    except:
+        config = {}
+
+    librerie_private = config.get('private_lib', [])
+    print("privat libraries: ", librerie_private)
+    # nome delle cartelle da non considerare per la mappatura
+    exclusion = config.get('exclude_folder', [])
+    # lista di librerie aggiuntive che non si vuole inseire nei requirements se fossero presenti
+    remove = config.get('exclude_lib', [])
+    # dizionario per sostituire alcuni nomi se serve
+    replace_dict = config.get('replace_lib', {})
+
+    # percorso della libreria
+    path = kwargs['path']
+    os.chdir(path)
+    os.chdir('..')
+    # nome della cartella che contiene la libreria, rappresenta il livello 0
+    lib_name = os.path.normpath(path).split('\\')
+    if lib_name[-1] == '':
+        lib_name = lib_name[-2]
+    else:
+        lib_name = lib_name[-1]
+
+    # se trovo il file setup.py e non ho un mode dagli argomenti passati allora imposto mode come lib
+    mode = 'lib' if os.path.exists('setup.py') else 'script'
+    mode = kwargs['mode'] if kwargs['mode'] is not None else mode
+
+    lmt = LibMapperTools(lib_name=lib_name, remove=remove, replace_dict=replace_dict, exclusion=exclusion,
+                         librerie_private=librerie_private, mode=mode)
+
+    requirements_pd = lmt.read_files()
+
+    requirements_pd = lmt.add_path(requirements_pd)
+
+    # applico la funzione che estrae le cross reference e la applico alla colonna delle librerie
+    requirements_pd.loc[:, 'cross'] = requirements_pd.loc[:, 'req'].apply(lmt.cross_reference_extraction)
+
+    requirements_pd.loc[:, 'req'] = requirements_pd.loc[:, 'req'].apply(lmt.cleaning)
+
+    lmt.write_mapping(requirements_pd, **kwargs)
+
+
+if __name__ == '__main__':
+
     main()
```

### Comparing `DependiPy-1.0.2/README.md` & `DependiPy-1.0.8/DependiPy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,295 +1,305 @@
-# DependiPy
-gli script in questa repository servono per mappare le dipendenze di una libreria in modo da poterle selezionare
-in modo modulare quando la libreria mappata viene installata, o in alternativa crea il file requirements.txt con
-le dimendenze esatte installate sul sistema da cui si sta lanciando lo script.
-
-## files
-sono presenti 2 files:
-- librarian.py, che contiene lo script main
-- archive.py, che contiene una classe usata da librarian.py
-
-## execution
-per usare le funzionalita di mapping venogno richiesti 1 parametro obligatorio e 3 opzionali:
-- obligatori
-  - **path**, percorso fino alla cartella della libreria o script
-- opzionali:
-  - **mode**, da scegliere tra 2 modalita, se non viene compilato lo script prova a capire in autonomia quale sia la modalita corretta:
-    - *lib*, se si vuole mappare le dipendenze di una libreria
-    - *script*, se si vuole mappare le dipendenze di una script con le librerie custom
-  - **config**, vuole il percorso ad un file di config con alcune info aggiuntive su enventuali modifiche dal funzionamento standard. Il config deve essere un file json.
-  - **docs_only**, se attivata questa modalita non genera i file dei requirements o setup.py ma solo i file per la documentazione
-
-Se si sta lavorando in lib la cartella indicata nel path è la cartella della libreria, non quella che contiene il setup.py ma quella un livello piu interno a setup.py.
-Se si sta lavorando in script la cartella indicata è quella che contiene lo/gli script.
-
-Librarian è in grado di mappare sia script dentro cartelle con nessun limite sui livelli di profondita.
-Libraria è in grado di mappare le cross dipendenze dentro la libreria indicata.
-
-l'esecuzione va invocata come di seguito:
-```bash
-DependiPy -p <path> -m <mode> -c <config.json>
-```
-
-Il file config deve avere la seguente struttura:
-```json
-{
-  "private_lib": ["lib1", "lib2"],
-  "replace_lib": {
-    "dateutil": ["python-dateutil"],
-    "sklearn": ["scikit-learn"],
-    "azure":
-    ["azure-common",
-      "azure-core",
-      "azure-identity",
-      "azure-mgmt-consumption",
-      "azure-mgmt-core",
-      "azure-mgmt-costmanagement"
-    ]},
-  "exclude_lib": ["tensorflow", "setuptools"],
-  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"]
-}
-```
-- **privat_lib**: sono le librerie private usate che non sono presenti su PyPi e che quindi non devono essere listate in un file di requirements, non potendo essere installate in automatico
-- **replace_lib**: sono le parole che devono essere sostituite nella ricerca delle librerie, dato che alcune librerie usano nomi diversi negli import dalle release su PyPi
-- **exclude_lib**: librerie che sono presenti nei file ma che non si vuole che vengano riportate
-- **exclude_folder**: cartelle che non devono essere considerate durante lo scan delle dipendenze
-
-**Le librerie inserite nel requirements.txt sono sempre e solo quelle che devono essere installate, per cui non verranno mai riportate le dipendenze native di Python**
-
-## lib/setup.py
-Se si sta lavorando in modalita lib, libraria produce un file alla fine della mappatura.
-Se il setup.py ha la forma seguente:
-```python
-from setuptools import find_packages, setup
-
-version = '1.0'
-
-# version go
-sqlalchemy = 'sqlalchemy'
-pyodbc = 'pyodbc'
-argparse = 'argparse'
-urllib3 = 'urllib3~=1.26.9'
-tqdm = 'tqdm~=4.64.0'
-requests = 'requests'
-pandas = 'pandas~=1.4.2'
-tabulate = 'tabulate~=0.8.9'
-# version end
-
-# start
-requires_dict = {
-'utilities': [pandas, requests, argparse, tabulate, tqdm, sqlalchemy, urllib3],
-'utilities.args': [argparse],
-'utilities.args.parser': [argparse],
-'utilities.decorators': [],
-'utilities.dictionary': [],
-'utilities.io': [pandas, requests, tabulate, tqdm, sqlalchemy, urllib3],
-'utilities.io.analytics_job_util': [pandas, requests, tabulate, tqdm, urllib3],
-'utilities.io.api': [tqdm, requests, urllib3],
-'utilities.io.database': [sqlalchemy],
-'utilities.io.exceptions.api': [],
-'utilities.io.pickle': [],
-'utilities.logs': [argparse],
-'utilities.logs.logger': [argparse],
-'utilities.notification': [requests],
-'utilities.notification.telegram': [requests],
-}
-# stop
-
-setup(
-    name='utilities',
-    version=version,
-    packages=find_packages(include=['utilities']),
-    license='',
-    author='Andrea Jacassi',
-    author_email='',
-    description='',
-    url="https://github.com/utilities.git",
-    extras_require=requires_dict,
-    install_requires=[],
-)
-```
-Sono necessarie le seguenti chiavi nel setup.py: **# start**, uno **# stop**, uno **# version go** e uno **# version end**.
-Librarian andra a scrivere la mappatura direttamente nel setup.py.
-
-## script/k8s_config.json
-Se si sta lavorando in modalita script, librarian cerchera tutte le dipendenze con le libreria custom indicate nel codice.
-Per modificare o aggiungere tali librerie fare riferimento al config con la forma:
-```json
-"private_lib": ["Tages", "utilities"]
-```
-nell'esempio qui indicato vengono cercate le dipendenze con le librerie **Tages** e **utilities**.
-
-Librarian mappera le connessioni con tali librerie e produrra un risultato sul terminale nella forma:
-```powershell
-[Tages.utilities.generic,Tages.preprocess.time_series.data_preparation,Tages.preprocess.data_preparation]
-
-[utilities.args.parser,utilities.io.analytics_job_util]
-```
-una riga per libreria indicata.
-
-Queste righe vanno copiate e incollate in fare di installazione dello script per installare le sole dipendenze delle librerie necessarie per il funzionamento dello scritp
-
-## escludere alcune librerie o cartelle specifiche
-Per escludere cartelle specifiche dalla mappatura in modalita lib è possibile aggiungere nomi di cartelle alla lista:
-```json
-"exclude_folder": ['tests', '__pycache__', 'discontinue']
-```
-Mentre se si vuole escludere alcune librerie dal mappaggio:
-```json
-"exclude_lib": ['os', 'string', 'inspect', 'logging', 'sys', 'abc', 'statistics', 'pickle', 'collections', 'functools',
-                 'json', 'itertools', 'warnings', 'typing', 'calendar', 'datetime', 'hashlib', 'time', 'random']
-```
-
-## come usare i moduli su pip
-Quando si deve pip installare una libreria per usarla in relazione ad uno script è sempre possibile indicare delle specifiche sotto
-categorie di dipendenze con i moduli di pip (se precedentemenete mappati).
-
-Un esempio di installazione di **Tages** con le dipendenze necessarie per uno specifico script al suo interno puo essere scritto come:
-```bash
-pip install -e ./AI_lib[Tages.preprocess.time_series.data_preparation]
-```
-
-La mappatura fatta permette di indicare i singoli file o cartelle, facendo cosi verranno incluse le sole dipendenze
-necessarie richieste dagli script selezionati.
-
-E' possibile concatenare piu moduli se si sta usando piu parti della libreria mappata
-```bash
-pip install -e ./utilities[utilities.args.parser,utilities.io.analytics_job_util]
-```
-
-# Documentation
-
-E' possibile generare automaticamente la documentazione del codice, assieme a documentazione scritta a mano, su un sito autogenerato da github (per le sole repository publiche).
-**Requirements_mapper** permette di generare i file che servono per autodocumentare il codice tramite la documentazione riportata nei docsting.
-
-## guida all'uso di mkdocs
-
-i passi da fare sono i seguenti:
-1. installare le seguenti librerie
-    ```bash
-    pip install mkdocs
-    pip install "mkdocstrings[python]"
-    pip install mkdocs-material
-    ```
-2. con il seguente comando vengono create le cartelle necessarie alla formazione della documentazione, lanciarlo dentro alla cartella del codice (se si tratta di una libreria, farlo allo stesso livello di setup.py)
-    ```bash
-    mkdocs new .
-    ```
-3. viene quindi creata una cartella **docs** ed un file **mkdocs.yaml**. Il file **mkdocs.yaml** deve essere composta da un testo simile al seguente:
-    ```yaml
-    site_name: titolo sito
-    site_description: description del sito
-    site_url: url di riferimento
-    
-    theme:
-      name: material
-      features:
-        - search.suggest
-        - search.highlight
-        - content.tabs.link
-        - content.tooltips
-    #    - navigation.tabs
-    #    - navigation.tabs.sticky
-        - navigation.sections
-    #    - navigation.path
-        - navigation.top
-        - navigation.expand
-        - content.code.annotate
-        - content.code.copy
-        - content.code.select
-    #    - toc.integrate
-        - toc.follow
-        - header.autohide
-    
-      language: en
-      palette:
-        - scheme: default
-          toggle:
-            icon: material/toggle-switch-off-outline
-            name: Switch to dark mode
-          primary: orange
-          accent: purple
-        - scheme: slate
-          toggle:
-            icon: material/toggle-switch
-            name: Switch to light mode
-          primary: orange
-          accent: lime
-    
-    repo_name: name repository github
-    repo_url: url repository github
-    
-    plugins:
-      - mkdocstrings
-        - search
-    
-    markdown_extensions:
-      - pymdownx.highlight:
-          anchor_linenums: true
-        - pymdownx.inlinehilite
-        - pymdownx.snippets
-        - admonition
-        - pymdownx.arithmatex:
-            generic: true
-        - footnotes
-        - pymdownx.details
-        - pymdownx.superfences
-        - pymdownx.mark
-        - attr_list
-    
-    nav:
-      - index.md
-      - Installation: installation.md
-      - User Guide: user_guide.md
-      - Developer Guide: dev_guide.md
-      - XA information: info.md
-    
-    copyright:
-      mit
-    ```
-4. nella cartella docs devono essere messi i testi che si vogliono far comparire nella documentazione online, sotto forma di file markdown
-5. nella sezione **nav** dello yaml devono essere inseriti i file aggiunti alla cartella docs
-6. a questo punto si deve lanciare **requirements_mapper**, che andra ad aggiungere file e riferimenti al codice per la documentazione
-7. per osservare il risultato in una versione demo si puo lanciare il codice
-    ```bash
-    mkdocs serve
-    ```
-8. si deve creare una cartella **.github** al cui interno va creata una cartella **workflowa**
-9. dentro a **workflows** deve essere aggiunto un file **ci.yml** il cui contenuto e' il seguente:
-    ```yaml
-    name: ci
-    on:
-      push:
-        branches:
-          - master
-          - main
-    permissions:
-      contents: write
-    jobs:
-      deploy:
-        runs-on: ubuntu-latest
-        steps:
-          - uses: actions/checkout@v3
-          - uses: actions/setup-python@v4
-            with:
-              python-version: 3.x
-          - uses: actions/cache@v2
-            with:
-              key: ${{ github.ref }}
-              path: .cache
-          - run: pip install mkdocs-material
-          - run: pip install "mkdocstrings[python]"
-          - run: pip install pillow cairosvg
-          - run: mkdocs gh-deploy --force
-    ```
-10. si pusha il primo commit
-11. si va su github sulla repo e si cerca la sezione **github pages**
-    1. si naviga in settings
-    2. si naviga in pages
-    3. si naviga in source
-       1. deploy from branch
-    4. branch
-       1. gh-pages
-       2. root/
-12. dal prossimo commit verra generata automaticamente la documentazione
-13. **nel caso venissero creati nuovi file di codice si deve sempre rilanciare requirements_mapper per generare i file con i nuovi docstring
+Metadata-Version: 2.1
+Name: DependiPy
+Version: 1.0.8
+Home-page: https://github.com/ajacassi/DependiPy.git
+Author: Andrea Jacassi
+Author-email: 
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DependiPy
+gli script in questa repository servono per mappare le dipendenze di una libreria in modo da poterle selezionare
+in modo modulare quando la libreria mappata viene installata, o in alternativa crea il file requirements.txt con
+le dimendenze esatte installate sul sistema da cui si sta lanciando lo script.
+
+## files
+sono presenti 2 files:
+- librarian.py, che contiene lo script main
+- archive.py, che contiene una classe usata da librarian.py
+
+## execution
+per usare le funzionalita di mapping venogno richiesti 1 parametro obligatorio e 3 opzionali:
+- obligatori
+  - **path**, percorso fino alla cartella della libreria o script
+- opzionali:
+  - **mode**, da scegliere tra 2 modalita, se non viene compilato lo script prova a capire in autonomia quale sia la modalita corretta:
+    - *lib*, se si vuole mappare le dipendenze di una libreria
+    - *script*, se si vuole mappare le dipendenze di una script con le librerie custom
+  - **config**, vuole il percorso ad un file di config con alcune info aggiuntive su enventuali modifiche dal funzionamento standard. Il config deve essere un file json.
+  - **docs_only**, se attivata questa modalita non genera i file dei requirements o setup.py ma solo i file per la documentazione
+
+Se si sta lavorando in lib la cartella indicata nel path è la cartella della libreria, non quella che contiene il setup.py ma quella un livello piu interno a setup.py.
+Se si sta lavorando in script la cartella indicata è quella che contiene lo/gli script.
+
+Librarian è in grado di mappare sia script dentro cartelle con nessun limite sui livelli di profondita.
+Libraria è in grado di mappare le cross dipendenze dentro la libreria indicata.
+
+l'esecuzione va invocata come di seguito:
+```bash
+DependiPy -p <path> -m <mode> -c <config.json>
+```
+
+Il file config deve avere la seguente struttura:
+```json
+{
+  "private_lib": ["lib1", "lib2"],
+  "replace_lib": {
+    "dateutil": ["python-dateutil"],
+    "sklearn": ["scikit-learn"],
+    "azure":
+    ["azure-common",
+      "azure-core",
+      "azure-identity",
+      "azure-mgmt-consumption",
+      "azure-mgmt-core",
+      "azure-mgmt-costmanagement"
+    ]},
+  "exclude_lib": ["tensorflow", "setuptools"],
+  "exclude_folder": ["tests", "__pycache__", "discontinue", "git", "idea"]
+}
+```
+- **privat_lib**: sono le librerie private usate che non sono presenti su PyPi e che quindi non devono essere listate in un file di requirements, non potendo essere installate in automatico
+- **replace_lib**: sono le parole che devono essere sostituite nella ricerca delle librerie, dato che alcune librerie usano nomi diversi negli import dalle release su PyPi
+- **exclude_lib**: librerie che sono presenti nei file ma che non si vuole che vengano riportate
+- **exclude_folder**: cartelle che non devono essere considerate durante lo scan delle dipendenze
+
+**Le librerie inserite nel requirements.txt sono sempre e solo quelle che devono essere installate, per cui non verranno mai riportate le dipendenze native di Python**
+
+## lib/setup.py
+Se si sta lavorando in modalita lib, libraria produce un file alla fine della mappatura.
+Se il setup.py ha la forma seguente:
+```python
+from setuptools import find_packages, setup
+
+version = '1.0'
+
+# version go
+sqlalchemy = 'sqlalchemy'
+pyodbc = 'pyodbc'
+argparse = 'argparse'
+urllib3 = 'urllib3~=1.26.9'
+tqdm = 'tqdm~=4.64.0'
+requests = 'requests'
+pandas = 'pandas~=1.4.2'
+tabulate = 'tabulate~=0.8.9'
+# version end
+
+# start
+requires_dict = {
+'utilities': [pandas, requests, argparse, tabulate, tqdm, sqlalchemy, urllib3],
+'utilities.args': [argparse],
+'utilities.args.parser': [argparse],
+'utilities.decorators': [],
+'utilities.dictionary': [],
+'utilities.io': [pandas, requests, tabulate, tqdm, sqlalchemy, urllib3],
+'utilities.io.analytics_job_util': [pandas, requests, tabulate, tqdm, urllib3],
+'utilities.io.api': [tqdm, requests, urllib3],
+'utilities.io.database': [sqlalchemy],
+'utilities.io.exceptions.api': [],
+'utilities.io.pickle': [],
+'utilities.logs': [argparse],
+'utilities.logs.logger': [argparse],
+'utilities.notification': [requests],
+'utilities.notification.telegram': [requests],
+}
+# stop
+
+setup(
+    name='utilities',
+    version=version,
+    packages=find_packages(include=['utilities']),
+    license='',
+    author='Andrea Jacassi',
+    author_email='',
+    description='',
+    url="https://github.com/utilities.git",
+    extras_require=requires_dict,
+    install_requires=[],
+)
+```
+Sono necessarie le seguenti chiavi nel setup.py: **# start**, uno **# stop**, uno **# version go** e uno **# version end**.
+Librarian andra a scrivere la mappatura direttamente nel setup.py.
+
+## script/k8s_config.json
+Se si sta lavorando in modalita script, librarian cerchera tutte le dipendenze con le libreria custom indicate nel codice.
+Per modificare o aggiungere tali librerie fare riferimento al config con la forma:
+```json
+"private_lib": ["Tages", "utilities"]
+```
+nell'esempio qui indicato vengono cercate le dipendenze con le librerie **Tages** e **utilities**.
+
+Librarian mappera le connessioni con tali librerie e produrra un risultato sul terminale nella forma:
+```powershell
+[Tages.utilities.generic,Tages.preprocess.time_series.data_preparation,Tages.preprocess.data_preparation]
+
+[utilities.args.parser,utilities.io.analytics_job_util]
+```
+una riga per libreria indicata.
+
+Queste righe vanno copiate e incollate in fare di installazione dello script per installare le sole dipendenze delle librerie necessarie per il funzionamento dello scritp
+
+## escludere alcune librerie o cartelle specifiche
+Per escludere cartelle specifiche dalla mappatura in modalita lib è possibile aggiungere nomi di cartelle alla lista:
+```json
+"exclude_folder": ['tests', '__pycache__', 'discontinue']
+```
+Mentre se si vuole escludere alcune librerie dal mappaggio:
+```json
+"exclude_lib": ['os', 'string', 'inspect', 'logging', 'sys', 'abc', 'statistics', 'pickle', 'collections', 'functools',
+                 'json', 'itertools', 'warnings', 'typing', 'calendar', 'datetime', 'hashlib', 'time', 'random']
+```
+
+## come usare i moduli su pip
+Quando si deve pip installare una libreria per usarla in relazione ad uno script è sempre possibile indicare delle specifiche sotto
+categorie di dipendenze con i moduli di pip (se precedentemenete mappati).
+
+Un esempio di installazione di **Tages** con le dipendenze necessarie per uno specifico script al suo interno puo essere scritto come:
+```bash
+pip install -e ./AI_lib[Tages.preprocess.time_series.data_preparation]
+```
+
+La mappatura fatta permette di indicare i singoli file o cartelle, facendo cosi verranno incluse le sole dipendenze
+necessarie richieste dagli script selezionati.
+
+E' possibile concatenare piu moduli se si sta usando piu parti della libreria mappata
+```bash
+pip install -e ./utilities[utilities.args.parser,utilities.io.analytics_job_util]
+```
+
+# Documentation
+
+E' possibile generare automaticamente la documentazione del codice, assieme a documentazione scritta a mano, su un sito autogenerato da github (per le sole repository publiche).
+**Requirements_mapper** permette di generare i file che servono per autodocumentare il codice tramite la documentazione riportata nei docsting.
+
+## guida all'uso di mkdocs
+
+i passi da fare sono i seguenti:
+1. installare le seguenti librerie
+    ```bash
+    pip install mkdocs
+    pip install "mkdocstrings[python]"
+    pip install mkdocs-material
+    ```
+2. con il seguente comando vengono create le cartelle necessarie alla formazione della documentazione, lanciarlo dentro alla cartella del codice (se si tratta di una libreria, farlo allo stesso livello di setup.py)
+    ```bash
+    mkdocs new .
+    ```
+3. viene quindi creata una cartella **docs** ed un file **mkdocs.yaml**. Il file **mkdocs.yaml** deve essere composta da un testo simile al seguente:
+    ```yaml
+    site_name: titolo sito
+    site_description: description del sito
+    site_url: url di riferimento
+    
+    theme:
+      name: material
+      features:
+        - search.suggest
+        - search.highlight
+        - content.tabs.link
+        - content.tooltips
+    #    - navigation.tabs
+    #    - navigation.tabs.sticky
+        - navigation.sections
+    #    - navigation.path
+        - navigation.top
+        - navigation.expand
+        - content.code.annotate
+        - content.code.copy
+        - content.code.select
+    #    - toc.integrate
+        - toc.follow
+        - header.autohide
+    
+      language: en
+      palette:
+        - scheme: default
+          toggle:
+            icon: material/toggle-switch-off-outline
+            name: Switch to dark mode
+          primary: orange
+          accent: purple
+        - scheme: slate
+          toggle:
+            icon: material/toggle-switch
+            name: Switch to light mode
+          primary: orange
+          accent: lime
+    
+    repo_name: name repository github
+    repo_url: url repository github
+    
+    plugins:
+      - mkdocstrings
+        - search
+    
+    markdown_extensions:
+      - pymdownx.highlight:
+          anchor_linenums: true
+        - pymdownx.inlinehilite
+        - pymdownx.snippets
+        - admonition
+        - pymdownx.arithmatex:
+            generic: true
+        - footnotes
+        - pymdownx.details
+        - pymdownx.superfences
+        - pymdownx.mark
+        - attr_list
+    
+    nav:
+      - index.md
+      - Installation: installation.md
+      - User Guide: user_guide.md
+      - Developer Guide: dev_guide.md
+      - XA information: info.md
+    
+    copyright:
+      mit
+    ```
+4. nella cartella docs devono essere messi i testi che si vogliono far comparire nella documentazione online, sotto forma di file markdown
+5. nella sezione **nav** dello yaml devono essere inseriti i file aggiunti alla cartella docs
+6. a questo punto si deve lanciare **requirements_mapper**, che andra ad aggiungere file e riferimenti al codice per la documentazione
+7. per osservare il risultato in una versione demo si puo lanciare il codice
+    ```bash
+    mkdocs serve
+    ```
+8. si deve creare una cartella **.github** al cui interno va creata una cartella **workflowa**
+9. dentro a **workflows** deve essere aggiunto un file **ci.yml** il cui contenuto e' il seguente:
+    ```yaml
+    name: ci
+    on:
+      push:
+        branches:
+          - master
+          - main
+    permissions:
+      contents: write
+    jobs:
+      deploy:
+        runs-on: ubuntu-latest
+        steps:
+          - uses: actions/checkout@v3
+          - uses: actions/setup-python@v4
+            with:
+              python-version: 3.x
+          - uses: actions/cache@v2
+            with:
+              key: ${{ github.ref }}
+              path: .cache
+          - run: pip install mkdocs-material
+          - run: pip install "mkdocstrings[python]"
+          - run: pip install pillow cairosvg
+          - run: mkdocs gh-deploy --force
+    ```
+10. si pusha il primo commit
+11. si va su github sulla repo e si cerca la sezione **github pages**
+    1. si naviga in settings
+    2. si naviga in pages
+    3. si naviga in source
+       1. deploy from branch
+    4. branch
+       1. gh-pages
+       2. root/
+12. dal prossimo commit verra generata automaticamente la documentazione
+13. **nel caso venissero creati nuovi file di codice si deve sempre rilanciare requirements_mapper per generare i file con i nuovi docstring
```

