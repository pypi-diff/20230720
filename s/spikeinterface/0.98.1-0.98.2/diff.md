# Comparing `tmp/spikeinterface-0.98.1.tar.gz` & `tmp/spikeinterface-0.98.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikeinterface-0.98.1.tar", last modified: Tue Jul 18 09:06:10 2023, max compression
+gzip compressed data, was "spikeinterface-0.98.2.tar", last modified: Thu Jul 20 12:44:43 2023, max compression
```

## Comparing `spikeinterface-0.98.1.tar` & `spikeinterface-0.98.2.tar`

### file list

```diff
@@ -1,383 +1,383 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.951110 spikeinterface-0.98.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.959110 spikeinterface-0.98.1/src/spikeinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.963110 spikeinterface-0.98.1/src/spikeinterface/comparison/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/basecomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/collisioncomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/collisionstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/comparisontools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramcomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/groundtruthstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/multicomparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    25783 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/paircomparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/studytools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.967110 spikeinterface-0.98.1/src/spikeinterface/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41463 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/baseevent.py
--rw-r--r--   0 runner    (1001) docker     (123)    29103 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/baserecording.py
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/baserecordingsnippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/basesnippets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/basesorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/binaryfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/binaryrecordingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/channelsaggregationrecording.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/channelslice.py
--rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/core_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/frameslicerecording.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/frameslicesorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/injecttemplates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/job_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npyfoldersnippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npysnippetsextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npzfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npzsortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/numpyextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/old_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/recording_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    25339 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/segmentutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/snippets_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/sparsity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/template_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/unitsaggregationsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/unitsselectionsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    77909 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/waveform_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/waveform_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/zarrrecordingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.971110 spikeinterface-0.98.1/src/spikeinterface/curation/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/auto_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/curation_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/curationsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/mergeunitssorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/remove_duplicated_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/remove_excess_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/remove_redundant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/sortingview_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/splitunitsorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.971110 spikeinterface-0.98.1/src/spikeinterface/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/exporters/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/exporters/to_phy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.975110 spikeinterface-0.98.1/src/spikeinterface/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/alfsortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/bids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/cbin_ibl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/cellexplorersortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/combinatoextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/extractorlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/hdsortextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/herdingspikesextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/iblstreamingrecording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/klustaextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/matlabhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/mclustextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/mcsh5extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/mdaextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.983111 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/alphaomega.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/biocam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/blackrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/ced.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/edf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/intan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/maxwell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/mcsraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/mearec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neobaseextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuralynx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuroscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/nix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/plexon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spike2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikegadgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/tdt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neuropixels_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/nwbextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/phykilosortextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/shybridextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/spykingcircusextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/toy_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/tridesclousextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/waveclussnippetstextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/waveclustextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/yassextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/full.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.987110 spikeinterface-0.98.1/src/spikeinterface/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/alignsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/amplitude_scalings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/correlograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/isi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/noise_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/principal_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    22736 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/unit_localization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.995111 spikeinterface-0.98.1/src/spikeinterface/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/align_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/average_across_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/basepreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/common_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/correct_lsb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.995111 spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/depth_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/detect_bad_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/directional_derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_opencl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/highpass_spatial_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/interpolate_bad_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/normalize_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/phase_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessinglist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/rectify.py
--rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/remove_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/silence_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/unsigned_to_signed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/whiten.py
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/zero_channel_pad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.999111 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41381 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/misc_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/pca_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.999111 spikeinterface-0.98.1/src/spikeinterface/sorters/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/basesorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.007111 spikeinterface-0.98.1/src/spikeinterface/sorters/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/combinato.py
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/herdingspikes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/ironclust.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort.py
--rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_master.m
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort_master.m
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosortbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta_config_default.prm
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort4.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort5.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/pykilosort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/sc_config_default.params
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/spyking_circus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/tridesclous.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets_master.m
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass_config_default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.011111 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/si_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/spyking_circus2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/tridesclous2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/runsorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/sorterlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.011111 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/constructNPYheader.m
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/shellscript.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/writeNPY.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.015111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.015111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    29179 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.019111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/circus.py
--rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/isocut5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/method_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/random_projections.py
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py
--rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/triage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/features_from_peaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.023111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33854 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/circus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/method_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/tdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    44820 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/wobble.py
--rw-r--r--   0 runner    (1001) docker     (123)    59332 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    40384 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.023111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.031112 spikeinterface-0.98.1/src/spikeinterface/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.039112 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/all_amplitudes_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/autocorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/crosscorrelograms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.043112 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.051112 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/autocorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/base_mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sorting_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/autocorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/base_sortingview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/crosscorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/sorting_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/spikes_on_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms_density_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/widget_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.959110 spikeinterface-0.98.1/src/spikeinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.766803 spikeinterface-0.98.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-20 12:44:43.766803 spikeinterface-0.98.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:44:43.766803 spikeinterface-0.98.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.714800 spikeinterface-0.98.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.714800 spikeinterface-0.98.2/src/spikeinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.718800 spikeinterface-0.98.2/src/spikeinterface/comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/basecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/collisioncomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/collisionstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/comparisontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/correlogramcomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/correlogramstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/groundtruthstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/multicomparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25783 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/paircomparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/comparison/studytools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.722800 spikeinterface-0.98.2/src/spikeinterface/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41463 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/baseevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/baserecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/baserecordingsnippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/basesnippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/basesorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/binaryfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/binaryrecordingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/channelsaggregationrecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/channelslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/core_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/frameslicerecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/frameslicesorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/injecttemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/job_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/npyfoldersnippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/npysnippetsextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/npzfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/npzsortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/numpyextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/old_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/recording_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25339 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/segmentutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/snippets_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/template_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/unitsaggregationsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/unitsselectionsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77909 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/waveform_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/waveform_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/core/zarrrecordingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.726801 spikeinterface-0.98.2/src/spikeinterface/curation/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/auto_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/curation_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/curationsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/mergeunitssorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/remove_duplicated_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/remove_excess_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/remove_redundant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/sortingview_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/curation/splitunitsorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.726801 spikeinterface-0.98.2/src/spikeinterface/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/exporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/exporters/to_phy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.730801 spikeinterface-0.98.2/src/spikeinterface/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/alfsortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/bids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/cbin_ibl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/cellexplorersortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/combinatoextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/extractorlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/hdsortextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/herdingspikesextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/iblstreamingrecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/klustaextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/matlabhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/mclustextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/mcsh5extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/mdaextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.734801 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/alphaomega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/biocam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/blackrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/ced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/intan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/maxwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/mcsraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/mearec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neobaseextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neuralynx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neuroscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/nix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/plexon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/spike2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/spikegadgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/tdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/neuropixels_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/nwbextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/phykilosortextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/shybridextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/spykingcircusextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/toy_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/tridesclousextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/waveclussnippetstextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/waveclustextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/extractors/yassextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/full.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.734801 spikeinterface-0.98.2/src/spikeinterface/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/alignsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/amplitude_scalings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/correlograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/isi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/noise_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/principal_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/spike_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/template_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22736 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/postprocessing/unit_localization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.738802 spikeinterface-0.98.2/src/spikeinterface/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/align_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/average_across_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/basepreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/common_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/correct_lsb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.738802 spikeinterface-0.98.2/src/spikeinterface/preprocessing/deepinterpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/deepinterpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/depth_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/detect_bad_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/directional_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/filter_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/filter_opencl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/highpass_spatial_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/interpolate_bad_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/normalize_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/phase_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/preprocessing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/preprocessinglist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/rectify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/remove_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/silence_periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/unsigned_to_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/whiten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/preprocessing/zero_channel_pad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.738802 spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41381 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/misc_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/pca_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/quality_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/quality_metric_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.742802 spikeinterface-0.98.2/src/spikeinterface/sorters/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/basesorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.746802 spikeinterface-0.98.2/src/spikeinterface/sorters/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/combinato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/hdsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/hdsort_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/herdingspikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/ironclust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2_5_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort3_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosortbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/klusta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/klusta_config_default.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/mountainsort4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/mountainsort5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/pykilosort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/sc_config_default.params
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/spyking_circus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/tridesclous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus_snippets_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/yass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/external/yass_config_default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.746802 spikeinterface-0.98.2/src/spikeinterface/sorters/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/internal/si_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/internal/spyking_circus2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/internal/tridesclous2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/runsorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/sorterlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.746802 spikeinterface-0.98.2/src/spikeinterface/sorters/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/utils/constructNPYheader.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/utils/shellscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sorters/utils/writeNPY.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.746802 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.750802 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29179 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.750802 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/circus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27275 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/isocut5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position_and_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/random_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/triage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/features_from_peaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.754803 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33854 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/circus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/tdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44820 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/wobble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59332 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/motion_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/motion_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40384 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.754803 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.758803 spikeinterface-0.98.2/src/spikeinterface/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.762803 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/all_amplitudes_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/autocorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/crosscorrelograms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.762803 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.766803 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/autocorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/base_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sorting_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.766803 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/autocorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/base_sortingview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/crosscorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/sorting_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/spikes_on_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/unit_depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/unit_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/unit_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/unit_waveforms_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-20 12:42:50.000000 spikeinterface-0.98.2/src/spikeinterface/widgets/widget_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:44:43.718800 spikeinterface-0.98.2/src/spikeinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-20 12:44:43.000000 spikeinterface-0.98.2/src/spikeinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-20 12:44:43.000000 spikeinterface-0.98.2/src/spikeinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:44:43.000000 spikeinterface-0.98.2/src/spikeinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-20 12:44:43.000000 spikeinterface-0.98.2/src/spikeinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 12:44:43.000000 spikeinterface-0.98.2/src/spikeinterface.egg-info/top_level.txt
```

### Comparing `spikeinterface-0.98.1/LICENSE` & `spikeinterface-0.98.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/PKG-INFO` & `spikeinterface-0.98.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface
-Version: 0.98.1
+Version: 0.98.2
 Summary: Python toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface
 Project-URL: documentation, https://spikeinterface.readthedocs.io/
 Project-URL: changelog, https://spikeinterface.readthedocs.io/en/latest/whatisnew.html
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.1 Summary: Python
+Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.2 Summary: Python
 toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino
 buccino@gmail.com>, Samuel Garcia
 garcia.die@gmail.com> Project-URL: homepage, https://github.com/SpikeInterface/
 spikeinterface Project-URL: repository, https://github.com/SpikeInterface/
 spikeinterface Project-URL: documentation, https://
 spikeinterface.readthedocs.io/ Project-URL: changelog, https://
```

### Comparing `spikeinterface-0.98.1/README.md` & `spikeinterface-0.98.2/README.md`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/pyproject.toml` & `spikeinterface-0.98.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spikeinterface"
-version = "0.98.1"
+version = "0.98.2"
 authors = [
   { name="Alessio Buccino", email="alessiop.buccino@gmail.com" },
   { name="Samuel Garcia", email="sam.garcia.die@gmail.com" },
 ]
 description = "Python toolkit for analysis, visualization, and comparison of spike sorting output"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
@@ -14,14 +14,15 @@
     "Intended Audience :: Science/Research",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: OS Independent"
 ]
 
+
 dependencies = [
     "numpy",
     "neo>=0.12.0",
     "joblib",
     "threadpoolctl",
     "tqdm",
     "probeinterface>=0.2.17",
@@ -95,15 +96,14 @@
 ]
 
 widgets = [
     "matplotlib",
     "ipympl",
     "ipywidgets",
     "sortingview>=0.11.15",
-    "figurl-jupyter"
 ]
 
 test_core = [
     "pytest",
     "zarr",
     "psutil",
 ]
@@ -114,54 +114,53 @@
 
     # zarr is needed for testing
     "zarr",
     "xarray",
     "huggingface_hub",
 
     # tridesclous
-    "numpy<1.24",
     "numba",
-    "hdbscan",
+    "hdbscan>=0.8.33",  # Previous version had a broken wheel
 
     # for sortingview backend
     "sortingview",
 
     # recent datalad need a too recent version for git-annex
     # so we use an old one here
     "datalad==0.16.2",
 
     ## install tridesclous for testing ##
-    "tridesclous>=1.6.6.1",
+    "tridesclous>=1.6.8",
 
     ## sliding_nn
     "pymde",
     "torch",
     "pynndescent",
 
     # for github test : probeinterface and neo from master
     # for release we need pypi, so this need to be commented
-    # "probeinterface @ git+https://github.com/SpikeInterface/probeinterface.git",
-    # "neo @ git+https://github.com/NeuralEnsemble/python-neo.git",
+    # "probeinterface @ git+https://github.com/SpikeInterface/probeinterface.git",
+    # "neo @ git+https://github.com/NeuralEnsemble/python-neo.git",
 ]
 
 docs = [
     "Sphinx==5.1.1",
     "sphinx_rtd_theme==1.0.0",
     "sphinx-gallery",
     "numpydoc",
 
     # for notebooks in the gallery
     "MEArec",   # Use as an example
     "datalad==0.16.2",  # Download mearec data, not sure if needed as is installed with conda as well because of git-annex
     "pandas", # Don't know where this is needed
-    "hdbscan",   # For sorters, probably spikingcircus
+    "hdbscan>=0.8.33",   # For sorters, probably spikingcircus
     "numba", # For sorters, probably spikingcircus
     # for release we need pypi, so this needs to be commented
-    # "probeinterface @ git+https://github.com/SpikeInterface/probeinterface.git",  # We always build from the latest version
-    # "neo @ git+https://github.com/NeuralEnsemble/python-neo.git",  # We always build from the latest version
+    # "probeinterface @ git+https://github.com/SpikeInterface/probeinterface.git",  # We always build from the latest version
+    # "neo @ git+https://github.com/NeuralEnsemble/python-neo.git",  # We always build from the latest version
 
 ]
 
 [tool.pytest.ini_options]
 markers = [
     "core",
     "extractors",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/basecomparison.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/basecomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/collisioncomparison.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/collisioncomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/collisionstudy.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/collisionstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/comparisontools.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/comparisontools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramcomparison.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/correlogramcomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramstudy.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/correlogramstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/groundtruthstudy.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/groundtruthstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/hybrid.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/hybrid.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/multicomparisons.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/multicomparisons.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/paircomparisons.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/paircomparisons.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/comparison/studytools.py` & `spikeinterface-0.98.2/src/spikeinterface/comparison/studytools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/base.py` & `spikeinterface-0.98.2/src/spikeinterface/core/base.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/baseevent.py` & `spikeinterface-0.98.2/src/spikeinterface/core/baseevent.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/baserecording.py` & `spikeinterface-0.98.2/src/spikeinterface/core/baserecording.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,14 +441,16 @@
             file_paths = [folder / f"traces_cached_seg{i}.raw" for i in range(self.get_num_segments())]
             dtype = kwargs.get("dtype", None) or self.get_dtype()
 
             write_binary_recording(self, file_paths=file_paths, dtype=dtype, **job_kwargs)
 
             from .binaryrecordingextractor import BinaryRecordingExtractor
 
+            # This is created so it can be saved as json because the `BinaryFolderRecording` requires it loading
+            # See the __init__ of `BinaryFolderRecording`
             binary_rec = BinaryRecordingExtractor(
                 file_paths=file_paths,
                 sampling_frequency=self.get_sampling_frequency(),
                 num_channels=self.get_num_channels(),
                 dtype=dtype,
                 t_starts=t_starts,
                 channel_ids=self.get_channel_ids(),
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/baserecordingsnippets.py` & `spikeinterface-0.98.2/src/spikeinterface/core/baserecordingsnippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/basesnippets.py` & `spikeinterface-0.98.2/src/spikeinterface/core/basesnippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/basesorting.py` & `spikeinterface-0.98.2/src/spikeinterface/core/basesorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/binaryfolder.py` & `spikeinterface-0.98.2/src/spikeinterface/core/binaryfolder.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/binaryrecordingextractor.py` & `spikeinterface-0.98.2/src/spikeinterface/core/binaryrecordingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/channelsaggregationrecording.py` & `spikeinterface-0.98.2/src/spikeinterface/core/channelsaggregationrecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/channelslice.py` & `spikeinterface-0.98.2/src/spikeinterface/core/channelslice.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/core_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/core/core_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/datasets.py` & `spikeinterface-0.98.2/src/spikeinterface/core/datasets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/frameslicerecording.py` & `spikeinterface-0.98.2/src/spikeinterface/core/frameslicerecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/frameslicesorting.py` & `spikeinterface-0.98.2/src/spikeinterface/core/frameslicesorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/generate.py` & `spikeinterface-0.98.2/src/spikeinterface/core/generate.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/globals.py` & `spikeinterface-0.98.2/src/spikeinterface/core/globals.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/injecttemplates.py` & `spikeinterface-0.98.2/src/spikeinterface/core/injecttemplates.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/job_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/core/job_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/npyfoldersnippets.py` & `spikeinterface-0.98.2/src/spikeinterface/core/npyfoldersnippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/npysnippetsextractor.py` & `spikeinterface-0.98.2/src/spikeinterface/core/npysnippetsextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/npzfolder.py` & `spikeinterface-0.98.2/src/spikeinterface/core/npzfolder.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/npzsortingextractor.py` & `spikeinterface-0.98.2/src/spikeinterface/core/npzsortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/numpyextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/core/numpyextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/old_api_utils.py` & `spikeinterface-0.98.2/src/spikeinterface/core/old_api_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/recording_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/core/recording_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,17 +308,17 @@
 
     Parameters
     ----------
     recording : BaseRecording
         The input recording
     channel_ids : list/array or None
         If given, a subset of channels to order locations for
-    dimensions : str or tuple
+    dimensions : str, tuple, or list
         If str, it needs to be 'x', 'y', 'z'.
-        If tuple, it sorts the locations in two dimensions using lexsort.
+        If tuple or list, it sorts the locations in two dimensions using lexsort.
         This approach is recommended since there is less ambiguity, by default ('x', 'y')
 
     Returns
     -------
     order_f : np.array
         Array with sorted indices
     order_r : np.array
@@ -330,15 +330,15 @@
     locations = locations[channel_inds, :]
 
     if isinstance(dimensions, str):
         dim = ["x", "y", "z"].index(dimensions)
         assert dim < ndim, "Invalid dimensions!"
         order_f = np.argsort(locations[:, dim], kind="stable")
     else:
-        assert isinstance(dimensions, tuple), "dimensions can be a str or a tuple"
+        assert isinstance(dimensions, (tuple, list)), "dimensions can be str, tuple, or list"
         locations_to_sort = ()
         for dim in dimensions:
             dim = ["x", "y", "z"].index(dim)
             assert dim < ndim, "Invalid dimensions!"
             locations_to_sort += (locations[:, dim],)
         order_f = np.lexsort(locations_to_sort)
     order_r = np.argsort(order_f, kind="stable")
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/segmentutils.py` & `spikeinterface-0.98.2/src/spikeinterface/core/segmentutils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/snippets_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/core/snippets_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/sparsity.py` & `spikeinterface-0.98.2/src/spikeinterface/core/sparsity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/template_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/core/template_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/testing.py` & `spikeinterface-0.98.2/src/spikeinterface/core/testing.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/unitsaggregationsorting.py` & `spikeinterface-0.98.2/src/spikeinterface/core/unitsaggregationsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/unitsselectionsorting.py` & `spikeinterface-0.98.2/src/spikeinterface/core/unitsselectionsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/waveform_extractor.py` & `spikeinterface-0.98.2/src/spikeinterface/core/waveform_extractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/waveform_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/core/waveform_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/core/zarrrecordingextractor.py` & `spikeinterface-0.98.2/src/spikeinterface/core/zarrrecordingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/auto_merge.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/auto_merge.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/curation_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/curation_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/curationsorting.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/curationsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/mergeunitssorting.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/mergeunitssorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/remove_duplicated_spikes.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/remove_duplicated_spikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/remove_excess_spikes.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/remove_excess_spikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/remove_redundant.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/remove_redundant.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/sortingview_curation.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/sortingview_curation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/curation/splitunitsorting.py` & `spikeinterface-0.98.2/src/spikeinterface/curation/splitunitsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/exporters/report.py` & `spikeinterface-0.98.2/src/spikeinterface/exporters/report.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/exporters/to_phy.py` & `spikeinterface-0.98.2/src/spikeinterface/exporters/to_phy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/alfsortingextractor.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/alfsortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/bids.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/bids.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/cbin_ibl.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/cbin_ibl.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/cellexplorersortingextractor.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/cellexplorersortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/combinatoextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/combinatoextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/extractorlist.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/extractorlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/hdsortextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/hdsortextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/herdingspikesextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/herdingspikesextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/iblstreamingrecording.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/iblstreamingrecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/klustaextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/klustaextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/matlabhelpers.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/matlabhelpers.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/mclustextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/mclustextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/mcsh5extractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/mcsh5extractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/mdaextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/mdaextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/alphaomega.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/alphaomega.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/axona.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/axona.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/biocam.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/biocam.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/blackrock.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/blackrock.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/ced.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/ced.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/edf.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/edf.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/intan.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/intan.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/maxwell.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/maxwell.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/mcsraw.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/mcsraw.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/mearec.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/mearec.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 import numpy as np
 
 import probeinterface as pi
 
 from .neobaseextractor import NeoBaseRecordingExtractor, NeoBaseSortingExtractor
 
 
-def drop_neo_arguments_in_version_0_11_0(neo_kwargs):
-    # Temporary function until neo version 0.12.0 is released
+def drop_invalid_neo_arguments_before_version_0_13_0(neo_kwargs):
+    # Temporary function until neo version 0.13.0 is released
     from packaging.version import parse as parse_version
     from importlib.metadata import version
 
     neo_version = version("neo")
     minor_version = parse_version(neo_version).minor
 
     # The possibility of loading only spike_trains or only analog_signals is not present in neo <= 0.11.0
-    if minor_version < 12:
+    if minor_version < 13:
         neo_kwargs.pop("load_spiketrains")
         neo_kwargs.pop("load_analogsignal")
 
     return neo_kwargs
 
 
 class MEArecRecordingExtractor(NeoBaseRecordingExtractor):
@@ -64,16 +64,15 @@
         file_path,
     ):
         neo_kwargs = {
             "filename": str(file_path),
             "load_spiketrains": False,
             "load_analogsignal": True,
         }
-        # The possibility of loading only spike_trains or only analog_signals will be added in neo version 0.12.0
-        neo_kwargs = drop_neo_arguments_in_version_0_11_0(neo_kwargs=neo_kwargs)
+        neo_kwargs = drop_invalid_neo_arguments_before_version_0_13_0(neo_kwargs=neo_kwargs)
         return neo_kwargs
 
 
 class MEArecSortingExtractor(NeoBaseSortingExtractor):
     mode = "file"
     NeoRawIOClass = "MEArecRawIO"
     neo_returns_frames = False
@@ -90,16 +89,15 @@
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {
             "filename": str(file_path),
             "load_spiketrains": True,
             "load_analogsignal": False,
         }
-        # The possibility of loading only spike_trains or only analog_signals will be added in neo version 0.12.0
-        neo_kwargs = drop_neo_arguments_in_version_0_11_0(neo_kwargs=neo_kwargs)
+        neo_kwargs = drop_invalid_neo_arguments_before_version_0_13_0(neo_kwargs=neo_kwargs)
 
         return neo_kwargs
 
     def read_sampling_frequency(self, file_path: Union[str, Path]) -> float:
         from h5py import File
 
         with File(file_path, "r") as f:
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neo_utils.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neo_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neobaseextractor.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neobaseextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuralynx.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neuralynx.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuroscope.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/neuroscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,17 @@
     @classmethod
     def map_to_neo_kwargs(cls, file_path, xml_file_path=None):
         # For this because of backwards compatibility we have a strange convention
         # filename is the xml file
         # binary_file is the binary file in .dat, .lfp, .eeg
 
         if xml_file_path is not None:
-            neo_kwargs = {"binary_file": str(file_path), "filename": str(xml_file_path)}
+            neo_kwargs = {"binary_file": Path(file_path), "filename": Path(xml_file_path)}
         else:
-            neo_kwargs = {"filename": str(file_path)}
+            neo_kwargs = {"filename": Path(file_path)}
 
         return neo_kwargs
 
 
 class NeuroScopeSortingExtractor(BaseSorting):
     """
     Extracts spiking information from an arbitrary number of .res.%i and .clu.%i files in the general folder path.
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/nix.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/nix.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/openephys.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/openephys.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/plexon.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/plexon.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spike2.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/spike2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikegadgets.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/spikegadgets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikeglx.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/spikeglx.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/tdt.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neoextractors/tdt.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/neuropixels_utils.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/neuropixels_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/nwbextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/nwbextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/phykilosortextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/phykilosortextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/shybridextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/shybridextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/spykingcircusextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/spykingcircusextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/toy_example.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/toy_example.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/tridesclousextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/tridesclousextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/waveclussnippetstextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/waveclussnippetstextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/waveclustextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/waveclustextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/extractors/yassextractors.py` & `spikeinterface-0.98.2/src/spikeinterface/extractors/yassextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/full.py` & `spikeinterface-0.98.2/src/spikeinterface/full.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/alignsorting.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/alignsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/amplitude_scalings.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/amplitude_scalings.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/correlograms.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/correlograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/isi.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/isi.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/noise_level.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/noise_level.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/principal_component.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/principal_component.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_amplitudes.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/spike_amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/template_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_similarity.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/template_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/postprocessing/unit_localization.py` & `spikeinterface-0.98.2/src/spikeinterface/postprocessing/unit_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/align_snippets.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/align_snippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/astype.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/astype.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/average_across_direction.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/average_across_direction.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/basepreprocessor.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/basepreprocessor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/clip.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/clip.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/common_reference.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/common_reference.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/correct_lsb.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/correct_lsb.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/depth_order.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/depth_order.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
     Parameters
     ----------
     recording : BaseRecording
         The recording to re-order.
     channel_ids : list/array or None
         If given, a subset of channels to order locations for
-    dimensions : str or tuple
+    dimensions : str, tuple, list
         If str, it needs to be 'x', 'y', 'z'.
-        If tuple, it sorts the locations in two dimensions using lexsort.
+        If tuple or list, it sorts the locations in two dimensions using lexsort.
         This approach is recommended since there is less ambiguity, by default ('x', 'y')
     """
 
     name = "depth_order"
     installed = True
 
     def __init__(self, parent_recording, channel_ids=None, dimensions=("x", "y")):
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/detect_bad_channels.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/detect_bad_channels.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/directional_derivative.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/directional_derivative.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_gaussian.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/filter_gaussian.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_opencl.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/filter_opencl.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/highpass_spatial_filter.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/highpass_spatial_filter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/interpolate_bad_channels.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/interpolate_bad_channels.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/motion.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/motion.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/normalize_scale.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/phase_shift.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/phase_shift.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessing_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/preprocessing_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessinglist.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/preprocessinglist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/rectify.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/rectify.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/remove_artifacts.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/remove_artifacts.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/resample.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/resample.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/silence_periods.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/silence_periods.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/unsigned_to_signed.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/unsigned_to_signed.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/whiten.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/whiten.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/preprocessing/zero_channel_pad.py` & `spikeinterface-0.98.2/src/spikeinterface/preprocessing/zero_channel_pad.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/misc_metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/misc_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/pca_metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/pca_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_calculator.py` & `spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/quality_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_list.py` & `spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/quality_metric_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/utils.py` & `spikeinterface-0.98.2/src/spikeinterface/qualitymetrics/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/basesorter.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/basesorter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/combinato.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/combinato.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/hdsort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort_master.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/hdsort_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/herdingspikes.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/herdingspikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/ironclust.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/ironclust.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2_5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5_master.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2_5_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_master.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort2_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort3.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3_master.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort3_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort_master.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosort_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosortbase.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/kilosortbase.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/klusta.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta_config_default.prm` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/klusta_config_default.prm`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort4.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/mountainsort4.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort5.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/mountainsort5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/pykilosort.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/pykilosort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/sc_config_default.params` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/sc_config_default.params`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/spyking_circus.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/spyking_circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/tridesclous.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/tridesclous.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_master.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus_snippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets_master.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/waveclus_snippets_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/yass.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass_config_default.yaml` & `spikeinterface-0.98.2/src/spikeinterface/sorters/external/yass_config_default.yaml`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/internal/si_based.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/internal/si_based.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/internal/spyking_circus2.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/internal/spyking_circus2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/internal/tridesclous2.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/internal/tridesclous2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/launcher.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/launcher.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/runsorter.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/runsorter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/sorterlist.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/sorterlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/constructNPYheader.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/utils/constructNPYheader.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/misc.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/shellscript.py` & `spikeinterface-0.98.2/src/spikeinterface/sorters/utils/shellscript.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/writeNPY.m` & `spikeinterface-0.98.2/src/spikeinterface/sorters/utils/writeNPY.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/circus.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
 
     f = open(tmp_filename, "wb")
     f.write(blanck)
     f.write(zdata.flatten())
     f.write(blanck)
     f.close()
 
-    recording = BinaryRecordingExtractor(tmp_filename, num_chan=num_chans, sampling_frequency=fs, dtype="float32")
+    recording = BinaryRecordingExtractor(tmp_filename, num_channels=num_chans, sampling_frequency=fs, dtype="float32")
     recording.annotate(is_filtered=True)
 
     margin = 2 * max(waveform_extractor.nbefore, waveform_extractor.nafter)
     half_marging = margin // 2
 
     chunk_size = duration + 3 * margin
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/isocut5.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/isocut5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/main.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/main.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/method_list.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/method_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_features.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position_and_features.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/random_projections.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/random_projections.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/triage.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/clustering/triage.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/features_from_peaks.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/features_from_peaks.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/circus.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/main.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/main.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/naive.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/naive.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/tdc.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/tdc.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/wobble.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/matching/wobble.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_estimation.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/motion_estimation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_interpolation.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/motion_interpolation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_detection.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_detection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_localization.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_pipeline.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_pipeline.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_selection.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/peak_selection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/tools.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py` & `spikeinterface-0.98.2/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/all_amplitudes_distributions.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/all_amplitudes_distributions.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/amplitudes.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/base.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/base.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/crosscorrelograms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/crosscorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/amplitudes.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spike_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/timeseries.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/utils.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/ipywidgets/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/amplitudes.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/autocorrelograms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/base_mpl.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/base_mpl.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/motion.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/motion.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spike_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/template_similarity.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/timeseries.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_depths.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_depths.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_summary.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_waveforms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/motion.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/motion.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/quality_metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sorting_summary.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sorting_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/__init__.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/amplitudes.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/autocorrelograms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/base_sortingview.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/base_sortingview.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,17 @@
             else:
                 return False  # Other type (?)
         except NameError:
             return False
 
     def handle_display_and_url(self, view, **backend_kwargs):
         self.set_view(view)
-        if self.is_notebook() and backend_kwargs["display"]:
-            display(self.view.jupyter(height=backend_kwargs["height"]))
+        # figurl_jupyter is broken. Comment it out for now.
+        # if self.is_notebook() and backend_kwargs["display"]:
+        #     display(self.view.jupyter(height=backend_kwargs["height"]))
         if backend_kwargs["generate_url"]:
             figlabel = backend_kwargs.get("figlabel")
             if figlabel is None:
                 figlabel = self.default_label
             url = view.url(label=figlabel)
             self.set_url(url)
             print(url)
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/crosscorrelograms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/crosscorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/sorting_summary.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/sorting_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/spike_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/template_similarity.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/timeseries.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_templates.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/sortingview/unit_templates.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/spike_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/spikes_on_traces.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/spikes_on_traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/template_metrics.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/template_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/template_similarity.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/timeseries.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_depths.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/unit_depths.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_locations.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_summary.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/unit_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/unit_waveforms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms_density_map.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/unit_waveforms_density_map.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/utils.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface/widgets/widget_list.py` & `spikeinterface-0.98.2/src/spikeinterface/widgets/widget_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface.egg-info/PKG-INFO` & `spikeinterface-0.98.2/src/spikeinterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface
-Version: 0.98.1
+Version: 0.98.2
 Summary: Python toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface
 Project-URL: documentation, https://spikeinterface.readthedocs.io/
 Project-URL: changelog, https://spikeinterface.readthedocs.io/en/latest/whatisnew.html
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.1 Summary: Python
+Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.2 Summary: Python
 toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino
 buccino@gmail.com>, Samuel Garcia
 garcia.die@gmail.com> Project-URL: homepage, https://github.com/SpikeInterface/
 spikeinterface Project-URL: repository, https://github.com/SpikeInterface/
 spikeinterface Project-URL: documentation, https://
 spikeinterface.readthedocs.io/ Project-URL: changelog, https://
```

### Comparing `spikeinterface-0.98.1/src/spikeinterface.egg-info/SOURCES.txt` & `spikeinterface-0.98.2/src/spikeinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.1/src/spikeinterface.egg-info/requires.txt` & `spikeinterface-0.98.2/src/spikeinterface.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Sphinx==5.1.1
 sphinx_rtd_theme==1.0.0
 sphinx-gallery
 numpydoc
 MEArec
 datalad==0.16.2
 pandas
-hdbscan
+hdbscan>=0.8.33
 numba
 
 [extractors]
 MEArec>=1.8
 pynwb>=2.3.0
 pyedflib>=0.1.30
 lxml
@@ -54,28 +54,26 @@
 
 [test]
 pytest
 pytest-cov
 zarr
 xarray
 huggingface_hub
-numpy<1.24
 numba
-hdbscan
+hdbscan>=0.8.33
 sortingview
 datalad==0.16.2
-tridesclous>=1.6.6.1
+tridesclous>=1.6.8
 pymde
 torch
 pynndescent
 
 [test_core]
 pytest
 zarr
 psutil
 
 [widgets]
 matplotlib
 ipympl
 ipywidgets
 sortingview>=0.11.15
-figurl-jupyter
```

