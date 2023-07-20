# Comparing `tmp/easydock-0.2.3.tar.gz` & `tmp/easydock-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easydock-0.2.3.tar", last modified: Mon Jul  3 14:31:45 2023, max compression
+gzip compressed data, was "easydock-0.2.4.tar", last modified: Thu Jul 20 19:34:57 2023, max compression
```

## Comparing `easydock-0.2.3.tar` & `easydock-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-03 14:31:45.000000 easydock-0.2.3/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2019-11-25 13:17:56.000000 easydock-0.2.3/LICENSE.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10179 2023-07-03 14:31:45.000000 easydock-0.2.3/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-07-03 14:31:45.000000 easydock-0.2.3/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7814 2023-06-30 15:44:58.000000 easydock-0.2.3/easydock/preparation_for_docking.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    13959 2023-06-30 15:44:57.000000 easydock-0.2.3/easydock/run_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    17149 2023-07-03 06:43:04.000000 easydock-0.2.3/easydock/database.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/vina_dock_cli.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/read_input.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-07-03 14:22:44.000000 easydock-0.2.3/easydock/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5965 2023-05-30 12:11:29.000000 easydock-0.2.3/easydock/get_sdf_from_dock_db.py
--rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5288 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/vina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2713 2023-05-16 09:01:52.000000 easydock-0.2.3/easydock/gnina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       91 2023-06-30 16:25:46.000000 easydock-0.2.3/easydock/auxiliary.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7988 2023-07-03 14:29:59.000000 easydock-0.2.3/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10179 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      482 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      111 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-07-03 14:31:45.000000 easydock-0.2.3/easydock.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-05-16 09:01:52.000000 easydock-0.2.3/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-20 19:34:57.863822 easydock-0.2.4/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2019-11-25 13:17:56.000000 easydock-0.2.4/LICENSE.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8931 2023-07-20 19:34:57.863822 easydock-0.2.4/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8338 2023-07-20 19:25:49.000000 easydock-0.2.4/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-20 19:34:57.859822 easydock-0.2.4/easydock/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2023-07-20 19:26:00.000000 easydock-0.2.4/easydock/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       91 2023-06-30 16:25:46.000000 easydock-0.2.4/easydock/auxiliary.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    17214 2023-07-11 06:16:22.000000 easydock-0.2.4/easydock/database.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5965 2023-05-30 12:11:29.000000 easydock-0.2.4/easydock/get_sdf_from_dock_db.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2713 2023-05-16 09:01:52.000000 easydock-0.2.4/easydock/gnina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7814 2023-06-30 15:44:58.000000 easydock-0.2.4/easydock/preparation_for_docking.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-05-16 09:01:52.000000 easydock-0.2.4/easydock/read_input.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    14136 2023-07-20 19:21:03.000000 easydock-0.2.4/easydock/run_dock.py
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5288 2023-05-16 09:01:52.000000 easydock-0.2.4/easydock/vina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-05-16 09:01:52.000000 easydock-0.2.4/easydock/vina_dock_cli.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-07-20 19:34:57.863822 easydock-0.2.4/easydock.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8931 2023-07-20 19:34:57.000000 easydock-0.2.4/easydock.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      482 2023-07-20 19:34:57.000000 easydock-0.2.4/easydock.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-07-20 19:34:57.000000 easydock-0.2.4/easydock.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      110 2023-07-20 19:34:57.000000 easydock-0.2.4/easydock.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2023-07-20 19:34:57.000000 easydock-0.2.4/easydock.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2023-07-20 19:34:57.000000 easydock-0.2.4/easydock.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2023-07-20 19:34:57.863822 easydock-0.2.4/setup.cfg
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-05-16 09:01:52.000000 easydock-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `easydock-0.2.3/LICENSE.txt` & `easydock-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easydock-0.2.3/PKG-INFO` & `easydock-0.2.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,214 +1,223 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.2.3
+Version: 0.2.4
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
-License: UNKNOWN
-Description: # EasyDock - Python module to automate molecular docking
-        
-        ### Installation
-        
-        ```
-        pip install easydock
-        ```
-        or the latest version from github
-        ```
-        pip install git+https://github.com/ci-lab-cz/easydock.git
-        ```
-        
-        ### Dependencies
-        
-        from conda
-        ```
-        conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
-        ```
-        
-        from pypi
-        ```
-        pip install meeko
-        ```
-        
-        Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
-        
-        Installation of `gnina` is described at https://github.com/gnina/gnina
-        
-        ### Description
-        
-        Fully automatic pipeline for molecular docking.  
-        
-        Features:
-        - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
-        - can be used as a command line utility or imported as a python module
-        - supports distributed computing using `dask` library
-        - supports docking of boron-containing compounds using `vina` and `smina` (boron is replaced with carbon before docking and returned back)
-        - all outputs are stored in an SQLite database
-        - interrupted calculations can be restarted by invoking the same command or by supplying just a single argument - the existing output database
-        - `get_sdf_from_dock_db` is used to extract data from output DB
-        
-        Pipeline:
-        - input SMILES are converted in 3D by RDKit, if input is 3D structures in SDF their conformations wil be taken as starting without changes.
-        - ligands are protonated by chemaxon at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
-        - molecules are converted in PDBQT format using Meeko
-        - docking with `vina`/`gnina`
-        - output poses are converted in MOL format and stored into output DB along with docking scores
-        
-        ### Example
-        
-        ##### Docking from command line
-        
-        Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used (4 molecules will be dock in parallel). When docking will finish an SDF file will be created with top docking poses for each ligand. 
-        ```
-        run_dock -i input.smi -o output.db --program vina --config config.yml --no_protonation -c 4 --sdf
-        ``` 
-        
-        Example of config.yml for `vina` docking  
-        ```
-        protein: /path/to/protein.pdbqt
-        protein_setup: /path/to/grid.txt
-        exhaustiveness: 8
-        seed: 0
-        n_poses: 5
-        ncpu: 5
-        ```
-        
-        NOTE: ncpu argument in `run_dock` and `config.yml` has different meaning. In `run_dock` it means the number of molecules docked in parallel. In `config.yml` it means the number of CPUs used for docking of a single molecule. The product of these two values should be equal or a little bit more than the number of CPUs on a computer.
-        
-        The same but using `gnina`
-        ```
-        run_dock -i input.smi -o output.db --program gnina --config config.yml --no_protonation -c 4 --sdf
-        ``` 
-        
-        Example of config.yml for `gnina` docking  
-        ```
-        script_file: /path/to/gnina_executable
-        protein: /path/to/protein.pdbqt
-        protein_setup: /path/to/grid.txt
-        exhaustiveness: 8
-        scoring: default
-        cnn_scoring: rescore
-        cnn: dense_ensemble
-        n_poses: 10
-        addH: False
-        ncpu: 1
-        seed: 0
-        ```
-        
-        To use `smina` invoke `gnina` as shown above and make corresponding changes in config.yml
-        ```
-        script_file: /path/to/gnina_executable
-        protein: /path/to/protein.pdbqt
-        protein_setup: /path/to/grid.txt
-        exhaustiveness: 8
-        scoring: vinardo
-        cnn_scoring: None
-        cnn: dense_ensemble
-        n_poses: 10
-        addH: False
-        ncpu: 1
-        seed: 0
-        ```
-        
-        ##### Docking using multiple servers
-        
-        To distribute docking over multiple servers one have to start dask cluster and call the script
-        
-        ```bash
-        dask ssh --hostfile $PBS_NODEFILE --nworkers 15 --nthreads 1 &
-        sleep 10
-        run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf --hostfile $PBS_NODEFILE --dask_report
-        ```
-        `$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
-        
-        `--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
-        
-        `--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
-          
-        `--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).
-          
-        **Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
-        
-        ##### Data retrieval from the output database
-        
-        To extract data from the database one may use the script `get_sdf_from_dock_db`.
-        
-        Extract top poses with their scores (additional information in DB fields can be extracted only for the top poses):
-        ```
-        get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score
-        ```
-        Retrieve second poses for compounds `mol_1` and `mol_4` in SDF format:
-        ```
-        get_sdf_from_dock_db -i output.db -o output.sdf -d mol_1 mol_4 --poses 2 
-        ```
-        Instead of a list of ids a text file can be supplied as an argument `-d`.
-        
-        Retrieve top poses for compounds with docking score less then -10:
-        ```
-        get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score --add_sql 'docking_score < -10' 
-        ```
-        
-        ##### Docking from Python
-        
-        Dock a list of molecules on a local computer. Import `mol_dock` function from a corresponding submodule.
-        ```python
-        from easydock.run_dock import docking
-        from easydock.vina_dock import mol_dock
-        # from easydock.gnina_dock import mol_dock  # <- enable gnina docking
-        from rdkit import Chem
-        
-        smiles = ['CC(=O)O', 'NCC(=O)O', 'NC(C)C(=O)O']
-        mols = [Chem.MolFromSmiles(smi) for smi in smiles]
-        
-        # assign names, because this will be an identifier of docking outputs of a molecule 
-        for mol, smi in zip(mols, smiles):
-            mol.SetProp('_Name', smi)
-        
-        for mol_id, res in docking(mols, dock_func=mol_dock, dock_config='config.yml', ncpu=4):
-            print(mol_id, res)
-        ```
-        
-        ##### Customization
-        
-        To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
-        
-        ### Changelog
-        
-        **0.2.3**
-        - improve descriptions of examples on README
-        - catch all exceptions in conversion of PDBQT to Mol
-        - move DB related functions to a new database.py module
-        - use SMILES temporary file to protonate molecules with cxcalc
-        - add functions to get molecules from DB in Python (get_mols, select_from_db)
-        
-        **0.2.2**
-        - fix bug with continuation of calculations after db was transferred to other machine
-        - restrict precedence of command line arguments over arguments restored from DB only to specific ones (output, hostfile, dask_report, ncpu, verbose)
-        
-        **0.2.1**
-        - fix treatment of molecule ids in get_sdf_from_dock_db
-        - change installation instructions, vina must be installed from sources
-        - add argument no_tautomerization to disable tautomerization during protonation
-        - (critical) fix conversion of PDBQT to Mol which could not assign bond orders and returned molecules with only single bonds 
-        
-        **0.2.0**
-        - the stable version with multiple fixes and updates
-        - dask library was fully integrated and tested
-        - API was redesigned
-        - docking of boron-containing compounds was implemented (Vina, smina)
-        - a function to predict docking runtime was introduced   
-        
-        **0.1.2**
-        - (bugfix) docking of macrocycles is rigid (in future may be changed)
-        
-        ### Licence
-        BSD-3
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: rdkit
+License-File: LICENSE.txt
+
+# EasyDock - Python module to automate molecular docking
+
+### Installation
+
+```
+pip install easydock
+```
+or the latest version from github
+```
+pip install git+https://github.com/ci-lab-cz/easydock.git
+```
+
+### Dependencies
+
+from conda
+```
+conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
+```
+
+from pypi
+```
+pip install meeko
+```
+
+to use multiple servers for docking install `paramiko` (backend of `dask` if launched from the command line)
+```
+pip install paramiko
+```
+
+Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
+
+Installation of `gnina` is described at https://github.com/gnina/gnina
+
+### Description
+
+Fully automatic pipeline for molecular docking.  
+
+Features:
+- the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
+- can be used as a command line utility or imported as a python module
+- supports distributed computing using `dask` library
+- supports docking of boron-containing compounds using `vina` and `smina` (boron is replaced with carbon before docking and returned back)
+- all outputs are stored in an SQLite database
+- interrupted calculations can be restarted by invoking the same command or by supplying just a single argument - the existing output database
+- `get_sdf_from_dock_db` is used to extract data from output DB
+
+Pipeline:
+- input SMILES are converted in 3D by RDKit, if input is 3D structures in SDF their conformations wil be taken as starting without changes.
+- ligands are protonated by chemaxon at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
+- molecules are converted in PDBQT format using Meeko
+- docking with `vina`/`gnina`
+- output poses are converted in MOL format and stored into output DB along with docking scores
+
+### Example
+
+##### Docking from command line
+
+Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used (4 molecules will be dock in parallel). When docking will finish an SDF file will be created with top docking poses for each ligand. 
+```
+run_dock -i input.smi -o output.db --program vina --config config.yml --no_protonation -c 4 --sdf
+``` 
+
+Example of config.yml for `vina` docking  
+```
+protein: /path/to/protein.pdbqt
+protein_setup: /path/to/grid.txt
+exhaustiveness: 8
+seed: 0
+n_poses: 5
+ncpu: 5
+```
+
+NOTE: ncpu argument in `run_dock` and `config.yml` has different meaning. In `run_dock` it means the number of molecules docked in parallel. In `config.yml` it means the number of CPUs used for docking of a single molecule. The product of these two values should be equal or a little bit more than the number of CPUs on a computer.
+
+The same but using `gnina`
+```
+run_dock -i input.smi -o output.db --program gnina --config config.yml --no_protonation -c 4 --sdf
+``` 
+
+Example of config.yml for `gnina` docking  
+```
+script_file: /path/to/gnina_executable
+protein: /path/to/protein.pdbqt
+protein_setup: /path/to/grid.txt
+exhaustiveness: 8
+scoring: default
+cnn_scoring: rescore
+cnn: dense_ensemble
+n_poses: 10
+addH: False
+ncpu: 1
+seed: 0
+```
+
+To use `smina` invoke `gnina` as shown above and make corresponding changes in config.yml
+```
+script_file: /path/to/gnina_executable
+protein: /path/to/protein.pdbqt
+protein_setup: /path/to/grid.txt
+exhaustiveness: 8
+scoring: vinardo
+cnn_scoring: None
+cnn: dense_ensemble
+n_poses: 10
+addH: False
+ncpu: 1
+seed: 0
+```
+
+##### Docking using multiple servers
+
+To distribute docking over multiple servers one have to start dask cluster and call the script
+
+```bash
+dask ssh --hostfile $PBS_NODEFILE --nworkers 15 --nthreads 1 &
+sleep 10
+run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf --hostfile $PBS_NODEFILE --dask_report
+```
+`$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
+
+`--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
+
+`--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
+  
+`--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).  
+  
+**Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
+
+##### Data retrieval from the output database
+
+To extract data from the database one may use the script `get_sdf_from_dock_db`.
+
+Extract top poses with their scores (additional information in DB fields can be extracted only for the top poses):
+```
+get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score
+```
+Retrieve second poses for compounds `mol_1` and `mol_4` in SDF format:
+```
+get_sdf_from_dock_db -i output.db -o output.sdf -d mol_1 mol_4 --poses 2 
+```
+Instead of a list of ids a text file can be supplied as an argument `-d`.
+
+Retrieve top poses for compounds with docking score less then -10:
+```
+get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score --add_sql 'docking_score < -10' 
+```
+
+##### Docking from Python
+
+Dock a list of molecules on a local computer. Import `mol_dock` function from a corresponding submodule.
+```python
+from easydock.run_dock import docking
+from easydock.vina_dock import mol_dock
+# from easydock.gnina_dock import mol_dock  # <- enable gnina docking
+from rdkit import Chem
+
+smiles = ['CC(=O)O', 'NCC(=O)O', 'NC(C)C(=O)O']
+mols = [Chem.MolFromSmiles(smi) for smi in smiles]
+
+# assign names, because this will be an identifier of docking outputs of a molecule 
+for mol, smi in zip(mols, smiles):
+    mol.SetProp('_Name', smi)
+
+for mol_id, res in docking(mols, dock_func=mol_dock, dock_config='config.yml', ncpu=4):
+    print(mol_id, res)
+```
+
+##### Customization
+
+To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
+
+### Changelog
+
+**0.2.4**
+- close pool explicitly to solve issue with multiprocessing
+- replace subprocess calls with run
+- explicitly set types of command line arguments which a file paths (solve issue with relative paths)
+
+**0.2.3**
+- improve descriptions of examples on README
+- catch all exceptions in conversion of PDBQT to Mol
+- move DB related functions to a new database.py module
+- use SMILES temporary file to protonate molecules with cxcalc
+- add functions to get molecules from DB in Python (get_mols, select_from_db)
+
+**0.2.2**
+- fix bug with continuation of calculations after db was transferred to other machine
+- restrict precedence of command line arguments over arguments restored from DB only to specific ones (output, hostfile, dask_report, ncpu, verbose)
+
+**0.2.1**
+- fix treatment of molecule ids in get_sdf_from_dock_db
+- change installation instructions, vina must be installed from sources
+- add argument no_tautomerization to disable tautomerization during protonation
+- (critical) fix conversion of PDBQT to Mol which could not assign bond orders and returned molecules with only single bonds 
+
+**0.2.0**
+- the stable version with multiple fixes and updates
+- dask library was fully integrated and tested
+- API was redesigned
+- docking of boron-containing compounds was implemented (Vina, smina)
+- a function to predict docking runtime was introduced   
+
+**0.1.2**
+- (bugfix) docking of macrocycles is rigid (in future may be changed)
+
+### Licence
+BSD-3
```

### Comparing `easydock-0.2.3/easydock/preparation_for_docking.py` & `easydock-0.2.4/easydock/preparation_for_docking.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.3/easydock/run_dock.py` & `easydock-0.2.4/easydock/run_dock.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,31 +66,67 @@
                 try:
                     mol = next(mols)
                     new_future = dask_client.submit(dock_func, mol, priority=priority_func(mol), config=dock_config)
                     seq.add(new_future)
                 except StopIteration:
                     continue
     else:
-        with Pool(ncpu) as pool:
+        pool = Pool(ncpu)
+        try:
             for mol_id, res in pool.imap_unordered(partial(dock_func, config=dock_config), tuple(mols), chunksize=1):
                 yield mol_id, res
+        finally:
+            pool.close()
+            pool.join()
+
+
+def create_dask_client(hostfile):
+    Chem.SetDefaultPickleProperties(Chem.PropertyPickleOptions.AllProps)
+    if hostfile is not None:
+        from dask.distributed import Client
+        # import dask
+        # dask.config.set({'distributed.client.heartbeat': '20s'})
+        # dask.config.set({'distributed.client.scheduler-info-interval': '10s'})
+        # dask.config.set({'distributed.scheduler.allowed-failures': 30})
+        # dask.config.set({'distributed.scheduler.work-stealing-interval': '1minutes'})
+        # dask.config.set({'distributed.scheduler.worker-ttl': None})
+        # dask.config.set({'distributed.scheduler.unknown-task-duration': '1h'})
+        # dask.config.set({'distributed.scheduler.work-stealing': False})
+        # dask.config.set({'distributed.scheduler.unknown-task-duration': '5minutes'})
+        # dask.config.set({'distributed.worker.lifetime.restart': True})
+        # dask.config.set({'distributed.worker.profile.interval': '500ms'})
+        # dask.config.set({'distributed.worker.profile.cycle': '5s'})
+        # dask.config.set({'distributed.worker.memory.monitor-interval': '1s'})
+        # dask.config.set({'distributed.comm.timeouts.connect': '30minutes'})
+        # dask.config.set({'distributed.comm.timeouts.tcp': '30minutes'})
+        # dask.config.set({'distributed.comm.retry.count': 20})
+        # dask.config.set({'distributed.admin.tick.limit': '3h'})
+        # dask.config.set({'distributed.admin.tick.interval': '500ms'})
+        # dask.config.set({'distributed.deploy.lost-worker-timeout': '30minutes'})
+        with open(hostfile) as f:
+            hosts = [line.strip() for line in f]
+        dask_client = Client(hosts[0] + ':8786', connection_limit=2048)
+        # dask_client = Client()   # to test dask locally
+    else:
+        dask_client = None
+    return dask_client
 
 
 def main():
     parser = argparse.ArgumentParser(description='Perform docking of input molecules using Vina 1.2 or Gnina. '
                                                  'The script automates the whole pipeline: protonates molecules, '
                                                  'creates 3D structures, converts to PDBQT format, run docking using '
                                                  'a single machine (multiprocessing) or a cluster of servers (dask), '
                                                  'stores the best scores and poses in PDBQT and MOL formats to DB.\n'
                                                  'To run on a single machine:\n'
-                                                 '  run_dock.py -i input.smi -o output.db --program vina --config config.yml -c 4 -v\n\n'
+                                                 '  run_dock -i input.smi -o output.db --program vina --config config.yml -c 4 -v\n\n'
                                                  'To run on several machines using dask ssh-cluster (on PBS system):\n'
                                                  '  dask ssh --hostfile $PBS_NODEFILE --nprocs 8 --nthreads 5 &\n'
                                                  '  sleep 10\n'
-                                                 '  run_dock.py -i input.smi -o output.db --program vina --config config.yml -hostfile $PBS_NODEFILE\n\n'
+                                                 '  run_dock -i input.smi -o output.db --program vina --config config.yml -hostfile $PBS_NODEFILE\n\n'
                                                  '  $PBS_NODEFILE contains the list of addresses of computational nodes\n'
                                                  'To continue interrupted calculations it is enough to run the script '
                                                  'with just the output argument, all other arguments and data is '
                                                  'stored in DB. If you supply other arguments in a command line they '
                                                  'will be ignored with the exception of hostfile, dask_report, ncpu '
                                                  'and verbose.',
                                      formatter_class=RawTextArgumentDefaultsHelpFormatter)
@@ -100,15 +136,15 @@
                              'point.')
     parser.add_argument('-o', '--output', metavar='FILENAME', required=True, type=filepath_type,
                         help='output SQLite DB with scores and poses in PDBQT and MOL formats. It also stores '
                              'other information (input structures, protein pdbqt file and grid box config). '
                              'If output DB exists all other inputs will be ignored and calculations will be continued.')
     parser.add_argument('--program', metavar='STRING', required=False, choices=['vina', 'gnina'],
                         help='name of a docking program. Choices: vina, gnina')
-    parser.add_argument('--config', metavar='FILENAME', required=False,
+    parser.add_argument('--config', metavar='FILENAME', required=False, type=filepath_type,
                         help='YAML file with parameters used by docking program.\n'
                              'vina.yml\n'
                              'protein: path to pdbqt file with a protein\n'
                              'protein_setup: path to a text file with coordinates of a binding site\n'
                              'exhaustiveness: 8\n'
                              'n_poses: 10\n'
                              'seed: -1\n'
@@ -121,15 +157,15 @@
     parser.add_argument('--sdf', action='store_true', default=False,
                         help='save best docked poses to SDF file with the same name as output DB.')
     parser.add_argument('--hostfile', metavar='FILENAME', required=False, type=filepath_type, default=None,
                         help='text file with addresses of nodes of dask SSH cluster. The most typical, it can be '
                              'passed as $PBS_NODEFILE variable from inside a PBS script. The first line in this file '
                              'will be the address of the scheduler running on the standard port 8786. If omitted, '
                              'calculations will run on a single machine as usual.')
-    parser.add_argument('--dask_report', action='store_true', default=False,
+    parser.add_argument('--dask_report', action='store_true', default=False, type=filepath_type,
                         help='save Dask report to HTML file. It will have the same name as the output database.')
     # parser.add_argument('--tmpdir', metavar='DIRNAME', required=False, type=filepath_type, default=None,
     #                     help='path to a dir where to store temporary files accessible to a program. '
     #                          'Normally should be used,')
     parser.add_argument('--prefix', metavar='STRING', required=False, type=str, default=None,
                         help='prefix which will be added to all molecule names. This might be useful if multiple '
                              'repeated runs are made which will be analyzed together.')
@@ -160,42 +196,15 @@
             args_dict, tmpfiles = restore_setup_from_db(args.output)
             # this will ignore stored values of those args which were supplied via command line
             # command line args have precedence over stored ones
             for arg in supplied_args:
                 del args_dict[arg]
             args.__dict__.update(args_dict)
 
-        if args.hostfile is not None:
-            import dask
-            from dask.distributed import Client
-            # dask.config.set({'distributed.client.heartbeat': '20s'})
-            # dask.config.set({'distributed.client.scheduler-info-interval': '10s'})
-            # dask.config.set({'distributed.scheduler.allowed-failures': 30})
-            # dask.config.set({'distributed.scheduler.work-stealing-interval': '1minutes'})
-            # dask.config.set({'distributed.scheduler.worker-ttl': None})
-            # dask.config.set({'distributed.scheduler.unknown-task-duration': '1h'})
-            # dask.config.set({'distributed.scheduler.work-stealing': False})
-            # dask.config.set({'distributed.scheduler.unknown-task-duration': '5minutes'})
-            # dask.config.set({'distributed.worker.lifetime.restart': True})
-            # dask.config.set({'distributed.worker.profile.interval': '500ms'})
-            # dask.config.set({'distributed.worker.profile.cycle': '5s'})
-            # dask.config.set({'distributed.worker.memory.monitor-interval': '1s'})
-            # dask.config.set({'distributed.comm.timeouts.connect': '30minutes'})
-            # dask.config.set({'distributed.comm.timeouts.tcp': '30minutes'})
-            # dask.config.set({'distributed.comm.retry.count': 20})
-            # dask.config.set({'distributed.admin.tick.limit': '3h'})
-            # dask.config.set({'distributed.admin.tick.interval': '500ms'})
-            # dask.config.set({'distributed.deploy.lost-worker-timeout': '30minutes'})
-
-            with open(args.hostfile) as f:
-                hosts = [line.strip() for line in f]
-            dask_client = Client(hosts[0] + ':8786', connection_limit=2048)
-            # dask_client = Client()   # to test dask locally
-        else:
-            dask_client = None
+        dask_client = create_dask_client(args.hostfile)
 
         if not args.no_protonation:
             add_protonation(args.output, not args.no_tautomerization)
 
         if args.program == 'vina':
             from easydock.vina_dock import mol_dock, pred_dock_time
         elif args.program == 'gnina':
```

### Comparing `easydock-0.2.3/easydock/database.py` & `easydock-0.2.4/easydock/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,17 +302,18 @@
         output_data_mol = []
         with tempfile.NamedTemporaryFile(suffix='.smi', mode='w', encoding='utf-8') as tmp:
             fd, output = tempfile.mkstemp()  # use output file to avoid overflow of stdout in extreme cases
             try:
                 for smi, _, mol_id in data_list:
                     tmp.write(f'{smi}\t{mol_id}\n')
                 tmp.flush()
-                cmd_run = f"cxcalc -S --ignore-error majormicrospecies -H 7.4 " \
-                          f"{'-M' if tautomerize else ''} -K '{tmp.name}' > '{output}'"
-                subprocess.call(cmd_run, shell=True)
+                cmd_run = ['cxcalc', '-S', '--ignore-error', 'majormicrospecies', '-H', '7.4', '-K',
+                           f'{"-M" if tautomerize else ""}', tmp.name]
+                with open(output, 'w') as file:
+                    subprocess.run(cmd_run, stdout=file, text=True)
                 for mol in Chem.SDMolSupplier(output, sanitize=False):
                     if mol:
                         mol_name = mol.GetProp('_Name')
                         smi = mol.GetPropsAsDict().get('MAJORMS', None)
                         if smi is not None:
                             try:
                                 cansmi = Chem.CanonSmiles(smi)
```

### Comparing `easydock-0.2.3/easydock/vina_dock_cli.py` & `easydock-0.2.4/easydock/vina_dock_cli.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.3/easydock/read_input.py` & `easydock-0.2.4/easydock/read_input.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.3/easydock/get_sdf_from_dock_db.py` & `easydock-0.2.4/easydock/get_sdf_from_dock_db.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.3/easydock/vina_dock.py` & `easydock-0.2.4/easydock/vina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.3/easydock/gnina_dock.py` & `easydock-0.2.4/easydock/gnina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.2.3/README.md` & `easydock-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 ```
 
 from pypi
 ```
 pip install meeko
 ```
 
+to use multiple servers for docking install `paramiko` (backend of `dask` if launched from the command line)
+```
+pip install paramiko
+```
+
 Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
 
 Installation of `gnina` is described at https://github.com/gnina/gnina
 
 ### Description
 
 Fully automatic pipeline for molecular docking.  
@@ -113,15 +118,15 @@
 ```
 `$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
 
 `--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
 
 `--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
   
-`--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).
+`--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).  
   
 **Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
 
 ##### Data retrieval from the output database
 
 To extract data from the database one may use the script `get_sdf_from_dock_db`.
 
@@ -162,14 +167,19 @@
 
 ##### Customization
 
 To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
 
 ### Changelog
 
+**0.2.4**
+- close pool explicitly to solve issue with multiprocessing
+- replace subprocess calls with run
+- explicitly set types of command line arguments which a file paths (solve issue with relative paths)
+
 **0.2.3**
 - improve descriptions of examples on README
 - catch all exceptions in conversion of PDBQT to Mol
 - move DB related functions to a new database.py module
 - use SMILES temporary file to protonate molecules with cxcalc
 - add functions to get molecules from DB in Python (get_mols, select_from_db)
```

### Comparing `easydock-0.2.3/easydock.egg-info/PKG-INFO` & `easydock-0.2.4/easydock.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,214 +1,223 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.2.3
+Version: 0.2.4
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
-License: UNKNOWN
-Description: # EasyDock - Python module to automate molecular docking
-        
-        ### Installation
-        
-        ```
-        pip install easydock
-        ```
-        or the latest version from github
-        ```
-        pip install git+https://github.com/ci-lab-cz/easydock.git
-        ```
-        
-        ### Dependencies
-        
-        from conda
-        ```
-        conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
-        ```
-        
-        from pypi
-        ```
-        pip install meeko
-        ```
-        
-        Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
-        
-        Installation of `gnina` is described at https://github.com/gnina/gnina
-        
-        ### Description
-        
-        Fully automatic pipeline for molecular docking.  
-        
-        Features:
-        - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
-        - can be used as a command line utility or imported as a python module
-        - supports distributed computing using `dask` library
-        - supports docking of boron-containing compounds using `vina` and `smina` (boron is replaced with carbon before docking and returned back)
-        - all outputs are stored in an SQLite database
-        - interrupted calculations can be restarted by invoking the same command or by supplying just a single argument - the existing output database
-        - `get_sdf_from_dock_db` is used to extract data from output DB
-        
-        Pipeline:
-        - input SMILES are converted in 3D by RDKit, if input is 3D structures in SDF their conformations wil be taken as starting without changes.
-        - ligands are protonated by chemaxon at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
-        - molecules are converted in PDBQT format using Meeko
-        - docking with `vina`/`gnina`
-        - output poses are converted in MOL format and stored into output DB along with docking scores
-        
-        ### Example
-        
-        ##### Docking from command line
-        
-        Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used (4 molecules will be dock in parallel). When docking will finish an SDF file will be created with top docking poses for each ligand. 
-        ```
-        run_dock -i input.smi -o output.db --program vina --config config.yml --no_protonation -c 4 --sdf
-        ``` 
-        
-        Example of config.yml for `vina` docking  
-        ```
-        protein: /path/to/protein.pdbqt
-        protein_setup: /path/to/grid.txt
-        exhaustiveness: 8
-        seed: 0
-        n_poses: 5
-        ncpu: 5
-        ```
-        
-        NOTE: ncpu argument in `run_dock` and `config.yml` has different meaning. In `run_dock` it means the number of molecules docked in parallel. In `config.yml` it means the number of CPUs used for docking of a single molecule. The product of these two values should be equal or a little bit more than the number of CPUs on a computer.
-        
-        The same but using `gnina`
-        ```
-        run_dock -i input.smi -o output.db --program gnina --config config.yml --no_protonation -c 4 --sdf
-        ``` 
-        
-        Example of config.yml for `gnina` docking  
-        ```
-        script_file: /path/to/gnina_executable
-        protein: /path/to/protein.pdbqt
-        protein_setup: /path/to/grid.txt
-        exhaustiveness: 8
-        scoring: default
-        cnn_scoring: rescore
-        cnn: dense_ensemble
-        n_poses: 10
-        addH: False
-        ncpu: 1
-        seed: 0
-        ```
-        
-        To use `smina` invoke `gnina` as shown above and make corresponding changes in config.yml
-        ```
-        script_file: /path/to/gnina_executable
-        protein: /path/to/protein.pdbqt
-        protein_setup: /path/to/grid.txt
-        exhaustiveness: 8
-        scoring: vinardo
-        cnn_scoring: None
-        cnn: dense_ensemble
-        n_poses: 10
-        addH: False
-        ncpu: 1
-        seed: 0
-        ```
-        
-        ##### Docking using multiple servers
-        
-        To distribute docking over multiple servers one have to start dask cluster and call the script
-        
-        ```bash
-        dask ssh --hostfile $PBS_NODEFILE --nworkers 15 --nthreads 1 &
-        sleep 10
-        run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf --hostfile $PBS_NODEFILE --dask_report
-        ```
-        `$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
-        
-        `--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
-        
-        `--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
-          
-        `--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).
-          
-        **Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
-        
-        ##### Data retrieval from the output database
-        
-        To extract data from the database one may use the script `get_sdf_from_dock_db`.
-        
-        Extract top poses with their scores (additional information in DB fields can be extracted only for the top poses):
-        ```
-        get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score
-        ```
-        Retrieve second poses for compounds `mol_1` and `mol_4` in SDF format:
-        ```
-        get_sdf_from_dock_db -i output.db -o output.sdf -d mol_1 mol_4 --poses 2 
-        ```
-        Instead of a list of ids a text file can be supplied as an argument `-d`.
-        
-        Retrieve top poses for compounds with docking score less then -10:
-        ```
-        get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score --add_sql 'docking_score < -10' 
-        ```
-        
-        ##### Docking from Python
-        
-        Dock a list of molecules on a local computer. Import `mol_dock` function from a corresponding submodule.
-        ```python
-        from easydock.run_dock import docking
-        from easydock.vina_dock import mol_dock
-        # from easydock.gnina_dock import mol_dock  # <- enable gnina docking
-        from rdkit import Chem
-        
-        smiles = ['CC(=O)O', 'NCC(=O)O', 'NC(C)C(=O)O']
-        mols = [Chem.MolFromSmiles(smi) for smi in smiles]
-        
-        # assign names, because this will be an identifier of docking outputs of a molecule 
-        for mol, smi in zip(mols, smiles):
-            mol.SetProp('_Name', smi)
-        
-        for mol_id, res in docking(mols, dock_func=mol_dock, dock_config='config.yml', ncpu=4):
-            print(mol_id, res)
-        ```
-        
-        ##### Customization
-        
-        To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
-        
-        ### Changelog
-        
-        **0.2.3**
-        - improve descriptions of examples on README
-        - catch all exceptions in conversion of PDBQT to Mol
-        - move DB related functions to a new database.py module
-        - use SMILES temporary file to protonate molecules with cxcalc
-        - add functions to get molecules from DB in Python (get_mols, select_from_db)
-        
-        **0.2.2**
-        - fix bug with continuation of calculations after db was transferred to other machine
-        - restrict precedence of command line arguments over arguments restored from DB only to specific ones (output, hostfile, dask_report, ncpu, verbose)
-        
-        **0.2.1**
-        - fix treatment of molecule ids in get_sdf_from_dock_db
-        - change installation instructions, vina must be installed from sources
-        - add argument no_tautomerization to disable tautomerization during protonation
-        - (critical) fix conversion of PDBQT to Mol which could not assign bond orders and returned molecules with only single bonds 
-        
-        **0.2.0**
-        - the stable version with multiple fixes and updates
-        - dask library was fully integrated and tested
-        - API was redesigned
-        - docking of boron-containing compounds was implemented (Vina, smina)
-        - a function to predict docking runtime was introduced   
-        
-        **0.1.2**
-        - (bugfix) docking of macrocycles is rigid (in future may be changed)
-        
-        ### Licence
-        BSD-3
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: rdkit
+License-File: LICENSE.txt
+
+# EasyDock - Python module to automate molecular docking
+
+### Installation
+
+```
+pip install easydock
+```
+or the latest version from github
+```
+pip install git+https://github.com/ci-lab-cz/easydock.git
+```
+
+### Dependencies
+
+from conda
+```
+conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
+```
+
+from pypi
+```
+pip install meeko
+```
+
+to use multiple servers for docking install `paramiko` (backend of `dask` if launched from the command line)
+```
+pip install paramiko
+```
+
+Installation of `vina`. There is a strict recommendation to install `vina` from sources https://github.com/ccsb-scripps/AutoDock-Vina, because version 1.2.3 (available from pip) contains a bug which result in very unstable docking scores. The fix will be included in later releases.
+
+Installation of `gnina` is described at https://github.com/gnina/gnina
+
+### Description
+
+Fully automatic pipeline for molecular docking.  
+
+Features:
+- the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
+- can be used as a command line utility or imported as a python module
+- supports distributed computing using `dask` library
+- supports docking of boron-containing compounds using `vina` and `smina` (boron is replaced with carbon before docking and returned back)
+- all outputs are stored in an SQLite database
+- interrupted calculations can be restarted by invoking the same command or by supplying just a single argument - the existing output database
+- `get_sdf_from_dock_db` is used to extract data from output DB
+
+Pipeline:
+- input SMILES are converted in 3D by RDKit, if input is 3D structures in SDF their conformations wil be taken as starting without changes.
+- ligands are protonated by chemaxon at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
+- molecules are converted in PDBQT format using Meeko
+- docking with `vina`/`gnina`
+- output poses are converted in MOL format and stored into output DB along with docking scores
+
+### Example
+
+##### Docking from command line
+
+Docking using `vina` takes input SMILES and a config file. Ligands will not be protonated with Chemaxon, so their supplied charged states will be used. 4 CPU cores will be used (4 molecules will be dock in parallel). When docking will finish an SDF file will be created with top docking poses for each ligand. 
+```
+run_dock -i input.smi -o output.db --program vina --config config.yml --no_protonation -c 4 --sdf
+``` 
+
+Example of config.yml for `vina` docking  
+```
+protein: /path/to/protein.pdbqt
+protein_setup: /path/to/grid.txt
+exhaustiveness: 8
+seed: 0
+n_poses: 5
+ncpu: 5
+```
+
+NOTE: ncpu argument in `run_dock` and `config.yml` has different meaning. In `run_dock` it means the number of molecules docked in parallel. In `config.yml` it means the number of CPUs used for docking of a single molecule. The product of these two values should be equal or a little bit more than the number of CPUs on a computer.
+
+The same but using `gnina`
+```
+run_dock -i input.smi -o output.db --program gnina --config config.yml --no_protonation -c 4 --sdf
+``` 
+
+Example of config.yml for `gnina` docking  
+```
+script_file: /path/to/gnina_executable
+protein: /path/to/protein.pdbqt
+protein_setup: /path/to/grid.txt
+exhaustiveness: 8
+scoring: default
+cnn_scoring: rescore
+cnn: dense_ensemble
+n_poses: 10
+addH: False
+ncpu: 1
+seed: 0
+```
+
+To use `smina` invoke `gnina` as shown above and make corresponding changes in config.yml
+```
+script_file: /path/to/gnina_executable
+protein: /path/to/protein.pdbqt
+protein_setup: /path/to/grid.txt
+exhaustiveness: 8
+scoring: vinardo
+cnn_scoring: None
+cnn: dense_ensemble
+n_poses: 10
+addH: False
+ncpu: 1
+seed: 0
+```
+
+##### Docking using multiple servers
+
+To distribute docking over multiple servers one have to start dask cluster and call the script
+
+```bash
+dask ssh --hostfile $PBS_NODEFILE --nworkers 15 --nthreads 1 &
+sleep 10
+run_dock -i input.smi -o output.db --program vina -c config.yml --no_protonation -c 4 --sdf --hostfile $PBS_NODEFILE --dask_report
+```
+`$PBS_NODEFILE` is a file containing list of IP addresses of servers. The first one from the list will be used by a dask scheduler, but it will also participate in computations.
+
+`--nworkers` is the number of workers per host. This is the number of molecules which are docked in parallel on a single host.
+
+`--nthreads` can be any value. The number of CPUs used for docking of a single molecule will be taken from `config.yml`.
+  
+`--dask_report` argument will create at the end of calculations an html-file with performance report (may be useful to tweak docking parameters).  
+  
+**Important setup issue** - the limit of open files on every server should be increased to the level at least twice the total number of requested workers (file streams are used for inter-node communication by dask).
+
+##### Data retrieval from the output database
+
+To extract data from the database one may use the script `get_sdf_from_dock_db`.
+
+Extract top poses with their scores (additional information in DB fields can be extracted only for the top poses):
+```
+get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score
+```
+Retrieve second poses for compounds `mol_1` and `mol_4` in SDF format:
+```
+get_sdf_from_dock_db -i output.db -o output.sdf -d mol_1 mol_4 --poses 2 
+```
+Instead of a list of ids a text file can be supplied as an argument `-d`.
+
+Retrieve top poses for compounds with docking score less then -10:
+```
+get_sdf_from_dock_db -i output.db -o output.sdf --fields docking_score --add_sql 'docking_score < -10' 
+```
+
+##### Docking from Python
+
+Dock a list of molecules on a local computer. Import `mol_dock` function from a corresponding submodule.
+```python
+from easydock.run_dock import docking
+from easydock.vina_dock import mol_dock
+# from easydock.gnina_dock import mol_dock  # <- enable gnina docking
+from rdkit import Chem
+
+smiles = ['CC(=O)O', 'NCC(=O)O', 'NC(C)C(=O)O']
+mols = [Chem.MolFromSmiles(smi) for smi in smiles]
+
+# assign names, because this will be an identifier of docking outputs of a molecule 
+for mol, smi in zip(mols, smiles):
+    mol.SetProp('_Name', smi)
+
+for mol_id, res in docking(mols, dock_func=mol_dock, dock_config='config.yml', ncpu=4):
+    print(mol_id, res)
+```
+
+##### Customization
+
+To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and an yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
+
+### Changelog
+
+**0.2.4**
+- close pool explicitly to solve issue with multiprocessing
+- replace subprocess calls with run
+- explicitly set types of command line arguments which a file paths (solve issue with relative paths)
+
+**0.2.3**
+- improve descriptions of examples on README
+- catch all exceptions in conversion of PDBQT to Mol
+- move DB related functions to a new database.py module
+- use SMILES temporary file to protonate molecules with cxcalc
+- add functions to get molecules from DB in Python (get_mols, select_from_db)
+
+**0.2.2**
+- fix bug with continuation of calculations after db was transferred to other machine
+- restrict precedence of command line arguments over arguments restored from DB only to specific ones (output, hostfile, dask_report, ncpu, verbose)
+
+**0.2.1**
+- fix treatment of molecule ids in get_sdf_from_dock_db
+- change installation instructions, vina must be installed from sources
+- add argument no_tautomerization to disable tautomerization during protonation
+- (critical) fix conversion of PDBQT to Mol which could not assign bond orders and returned molecules with only single bonds 
+
+**0.2.0**
+- the stable version with multiple fixes and updates
+- dask library was fully integrated and tested
+- API was redesigned
+- docking of boron-containing compounds was implemented (Vina, smina)
+- a function to predict docking runtime was introduced   
+
+**0.1.2**
+- (bugfix) docking of macrocycles is rigid (in future may be changed)
+
+### Licence
+BSD-3
```

### Comparing `easydock-0.2.3/setup.py` & `easydock-0.2.4/setup.py`

 * *Files identical despite different names*

