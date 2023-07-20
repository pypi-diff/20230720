# Comparing `tmp/nanoCEM-0.0.2.2.tar.gz` & `tmp/nanoCEM-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.2.2.tar", last modified: Sat Jul 15 03:22:23 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.2.3.tar", last modified: Thu Jul 20 08:06:12 2023, max compression
```

## Comparing `nanoCEM-0.0.2.2.tar` & `nanoCEM-0.0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.2/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10150 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9567 2023-07-14 09:50:15.000000 nanoCEM-0.0.2.2/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9760 2023-07-15 03:18:59.000000 nanoCEM-0.0.2.2/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.2/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.2/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8163 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.2/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.2/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.2/nanoCEM/extract_sub_fastq_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.2/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.2/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.2/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.2/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10150 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      467 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-15 03:22:23.000000 nanoCEM-0.0.2.2/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-15 03:22:23.214313 nanoCEM-0.0.2.2/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1201 2023-07-15 03:21:32.000000 nanoCEM-0.0.2.2/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-20 08:06:12.052271 nanoCEM-0.0.2.3/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.3/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10204 2023-07-20 08:06:12.048271 nanoCEM-0.0.2.3/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9621 2023-07-20 08:05:38.000000 nanoCEM-0.0.2.3/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-20 08:06:12.048271 nanoCEM-0.0.2.3/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10038 2023-07-20 07:04:18.000000 nanoCEM-0.0.2.3/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.3/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.3/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8275 2023-07-20 06:58:56.000000 nanoCEM-0.0.2.3/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.3/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.3/nanoCEM/extract_sub_fastq_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.3/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.3/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11524 2023-07-15 03:17:36.000000 nanoCEM-0.0.2.3/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.3/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-20 08:06:12.048271 nanoCEM-0.0.2.3/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10204 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      458 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-20 08:06:12.000000 nanoCEM-0.0.2.3/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-20 08:06:12.052271 nanoCEM-0.0.2.3/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1192 2023-07-20 08:05:38.000000 nanoCEM-0.0.2.3/setup.py
```

### Comparing `nanoCEM-0.0.2.2/LICENSE` & `nanoCEM-0.0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/PKG-INFO` & `nanoCEM-0.0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,52 @@
-Metadata-Version: 2.1
-Name: nanoCEM
-Version: 0.0.2.2
-Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
-Home-page: https://github.com/lrslab/nanoCEM
-Author: GUO Zhihao
-Author-email: qhuozhihao@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
 ```sh
 pip install nanoCEM
 git clone https://github.com/lrslab/nanoCEM
 cd nanoCEM/example
 # tackle f5c result
-current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 # tackle tombo result
-current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+current_events_magnifier tombo -i data/wt/single -c data/ivt/single -o tombo_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
-In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
-This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
-Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
+The electric current signal level data produced from a nanopore read is referred to as a **squiggle**.
+Base calling this squiggle information generally contains some errors compared to a reference sequence. 
+The re-squiggle algorithm defines a new assignment from squiggle to reference sequence, hence a **re-squiggle**.
+Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but resquiggle is a more fine alignment than the move table in most cases.
+
+<center>
+
+![alt text](example/resquiggle.png)
+
+</center>
+
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 
 ![alt text](example/data_format.png)
 
 In our program, we assume that the input provided by the user is the **multi-fast5** format by default.
 ### Reference and alignment
@@ -72,15 +66,15 @@
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-current_events_magnifier.py tombo -h
+current_events_magnifier tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -98,15 +92,15 @@
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
   --norm                Turn on the normalization
 ```
 ### read_f5c_resquiggle
 ```sh
-current_events_magnifier.py f5c -h
+current_events_magnifier f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -125,14 +119,15 @@
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 # q 30 is recommended but you can try other filter in your data
+# guppy is just an example, and other basecalling software such as Bonito and Dorado can also be used.
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
@@ -140,17 +135,17 @@
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+extract_sub_fast5_from_bam -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 # Remember to sample fastq if you sampled your fast5
-extract_sub_fastq_from_bam.py -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
+extract_sub_fastq_from_bam -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
 Step 1 and 2 should run on your two sample respectively, before the step 5.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
@@ -169,15 +164,15 @@
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # tackle tombo result
-current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+current_events_magnifier tombo -i data/wt/single -c data/ivt/single -o tombo_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 #### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
@@ -194,15 +189,15 @@
 ```sh
 
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 ```
```

### Comparing `nanoCEM-0.0.2.2/README.md` & `nanoCEM-0.0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,66 @@
+Metadata-Version: 2.1
+Name: nanoCEM
+Version: 0.0.2.3
+Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
+Home-page: https://github.com/lrslab/nanoCEM
+Author: GUO Zhihao
+Author-email: qhuozhihao@icloud.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7,<3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nanoCEM
 The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
 ```sh
 pip install nanoCEM
 git clone https://github.com/lrslab/nanoCEM
 cd nanoCEM/example
 # tackle f5c result
-current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 # tackle tombo result
-current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+current_events_magnifier tombo -i data/wt/single -c data/ivt/single -o tombo_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
-In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
-This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
-Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
+The electric current signal level data produced from a nanopore read is referred to as a **squiggle**.
+Base calling this squiggle information generally contains some errors compared to a reference sequence. 
+The re-squiggle algorithm defines a new assignment from squiggle to reference sequence, hence a **re-squiggle**.
+Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but resquiggle is a more fine alignment than the move table in most cases.
+
+<center>
+
+![alt text](example/resquiggle.png)
+
+</center>
+
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 
 ![alt text](example/data_format.png)
 
 In our program, we assume that the input provided by the user is the **multi-fast5** format by default.
 ### Reference and alignment
@@ -58,15 +80,15 @@
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-current_events_magnifier.py tombo -h
+current_events_magnifier tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -84,15 +106,15 @@
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
   --norm                Turn on the normalization
 ```
 ### read_f5c_resquiggle
 ```sh
-current_events_magnifier.py f5c -h
+current_events_magnifier f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -111,14 +133,15 @@
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 # q 30 is recommended but you can try other filter in your data
+# guppy is just an example, and other basecalling software such as Bonito and Dorado can also be used.
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
@@ -126,17 +149,17 @@
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+extract_sub_fast5_from_bam -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 # Remember to sample fastq if you sampled your fast5
-extract_sub_fastq_from_bam.py -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
+extract_sub_fastq_from_bam -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
 Step 1 and 2 should run on your two sample respectively, before the step 5.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
@@ -155,15 +178,15 @@
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # tackle tombo result
-current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+current_events_magnifier tombo -i data/wt/single -c data/ivt/single -o tombo_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 #### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
@@ -180,15 +203,15 @@
 ```sh
 
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 ```
```

### Comparing `nanoCEM-0.0.2.2/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.2.3/nanoCEM/CE_magnifier_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,74 +1,84 @@
 #!/usr/bin/env python
 import argparse
 import os
-from nanoCEM.cem_utils import read_fasta_to_dic,reverse_fasta
+import time
+import warnings
+
 import pandas as pd
-from nanoCEM.plot import signal_plot
 from plotnine.exceptions import PlotnineWarning
-import warnings
-import time
+
+from nanoCEM.cem_utils import read_fasta_to_dic, reverse_fasta
+from nanoCEM.plot import signal_plot
+
 warnings.filterwarnings("ignore", category=PlotnineWarning)
-import numpy as np
+
+
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
-        parser_input.add_argument('--norm', action='store_true', help='normalization mode')
+        parser_input.add_argument('--norm', action='store_true', help='Turn on the normalization mode')
         parser_input.add_argument("--overplot-number", default=500, type=int,
                                   help="Number of read will be used to plot")
-        parser_input.add_argument('--rna', action='store_true', help='RNA mode')
+        parser_input.add_argument('--rna', action='store_true', help='Turn on the RNA mode')
+
     # Define the argument parser
-    parser = argparse.ArgumentParser(description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
+    parser = argparse.ArgumentParser(
+        description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
     # tombo subparser
     parser_tombo = subparsers.add_parser('tombo', help='tackle tombo re-squiggle')
     parser_tombo.add_argument('--basecall_group', default="RawGenomeCorrected_000",
-                        help='The attribute group to extract the training data from. e.g. RawGenomeCorrected_000')
+                              help='The attribute group to extract the training data from. e.g. RawGenomeCorrected_000')
     parser_tombo.add_argument('--basecall_subgroup', default='BaseCalled_template',
-                        help='Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template')
+                              help='Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template')
     parser_tombo.add_argument('-i', "--input_fast5", required=True,
-                        help="input_fast5_file")
+                              help="input_fast5_file")
     parser_tombo.add_argument('-c', "--control_fast5",
-                        help="control_fast5_file")
+                              help="control_fast5_file")
+    # parser_tombo.add_argument('-b', "--bam", help="bam file to help index to speed up")
     parser_tombo.add_argument('-o', "--output", default="tombo_result", help="output_file")
     parser_tombo.add_argument('-t', "--cpu", default=4, type=int, help="num of process")
     add_public_argument(parser_tombo)
 
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
-                        help="blow5_path")
+                            help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
-                        help="control_blow5_path")
+                            help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
 
-    parser_f5c.add_argument('--base_shift',type=int, default=0, help="output_file")
+    parser_f5c.add_argument('--base_shift', type=int, default=2, help="output_file")
     add_public_argument(parser_f5c)
     # parser.set_defaults(function='tombo', chrom="1", pos=150280972, len=10, strand='+', cpu=1,input_fast5='/data/current_test_data/samp/cem_test_dna/WGS/single/',\
     #                     control_fast5='/data/current_test_data/samp/cem_test_dna/WGA/single/',output='tombo_result_dna',\
     #                     overplot_number=300,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",\
     #                     basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=False)
     # parser.set_defaults(function='tombo', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,input_fast5='/data/Ecoli_23s/data/L_rep2/single/',\
     #                     control_fast5='/data/Ecoli_23s/data/IVT_negative/single/',output='tombo_result_rna',overplot_number=500,\
     #                     ref="/data/Ecoli_23s/23S_rRNA.fasta",\
     #                      basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=True)
-    parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=4,input='/data/Ecoli_23s/data/L_rep2/file',\
-                        control='/data/Ecoli_23s/data/IVT_negative/file',\
-                        output='f5c_result_rna_new_re',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA.fasta",rna=True,base_shift=0,norm=True)
+    parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=4,
+                        input='/data/Ecoli_23s/data/L_rep2/file', \
+                        control='/data/Ecoli_23s/data/IVT_negative/file', \
+                        output='f5c_result_rna_new_re', overplot_number=1000, ref="/data/Ecoli_23s/23S_rRNA.fasta",
+                        rna=True, base_shift=0, norm=True)
     # parser.set_defaults(function='f5c', chrom="1", pos=148545690, len=10, strand='+', cpu=4,input='/data/current_test_data/r1041_test/file',\
     #                     control='/data/current_test_data/r1041_wga/file',\
     #                     output='f5c_result_dna_new_norm',overplot_number=1000,ref="/data/current_test_data/r1041_test/hg38.fa",rna=False,base_shift=2,norm=False)
 
     return parser
 
+
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
     aligned_num_wt = 0
     aligned_num_ivt = 0
     # read reference
@@ -87,31 +97,31 @@
         base_list = "".join(list(reversed(base_list)))
         base_list = reverse_fasta(base_list)
 
     title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 2) + ':' + args.strand
     if args.rna:
         base_list = base_list.replace("T", "U")
         print("Running RNA mode ...")
-        title ='RNA  ' + title
+        title = 'RNA  ' + title
     else:
         print("Running DNA mode ...")
         title = 'DNA  ' + title
 
     results_path = args.output
     if not os.path.exists(results_path):
         os.mkdir(results_path)
     else:
         print("Output file existed! It will be overwrite after 5 secs ...")
         time.sleep(5)
         print("Continue ...")
 
+    if args.function == 'tombo':
 
-    if args.function == 'tombo' :
+        from nanoCEM.read_tombo_resquiggle import create_read_list_file, extract_group
 
-        from  nanoCEM.read_tombo_resquiggle import create_read_list_file,extract_group
         wt_file = create_read_list_file(args.input_fast5, results_path)
         df_wt, aligned_num_wt = extract_group(args, wt_file, subsample_num)
         df_wt['type'] = 'Sample'
         try:
             ivt_file = create_read_list_file(args.control_fast5, results_path)
             df_ivt, aligned_num_ivt = extract_group(args, ivt_file, subsample_num)
             df_ivt['type'] = 'Control'
@@ -123,57 +133,57 @@
             args.control_fast5 = None
         if args.control_fast5 is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from nanoCEM.read_f5c_resquiggle import read_blow5
+
         if args.base_shift < 0:
             raise RuntimeError("base_shift should not less than 0")
         # if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
         #     args.pos = args.pos + args.base_shift
         # else:
         #     args.pos = args.pos - args.base_shift
-        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift,args.norm)
+        df_wt, aligned_num_wt, nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,
+                                                            subsample_num, args.base_shift, args.norm)
         df_wt['type'] = 'Sample'
-        if nucleotide_type=='RNA' and not args.rna:
+        if nucleotide_type == 'RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
-            df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
-                                                 subsample_num,args.base_shift,args.norm)
+            df_ivt, aligned_num_ivt, _ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
+                                                    subsample_num, args.base_shift, args.norm)
             df_ivt['type'] = 'Control'
 
             df = pd.concat([df_wt, df_ivt])
             category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
             df['type'] = df['type'].astype(category)
 
             title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
         except:
             args.control = None
         if args.control is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
 
-
     category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
-
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
-    print("Start to generate plots and save  in "+ results_path)
+    print("Start to generate plots and save  in " + results_path)
     df.to_csv(results_path + '/feature.csv', index=None)
     # if args.function == 'f5c':
     #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
     #         args.pos = args.pos - args.base_shift
     #     else:
     #         args.pos = args.pos + args.base_shift
-    percentile_filter=False
+    percentile_filter = False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
-        percentile_filter=True
+        percentile_filter = True
 
-    signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
+    signal_plot(df, results_path, args.pos, base_list, title, 'merged', percentile_filter)
     # signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     # signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `nanoCEM-0.0.2.2/nanoCEM/cem_utils.py` & `nanoCEM-0.0.2.3/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.2.3/nanoCEM/current_events_magnifier`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 #!/usr/bin/env python
 import argparse
 import os
-from nanoCEM.cem_utils import read_fasta_to_dic,reverse_fasta
+import time
+import warnings
+
 import pandas as pd
-from nanoCEM.plot import signal_plot
 from plotnine.exceptions import PlotnineWarning
-import warnings
-import time
+
+from nanoCEM.cem_utils import read_fasta_to_dic, reverse_fasta
+from nanoCEM.plot import signal_plot
+
 warnings.filterwarnings("ignore", category=PlotnineWarning)
-import numpy as np
+
+
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
         parser_input.add_argument('--norm', action='store_true', help='Turn on the normalization mode')
         parser_input.add_argument("--overplot-number", default=500, type=int,
                                   help="Number of read will be used to plot")
         parser_input.add_argument('--rna', action='store_true', help='Turn on the RNA mode')
+
     # Define the argument parser
-    parser = argparse.ArgumentParser(description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
+    parser = argparse.ArgumentParser(
+        description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
     # tombo subparser
     parser_tombo = subparsers.add_parser('tombo', help='tackle tombo re-squiggle')
     parser_tombo.add_argument('--basecall_group', default="RawGenomeCorrected_000",
-                        help='The attribute group to extract the training data from. e.g. RawGenomeCorrected_000')
+                              help='The attribute group to extract the training data from. e.g. RawGenomeCorrected_000')
     parser_tombo.add_argument('--basecall_subgroup', default='BaseCalled_template',
-                        help='Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template')
+                              help='Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template')
     parser_tombo.add_argument('-i', "--input_fast5", required=True,
-                        help="input_fast5_file")
+                              help="input_fast5_file")
     parser_tombo.add_argument('-c', "--control_fast5",
-                        help="control_fast5_file")
+                              help="control_fast5_file")
     # parser_tombo.add_argument('-b', "--bam", help="bam file to help index to speed up")
     parser_tombo.add_argument('-o', "--output", default="tombo_result", help="output_file")
     parser_tombo.add_argument('-t', "--cpu", default=4, type=int, help="num of process")
     add_public_argument(parser_tombo)
 
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
-                        help="blow5_path")
+                            help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
-                        help="control_blow5_path")
+                            help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
 
-    parser_f5c.add_argument('--base_shift',type=int, default=2, help="output_file")
+    parser_f5c.add_argument('--base_shift', type=int, default=2, help="output_file")
     add_public_argument(parser_f5c)
     return parser
 
+
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
     aligned_num_wt = 0
     aligned_num_ivt = 0
     # read reference
@@ -74,31 +81,31 @@
         base_list = "".join(list(reversed(base_list)))
         base_list = reverse_fasta(base_list)
 
     title = args.chrom + ':' + str(args.pos - args.len + 1) + '-' + str(args.pos + args.len + 2) + ':' + args.strand
     if args.rna:
         base_list = base_list.replace("T", "U")
         print("Running RNA mode ...")
-        title ='RNA  ' + title
+        title = 'RNA  ' + title
     else:
         print("Running DNA mode ...")
         title = 'DNA  ' + title
 
     results_path = args.output
     if not os.path.exists(results_path):
         os.mkdir(results_path)
     else:
         print("Output file existed! It will be overwrite after 5 secs ...")
         time.sleep(5)
         print("Continue ...")
 
+    if args.function == 'tombo':
 
-    if args.function == 'tombo' :
+        from nanoCEM.read_tombo_resquiggle import create_read_list_file, extract_group
 
-        from  nanoCEM.read_tombo_resquiggle import create_read_list_file,extract_group
         wt_file = create_read_list_file(args.input_fast5, results_path)
         df_wt, aligned_num_wt = extract_group(args, wt_file, subsample_num)
         df_wt['type'] = 'Sample'
         try:
             ivt_file = create_read_list_file(args.control_fast5, results_path)
             df_ivt, aligned_num_ivt = extract_group(args, ivt_file, subsample_num)
             df_ivt['type'] = 'Control'
@@ -110,57 +117,57 @@
             args.control_fast5 = None
         if args.control_fast5 is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from nanoCEM.read_f5c_resquiggle import read_blow5
+
         if args.base_shift < 0:
             raise RuntimeError("base_shift should not less than 0")
         # if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
         #     args.pos = args.pos + args.base_shift
         # else:
         #     args.pos = args.pos - args.base_shift
-        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift,args.norm)
+        df_wt, aligned_num_wt, nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,
+                                                            subsample_num, args.base_shift, args.norm)
         df_wt['type'] = 'Sample'
-        if nucleotide_type=='RNA' and not args.rna:
+        if nucleotide_type == 'RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
-            df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
-                                                 subsample_num,args.base_shift,args.norm)
+            df_ivt, aligned_num_ivt, _ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
+                                                    subsample_num, args.base_shift, args.norm)
             df_ivt['type'] = 'Control'
 
             df = pd.concat([df_wt, df_ivt])
             category = pd.api.types.CategoricalDtype(categories=['Sample', "Control"], ordered=True)
             df['type'] = df['type'].astype(category)
 
             title = title + '   Sample:' + str(aligned_num_wt) + '  Control:' + str(aligned_num_ivt)
         except:
             args.control = None
         if args.control is None:
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
 
-
     category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
-
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
-    print("Start to generate plots and save  in "+ results_path)
-    df.to_csv(results_path+'/feature.csv',index=None)
-   # if args.function == 'f5c':
+    print("Start to generate plots and save  in " + results_path)
+    df.to_csv(results_path + '/feature.csv', index=None)
+    # if args.function == 'f5c':
     #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
     #         args.pos = args.pos - args.base_shift
     #     else:
     #         args.pos = args.pos + args.base_shift
-    percentile_filter=False
+    percentile_filter = False
     if aligned_num_wt > 50 and aligned_num_ivt > 50:
-        percentile_filter=True
+        percentile_filter = True
 
-    signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
+    signal_plot(df, results_path, args.pos, base_list, title, 'merged', percentile_filter)
     # signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     # signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `nanoCEM-0.0.2.2/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.2.3/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/nanoCEM/extract_sub_fastq_from_bam.py` & `nanoCEM-0.0.2.3/nanoCEM/extract_sub_fastq_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/nanoCEM/normalization.py` & `nanoCEM-0.0.2.3/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/nanoCEM/plot.py` & `nanoCEM-0.0.2.3/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.2.3/nanoCEM/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.2.3/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.2/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.2.3/nanoCEM.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,37 +22,45 @@
 ## Example
 Here is an example to help the user confirm the installation of A2030 on 23S rRNA:
 ```sh
 pip install nanoCEM
 git clone https://github.com/lrslab/nanoCEM
 cd nanoCEM/example
 # tackle f5c result
-current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 # tackle tombo result
-current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+current_events_magnifier tombo -i data/wt/single -c data/ivt/single -o tombo_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
 ## Data release
 For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
-In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
-This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
-Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
+The electric current signal level data produced from a nanopore read is referred to as a **squiggle**.
+Base calling this squiggle information generally contains some errors compared to a reference sequence. 
+The re-squiggle algorithm defines a new assignment from squiggle to reference sequence, hence a **re-squiggle**.
+Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but resquiggle is a more fine alignment than the move table in most cases.
+
+<center>
+
+![alt text](example/resquiggle.png)
+
+</center>
+
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
 
 ![alt text](example/data_format.png)
 
 In our program, we assume that the input provided by the user is the **multi-fast5** format by default.
 ### Reference and alignment
@@ -72,15 +80,15 @@
 ```sh
 pip install ont-fast5-api pod5
 conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-current_events_magnifier.py tombo -h
+current_events_magnifier tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -98,15 +106,15 @@
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
   --norm                Turn on the normalization
 ```
 ### read_f5c_resquiggle
 ```sh
-current_events_magnifier.py f5c -h
+current_events_magnifier f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -125,14 +133,15 @@
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
 # q 30 is recommended but you can try other filter in your data
+# guppy is just an example, and other basecalling software such as Bonito and Dorado can also be used.
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
 minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
@@ -140,17 +149,17 @@
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
 Re-squiggle is a really time-consuming program, it will be applied on all reads not only the reads around interest region.
 So I provide a simple py file to help extract the reads you want to visualize.
 And the new reads will be copied to ```subsample_single/```
 ```sh
 multi_to_single_fast5 -i fast5/ -s single/ --recursive -t 16
-extract_sub_fast5_from_bam.py -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
+extract_sub_fast5_from_bam -i single/ -o subsample_single/ -b file.bam --chrom NR_103073.1 --pos 2030 
 # Remember to sample fastq if you sampled your fast5
-extract_sub_fastq_from_bam.py -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
+extract_sub_fastq_from_bam -i all.fastq -o final.fastq -b file.bam --chrom NR_103073.1 --pos 2030 
 ```
 ### 4 Re-squiggle
 #### 4.1 Tombo resquiggle (v1.5.0)
 Step 1 and 2 should run on your two sample respectively, before the step 5.
 1. Data format conversion
 
 If you did the subsample,skip this step and used ```subsample_single``` as the following input rather than ```single/```
@@ -169,15 +178,15 @@
 # Tombo resquiggle will take various of time, which means subsample your aligned reads of the special region is recommended
 # Run the Tombo pipeline above for your two sample respective, the SSD disk is recommended 
 # If you ran step2, run the tombo command on subsample_single but single
 ```
 3. Run current_events_magnifier to plot
 ```sh
 # tackle tombo result
-current_events_magnifier.py tombo -i data/wt/single -c data/ivt/single -o tombo_result \
+current_events_magnifier tombo -i data/wt/single -c data/ivt/single -o tombo_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 #### 4.2 F5c resquiggle (v1.2) (support R10)
 Step 1 and 2 should run on your two sample respectively, before the step 3.
@@ -194,15 +203,15 @@
 ```sh
 
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-current_events_magnifier.py f5c -i data/wt/file -c data/ivt/file -o f5c_result \
+current_events_magnifier f5c -i data/wt/file -c data/ivt/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 2030 \
 --ref data/23S_rRNA.fasta \
 --base_shift 2 --rna --norm
 ```
```

### Comparing `nanoCEM-0.0.2.2/setup.py` & `nanoCEM-0.0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.2.2",
+    version="0.0.2.3",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
@@ -27,9 +27,9 @@
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
         "pyslow5>=1.0.0",
         "vbz_h5py_plugin>=1.0.1",
         "biopython>=1.80"
     ],
-    scripts=['nanoCEM/current_events_magnifier.py','nanoCEM/extract_sub_fast5_from_bam.py','nanoCEM/extract_sub_fastq_from_bam.py']
+    scripts=['nanoCEM/current_events_magnifier','nanoCEM/extract_sub_fast5_from_bam','nanoCEM/extract_sub_fastq_from_bam']
 )
```

