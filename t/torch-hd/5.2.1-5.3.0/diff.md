# Comparing `tmp/torch-hd-5.2.1.tar.gz` & `tmp/torch-hd-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-hd-5.2.1.tar", last modified: Sat Jul  8 22:00:35 2023, max compression
+gzip compressed data, was "torch-hd-5.3.0.tar", last modified: Thu Jul 20 21:21:55 2023, max compression
```

## Comparing `torch-hd-5.2.1.tar` & `torch-hd-5.3.0.tar`

### file list

```diff
@@ -1,181 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.664175 torch-hd-5.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-08 22:00:25.000000 torch-hd-5.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-08 22:00:35.664175 torch-hd-5.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-08 22:00:25.000000 torch-hd-5.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 22:00:35.664175 torch-hd-5.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-08 22:00:25.000000 torch-hd-5.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.628174 torch-hd-5.2.1/torch_hd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 22:00:35.000000 torch-hd-5.2.1/torch_hd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.628174 torch-hd-5.2.1/torchhd/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.656175 torch-hd-5.2.1/torchhd/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/abalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/acute_inflammation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/acute_nephritis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/adult.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/airfoil_self_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/annealing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/arrhythmia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/audiology_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/balance_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/beijing_air_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/blood.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_diag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_prog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/breast_tissue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/car.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/cardiotocography_10clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/cardiotocography_3clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ccpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/chess_krvk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/chess_krvkp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/congressional_voting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/conn_bench_sonar_mines_rocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/conn_bench_vowel_deterding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/connect_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/contrac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/credit_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/cylinder_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/dermatology.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/echocardiogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ecoli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/emg_hand_gestures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/energy_y1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/energy_y2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/european_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/fertility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/glass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/haberman_survival.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/hayes_roth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_cleveland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_hungarian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_switzerland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/heart_va.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/hepatitis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/hill_valley.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/horse_colic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ilpd_indian_liver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ionosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/isolet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/led_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/letter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/libras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/low_res_spect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/lung_cancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/lymphography.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/mammographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/miniboone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/molec_biol_promoter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/molec_biol_splice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/monks_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/monks_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/monks_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/mushroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/musk_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/musk_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/nursery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_nucleus_4d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_states_2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_states_5b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/optical.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ozone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/page_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pamap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/parkinsons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pendigits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_material.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_rel_l.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_t_or_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/planning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/plant_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/plant_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/plant_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/post_operative.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/primary_tumor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ringnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/semeion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/soybean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/spambase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/spect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/spectf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_australian_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_german_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_heart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_landsat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_shuttle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/statlog_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/steel_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/synthetic_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/teaching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/thyroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/trains.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/twonorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/ucihar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/vertebral_column_2clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/vertebral_column_3clases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wall_following.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/waveform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wine_quality_red.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/wine_quality_white.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/yeast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/datasets/zoo.py
--rw-r--r--   0 runner    (1001) docker     (123)    49027 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)    59891 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    38319 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.660174 torch-hd-5.2.1/torchhd/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/bsc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/fhrr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/hrr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tensors/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.624174 torch-hd-5.2.1/torchhd/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.660174 torch-hd-5.2.1/torchhd/tests/basis_hv/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_base_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_circular_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_empty_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_identity_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_level_hv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/basis_hv/test_random_hv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:00:35.664175 torch-hd-5.2.1/torchhd/tests/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_distinct_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_hashtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_multiset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/tests/structures/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-08 22:00:25.000000 torch-hd-5.2.1/torchhd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.990383 torch-hd-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-20 21:21:45.000000 torch-hd-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-20 21:21:55.990383 torch-hd-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-20 21:21:45.000000 torch-hd-5.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:21:55.990383 torch-hd-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-20 21:21:45.000000 torch-hd-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.970383 torch-hd-5.3.0/torch_hd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-20 21:21:55.000000 torch-hd-5.3.0/torch_hd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-20 21:21:55.000000 torch-hd-5.3.0/torch_hd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:21:55.000000 torch-hd-5.3.0/torch_hd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-20 21:21:55.000000 torch-hd-5.3.0/torch_hd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 21:21:55.000000 torch-hd-5.3.0/torch_hd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.970383 torch-hd-5.3.0/torchhd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.986383 torch-hd-5.3.0/torchhd/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/abalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/acute_inflammation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/acute_nephritis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/adult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/airfoil_self_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/annealing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/arrhythmia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/audiology_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/balance_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/beijing_air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/blood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/breast_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/breast_cancer_wisc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/breast_cancer_wisc_diag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/breast_cancer_wisc_prog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/breast_tissue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/cardiotocography_10clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/cardiotocography_3clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/ccpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/chess_krvk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/chess_krvkp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/congressional_voting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/conn_bench_sonar_mines_rocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/conn_bench_vowel_deterding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/connect_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/contrac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/credit_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/cylinder_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/dermatology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/echocardiogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/ecoli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/emg_hand_gestures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/energy_y1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/energy_y2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/european_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/fertility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/glass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/haberman_survival.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/hayes_roth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/heart_cleveland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/heart_hungarian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/heart_switzerland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/heart_va.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/hepatitis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/hill_valley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/horse_colic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/ilpd_indian_liver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/ionosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/isolet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/led_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/letter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/libras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/low_res_spect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/lung_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/lymphography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/mammographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/miniboone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/molec_biol_promoter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/molec_biol_splice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/monks_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/monks_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/monks_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/mushroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/musk_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/musk_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/nursery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/oocytes_merluccius_nucleus_4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/oocytes_merluccius_states_2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/oocytes_trisopterus_states_5b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/optical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/ozone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/page_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pamap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/parkinsons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pendigits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_rel_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_t_or_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/planning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/plant_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/plant_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/plant_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/post_operative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/primary_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/ringnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/semeion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/soybean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/spambase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/spect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/spectf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/statlog_australian_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/statlog_german_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/statlog_heart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/statlog_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/statlog_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/statlog_shuttle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/statlog_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/steel_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/synthetic_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/teaching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/thyroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/trains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/twonorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/ucihar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/vertebral_column_2clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/vertebral_column_3clases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/wall_following.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/waveform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/wine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/wine_quality_red.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/wine_quality_white.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/yeast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/datasets/zoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50034 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60230 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38319 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.986383 torch-hd-5.3.0/torchhd/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/bsbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/bsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/fhrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/hrr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tensors/vtb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.970383 torch-hd-5.3.0/torchhd/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.986383 torch-hd-5.3.0/torchhd/tests/basis_hv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/basis_hv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/basis_hv/test_base_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/basis_hv/test_circular_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/basis_hv/test_empty_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/basis_hv/test_identity_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/basis_hv/test_level_hv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/basis_hv/test_random_hv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:21:55.990383 torch-hd-5.3.0/torchhd/tests/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_distinct_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_hashtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_multiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/tests/structures/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-20 21:21:45.000000 torch-hd-5.3.0/torchhd/version.py
```

### Comparing `torch-hd-5.2.1/LICENSE` & `torch-hd-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/PKG-INFO` & `torch-hd-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-hd
-Version: 5.2.1
+Version: 5.3.0
 Summary: Torchhd is a Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd
 License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torch-hd Version: 5.2.1 Summary: Torchhd is a
+Metadata-Version: 2.1 Name: torch-hd Version: 5.3.0 Summary: Torchhd is a
 Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io Requires-Python:
 >=3.6, <4 Description-Content-Type: text/markdown License-File: LICENSE
   [GitHub_license] [pypi_version] [conda_version] [tests_status][PRs Welcome]
                                 [Torchhd_logo]
```

### Comparing `torch-hd-5.2.1/README.md` & `torch-hd-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/setup.py` & `torch-hd-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torch_hd.egg-info/PKG-INFO` & `torch-hd-5.3.0/torch_hd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-hd
-Version: 5.2.1
+Version: 5.3.0
 Summary: Torchhd is a Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd
 License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torch-hd Version: 5.2.1 Summary: Torchhd is a
+Metadata-Version: 2.1 Name: torch-hd Version: 5.3.0 Summary: Torchhd is a
 Python library for Hyperdimensional Computing and Vector Symbolic Architectures
 Home-page: https://github.com/hyperdimensional-computing/torchhd License: MIT
 Project-URL: Source, https://github.com/hyperdimensional-computing/torchhd
 Project-URL: Documentation, https://torchhd.readthedocs.io Requires-Python:
 >=3.6, <4 Description-Content-Type: text/markdown License-File: LICENSE
   [GitHub_license] [pypi_version] [conda_version] [tests_status][PRs Welcome]
                                 [Torchhd_logo]
```

### Comparing `torch-hd-5.2.1/torch_hd.egg-info/SOURCES.txt` & `torch-hd-5.3.0/torch_hd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -145,18 +145,20 @@
 torchhd/datasets/wine.py
 torchhd/datasets/wine_quality_red.py
 torchhd/datasets/wine_quality_white.py
 torchhd/datasets/yeast.py
 torchhd/datasets/zoo.py
 torchhd/tensors/__init__.py
 torchhd/tensors/base.py
+torchhd/tensors/bsbc.py
 torchhd/tensors/bsc.py
 torchhd/tensors/fhrr.py
 torchhd/tensors/hrr.py
 torchhd/tensors/map.py
+torchhd/tensors/vtb.py
 torchhd/tests/basis_hv/__init__.py
 torchhd/tests/basis_hv/test_base_tensor.py
 torchhd/tests/basis_hv/test_circular_hv.py
 torchhd/tests/basis_hv/test_empty_hv.py
 torchhd/tests/basis_hv/test_identity_hv.py
 torchhd/tests/basis_hv/test_level_hv.py
 torchhd/tests/basis_hv/test_random_hv.py
```

### Comparing `torch-hd-5.2.1/torchhd/__init__.py` & `torch-hd-5.3.0/torchhd/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 import torchhd.utils as utils
 
 from torchhd.tensors.base import VSATensor
 from torchhd.tensors.bsc import BSCTensor
 from torchhd.tensors.map import MAPTensor
 from torchhd.tensors.hrr import HRRTensor
 from torchhd.tensors.fhrr import FHRRTensor
+from torchhd.tensors.bsbc import BSBCTensor
+from torchhd.tensors.vtb import VTBTensor
 
 from torchhd.functional import (
     ensure_vsa_tensor,
     empty,
     identity,
     random,
     level,
@@ -80,14 +82,16 @@
 __all__ = [
     "__version__",
     "VSATensor",
     "BSCTensor",
     "MAPTensor",
     "HRRTensor",
     "FHRRTensor",
+    "BSBCTensor",
+    "VTBTensor",
     "functional",
     "embeddings",
     "structures",
     "models",
     "memory",
     "datasets",
     "utils",
```

### Comparing `torch-hd-5.2.1/torchhd/datasets/__init__.py` & `torch-hd-5.3.0/torchhd/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/abalone.py` & `torch-hd-5.3.0/torchhd/datasets/abalone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/acute_inflammation.py` & `torch-hd-5.3.0/torchhd/datasets/acute_inflammation.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/acute_nephritis.py` & `torch-hd-5.3.0/torchhd/datasets/acute_nephritis.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/adult.py` & `torch-hd-5.3.0/torchhd/datasets/adult.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/airfoil_self_noise.py` & `torch-hd-5.3.0/torchhd/datasets/airfoil_self_noise.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/annealing.py` & `torch-hd-5.3.0/torchhd/datasets/annealing.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/arrhythmia.py` & `torch-hd-5.3.0/torchhd/datasets/arrhythmia.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/audiology_std.py` & `torch-hd-5.3.0/torchhd/datasets/audiology_std.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/balance_scale.py` & `torch-hd-5.3.0/torchhd/datasets/balance_scale.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/balloons.py` & `torch-hd-5.3.0/torchhd/datasets/balloons.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/bank.py` & `torch-hd-5.3.0/torchhd/datasets/bank.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/beijing_air_quality.py` & `torch-hd-5.3.0/torchhd/datasets/beijing_air_quality.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/blood.py` & `torch-hd-5.3.0/torchhd/datasets/blood.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/breast_cancer.py` & `torch-hd-5.3.0/torchhd/datasets/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc.py` & `torch-hd-5.3.0/torchhd/datasets/breast_cancer_wisc.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_diag.py` & `torch-hd-5.3.0/torchhd/datasets/breast_cancer_wisc_diag.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/breast_cancer_wisc_prog.py` & `torch-hd-5.3.0/torchhd/datasets/breast_cancer_wisc_prog.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/breast_tissue.py` & `torch-hd-5.3.0/torchhd/datasets/breast_tissue.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/car.py` & `torch-hd-5.3.0/torchhd/datasets/car.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/cardiotocography_10clases.py` & `torch-hd-5.3.0/torchhd/datasets/cardiotocography_10clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/cardiotocography_3clases.py` & `torch-hd-5.3.0/torchhd/datasets/cardiotocography_3clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/ccpp.py` & `torch-hd-5.3.0/torchhd/datasets/ccpp.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/chess_krvk.py` & `torch-hd-5.3.0/torchhd/datasets/chess_krvk.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/chess_krvkp.py` & `torch-hd-5.3.0/torchhd/datasets/chess_krvkp.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/congressional_voting.py` & `torch-hd-5.3.0/torchhd/datasets/congressional_voting.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/conn_bench_sonar_mines_rocks.py` & `torch-hd-5.3.0/torchhd/datasets/conn_bench_sonar_mines_rocks.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/conn_bench_vowel_deterding.py` & `torch-hd-5.3.0/torchhd/datasets/conn_bench_vowel_deterding.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/connect_4.py` & `torch-hd-5.3.0/torchhd/datasets/connect_4.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/contrac.py` & `torch-hd-5.3.0/torchhd/datasets/contrac.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/credit_approval.py` & `torch-hd-5.3.0/torchhd/datasets/credit_approval.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/cylinder_bands.py` & `torch-hd-5.3.0/torchhd/datasets/cylinder_bands.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/dataset.py` & `torch-hd-5.3.0/torchhd/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/dermatology.py` & `torch-hd-5.3.0/torchhd/datasets/dermatology.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/echocardiogram.py` & `torch-hd-5.3.0/torchhd/datasets/echocardiogram.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/ecoli.py` & `torch-hd-5.3.0/torchhd/datasets/ecoli.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/emg_hand_gestures.py` & `torch-hd-5.3.0/torchhd/datasets/emg_hand_gestures.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/energy_y1.py` & `torch-hd-5.3.0/torchhd/datasets/energy_y1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/energy_y2.py` & `torch-hd-5.3.0/torchhd/datasets/energy_y2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/european_languages.py` & `torch-hd-5.3.0/torchhd/datasets/european_languages.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/fertility.py` & `torch-hd-5.3.0/torchhd/datasets/fertility.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/flags.py` & `torch-hd-5.3.0/torchhd/datasets/flags.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/glass.py` & `torch-hd-5.3.0/torchhd/datasets/glass.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/haberman_survival.py` & `torch-hd-5.3.0/torchhd/datasets/haberman_survival.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/hayes_roth.py` & `torch-hd-5.3.0/torchhd/datasets/hayes_roth.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/heart_cleveland.py` & `torch-hd-5.3.0/torchhd/datasets/heart_cleveland.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/heart_hungarian.py` & `torch-hd-5.3.0/torchhd/datasets/heart_hungarian.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/heart_switzerland.py` & `torch-hd-5.3.0/torchhd/datasets/heart_switzerland.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/heart_va.py` & `torch-hd-5.3.0/torchhd/datasets/heart_va.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/hepatitis.py` & `torch-hd-5.3.0/torchhd/datasets/hepatitis.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/hill_valley.py` & `torch-hd-5.3.0/torchhd/datasets/hill_valley.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/horse_colic.py` & `torch-hd-5.3.0/torchhd/datasets/horse_colic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/ilpd_indian_liver.py` & `torch-hd-5.3.0/torchhd/datasets/ilpd_indian_liver.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/image_segmentation.py` & `torch-hd-5.3.0/torchhd/datasets/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/ionosphere.py` & `torch-hd-5.3.0/torchhd/datasets/ionosphere.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/iris.py` & `torch-hd-5.3.0/torchhd/datasets/iris.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/isolet.py` & `torch-hd-5.3.0/torchhd/datasets/isolet.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/led_display.py` & `torch-hd-5.3.0/torchhd/datasets/led_display.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/lenses.py` & `torch-hd-5.3.0/torchhd/datasets/lenses.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/letter.py` & `torch-hd-5.3.0/torchhd/datasets/letter.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/libras.py` & `torch-hd-5.3.0/torchhd/datasets/libras.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/low_res_spect.py` & `torch-hd-5.3.0/torchhd/datasets/low_res_spect.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/lung_cancer.py` & `torch-hd-5.3.0/torchhd/datasets/lung_cancer.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/lymphography.py` & `torch-hd-5.3.0/torchhd/datasets/lymphography.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/magic.py` & `torch-hd-5.3.0/torchhd/datasets/magic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/mammographic.py` & `torch-hd-5.3.0/torchhd/datasets/mammographic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/miniboone.py` & `torch-hd-5.3.0/torchhd/datasets/miniboone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/molec_biol_promoter.py` & `torch-hd-5.3.0/torchhd/datasets/molec_biol_promoter.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/molec_biol_splice.py` & `torch-hd-5.3.0/torchhd/datasets/molec_biol_splice.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/monks_1.py` & `torch-hd-5.3.0/torchhd/datasets/monks_1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/monks_2.py` & `torch-hd-5.3.0/torchhd/datasets/monks_2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/monks_3.py` & `torch-hd-5.3.0/torchhd/datasets/monks_3.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/mushroom.py` & `torch-hd-5.3.0/torchhd/datasets/mushroom.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/musk_1.py` & `torch-hd-5.3.0/torchhd/datasets/musk_1.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/musk_2.py` & `torch-hd-5.3.0/torchhd/datasets/musk_2.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/nursery.py` & `torch-hd-5.3.0/torchhd/datasets/nursery.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_nucleus_4d.py` & `torch-hd-5.3.0/torchhd/datasets/oocytes_merluccius_nucleus_4d.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/oocytes_merluccius_states_2f.py` & `torch-hd-5.3.0/torchhd/datasets/oocytes_merluccius_states_2f.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py` & `torch-hd-5.3.0/torchhd/datasets/oocytes_trisopterus_nucleus_2f.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/oocytes_trisopterus_states_5b.py` & `torch-hd-5.3.0/torchhd/datasets/oocytes_trisopterus_states_5b.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/optical.py` & `torch-hd-5.3.0/torchhd/datasets/optical.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/ozone.py` & `torch-hd-5.3.0/torchhd/datasets/ozone.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/page_blocks.py` & `torch-hd-5.3.0/torchhd/datasets/page_blocks.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pamap.py` & `torch-hd-5.3.0/torchhd/datasets/pamap.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/parkinsons.py` & `torch-hd-5.3.0/torchhd/datasets/parkinsons.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pendigits.py` & `torch-hd-5.3.0/torchhd/datasets/pendigits.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pima.py` & `torch-hd-5.3.0/torchhd/datasets/pima.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_material.py` & `torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_material.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_rel_l.py` & `torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_rel_l.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_span.py` & `torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_span.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_t_or_d.py` & `torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_t_or_d.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/pittsburg_bridges_type.py` & `torch-hd-5.3.0/torchhd/datasets/pittsburg_bridges_type.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/planning.py` & `torch-hd-5.3.0/torchhd/datasets/planning.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/plant_margin.py` & `torch-hd-5.3.0/torchhd/datasets/plant_margin.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/plant_shape.py` & `torch-hd-5.3.0/torchhd/datasets/plant_shape.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/plant_texture.py` & `torch-hd-5.3.0/torchhd/datasets/plant_texture.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/post_operative.py` & `torch-hd-5.3.0/torchhd/datasets/post_operative.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/primary_tumor.py` & `torch-hd-5.3.0/torchhd/datasets/primary_tumor.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/ringnorm.py` & `torch-hd-5.3.0/torchhd/datasets/ringnorm.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/seeds.py` & `torch-hd-5.3.0/torchhd/datasets/seeds.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/semeion.py` & `torch-hd-5.3.0/torchhd/datasets/semeion.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/soybean.py` & `torch-hd-5.3.0/torchhd/datasets/soybean.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/spambase.py` & `torch-hd-5.3.0/torchhd/datasets/spambase.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/spect.py` & `torch-hd-5.3.0/torchhd/datasets/spect.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/spectf.py` & `torch-hd-5.3.0/torchhd/datasets/spectf.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/statlog_australian_credit.py` & `torch-hd-5.3.0/torchhd/datasets/statlog_australian_credit.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/statlog_german_credit.py` & `torch-hd-5.3.0/torchhd/datasets/statlog_german_credit.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/statlog_heart.py` & `torch-hd-5.3.0/torchhd/datasets/statlog_heart.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/statlog_image.py` & `torch-hd-5.3.0/torchhd/datasets/statlog_image.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/statlog_landsat.py` & `torch-hd-5.3.0/torchhd/datasets/statlog_landsat.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/statlog_shuttle.py` & `torch-hd-5.3.0/torchhd/datasets/statlog_shuttle.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/statlog_vehicle.py` & `torch-hd-5.3.0/torchhd/datasets/statlog_vehicle.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/steel_plates.py` & `torch-hd-5.3.0/torchhd/datasets/steel_plates.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/synthetic_control.py` & `torch-hd-5.3.0/torchhd/datasets/synthetic_control.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/teaching.py` & `torch-hd-5.3.0/torchhd/datasets/teaching.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/thyroid.py` & `torch-hd-5.3.0/torchhd/datasets/thyroid.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/tic_tac_toe.py` & `torch-hd-5.3.0/torchhd/datasets/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/titanic.py` & `torch-hd-5.3.0/torchhd/datasets/titanic.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/trains.py` & `torch-hd-5.3.0/torchhd/datasets/trains.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/twonorm.py` & `torch-hd-5.3.0/torchhd/datasets/twonorm.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/ucihar.py` & `torch-hd-5.3.0/torchhd/datasets/ucihar.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/utils.py` & `torch-hd-5.3.0/torchhd/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/vertebral_column_2clases.py` & `torch-hd-5.3.0/torchhd/datasets/vertebral_column_2clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/vertebral_column_3clases.py` & `torch-hd-5.3.0/torchhd/datasets/vertebral_column_3clases.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/wall_following.py` & `torch-hd-5.3.0/torchhd/datasets/wall_following.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/waveform.py` & `torch-hd-5.3.0/torchhd/datasets/waveform.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/waveform_noise.py` & `torch-hd-5.3.0/torchhd/datasets/waveform_noise.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/wine.py` & `torch-hd-5.3.0/torchhd/datasets/wine.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/wine_quality_red.py` & `torch-hd-5.3.0/torchhd/datasets/wine_quality_red.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/wine_quality_white.py` & `torch-hd-5.3.0/torchhd/datasets/wine_quality_white.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/yeast.py` & `torch-hd-5.3.0/torchhd/datasets/yeast.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/datasets/zoo.py` & `torch-hd-5.3.0/torchhd/datasets/zoo.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/embeddings.py` & `torch-hd-5.3.0/torchhd/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,22 +104,24 @@
         padding_idx: Optional[int] = None,
         max_norm: Optional[float] = None,
         norm_type: float = 2.0,
         scale_grad_by_freq: bool = False,
         sparse: bool = False,
         device=None,
         dtype=None,
+        **kwargs,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         # Have to call Module init explicitly in order not to use the Embedding init
         nn.Module.__init__(self)
 
         self.num_embeddings = num_embeddings
         self.embedding_dim = embedding_dim
         self.vsa = vsa
+        self.vsa_kwargs = kwargs
 
         if padding_idx is not None:
             if padding_idx > 0:
                 assert (
                     padding_idx < self.num_embeddings
                 ), "Padding_idx must be within num_embeddings"
             elif padding_idx < 0:
@@ -131,28 +133,32 @@
         self.padding_idx = padding_idx
         self.max_norm = max_norm
         self.norm_type = norm_type
         self.scale_grad_by_freq = scale_grad_by_freq
         self.sparse = sparse
 
         embeddings = functional.empty(
-            num_embeddings, embedding_dim, self.vsa, **factory_kwargs
+            num_embeddings, embedding_dim, self.vsa, **factory_kwargs, **self.vsa_kwargs
         )
         # Have to provide requires grad at the creation of the parameters to
         # prevent errors when instantiating a non-float embedding
         self.weight = Parameter(embeddings, requires_grad=requires_grad)
 
         # we don't need to set the padding to empty because it is already empty.
 
     def reset_parameters(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
 
         with torch.no_grad():
             embeddings = functional.empty(
-                self.num_embeddings, self.embedding_dim, self.vsa, **factory_kwargs
+                self.num_embeddings,
+                self.embedding_dim,
+                self.vsa,
+                **factory_kwargs,
+                **self.vsa_kwargs,
             )
             self.weight.copy_(embeddings)
 
     def forward(self, input: Tensor) -> Tensor:
         vsa_tensor = functional.get_vsa_tensor_class(self.vsa)
         return super().forward(input).as_subclass(vsa_tensor)
 
@@ -210,22 +216,24 @@
         padding_idx: Optional[int] = None,
         max_norm: Optional[float] = None,
         norm_type: float = 2.0,
         scale_grad_by_freq: bool = False,
         sparse: bool = False,
         device=None,
         dtype=None,
+        **kwargs,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         # Have to call Module init explicitly in order not to use the Embedding init
         nn.Module.__init__(self)
 
         self.num_embeddings = num_embeddings
         self.embedding_dim = embedding_dim
         self.vsa = vsa
+        self.vsa_kwargs = kwargs
 
         if padding_idx is not None:
             if padding_idx > 0:
                 assert (
                     padding_idx < self.num_embeddings
                 ), "Padding_idx must be within num_embeddings"
             elif padding_idx < 0:
@@ -237,40 +245,44 @@
         self.padding_idx = padding_idx
         self.max_norm = max_norm
         self.norm_type = norm_type
         self.scale_grad_by_freq = scale_grad_by_freq
         self.sparse = sparse
 
         embeddings = functional.identity(
-            num_embeddings, embedding_dim, self.vsa, **factory_kwargs
+            num_embeddings, embedding_dim, self.vsa, **factory_kwargs, **self.vsa_kwargs
         )
         # Have to provide requires grad at the creation of the parameters to
         # prevent errors when instantiating a non-float embedding
         self.weight = Parameter(embeddings, requires_grad=requires_grad)
 
         self._fill_padding_idx_with_empty()
 
     def reset_parameters(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
 
         with torch.no_grad():
             embeddings = functional.identity(
-                self.num_embeddings, self.embedding_dim, self.vsa, **factory_kwargs
+                self.num_embeddings,
+                self.embedding_dim,
+                self.vsa,
+                **factory_kwargs,
+                **self.vsa_kwargs,
             )
             self.weight.copy_(embeddings)
 
         self._fill_padding_idx_with_empty()
 
     def _fill_padding_idx_with_empty(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
 
         if self.padding_idx is not None:
             with torch.no_grad():
                 empty = functional.empty(
-                    1, self.embedding_dim, self.vsa, **factory_kwargs
+                    1, self.embedding_dim, self.vsa, **factory_kwargs, **self.vsa_kwargs
                 )
                 self.weight[self.padding_idx].copy_(empty.squeeze(0))
 
     def forward(self, input: Tensor) -> Tensor:
         vsa_tensor = functional.get_vsa_tensor_class(self.vsa)
         return super().forward(input).as_subclass(vsa_tensor)
 
@@ -328,22 +340,24 @@
         padding_idx: Optional[int] = None,
         max_norm: Optional[float] = None,
         norm_type: float = 2.0,
         scale_grad_by_freq: bool = False,
         sparse: bool = False,
         device=None,
         dtype=None,
+        **kwargs,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         # Have to call Module init explicitly in order not to use the Embedding init
         nn.Module.__init__(self)
 
         self.num_embeddings = num_embeddings
         self.embedding_dim = embedding_dim
         self.vsa = vsa
+        self.vsa_kwargs = kwargs
 
         if padding_idx is not None:
             if padding_idx > 0:
                 assert (
                     padding_idx < self.num_embeddings
                 ), "Padding_idx must be within num_embeddings"
             elif padding_idx < 0:
@@ -355,40 +369,44 @@
         self.padding_idx = padding_idx
         self.max_norm = max_norm
         self.norm_type = norm_type
         self.scale_grad_by_freq = scale_grad_by_freq
         self.sparse = sparse
 
         embeddings = functional.random(
-            num_embeddings, embedding_dim, self.vsa, **factory_kwargs
+            num_embeddings, embedding_dim, self.vsa, **factory_kwargs, **self.vsa_kwargs
         )
         # Have to provide requires grad at the creation of the parameters to
         # prevent errors when instantiating a non-float embedding
         self.weight = Parameter(embeddings, requires_grad=requires_grad)
 
         self._fill_padding_idx_with_empty()
 
     def reset_parameters(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
 
         with torch.no_grad():
             embeddings = functional.random(
-                self.num_embeddings, self.embedding_dim, self.vsa, **factory_kwargs
+                self.num_embeddings,
+                self.embedding_dim,
+                self.vsa,
+                **factory_kwargs,
+                **self.vsa_kwargs,
             )
             self.weight.copy_(embeddings)
 
         self._fill_padding_idx_with_empty()
 
     def _fill_padding_idx_with_empty(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
 
         if self.padding_idx is not None:
             with torch.no_grad():
                 empty = functional.empty(
-                    1, self.embedding_dim, self.vsa, **factory_kwargs
+                    1, self.embedding_dim, self.vsa, **factory_kwargs, **self.vsa_kwargs
                 )
                 self.weight[self.padding_idx].copy_(empty.squeeze(0))
 
     def forward(self, input: Tensor) -> Tensor:
         vsa_tensor = functional.get_vsa_tensor_class(self.vsa)
         return super().forward(input).as_subclass(vsa_tensor)
 
@@ -465,22 +483,24 @@
         requires_grad: bool = False,
         max_norm: Optional[float] = None,
         norm_type: float = 2.0,
         scale_grad_by_freq: bool = False,
         sparse: bool = False,
         device=None,
         dtype=None,
+        **kwargs,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         # Have to call Module init explicitly in order not to use the Embedding init
         nn.Module.__init__(self)
 
         self.num_embeddings = num_embeddings
         self.embedding_dim = embedding_dim
         self.vsa = vsa
+        self.vsa_kwargs = kwargs
         self.low = low
         self.high = high
         self.randomness = randomness
 
         self.padding_idx = None
         self.max_norm = max_norm
         self.norm_type = norm_type
@@ -489,14 +509,15 @@
 
         embeddings = functional.level(
             num_embeddings,
             embedding_dim,
             self.vsa,
             randomness=randomness,
             **factory_kwargs,
+            **self.vsa_kwargs,
         )
         # Have to provide requires grad at the creation of the parameters to
         # prevent errors when instantiating a non-float embedding
         self.weight = Parameter(embeddings, requires_grad=requires_grad)
 
     def reset_parameters(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
@@ -504,14 +525,15 @@
         with torch.no_grad():
             embeddings = functional.level(
                 self.num_embeddings,
                 self.embedding_dim,
                 self.vsa,
                 randomness=self.randomness,
                 **factory_kwargs,
+                **self.vsa_kwargs,
             )
             self.weight.copy_(embeddings)
 
     def forward(self, input: Tensor) -> Tensor:
         index = functional.value_to_index(
             input, self.low, self.high, self.num_embeddings
         )
@@ -588,44 +610,50 @@
         requires_grad: bool = False,
         max_norm: Optional[float] = None,
         norm_type: float = 2.0,
         scale_grad_by_freq: bool = False,
         sparse: bool = False,
         device=None,
         dtype=None,
+        **kwargs,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         # Have to call Module init explicitly in order not to use the Embedding init
         nn.Module.__init__(self)
 
         self.num_embeddings = num_embeddings
         self.embedding_dim = embedding_dim
         self.vsa = vsa
+        self.vsa_kwargs = kwargs
         self.low = low
         self.high = high
 
         self.padding_idx = None
         self.max_norm = max_norm
         self.norm_type = norm_type
         self.scale_grad_by_freq = scale_grad_by_freq
         self.sparse = sparse
 
         embeddings = functional.thermometer(
-            num_embeddings, embedding_dim, self.vsa, **factory_kwargs
+            num_embeddings, embedding_dim, self.vsa, **factory_kwargs, **self.vsa_kwargs
         )
         # Have to provide requires grad at the creation of the parameters to
         # prevent errors when instantiating a non-float embedding
         self.weight = Parameter(embeddings, requires_grad=requires_grad)
 
     def reset_parameters(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
 
         with torch.no_grad():
             embeddings = functional.thermometer(
-                self.num_embeddings, self.embedding_dim, self.vsa, **factory_kwargs
+                self.num_embeddings,
+                self.embedding_dim,
+                self.vsa,
+                **factory_kwargs,
+                **self.vsa_kwargs,
             )
             self.weight.copy_(embeddings)
 
     def forward(self, input: Tensor) -> Tensor:
         index = functional.value_to_index(
             input, self.low, self.high, self.num_embeddings
         )
@@ -700,22 +728,24 @@
         requires_grad: bool = False,
         max_norm: Optional[float] = None,
         norm_type: float = 2.0,
         scale_grad_by_freq: bool = False,
         sparse: bool = False,
         device=None,
         dtype=None,
+        **kwargs,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         # Have to call Module init explicitly in order not to use the Embedding init
         nn.Module.__init__(self)
 
         self.num_embeddings = num_embeddings
         self.embedding_dim = embedding_dim
         self.vsa = vsa
+        self.vsa_kwargs = kwargs
         self.phase = phase
         self.period = period
         self.randomness = randomness
 
         self.padding_idx = None
         self.max_norm = max_norm
         self.norm_type = norm_type
@@ -724,14 +754,15 @@
 
         embeddings = functional.circular(
             num_embeddings,
             embedding_dim,
             self.vsa,
             randomness=randomness,
             **factory_kwargs,
+            **self.vsa_kwargs,
         )
         # Have to provide requires grad at the creation of the parameters to
         # prevent errors when instantiating a non-float embedding
         self.weight = Parameter(embeddings, requires_grad=requires_grad)
 
     def reset_parameters(self) -> None:
         factory_kwargs = {"device": self.weight.device, "dtype": self.weight.dtype}
@@ -739,14 +770,15 @@
         with torch.no_grad():
             embeddings = functional.circular(
                 self.num_embeddings,
                 self.embedding_dim,
                 self.vsa,
                 randomness=self.randomness,
                 **factory_kwargs,
+                **self.vsa_kwargs,
             )
             self.weight.copy_(embeddings)
 
     def forward(self, input: Tensor) -> Tensor:
         mapped = functional.map_range(
             input, self.phase, self.period, 0, self.num_embeddings
         )
@@ -802,17 +834,17 @@
     ):
         factory_kwargs = {"device": device, "dtype": dtype}
         super(Projection, self).__init__()
         self.in_features = in_features
         self.out_features = out_features
         self.vsa = vsa
 
-        if vsa not in {"MAP", "HRR"}:
+        if vsa not in {"MAP", "HRR", "VTB"}:
             raise ValueError(
-                f"Projection embedding only supports MAP and HRR but provided: {vsa}"
+                f"Projection embedding supports MAP, HRR, VTB but provided: {vsa}"
             )
 
         self.weight = nn.parameter.Parameter(
             torch.empty((out_features, in_features), **factory_kwargs),
             requires_grad=requires_grad,
         )
         self.reset_parameters()
@@ -873,17 +905,17 @@
     ):
         factory_kwargs = {"device": device, "dtype": dtype}
         super(Sinusoid, self).__init__()
         self.in_features = in_features
         self.out_features = out_features
         self.vsa = vsa
 
-        if vsa not in {"MAP", "HRR"}:
+        if vsa not in {"MAP", "HRR", "VTB"}:
             raise ValueError(
-                f"Sinusoid embedding only supports MAP and HRR but provided: {vsa}"
+                f"Sinusoid embedding supports MAP, HRR, VTB but provided: {vsa}"
             )
 
         self.weight = nn.parameter.Parameter(
             torch.empty((out_features, in_features), **factory_kwargs),
             requires_grad=requires_grad,
         )
 
@@ -941,27 +973,34 @@
         out_features: int,
         vsa: VSAOptions = "MAP",
         low: float = 0.0,
         high: float = 1.0,
         device=None,
         dtype=None,
         requires_grad: bool = False,
+        **kwargs,
     ):
         factory_kwargs = {
             "device": device,
             "dtype": dtype,
             "requires_grad": requires_grad,
         }
         super(Density, self).__init__()
 
         # A set of random vectors used as unique IDs for features of the dataset.
-        self.key = Random(in_features, out_features, vsa, **factory_kwargs)
+        self.key = Random(in_features, out_features, vsa, **factory_kwargs, **kwargs)
         # Thermometer encoding used for transforming input data.
         self.density_encoding = Thermometer(
-            out_features + 1, out_features, vsa, low=low, high=high, **factory_kwargs
+            out_features + 1,
+            out_features,
+            vsa,
+            low=low,
+            high=high,
+            **factory_kwargs,
+            **kwargs,
         )
 
     def reset_parameters(self) -> None:
         self.key.reset_parameters()
         self.density_encoding.reset_parameters()
 
     # Specify the steps needed to perform the encoding
```

### Comparing `torch-hd-5.2.1/torchhd/functional.py` & `torch-hd-5.3.0/torchhd/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from collections import deque
 
 from torchhd.tensors.base import VSATensor
 from torchhd.tensors.bsc import BSCTensor
 from torchhd.tensors.map import MAPTensor
 from torchhd.tensors.hrr import HRRTensor
 from torchhd.tensors.fhrr import FHRRTensor
+from torchhd.tensors.bsbc import BSBCTensor
+from torchhd.tensors.vtb import VTBTensor
 from torchhd.types import VSAOptions
 
 
 __all__ = [
     "ensure_vsa_tensor",
     "empty",
     "identity",
@@ -78,14 +80,18 @@
         return BSCTensor
     elif vsa == "MAP":
         return MAPTensor
     elif vsa == "HRR":
         return HRRTensor
     elif vsa == "FHRR":
         return FHRRTensor
+    elif vsa == "BSBC":
+        return BSBCTensor
+    elif vsa == "VTB":
+        return VTBTensor
 
     raise ValueError(f"Provided VSA model is not supported, specified: {vsa}")
 
 
 def ensure_vsa_tensor(
     data,
     vsa: VSAOptions = None,
@@ -344,15 +350,18 @@
     )
 
     hv = torch.empty(
         num_vectors,
         dimensions,
         dtype=span_hv.dtype,
         device=span_hv.device,
-    )
+    ).as_subclass(vsa_tensor)
+
+    if vsa == "BSBC":
+        hv.block_size = span_hv.block_size
 
     for i in range(num_vectors):
         span_idx = int(i // levels_per_span)
 
         # special case: if we are on a span border (e.g. on the first or last levels)
         # then set the orthogonal vector directly.
         # This also prevents an index out of bounds error for the last level
@@ -365,15 +374,15 @@
             t = 1 - (level_within_span / levels_per_span)
 
             span_start_hv = span_hv[span_idx]
             span_end_hv = span_hv[span_idx + 1]
             hv[i] = torch.where(threshold_v[span_idx] < t, span_start_hv, span_end_hv)
 
     hv.requires_grad = requires_grad
-    return hv.as_subclass(vsa_tensor)
+    return hv
 
 
 def thermometer(
     num_vectors: int,
     dimensions: int,
     vsa: VSAOptions = "MAP",
     *,
@@ -454,15 +463,15 @@
                 dimensions,
             ),
             -1,
             dtype=rand_hv.dtype,
             device=rand_hv.device,
         )
     else:
-        raise ValueError(f"{vsa_tensor} HD/VSA model is not defined.")
+        raise ValueError(f"{vsa_tensor} HD/VSA model is not (yet) supported.")
 
     # Create hypervectors using the obtained step
     for i in range(1, num_vectors):
         hv[i, 0 : i * step] = 1
 
     hv.requires_grad = requires_grad
     return hv.as_subclass(vsa_tensor)
@@ -536,17 +545,17 @@
                 [ 0.983-0.183j,  0.732+0.680j, -0.727-0.686j, -0.271+0.962j, -0.705-0.709j,  0.562-0.827j],
                 [ 0.983-0.183j,  0.732+0.680j, -0.727-0.686j, -0.271+0.962j, -0.705-0.709j,  0.562-0.827j],
                 [-0.887-0.460j, -0.906+0.421j, -0.727-0.686j, -0.271+0.962j, -0.705-0.709j,  0.562-0.827j]])
 
     """
     vsa_tensor = get_vsa_tensor_class(vsa)
 
-    if vsa_tensor == HRRTensor:
+    if vsa == "HRR" or vsa == "VTB":
         raise ValueError(
-            "The circular hypervectors don't currently work with the HRR model. We are not sure why, if you have any insight that could help please share it at: https://github.com/hyperdimensional-computing/torchhd/issues/108."
+            "The circular hypervectors do currently not work with the HRR and VTB models. We are not sure why, if you have any insight that could help please share it at: https://github.com/hyperdimensional-computing/torchhd/issues/108."
         )
 
     # convert from normalized "randomness" variable r to
     # number of levels between orthogonal pairs or "span"
     levels_per_span = ((1 - randomness) * (num_vectors / 2) + randomness * 1) * 2
     span = num_vectors / levels_per_span
 
@@ -568,15 +577,18 @@
     )
 
     hv = torch.empty(
         num_vectors,
         dimensions,
         dtype=span_hv.dtype,
         device=span_hv.device,
-    )
+    ).as_subclass(vsa_tensor)
+
+    if vsa == "BSBC":
+        hv.block_size = span_hv.block_size
 
     mutation_history = deque()
 
     # first vector is always a random vector
     hv[0] = span_hv[0]
     # mutation hypervector is the last generated vector while walking through the circle
     mutation_hv = span_hv[0]
@@ -611,15 +623,15 @@
         mut = mutation_history.popleft()
         mutation_hv = bind(mutation_hv, inverse(mut))
 
         if i % 2 == 0:
             hv[i // 2] = mutation_hv
 
     hv.requires_grad = requires_grad
-    return hv.as_subclass(vsa_tensor)
+    return hv
 
 
 def bind(input: VSATensor, other: VSATensor) -> VSATensor:
     r"""Binds two hypervectors which produces a hypervector dissimilar to both.
 
     Binding is used to associate information, for instance, to assign values to variables.
```

### Comparing `torch-hd-5.2.1/torchhd/memory.py` & `torch-hd-5.3.0/torchhd/memory.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/models.py` & `torch-hd-5.3.0/torchhd/models.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/structures.py` & `torch-hd-5.3.0/torchhd/structures.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tensors/__init__.py` & `torch-hd-5.3.0/torchhd/tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tensors/base.py` & `torch-hd-5.3.0/torchhd/tensors/base.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tensors/bsc.py` & `torch-hd-5.3.0/torchhd/tensors/bsc.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tensors/fhrr.py` & `torch-hd-5.3.0/torchhd/tensors/fhrr.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tensors/hrr.py` & `torch-hd-5.3.0/torchhd/tensors/hrr.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tensors/map.py` & `torch-hd-5.3.0/torchhd/tensors/map.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/basis_hv/__init__.py` & `torch-hd-5.3.0/torchhd/tests/basis_hv/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/basis_hv/test_base_tensor.py` & `torch-hd-5.3.0/torchhd/tests/basis_hv/test_base_tensor.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/basis_hv/test_circular_hv.py` & `torch-hd-5.3.0/torchhd/tests/basis_hv/test_circular_hv.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,76 +31,104 @@
 from ..utils import torch_dtypes, supported_dtype, vsa_tensors
 
 seed = 2147483644
 
 
 class Testcircular:
     @pytest.mark.parametrize("n", [1, 3, 55])
-    @pytest.mark.parametrize("d", [84, 10])
+    @pytest.mark.parametrize("d", [84, 16])
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_shape(self, n, d, vsa):
-        if vsa == "HRR":
+        if vsa == "HRR" or vsa == "VTB":
             return
 
-        hv = functional.circular(n, d, vsa)
+        if vsa == "BSBC":
+            hv = functional.circular(n, d, vsa, block_size=1024)
+        else:
+            hv = functional.circular(n, d, vsa)
 
         assert hv.dim() == 2
         assert hv.size(0) == n
         assert hv.size(1) == d
 
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_generator(self, vsa):
-        if vsa == "HRR":
+        if vsa == "HRR" or vsa == "VTB":
             return
 
         generator = torch.Generator()
         generator.manual_seed(seed)
-        hv1 = functional.circular(20, 10000, vsa, generator=generator)
+        if vsa == "BSBC":
+            hv1 = functional.circular(
+                20, 10000, vsa, generator=generator, block_size=1024
+            )
+        else:
+            hv1 = functional.circular(20, 10000, vsa, generator=generator)
 
         generator = torch.Generator()
         generator.manual_seed(seed)
-
-        hv2 = functional.circular(20, 10000, vsa, generator=generator)
+        if vsa == "BSBC":
+            hv2 = functional.circular(
+                20, 10000, vsa, generator=generator, block_size=1024
+            )
+        else:
+            hv2 = functional.circular(20, 10000, vsa, generator=generator)
         assert torch.all(hv1 == hv2).item()
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_value(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             with pytest.raises(ValueError):
-                functional.circular(3, 26, vsa, dtype=dtype)
+                if vsa == "BSBC":
+                    functional.circular(3, 26, vsa, dtype=dtype, block_size=1024)
+                else:
+                    functional.circular(3, 26, vsa, dtype=dtype)
 
             return
 
-        if vsa == "HRR":
+        if vsa == "HRR" or vsa == "VTB":
             with pytest.raises(ValueError):
                 functional.circular(3, 26, vsa, dtype=dtype)
 
             return
 
         generator = torch.Generator()
         generator.manual_seed(seed)
 
-        hv = functional.circular(50, 26000, vsa, dtype=dtype, generator=generator)
+        if vsa == "BSBC":
+            hv = functional.circular(
+                50, 26569, vsa, dtype=dtype, generator=generator, block_size=1024
+            )
+        else:
+            hv = functional.circular(50, 26569, vsa, dtype=dtype, generator=generator)
         assert hv.requires_grad == False
         assert hv.dim() == 2
         assert hv.size(0) == 50
-        assert hv.size(1) == 26000
+        assert hv.size(1) == 26569
 
         if vsa == "BSC":
             assert torch.all((hv == False) | (hv == True)).item()
 
         elif vsa == "MAP":
             assert torch.all((hv == -1) | (hv == 1)).item()
 
         elif vsa == "FHRR":
             mag = hv.abs()
             assert torch.allclose(mag, torch.tensor(1.0, dtype=mag.dtype))
 
-        hv = functional.circular(8, 1000000, vsa, generator=generator, dtype=dtype)
+        elif vsa == "BSBC":
+            assert torch.all((hv >= 0) | (hv < 1024)).item()
+
+        if vsa == "BSBC":
+            hv = functional.circular(
+                8, 1000000, vsa, generator=generator, dtype=dtype, block_size=1024
+            )
+        else:
+            hv = functional.circular(8, 1000000, vsa, generator=generator, dtype=dtype)
         sims = functional.cosine_similarity(hv[0], hv)
         sims_diff = sims[:-1] - sims[1:]
         assert torch.all(
             sims_diff.sign() == torch.tensor([1, 1, 1, 1, -1, -1, -1])
         ), "second half must get more similar"
 
         assert torch.allclose(
@@ -130,28 +158,33 @@
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     def test_device(self, dtype):
         if not supported_dtype(dtype):
             return
 
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        hv = functional.circular(3, 52, device=device, dtype=dtype)
+        hv = functional.circular(3, 49, device=device, dtype=dtype)
         assert hv.device.type == device.type
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_device(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             return
 
-        if vsa == "HRR":
+        if vsa == "HRR" or vsa == "VTB":
             return
 
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        hv = functional.circular(3, 52, vsa, device=device, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.circular(
+                3, 52, vsa, device=device, dtype=dtype, block_size=1024
+            )
+        else:
+            hv = functional.circular(3, 49, vsa, device=device, dtype=dtype)
         assert hv.device.type == device.type
 
     def test_uses_default_dtype(self):
         hv = functional.circular(3, 52, "BSC")
         assert hv.dtype == torch.bool
 
         torch.set_default_dtype(torch.float32)
@@ -161,13 +194,16 @@
         torch.set_default_dtype(torch.float64)
         hv = functional.circular(3, 52, "MAP")
         assert hv.dtype == torch.float64
 
         hv = functional.circular(3, 52, "FHRR")
         assert hv.dtype == torch.complex64
 
+        hv = functional.circular(3, 52, "BSBC", block_size=1024)
+        assert hv.dtype == torch.int64
+
     def test_requires_grad(self):
         hv = functional.circular(3, 52, "MAP", requires_grad=True)
         assert hv.requires_grad == True
 
         hv = functional.circular(3, 52, "FHRR", requires_grad=True)
         assert hv.requires_grad == True
```

### Comparing `torch-hd-5.2.1/torchhd/tests/basis_hv/test_empty_hv.py` & `torch-hd-5.3.0/torchhd/tests/basis_hv/test_empty_hv.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,76 +34,109 @@
 )
 
 seed = 2147483644
 
 
 class Testempty:
     @pytest.mark.parametrize("n", [1, 3, 55])
-    @pytest.mark.parametrize("d", [84, 10])
+    @pytest.mark.parametrize("d", [84, 16])
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_shape(self, n, d, vsa):
-        hv = functional.empty(n, d, vsa)
+        if vsa == "BSBC":
+            hv = functional.empty(n, d, vsa, block_size=1024)
+        elif vsa == "VTB" and d == 84:
+            with pytest.raises(ValueError):
+                hv = functional.empty(n, d, vsa)
+
+            return
+        else:
+            hv = functional.empty(n, d, vsa)
 
         assert hv.dim() == 2
         assert hv.size(0) == n
         assert hv.size(1) == d
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_value(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             with pytest.raises(ValueError):
-                functional.empty(3, 26, vsa, dtype=dtype)
+                if vsa == "BSBC":
+                    functional.empty(3, 25, vsa, dtype=dtype, block_size=1024)
+                else:
+                    functional.empty(3, 25, vsa, dtype=dtype)
 
             return
 
-        hv = functional.empty(8, 26, vsa, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.empty(8, 25, vsa, dtype=dtype, block_size=1024)
+        else:
+            hv = functional.empty(8, 25, vsa, dtype=dtype)
+
         assert hv.requires_grad == False
         assert hv.dim() == 2
         assert hv.size(0) == 8
-        assert hv.size(1) == 26
+        assert hv.size(1) == 25
 
         if vsa == "BSC":
             assert torch.all((hv == False) | (hv == True)).item()
 
+        elif vsa == "BSBC":
+            assert torch.all((hv >= 0) | (hv < 1024)).item()
+
         else:
-            hv = functional.empty(8, 26, vsa, dtype=dtype)
+            hv = functional.empty(8, 25, vsa, dtype=dtype)
             assert torch.all(hv == 0.0).item()
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_device(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             return
 
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        hv = functional.empty(3, 52, vsa, device=device, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.empty(
+                3, 52, vsa, device=device, dtype=dtype, block_size=1024
+            )
+        else:
+            hv = functional.empty(3, 49, vsa, device=device, dtype=dtype)
         assert hv.device.type == device.type
 
     def test_uses_default_dtype(self):
-        hv = functional.empty(3, 52, "BSC")
+        hv = functional.empty(3, 49, "BSC")
         assert hv.dtype == torch.bool
 
         torch.set_default_dtype(torch.float32)
-        hv = functional.empty(3, 52, "MAP")
+        hv = functional.empty(3, 49, "MAP")
+        assert hv.dtype == torch.float32
+        hv = functional.empty(3, 49, "HRR")
         assert hv.dtype == torch.float32
-        hv = functional.empty(3, 52, "HRR")
+        hv = functional.empty(3, 49, "VTB")
         assert hv.dtype == torch.float32
 
         torch.set_default_dtype(torch.float64)
-        hv = functional.empty(3, 52, "MAP")
+        hv = functional.empty(3, 49, "MAP")
+        assert hv.dtype == torch.float64
+        hv = functional.empty(3, 49, "HRR")
         assert hv.dtype == torch.float64
-        hv = functional.empty(3, 52, "HRR")
+        hv = functional.empty(3, 49, "VTB")
         assert hv.dtype == torch.float64
 
-        hv = functional.empty(3, 52, "FHRR")
+        hv = functional.empty(3, 49, "FHRR")
         assert hv.dtype == torch.complex64
 
+        hv = functional.empty(3, 52, "BSBC", block_size=1024)
+        assert hv.dtype == torch.int64
+
     def test_requires_grad(self):
-        hv = functional.empty(3, 52, "MAP", requires_grad=True)
+        hv = functional.empty(3, 49, "MAP", requires_grad=True)
+        assert hv.requires_grad == True
+
+        hv = functional.empty(3, 49, "HRR", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.empty(3, 52, "HRR", requires_grad=True)
+        hv = functional.empty(3, 49, "VTB", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.empty(3, 52, "FHRR", requires_grad=True)
+        hv = functional.empty(3, 49, "FHRR", requires_grad=True)
         assert hv.requires_grad == True
```

### Comparing `torch-hd-5.2.1/torchhd/tests/basis_hv/test_identity_hv.py` & `torch-hd-5.3.0/torchhd/tests/basis_hv/test_identity_hv.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,81 +34,118 @@
 )
 
 seed = 2147483644
 
 
 class Testidentity:
     @pytest.mark.parametrize("n", [1, 3, 55])
-    @pytest.mark.parametrize("d", [84, 10])
+    @pytest.mark.parametrize("d", [84, 16])
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_shape(self, n, d, vsa):
-        hv = functional.identity(n, d, vsa)
+        if vsa == "BSBC":
+            hv = functional.identity(n, d, vsa, block_size=1042)
+        elif vsa == "VTB" and d == 84:
+            with pytest.raises(ValueError):
+                hv = functional.identity(n, d, vsa)
+
+            return
+
+        else:
+            hv = functional.identity(n, d, vsa)
 
         assert hv.dim() == 2
         assert hv.size(0) == n
         assert hv.size(1) == d
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_value(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             with pytest.raises(ValueError):
-                functional.identity(3, 26, vsa, dtype=dtype)
+                if vsa == "BSBC":
+                    functional.identity(3, 26, vsa, dtype=dtype, block_size=1042)
+                else:
+                    functional.identity(3, 25, vsa, dtype=dtype)
 
             return
 
-        hv = functional.identity(8, 26, vsa, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.identity(8, 25, vsa, dtype=dtype, block_size=1042)
+        else:
+            hv = functional.identity(8, 25, vsa, dtype=dtype)
+
         assert hv.requires_grad == False
         assert hv.dim() == 2
         assert hv.size(0) == 8
-        assert hv.size(1) == 26
+        assert hv.size(1) == 25
 
         if vsa == "BSC":
             assert torch.all(hv == False).item()
 
         elif vsa == "HRR":
-            hv = functional.identity(8, 26, vsa, dtype=dtype)
+            hv = functional.identity(8, 25, vsa, dtype=dtype)
             x = torch.fft.fft(hv)
             assert torch.allclose(x, torch.full_like(x, 1.0))
 
+        elif vsa == "BSBC":
+            assert torch.all(hv == 0)
+
+        elif vsa == "VTB":
+            hv = functional.identity(8, 25, vsa, dtype=dtype)
+
         else:
-            hv = functional.identity(8, 26, vsa, dtype=dtype)
+            hv = functional.identity(8, 25, vsa, dtype=dtype)
             assert torch.all(hv == 1.0).item()
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_device(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             return
 
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        hv = functional.identity(3, 52, vsa, device=device, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.identity(
+                3, 52, vsa, device=device, dtype=dtype, block_size=1042
+            )
+        else:
+            hv = functional.identity(3, 49, vsa, device=device, dtype=dtype)
         assert hv.device.type == device.type
 
     def test_uses_default_dtype(self):
-        hv = functional.identity(3, 52, "BSC")
+        hv = functional.identity(3, 49, "BSC")
         assert hv.dtype == torch.bool
 
         torch.set_default_dtype(torch.float32)
-        hv = functional.identity(3, 52, "MAP")
+        hv = functional.identity(3, 49, "MAP")
         assert hv.dtype == torch.float32
-        hv = functional.identity(3, 52, "HRR")
+        hv = functional.identity(3, 49, "HRR")
+        assert hv.dtype == torch.float32
+        hv = functional.identity(3, 49, "VTB")
         assert hv.dtype == torch.float32
 
         torch.set_default_dtype(torch.float64)
-        hv = functional.identity(3, 52, "MAP")
+        hv = functional.identity(3, 49, "MAP")
+        assert hv.dtype == torch.float64
+        hv = functional.identity(3, 49, "HRR")
         assert hv.dtype == torch.float64
-        hv = functional.identity(3, 52, "HRR")
+        hv = functional.identity(3, 49, "VTB")
         assert hv.dtype == torch.float64
 
-        hv = functional.identity(3, 52, "FHRR")
+        hv = functional.identity(3, 49, "FHRR")
         assert hv.dtype == torch.complex64
 
+        hv = functional.identity(3, 52, "BSBC", block_size=1024)
+        assert hv.dtype == torch.int64
+
     def test_requires_grad(self):
-        hv = functional.identity(3, 52, "MAP", requires_grad=True)
+        hv = functional.identity(3, 49, "MAP", requires_grad=True)
+        assert hv.requires_grad == True
+
+        hv = functional.identity(3, 49, "HRR", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.identity(3, 52, "HRR", requires_grad=True)
+        hv = functional.identity(3, 49, "VTB", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.identity(3, 52, "FHRR", requires_grad=True)
+        hv = functional.identity(3, 49, "FHRR", requires_grad=True)
         assert hv.requires_grad == True
```

### Comparing `torch-hd-5.2.1/torchhd/tests/basis_hv/test_level_hv.py` & `torch-hd-5.3.0/torchhd/tests/basis_hv/test_level_hv.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,56 +30,86 @@
 from ..utils import torch_dtypes, supported_dtype, vsa_tensors
 
 seed = 2147483643
 
 
 class Testlevel:
     @pytest.mark.parametrize("n", [1, 3, 55])
-    @pytest.mark.parametrize("d", [84, 10])
+    @pytest.mark.parametrize("d", [84, 16])
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_shape(self, n, d, vsa):
-        hv = functional.level(n, d, vsa)
+        if vsa == "BSBC":
+            hv = functional.level(n, d, vsa, block_size=1024)
+
+        elif vsa == "VTB" and d == 84:
+            with pytest.raises(ValueError):
+                hv = functional.level(n, d, vsa)
+
+            return
+
+        else:
+            hv = functional.level(n, d, vsa)
+
+        if vsa == "BSBC":
+            assert hv.block_size == 1024
 
         assert hv.dim() == 2
         assert hv.size(0) == n
         assert hv.size(1) == d
 
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_generator(self, vsa):
         generator = torch.Generator()
         generator.manual_seed(seed)
-        hv1 = functional.level(20, 10000, vsa, generator=generator)
+        if vsa == "BSBC":
+            hv1 = functional.level(20, 10000, vsa, generator=generator, block_size=1024)
+        else:
+            hv1 = functional.level(20, 10000, vsa, generator=generator)
 
         generator = torch.Generator()
         generator.manual_seed(seed)
 
-        hv2 = functional.level(20, 10000, vsa, generator=generator)
+        if vsa == "BSBC":
+            hv2 = functional.level(20, 10000, vsa, generator=generator, block_size=1024)
+        else:
+            hv2 = functional.level(20, 10000, vsa, generator=generator)
         assert torch.all(hv1 == hv2).item()
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_value(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             with pytest.raises(ValueError):
-                functional.level(3, 26, vsa, dtype=dtype)
+                if vsa == "BSBC":
+                    functional.level(3, 25, vsa, dtype=dtype, block_size=1024)
+                else:
+                    functional.level(3, 25, vsa, dtype=dtype)
 
             return
 
         generator = torch.Generator()
         generator.manual_seed(seed)
 
-        hv = functional.level(50, 26000, vsa, dtype=dtype, generator=generator)
+        if vsa == "BSBC":
+            hv = functional.level(
+                50, 25921, vsa, dtype=dtype, generator=generator, block_size=1024
+            )
+        else:
+            hv = functional.level(50, 25921, vsa, dtype=dtype, generator=generator)
         assert hv.requires_grad == False
         assert hv.dim() == 2
         assert hv.size(0) == 50
-        assert hv.size(1) == 26000
+        assert hv.size(1) == 25921
 
         if vsa == "BSC":
             assert torch.all((hv == False) | (hv == True)).item()
 
+        elif vsa == "BSBC":
+            assert torch.all((hv >= 0) | (hv < 1024)).item()
+
         elif vsa == "MAP":
             assert torch.all((hv == -1) | (hv == 1)).item()
 
         elif vsa == "HRR":
             std, mean = torch.std_mean(hv)
             assert torch.allclose(
                 mean, torch.tensor(0.0, dtype=mean.dtype), atol=0.0001
@@ -89,15 +119,20 @@
             mag = hv.abs()
             assert torch.allclose(mag, torch.tensor(1.0, dtype=mag.dtype))
 
         sims = functional.cosine_similarity(hv[0], hv)
         sims_diff = sims[:-1] - sims[1:]
         assert torch.all(sims_diff > 0).item(), "similarity must be decreasing"
 
-        hv = functional.level(5, 1000000, vsa, generator=generator, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.level(
+                5, 1000000, vsa, generator=generator, dtype=dtype, block_size=1024
+            )
+        else:
+            hv = functional.level(5, 1000000, vsa, generator=generator, dtype=dtype)
         sims = functional.cosine_similarity(hv[0], hv)
         sims_diff = sims[:-1] - sims[1:]
         assert torch.allclose(
             sims_diff, torch.tensor(0.25, dtype=sims_diff.dtype), atol=0.005
         ), "similarity decreases linearly"
 
     @pytest.mark.parametrize("sparsity", [0.0, 0.1, 0.756, 1.0])
@@ -124,38 +159,53 @@
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_device(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             return
 
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        hv = functional.level(3, 52, vsa, device=device, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.level(
+                3, 49, vsa, device=device, dtype=dtype, block_size=1024
+            )
+        else:
+            hv = functional.level(3, 49, vsa, device=device, dtype=dtype)
         assert hv.device.type == device.type
 
     def test_uses_default_dtype(self):
-        hv = functional.level(3, 52, "BSC")
+        hv = functional.level(3, 49, "BSC")
         assert hv.dtype == torch.bool
 
         torch.set_default_dtype(torch.float32)
-        hv = functional.level(3, 52, "MAP")
+        hv = functional.level(3, 49, "MAP")
         assert hv.dtype == torch.float32
-        hv = functional.level(3, 52, "HRR")
+        hv = functional.level(3, 49, "HRR")
+        assert hv.dtype == torch.float32
+        hv = functional.level(3, 49, "VTB")
         assert hv.dtype == torch.float32
 
         torch.set_default_dtype(torch.float64)
-        hv = functional.level(3, 52, "MAP")
+        hv = functional.level(3, 49, "MAP")
+        assert hv.dtype == torch.float64
+        hv = functional.level(3, 49, "HRR")
         assert hv.dtype == torch.float64
-        hv = functional.level(3, 52, "HRR")
+        hv = functional.level(3, 49, "VTB")
         assert hv.dtype == torch.float64
 
-        hv = functional.level(3, 52, "FHRR")
+        hv = functional.level(3, 49, "FHRR")
         assert hv.dtype == torch.complex64
 
+        hv = functional.level(3, 52, "BSBC", block_size=1024)
+        assert hv.dtype == torch.int64
+
     def test_requires_grad(self):
-        hv = functional.level(3, 52, "MAP", requires_grad=True)
+        hv = functional.level(3, 49, "MAP", requires_grad=True)
+        assert hv.requires_grad == True
+
+        hv = functional.level(3, 49, "HRR", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.level(3, 52, "HRR", requires_grad=True)
+        hv = functional.level(3, 49, "VTB", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.level(3, 52, "FHRR", requires_grad=True)
+        hv = functional.level(3, 49, "FHRR", requires_grad=True)
         assert hv.requires_grad == True
```

### Comparing `torch-hd-5.2.1/torchhd/tests/basis_hv/test_random_hv.py` & `torch-hd-5.3.0/torchhd/tests/basis_hv/test_random_hv.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,69 +34,101 @@
 )
 
 seed = 2147483644
 
 
 class Testrandom:
     @pytest.mark.parametrize("n", [1, 3, 55])
-    @pytest.mark.parametrize("d", [84, 10])
+    @pytest.mark.parametrize("d", [84, 16])
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_shape(self, n, d, vsa):
-        hv = functional.random(n, d, vsa)
+        if vsa == "BSBC":
+            hv = functional.random(n, d, vsa, block_size=64)
+
+        elif vsa == "VTB" and d == 84:
+            with pytest.raises(ValueError):
+                hv = functional.random(n, d, vsa)
+
+            return
+
+        else:
+            hv = functional.random(n, d, vsa)
 
         assert hv.dim() == 2
         assert hv.size(0) == n
         assert hv.size(1) == d
 
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_generator(self, vsa):
         generator = torch.Generator()
         generator.manual_seed(seed)
-        hv1 = functional.random(20, 10000, vsa, generator=generator)
+
+        if vsa == "BSBC":
+            hv1 = functional.random(20, 10000, vsa, generator=generator, block_size=64)
+        else:
+            hv1 = functional.random(20, 10000, vsa, generator=generator)
 
         generator = torch.Generator()
         generator.manual_seed(seed)
 
-        hv2 = functional.random(20, 10000, vsa, generator=generator)
+        if vsa == "BSBC":
+            hv2 = functional.random(20, 10000, vsa, generator=generator, block_size=64)
+        else:
+            hv2 = functional.random(20, 10000, vsa, generator=generator)
         assert torch.all(hv1 == hv2).item()
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_value(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             with pytest.raises(ValueError):
-                functional.random(3, 26, vsa, dtype=dtype)
+                if vsa == "BSBC":
+                    functional.random(3, 25, vsa, dtype=dtype, block_size=64)
+                else:
+                    functional.random(3, 25, vsa, dtype=dtype)
 
             return
 
         generator = torch.Generator()
         generator.manual_seed(seed)
 
-        hv = functional.random(8, 26000, vsa, dtype=dtype, generator=generator)
+        if vsa == "BSBC":
+            hv = functional.random(
+                8, 25921, vsa, dtype=dtype, generator=generator, block_size=64
+            )
+        else:
+            hv = functional.random(8, 25921, vsa, dtype=dtype, generator=generator)
         assert hv.requires_grad == False
         assert hv.dim() == 2
         assert hv.size(0) == 8
-        assert hv.size(1) == 26000
+        assert hv.size(1) == 25921
 
         if vsa == "BSC":
             assert torch.all((hv == False) | (hv == True)).item()
 
         elif vsa == "MAP":
             assert torch.all((hv == -1) | (hv == 1)).item()
 
         elif vsa == "HRR":
             std, mean = torch.std_mean(hv)
             assert torch.allclose(
                 mean, torch.tensor(0.0, dtype=mean.dtype), atol=0.0001
             )
 
+        elif vsa == "VTB":
+            mag = torch.norm(hv, dim=-1)
+            assert torch.allclose(mag, torch.tensor(1.0, dtype=mag.dtype))
+
         elif vsa == "FHRR":
             mag = hv.abs()
             assert torch.allclose(mag, torch.tensor(1.0, dtype=mag.dtype))
 
+        elif vsa == "BSBC":
+            assert torch.all((hv < 64) & (hv >= 0))
+
     @pytest.mark.parametrize("sparsity", [0.0, 0.1, 0.756, 1.0])
     @pytest.mark.parametrize("dtype", torch_dtypes)
     def test_sparsity(self, sparsity, dtype):
         if not supported_dtype(dtype, "BSC"):
             return
 
         generator = torch.Generator()
@@ -119,51 +151,72 @@
     def test_orthogonality(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             return
 
         generator = torch.Generator()
         generator.manual_seed(seed)
 
-        hv = functional.random(100, 10000, vsa, dtype=dtype, generator=generator)
+        if vsa == "BSBC":
+            hv = functional.random(
+                100, 10000, vsa, dtype=dtype, generator=generator, block_size=1042
+            )
+        else:
+            hv = functional.random(100, 10000, vsa, dtype=dtype, generator=generator)
+
         sims = functional.cosine_similarity(hv[0], hv[1:])
         assert torch.allclose(
             sims.mean(), torch.tensor(0.0, dtype=sims.dtype), atol=0.002
         )
 
     @pytest.mark.parametrize("dtype", torch_dtypes)
     @pytest.mark.parametrize("vsa", vsa_tensors)
     def test_device(self, dtype, vsa):
         if not supported_dtype(dtype, vsa):
             return
 
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        hv = functional.random(3, 52, vsa, device=device, dtype=dtype)
+        if vsa == "BSBC":
+            hv = functional.random(
+                3, 49, vsa, device=device, dtype=dtype, block_size=64
+            )
+        else:
+            hv = functional.random(3, 49, vsa, device=device, dtype=dtype)
         assert hv.device.type == device.type
 
     def test_uses_default_dtype(self):
-        hv = functional.random(3, 52, "BSC")
+        hv = functional.random(3, 49, "BSC")
         assert hv.dtype == torch.bool
 
         torch.set_default_dtype(torch.float32)
-        hv = functional.random(3, 52, "MAP")
+        hv = functional.random(3, 49, "MAP")
+        assert hv.dtype == torch.float32
+        hv = functional.random(3, 49, "HRR")
         assert hv.dtype == torch.float32
-        hv = functional.random(3, 52, "HRR")
+        hv = functional.random(3, 49, "VTB")
         assert hv.dtype == torch.float32
 
         torch.set_default_dtype(torch.float64)
-        hv = functional.random(3, 52, "MAP")
+        hv = functional.random(3, 49, "MAP")
         assert hv.dtype == torch.float64
-        hv = functional.random(3, 52, "HRR")
+        hv = functional.random(3, 49, "HRR")
+        assert hv.dtype == torch.float64
+        hv = functional.random(3, 49, "VTB")
         assert hv.dtype == torch.float64
 
-        hv = functional.random(3, 52, "FHRR")
+        hv = functional.random(3, 49, "FHRR")
         assert hv.dtype == torch.complex64
 
+        hv = functional.random(3, 52, "BSBC", block_size=64)
+        assert hv.dtype == torch.int64
+
     def test_requires_grad(self):
-        hv = functional.random(3, 52, "MAP", requires_grad=True)
+        hv = functional.random(3, 49, "MAP", requires_grad=True)
+        assert hv.requires_grad == True
+
+        hv = functional.random(3, 49, "HRR", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.random(3, 52, "HRR", requires_grad=True)
+        hv = functional.random(3, 49, "VTB", requires_grad=True)
         assert hv.requires_grad == True
 
-        hv = functional.random(3, 52, "FHRR", requires_grad=True)
+        hv = functional.random(3, 49, "FHRR", requires_grad=True)
         assert hv.requires_grad == True
```

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/__init__.py` & `torch-hd-5.3.0/torchhd/tests/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_distinct_sequence.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_distinct_sequence.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_fsa.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_fsa.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_graph.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
         GD = structures.Graph(8, directed=True)
 
         e1 = GD.encode_edge(hv[0], hv[1])
         assert torch.allclose(
             e1, torch.tensor([-1.0, 1.0, -1.0, -1.0, -1.0, -1.0, 1.0, -1.0])
         )
         e2 = GD.encode_edge(hv[2], hv[3])
-        print(e2)
         assert torch.allclose(
             e2, torch.tensor([1.0, -1.0, 1.0, -1.0, 1.0, -1.0, 1.0, -1.0])
         )
 
     def test_node_neighbors(self):
         generator = torch.Generator()
         generator.manual_seed(seed)
```

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_hashtable.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_hashtable.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_memory.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_memory.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_multiset.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_multiset.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_sequence.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_sequence.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/tests/structures/test_tree.py` & `torch-hd-5.3.0/torchhd/tests/structures/test_tree.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/types.py` & `torch-hd-5.3.0/torchhd/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,10 +17,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-from typing import Literal
-
-VSAOptions = Literal["BSC", "MAP", "HRR", "FHRR"]
+__version__ = "5.3.0"
```

### Comparing `torch-hd-5.2.1/torchhd/utils.py` & `torch-hd-5.3.0/torchhd/utils.py`

 * *Files identical despite different names*

### Comparing `torch-hd-5.2.1/torchhd/version.py` & `torch-hd-5.3.0/torchhd/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
-__version__ = "5.2.1"
+from typing import Literal
+
+VSAOptions = Literal["BSC", "MAP", "HRR", "FHRR", "BSBC", "VTB"]
```

