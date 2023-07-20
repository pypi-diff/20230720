# Comparing `tmp/floatcsep-0.1.2.tar.gz` & `tmp/floatcsep-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floatcsep-0.1.2.tar", last modified: Mon May 22 16:19:27 2023, max compression
+gzip compressed data, was "floatcsep-0.1.3.tar", last modified: Thu Jul 20 11:05:04 2023, max compression
```

## Comparing `floatcsep-0.1.2.tar` & `floatcsep-0.1.3.tar`

### file list

```diff
@@ -1,204 +1,136 @@
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     5219 2023-05-17 10:40:43.000000 floatcsep-0.1.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     8212 2023-05-17 10:48:33.000000 floatcsep-0.1.2/CONTRIBUTING.md
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      439 2023-05-17 10:40:43.000000 floatcsep-0.1.2/CREDITS.md
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1518 2023-05-17 10:40:43.000000 floatcsep-0.1.2/LICENSE
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      455 2023-05-22 15:30:27.000000 floatcsep-0.1.2/MANIFEST.in
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     4642 2023-05-22 16:19:27.837100 floatcsep-0.1.2/PKG-INFO
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3977 2023-05-22 15:46:04.000000 floatcsep-0.1.2/README.md
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/docs/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      773 2023-05-17 10:47:57.000000 floatcsep-0.1.2/docs/Makefile
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/docs/_static/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    82639 2023-05-17 10:40:43.000000 floatcsep-0.1.2/docs/_static/CSEP2_Logo_CMYK.png
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    33945 2023-05-20 19:10:46.000000 floatcsep-0.1.2/docs/_static/floatCSEP_Logo_CMYK.png
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    65939 2023-05-20 22:56:57.000000 floatcsep-0.1.2/docs/_static/floatcsep_logo.svg
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1947 2023-05-20 19:07:45.000000 floatcsep-0.1.2/docs/conf.py
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/docs/deployment/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       42 2023-05-20 18:32:42.000000 floatcsep-0.1.2/docs/deployment/intro.rst
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/docs/examples/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     6130 2023-05-18 12:42:54.000000 floatcsep-0.1.2/docs/examples/case_a.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     2941 2023-05-18 12:06:04.000000 floatcsep-0.1.2/docs/examples/case_b.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     2619 2023-05-18 11:52:45.000000 floatcsep-0.1.2/docs/examples/case_c.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3710 2023-05-18 11:52:45.000000 floatcsep-0.1.2/docs/examples/case_d.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3148 2023-05-18 11:52:45.000000 floatcsep-0.1.2/docs/examples/case_e.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     5439 2023-05-18 12:50:10.000000 floatcsep-0.1.2/docs/examples/case_f.rst
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/docs/guide/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       62 2023-05-20 18:54:28.000000 floatcsep-0.1.2/docs/guide/config.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       46 2023-05-17 10:40:43.000000 floatcsep-0.1.2/docs/guide/model_config.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       40 2023-05-17 10:40:43.000000 floatcsep-0.1.2/docs/guide/region_config.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       50 2023-05-17 10:40:43.000000 floatcsep-0.1.2/docs/guide/tests_config.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       44 2023-05-17 10:40:43.000000 floatcsep-0.1.2/docs/guide/time_config.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1086 2023-05-22 15:11:53.000000 floatcsep-0.1.2/docs/index.rst
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/docs/intro/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1924 2023-05-20 18:32:42.000000 floatcsep-0.1.2/docs/intro/concepts.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1486 2023-05-20 18:17:15.000000 floatcsep-0.1.2/docs/intro/installation.rst
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/docs/reference/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3152 2023-05-17 10:57:36.000000 floatcsep-0.1.2/docs/reference/api_reference.rst
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/docs/reference/generated/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      130 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.accessors.from_git.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      139 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.accessors.from_zenodo.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      136 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.accessors.query_gcmt.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      113 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.cmd.main.plot.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      128 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.cmd.main.reproduce.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      110 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.cmd.main.run.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      159 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.compute.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      167 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.from_dict.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      173 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.get_catalog.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      176 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.prepare_args.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      610 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      161 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.to_dict.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      152 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.type.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      176 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.evaluation.Evaluation.write_result.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      161 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.catalog.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      164 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.from_yml.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      185 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.generate_report.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      167 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.get_model.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      176 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.plot_catalog.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      182 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.plot_forecasts.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      176 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.plot_results.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      176 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.read_results.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      887 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      147 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.run.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      170 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.set_models.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      167 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.set_tasks.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      178 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.set_test_cat.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      167 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.set_tests.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      176 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.stage_models.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      161 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.to_dict.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      158 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.experiment.Experiment.to_yml.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      161 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.binary_paired_t_test.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      209 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.binomial_conditional_likelihood_test.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      214 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.binomial_joint_log_likelihood_ndarray.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      162 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.binomial_spatial_test.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      130 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.brier_score.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      185 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.log_likelihood_point_process.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      188 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.negative_binomial_number_test.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      179 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.paired_ttest_point_process.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      180 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.sequential_information_gain.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      160 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.sequential_likelihood.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      172 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.extras.vector_poisson_t_w_test.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      155 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.create_forecast.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      166 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.forecast_from_file.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      166 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.forecast_from_func.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      137 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.from_dict.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      146 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.get_forecast.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      140 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.get_source.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      131 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.init_db.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      125 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.rm_db.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      688 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      123 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.stage.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      131 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.model.Model.to_dict.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      153 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.readers.ForecastParsers.csv.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      153 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.readers.ForecastParsers.dat.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      156 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.readers.ForecastParsers.hdf5.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      168 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.readers.ForecastParsers.quadtree.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      153 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.readers.ForecastParsers.xml.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      168 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.readers.HDF5Serializer.grid2hdf5.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      125 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.readers.serialize.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      140 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.Task.check_exist.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      292 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.Task.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      114 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.Task.run.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      147 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.magnitude_vs_time.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      141 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.parse_csep_func.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      162 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.parse_timedelta_string.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      174 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.plot_sequential_likelihood.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      150 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.read_region_config.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      144 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.read_time_config.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      134 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.timewindow2str.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      136 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.timewindows_td.rst
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      136 2023-05-20 19:08:51.000000 floatcsep-0.1.2/docs/reference/generated/floatcsep.utils.timewindows_ti.rst
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/floatcsep/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       21 2023-05-17 10:40:43.000000 floatcsep-0.1.2/floatcsep/__init__.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    11610 2023-05-20 23:52:58.000000 floatcsep-0.1.2/floatcsep/accessors.py
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/floatcsep/artifacts/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)   178905 2023-05-17 10:40:43.000000 floatcsep-0.1.2/floatcsep/artifacts/new_zealand_csep_testing.csv
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      810 2023-05-17 10:40:43.000000 floatcsep-0.1.2/floatcsep/artifacts/patterns.py
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/floatcsep/cmd/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     2612 2023-05-20 14:38:16.000000 floatcsep-0.1.2/floatcsep/cmd/main.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    14226 2023-05-18 13:00:48.000000 floatcsep-0.1.2/floatcsep/evaluation.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    35581 2023-05-20 16:55:50.000000 floatcsep-0.1.2/floatcsep/experiment.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    33199 2023-05-17 10:40:43.000000 floatcsep-0.1.2/floatcsep/extras.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1022 2023-05-20 23:56:46.000000 floatcsep-0.1.2/floatcsep/meta.yaml
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    18947 2023-05-22 15:12:26.000000 floatcsep-0.1.2/floatcsep/model.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    12017 2023-05-17 10:40:43.000000 floatcsep-0.1.2/floatcsep/readers.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     8798 2023-05-20 17:56:05.000000 floatcsep-0.1.2/floatcsep/registry.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3032 2023-05-20 16:56:43.000000 floatcsep-0.1.2/floatcsep/report.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    45669 2023-05-17 10:48:33.000000 floatcsep-0.1.2/floatcsep/utils.py
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/floatcsep.egg-info/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     4642 2023-05-22 16:19:27.000000 floatcsep-0.1.2/floatcsep.egg-info/PKG-INFO
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     7803 2023-05-22 16:19:27.000000 floatcsep-0.1.2/floatcsep.egg-info/SOURCES.txt
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        1 2023-05-22 16:19:27.000000 floatcsep-0.1.2/floatcsep.egg-info/dependency_links.txt
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       59 2023-05-22 16:19:27.000000 floatcsep-0.1.2/floatcsep.egg-info/entry_points.txt
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        1 2023-05-17 10:50:09.000000 floatcsep-0.1.2/floatcsep.egg-info/not-zip-safe
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      397 2023-05-22 16:19:27.000000 floatcsep-0.1.2/floatcsep.egg-info/requires.txt
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       10 2023-05-22 16:19:27.000000 floatcsep-0.1.2/floatcsep.egg-info/top_level.txt
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      179 2023-05-17 10:47:56.000000 floatcsep-0.1.2/pyproject.toml
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      118 2023-05-22 16:18:46.000000 floatcsep-0.1.2/requirements.txt
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      191 2023-05-20 22:51:28.000000 floatcsep-0.1.2/requirements_dev.txt
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1345 2023-05-22 16:19:27.837100 floatcsep-0.1.2/setup.cfg
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       69 2023-05-18 21:03:33.000000 floatcsep-0.1.2/setup.py
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/tests/
--rw-r--r--   0 pciturri  (1000) pciturri  (1000)    53248 2023-05-20 17:16:05.000000 floatcsep-0.1.2/tests/.coverage
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/tests/artifacts/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1064 2023-05-17 18:48:31.000000 floatcsep-0.1.2/tests/artifacts/catalog.json
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/tests/artifacts/evaluations/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      377 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/evaluations/tests_cfg.yml
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/tests/artifacts/gcmt/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1722 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/gcmt/vcr_search.yaml
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1347 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/gcmt/vcr_summary.yaml
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.829100 floatcsep-0.1.2/tests/artifacts/models/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      182 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/model.csv
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     4640 2023-05-20 23:21:26.000000 floatcsep-0.1.2/tests/artifacts/models/model.hdf5
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      184 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/model_cfg.yml
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     4640 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/model_h5.hdf5
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.833100 floatcsep-0.1.2/tests/artifacts/models/qtree/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)  5734026 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/qtree/TEAM=N10L11.csv
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)  2468253 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/qtree/TEAM=N25L11.csv
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/tests/artifacts/models/td_model/
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.833100 floatcsep-0.1.2/tests/artifacts/models/td_model/input/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       77 2023-05-20 23:21:16.000000 floatcsep-0.1.2/tests/artifacts/models/td_model/input/args.txt
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     2010 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/Dockerfile
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3522 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/README.md
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/docs/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/docs/userguide
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.821100 floatcsep-0.1.2/tests/artifacts/models/template/examples/
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/examples/case_3/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/examples/case_3/case3_run
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/examples/case_3/data/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/examples/case_3/data/case3_catalog
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/forecasts/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/forecasts/template_2023-01-01
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/input/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      169 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/input/catalog
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      715 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/parameters
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       35 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/requirements
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      768 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/run
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      138 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/run_tests
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      148 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/setup
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/source/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/source/lib_a
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/source/lib_b
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/source/main
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/template/tests/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/tests/test_liba
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/tests/test_libb
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)        0 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/models/template/tests/test_main
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/models/zenodo_test/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)      341 2023-05-17 10:55:35.000000 floatcsep-0.1.2/tests/artifacts/models/zenodo_test/datapackage.json
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     6144 2023-05-17 10:55:37.000000 floatcsep-0.1.2/tests/artifacts/models/zenodo_test/table.xls
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/artifacts/regions/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)   106101 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/regions/italy_midpoints
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)       23 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/artifacts/regions/mock_region
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/integration/
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1178 2023-05-17 10:40:43.000000 floatcsep-0.1.2/tests/integration/experiment typologies
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     1285 2023-05-17 14:33:11.000000 floatcsep-0.1.2/tests/integration/test_data.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3228 2023-05-17 10:47:56.000000 floatcsep-0.1.2/tests/integration/test_model_interface.py
-drwxrwxr-x   0 pciturri  (1000) pciturri  (1000)        0 2023-05-22 16:19:27.837100 floatcsep-0.1.2/tests/unit/
--rw-r--r--   0 pciturri  (1000) pciturri  (1000)    53248 2023-05-20 23:52:27.000000 floatcsep-0.1.2/tests/unit/.coverage
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3828 2023-05-20 23:52:16.000000 floatcsep-0.1.2/tests/unit/test_accessors.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     3068 2023-05-18 11:45:38.000000 floatcsep-0.1.2/tests/unit/test_evaluation.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     6810 2023-05-17 18:44:30.000000 floatcsep-0.1.2/tests/unit/test_experiment.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)    10762 2023-05-20 17:12:12.000000 floatcsep-0.1.2/tests/unit/test_model.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     7282 2023-05-17 10:47:57.000000 floatcsep-0.1.2/tests/unit/test_readers.py
--rw-rw-r--   0 pciturri  (1000) pciturri  (1000)     6881 2023-05-17 10:47:56.000000 floatcsep-0.1.2/tests/unit/test_utils.py
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     5219 2023-05-23 12:15:34.000000 floatcsep-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 pciturri (19030) rs        (1400)     8212 2023-05-23 12:15:34.000000 floatcsep-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 pciturri (19030) rs        (1400)      439 2023-05-23 12:15:34.000000 floatcsep-0.1.3/CREDITS.md
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1518 2023-05-23 12:15:34.000000 floatcsep-0.1.3/LICENSE
+-rw-r--r--   0 pciturri (19030) rs        (1400)      455 2023-05-31 12:03:11.000000 floatcsep-0.1.3/MANIFEST.in
+-rw-r--r--   0 pciturri (19030) rs        (1400)     4688 2023-07-20 11:05:04.920320 floatcsep-0.1.3/PKG-INFO
+-rw-r--r--   0 pciturri (19030) rs        (1400)     4023 2023-07-20 10:59:33.000000 floatcsep-0.1.3/README.md
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/docs/
+-rw-r--r--   0 pciturri (19030) rs        (1400)      773 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/Makefile
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/docs/_static/
+-rw-r--r--   0 pciturri (19030) rs        (1400)    82639 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/_static/CSEP2_Logo_CMYK.png
+-rw-r--r--   0 pciturri (19030) rs        (1400)    33945 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/_static/floatCSEP_Logo_CMYK.png
+-rw-r--r--   0 pciturri (19030) rs        (1400)    65939 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/_static/floatcsep_logo.svg
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1947 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/conf.py
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/docs/deployment/
+-rw-r--r--   0 pciturri (19030) rs        (1400)       42 2023-05-23 12:15:34.000000 floatcsep-0.1.3/docs/deployment/intro.rst
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/examples/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     6130 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_a.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)     2941 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_b.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)     2619 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_c.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3710 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_d.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3148 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_e.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)     5439 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/examples/case_f.rst
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/guide/
+-rw-r--r--   0 pciturri (19030) rs        (1400)       62 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/config.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)       46 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/model_config.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)       40 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/region_config.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)       50 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/tests_config.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)       44 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/guide/time_config.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1086 2023-05-31 13:57:12.000000 floatcsep-0.1.3/docs/index.rst
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/intro/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1924 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/intro/concepts.rst
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1486 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/intro/installation.rst
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/docs/reference/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3152 2023-05-23 12:15:35.000000 floatcsep-0.1.3/docs/reference/api_reference.rst
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep/
+-rw-r--r--   0 pciturri (19030) rs        (1400)      268 2023-07-20 10:59:33.000000 floatcsep-0.1.3/floatcsep/__init__.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    11610 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/accessors.py
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep/artifacts/
+-rw-r--r--   0 pciturri (19030) rs        (1400)   178905 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/artifacts/new_zealand_csep_testing.csv
+-rw-r--r--   0 pciturri (19030) rs        (1400)      810 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/artifacts/patterns.py
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep/cmd/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     2544 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/cmd/main.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    14225 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/evaluation.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    39254 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/experiment.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    33199 2023-05-23 12:15:35.000000 floatcsep-0.1.3/floatcsep/extras.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1223 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/logger.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    19583 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/model.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    12132 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/readers.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     9988 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/registry.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3175 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/report.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    54973 2023-07-19 14:28:35.000000 floatcsep-0.1.3/floatcsep/utils.py
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/floatcsep.egg-info/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     4688 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/PKG-INFO
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3090 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/SOURCES.txt
+-rw-r--r--   0 pciturri (19030) rs        (1400)        1 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/dependency_links.txt
+-rw-r--r--   0 pciturri (19030) rs        (1400)       59 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/entry_points.txt
+-rw-r--r--   0 pciturri (19030) rs        (1400)        1 2023-05-23 12:47:51.000000 floatcsep-0.1.3/floatcsep.egg-info/not-zip-safe
+-rw-r--r--   0 pciturri (19030) rs        (1400)      388 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/requires.txt
+-rw-r--r--   0 pciturri (19030) rs        (1400)       10 2023-07-20 11:05:04.000000 floatcsep-0.1.3/floatcsep.egg-info/top_level.txt
+-rw-r--r--   0 pciturri (19030) rs        (1400)      179 2023-05-23 12:15:35.000000 floatcsep-0.1.3/pyproject.toml
+-rw-r--r--   0 pciturri (19030) rs        (1400)      110 2023-07-19 14:28:35.000000 floatcsep-0.1.3/requirements.txt
+-rw-r--r--   0 pciturri (19030) rs        (1400)      204 2023-07-19 14:28:35.000000 floatcsep-0.1.3/requirements_dev.txt
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1336 2023-07-20 11:05:04.920320 floatcsep-0.1.3/setup.cfg
+-rw-r--r--   0 pciturri (19030) rs        (1400)       69 2023-05-23 12:15:35.000000 floatcsep-0.1.3/setup.py
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/
+-rw-r--r--   0 pciturri (19030) rs        (1400)    53248 2023-07-19 13:22:13.000000 floatcsep-0.1.3/tests/.coverage
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-31 12:15:02.000000 floatcsep-0.1.3/tests/.floatcsep.log
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1064 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/catalog.json
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/evaluations/
+-rw-r--r--   0 pciturri (19030) rs        (1400)      377 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/evaluations/tests_cfg.yml
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/gcmt/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1722 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/gcmt/vcr_search.yaml
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1347 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/gcmt/vcr_summary.yaml
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.912321 floatcsep-0.1.3/tests/artifacts/models/
+-rw-r--r--   0 pciturri (19030) rs        (1400)      182 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/model.csv
+-rw-r--r--   0 pciturri (19030) rs        (1400)      184 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/model_cfg.yml
+-rw-r--r--   0 pciturri (19030) rs        (1400)     4640 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/model_h5.hdf5
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.916320 floatcsep-0.1.3/tests/artifacts/models/qtree/
+-rw-r--r--   0 pciturri (19030) rs        (1400)  5734026 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N10L11.csv
+-rw-r--r--   0 pciturri (19030) rs        (1400)  2468253 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N25L11.csv
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/artifacts/models/td_model/
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.916320 floatcsep-0.1.3/tests/artifacts/models/td_model/input/
+-rw-r--r--   0 pciturri (19030) rs        (1400)       32 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/artifacts/models/td_model/input/args.txt
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.916320 floatcsep-0.1.3/tests/artifacts/models/template/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     2010 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/Dockerfile
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3522 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/README.md
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/docs/
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/docs/userguide
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/artifacts/models/template/examples/
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/case3_run
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/data/
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/examples/case_3/data/case3_catalog
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/forecasts/
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/forecasts/template_2023-01-01
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/input/
+-rw-r--r--   0 pciturri (19030) rs        (1400)      169 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/input/catalog
+-rw-r--r--   0 pciturri (19030) rs        (1400)      715 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/parameters
+-rw-r--r--   0 pciturri (19030) rs        (1400)       35 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/requirements
+-rw-r--r--   0 pciturri (19030) rs        (1400)      768 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/run
+-rw-r--r--   0 pciturri (19030) rs        (1400)      138 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/run_tests
+-rw-r--r--   0 pciturri (19030) rs        (1400)      148 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/setup
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/source/
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/source/lib_a
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/source/lib_b
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/source/main
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/template/tests/
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/tests/test_liba
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/tests/test_libb
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/models/template/tests/test_main
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/models/zenodo_test/
+-rw-r--r--   0 pciturri (19030) rs        (1400)      341 2023-05-23 14:47:58.000000 floatcsep-0.1.3/tests/artifacts/models/zenodo_test/datapackage.json
+-rw-r--r--   0 pciturri (19030) rs        (1400)     6144 2023-05-23 14:48:00.000000 floatcsep-0.1.3/tests/artifacts/models/zenodo_test/table.xls
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/artifacts/regions/
+-rw-r--r--   0 pciturri (19030) rs        (1400)   106101 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/regions/italy_midpoints
+-rw-r--r--   0 pciturri (19030) rs        (1400)       23 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/artifacts/regions/mock_region
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/integration/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1178 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/integration/experiment typologies
+-rw-r--r--   0 pciturri (19030) rs        (1400)     2423 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/integration/test_data.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3349 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/integration/test_model_interface.py
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/unit/
+-rw-r--r--   0 pciturri (19030) rs        (1400)    53248 2023-07-19 14:25:04.000000 floatcsep-0.1.3/tests/unit/.coverage
+-rw-r--r--   0 pciturri (19030) rs        (1400)        0 2023-05-31 12:31:59.000000 floatcsep-0.1.3/tests/unit/.floatcsep.log
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/unit/results/
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.908321 floatcsep-0.1.3/tests/unit/results/2021-01-01_2022-01-01/
+drwxr-xr-x   0 pciturri (19030) rs        (1400)        0 2023-07-20 11:05:04.920320 floatcsep-0.1.3/tests/unit/results/2021-01-01_2022-01-01/catalog/
+-rw-r--r--   0 pciturri (19030) rs        (1400)     1317 2023-07-19 14:25:04.000000 floatcsep-0.1.3/tests/unit/results/2021-01-01_2022-01-01/catalog/catalog.json
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3884 2023-05-31 12:35:27.000000 floatcsep-0.1.3/tests/unit/test_accessors.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     3068 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/unit/test_evaluation.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     6871 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/unit/test_experiment.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)    10846 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/unit/test_model.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     7282 2023-05-23 12:15:35.000000 floatcsep-0.1.3/tests/unit/test_readers.py
+-rw-r--r--   0 pciturri (19030) rs        (1400)     6854 2023-07-19 14:28:35.000000 floatcsep-0.1.3/tests/unit/test_utils.py
```

### Comparing `floatcsep-0.1.2/CODE_OF_CONDUCT.md` & `floatcsep-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/CONTRIBUTING.md` & `floatcsep-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/LICENSE` & `floatcsep-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/PKG-INFO` & `floatcsep-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floatcsep
-Version: 0.1.2
+Version: 0.1.3
 Summary: CSEP Floating Experiment application
 Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta
 Author-email: pciturri@gfz-potsdam.de
 License: BSD 3-Clause License
 Platform: unix
 Platform: linux
@@ -30,14 +30,16 @@
 
 <a href='https://floatcsep.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/floatcsep/badge/?version=latest' alt='Documentation Status' />
 </a>
 <a href='https://github.com/cseptesting/floatcsep/actions/workflows/build-test.yml'>
     <img src='https://github.com/cseptesting/floatcsep/actions/workflows/build-test.yml/badge.svg' alt='Documentation Status' />
 </a>
+<img alt="PyPI" src="https://img.shields.io/pypi/v/floatcsep">
+
 <a href="https://codecov.io/gh/cseptesting/floatcsep" > 
  <img src="https://codecov.io/gh/cseptesting/floatcsep/branch/main/graph/badge.svg?token=LI4RSDOKA1"/> 
  </a>
 <a href="https://doi.org/10.5281/zenodo.7953817"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7953817.svg" alt="DOI"></a>
 </p>
 
 * Set up a testing **experiment** for your earthquake forecasts using authoritative data sources and benchmarks.
@@ -96,15 +98,15 @@
 * Add functionality to compare original results and reproduced results
 * Add registry to filetrees (e.g. hash/byte count) for a proper experiment re-instantiation
 * Add report customization
 * Fix the hooks properly (user code) to be inserted into plotting/reporting functionalities.
 * Add multiple logging/levels
 * Create tool to check a TD model's interface with ``fecsep``
 * Define a dependency strategy to ensure experiments' reproducibility.
-* Publish in `pypi`/`conda` and Zenodo
+* Publish in `conda`
 
 # Contributing
 
 We encourage all types of contributions, from reporting bugs, suggesting enhancements, adding new features and more. Please refer to the [Contribution Guidelines](https://github.com/cseptesting/floatcsep/blob/main/CONTRIBUTING.md) and the [Code of Conduct](https://github.com/cseptesting/floatcsep/blob/main/CODE_OF_CONDUCT.md) for more information
 
 # License
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: floatcsep Version: 0.1.2 Summary: CSEP Floating
+Metadata-Version: 2.1 Name: floatcsep Version: 0.1.3 Summary: CSEP Floating
 Experiment application Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta Author-email: pciturri@gfz-potsdam.de License: BSD 3-
 Clause License Platform: unix Platform: linux Platform: osx Platform: win32
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: dev License-File: LICENSE # CSEP Floating
 Experiments [https://i.postimg.cc/6p5krRnB/float-CSEP-Logo-CMYK.png] **An
 application to deploy reproducible and prospective experiments of earthquake
 forecasting**
-[Documentation_Status] [Documentation_Status] [https://codecov.io/gh/
+[Documentation_Status] [Documentation_Status] [PyPI] [https://codecov.io/gh/
 cseptesting/floatcsep/branch/main/graph/badge.svg?token=LI4RSDOKA1] [DOI]
 * Set up a testing **experiment** for your earthquake forecasts using
 authoritative data sources and benchmarks. * **Encapsulate** the complete
 experiment's definition and rules in a couple of lines. * **Reproduce**,
 **reuse**, and **share** forecasting experiments from you, other researchers
 and institutions. # Table of Contents * [Installation](#installing-floatcsep) *
 [Documentation](https://floatcsep.readthedocs.io) * [Run and explore](#run-an-
@@ -39,17 +39,16 @@
 * `pyCSEP` [Github](https://github.com/sceccode/pycsep) * `pyCSEP`
 [Documentation](https://docs.cseptesting.org/) # Roadmap and Known Issues * Add
 functionality to compare original results and reproduced results * Add registry
 to filetrees (e.g. hash/byte count) for a proper experiment re-instantiation *
 Add report customization * Fix the hooks properly (user code) to be inserted
 into plotting/reporting functionalities. * Add multiple logging/levels * Create
 tool to check a TD model's interface with ``fecsep`` * Define a dependency
-strategy to ensure experiments' reproducibility. * Publish in `pypi`/`conda`
-and Zenodo # Contributing We encourage all types of contributions, from
-reporting bugs, suggesting enhancements, adding new features and more. Please
-refer to the [Contribution Guidelines](https://github.com/cseptesting/
-floatcsep/blob/main/CONTRIBUTING.md) and the [Code of Conduct](https://
-github.com/cseptesting/floatcsep/blob/main/CODE_OF_CONDUCT.md) for more
-information # License The `floatCSEP` (as well as `pyCSEP`) software is
-distributed under the BSD 3-Clause open-source license. Please see the [license
-file](https://github.com/cseptesting/floatcsep/blob/main/LICENSE) for more
-information.
+strategy to ensure experiments' reproducibility. * Publish in `conda` #
+Contributing We encourage all types of contributions, from reporting bugs,
+suggesting enhancements, adding new features and more. Please refer to the
+[Contribution Guidelines](https://github.com/cseptesting/floatcsep/blob/main/
+CONTRIBUTING.md) and the [Code of Conduct](https://github.com/cseptesting/
+floatcsep/blob/main/CODE_OF_CONDUCT.md) for more information # License The
+`floatCSEP` (as well as `pyCSEP`) software is distributed under the BSD 3-
+Clause open-source license. Please see the [license file](https://github.com/
+cseptesting/floatcsep/blob/main/LICENSE) for more information.
```

### Comparing `floatcsep-0.1.2/README.md` & `floatcsep-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 <a href='https://floatcsep.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/floatcsep/badge/?version=latest' alt='Documentation Status' />
 </a>
 <a href='https://github.com/cseptesting/floatcsep/actions/workflows/build-test.yml'>
     <img src='https://github.com/cseptesting/floatcsep/actions/workflows/build-test.yml/badge.svg' alt='Documentation Status' />
 </a>
+<img alt="PyPI" src="https://img.shields.io/pypi/v/floatcsep">
+
 <a href="https://codecov.io/gh/cseptesting/floatcsep" > 
  <img src="https://codecov.io/gh/cseptesting/floatcsep/branch/main/graph/badge.svg?token=LI4RSDOKA1"/> 
  </a>
 <a href="https://doi.org/10.5281/zenodo.7953817"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7953817.svg" alt="DOI"></a>
 </p>
 
 * Set up a testing **experiment** for your earthquake forecasts using authoritative data sources and benchmarks.
@@ -74,15 +76,15 @@
 * Add functionality to compare original results and reproduced results
 * Add registry to filetrees (e.g. hash/byte count) for a proper experiment re-instantiation
 * Add report customization
 * Fix the hooks properly (user code) to be inserted into plotting/reporting functionalities.
 * Add multiple logging/levels
 * Create tool to check a TD model's interface with ``fecsep``
 * Define a dependency strategy to ensure experiments' reproducibility.
-* Publish in `pypi`/`conda` and Zenodo
+* Publish in `conda`
 
 # Contributing
 
 We encourage all types of contributions, from reporting bugs, suggesting enhancements, adding new features and more. Please refer to the [Contribution Guidelines](https://github.com/cseptesting/floatcsep/blob/main/CONTRIBUTING.md) and the [Code of Conduct](https://github.com/cseptesting/floatcsep/blob/main/CODE_OF_CONDUCT.md) for more information
 
 # License
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # CSEP Floating Experiments [https://i.postimg.cc/6p5krRnB/float-CSEP-Logo-
 CMYK.png] **An application to deploy reproducible and prospective experiments
 of earthquake forecasting**
-[Documentation_Status] [Documentation_Status] [https://codecov.io/gh/
+[Documentation_Status] [Documentation_Status] [PyPI] [https://codecov.io/gh/
 cseptesting/floatcsep/branch/main/graph/badge.svg?token=LI4RSDOKA1] [DOI]
 * Set up a testing **experiment** for your earthquake forecasts using
 authoritative data sources and benchmarks. * **Encapsulate** the complete
 experiment's definition and rules in a couple of lines. * **Reproduce**,
 **reuse**, and **share** forecasting experiments from you, other researchers
 and institutions. # Table of Contents * [Installation](#installing-floatcsep) *
 [Documentation](https://floatcsep.readthedocs.io) * [Run and explore](#run-an-
@@ -30,17 +30,16 @@
 * `pyCSEP` [Github](https://github.com/sceccode/pycsep) * `pyCSEP`
 [Documentation](https://docs.cseptesting.org/) # Roadmap and Known Issues * Add
 functionality to compare original results and reproduced results * Add registry
 to filetrees (e.g. hash/byte count) for a proper experiment re-instantiation *
 Add report customization * Fix the hooks properly (user code) to be inserted
 into plotting/reporting functionalities. * Add multiple logging/levels * Create
 tool to check a TD model's interface with ``fecsep`` * Define a dependency
-strategy to ensure experiments' reproducibility. * Publish in `pypi`/`conda`
-and Zenodo # Contributing We encourage all types of contributions, from
-reporting bugs, suggesting enhancements, adding new features and more. Please
-refer to the [Contribution Guidelines](https://github.com/cseptesting/
-floatcsep/blob/main/CONTRIBUTING.md) and the [Code of Conduct](https://
-github.com/cseptesting/floatcsep/blob/main/CODE_OF_CONDUCT.md) for more
-information # License The `floatCSEP` (as well as `pyCSEP`) software is
-distributed under the BSD 3-Clause open-source license. Please see the [license
-file](https://github.com/cseptesting/floatcsep/blob/main/LICENSE) for more
-information.
+strategy to ensure experiments' reproducibility. * Publish in `conda` #
+Contributing We encourage all types of contributions, from reporting bugs,
+suggesting enhancements, adding new features and more. Please refer to the
+[Contribution Guidelines](https://github.com/cseptesting/floatcsep/blob/main/
+CONTRIBUTING.md) and the [Code of Conduct](https://github.com/cseptesting/
+floatcsep/blob/main/CODE_OF_CONDUCT.md) for more information # License The
+`floatCSEP` (as well as `pyCSEP`) software is distributed under the BSD 3-
+Clause open-source license. Please see the [license file](https://github.com/
+cseptesting/floatcsep/blob/main/LICENSE) for more information.
```

### Comparing `floatcsep-0.1.2/docs/Makefile` & `floatcsep-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/_static/CSEP2_Logo_CMYK.png` & `floatcsep-0.1.3/docs/_static/CSEP2_Logo_CMYK.png`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/_static/floatCSEP_Logo_CMYK.png` & `floatcsep-0.1.3/docs/_static/floatCSEP_Logo_CMYK.png`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/_static/floatcsep_logo.svg` & `floatcsep-0.1.3/docs/_static/floatcsep_logo.svg`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/conf.py` & `floatcsep-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/examples/case_a.rst` & `floatcsep-0.1.3/docs/examples/case_a.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/examples/case_b.rst` & `floatcsep-0.1.3/docs/examples/case_b.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/examples/case_c.rst` & `floatcsep-0.1.3/docs/examples/case_c.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/examples/case_d.rst` & `floatcsep-0.1.3/docs/examples/case_d.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/examples/case_e.rst` & `floatcsep-0.1.3/docs/examples/case_e.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/examples/case_f.rst` & `floatcsep-0.1.3/docs/examples/case_f.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/index.rst` & `floatcsep-0.1.3/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 floatCSEP: Floating Experiments
 ===============================
 
 Preliminary documentation.
 
 .. toctree::
-   :maxdepth: 0
+   :maxdepth: 1
    :caption: Get Started
 
    intro/installation.rst
    intro/concepts.rst
 
 
 .. toctree::
```

### Comparing `floatcsep-0.1.2/docs/intro/concepts.rst` & `floatcsep-0.1.3/docs/intro/concepts.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/intro/installation.rst` & `floatcsep-0.1.3/docs/intro/installation.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/docs/reference/api_reference.rst` & `floatcsep-0.1.3/docs/reference/api_reference.rst`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/floatcsep/accessors.py` & `floatcsep-0.1.3/floatcsep/accessors.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/floatcsep/artifacts/new_zealand_csep_testing.csv` & `floatcsep-0.1.3/floatcsep/artifacts/new_zealand_csep_testing.csv`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/floatcsep/artifacts/patterns.py` & `floatcsep-0.1.3/floatcsep/artifacts/patterns.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/floatcsep/evaluation.py` & `floatcsep-0.1.3/floatcsep/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         'conditional_likelihood_test': 'consistency',
         'negative_binomial_number_test': 'consistency',
         'binary_spatial_test': 'consistency',
         'binomial_spatial_test': 'consistency',
         'brier_score': 'consistency',
         'binary_conditional_likelihood_test': 'consistency',
         'paired_t_test': 'comparative',
+        'paired_ttest_point_process': 'comparative',
         'w_test': 'comparative',
         'binary_paired_t_test': 'comparative',
         'vector_poisson_t_w_test': 'batch',
         'sequential_likelihood': 'sequential',
         'sequential_information_gain': 'sequential_comparative'
     }
 
@@ -293,16 +294,16 @@
             if self.type in ['consistency', 'comparative']:
 
                 try:
                     for time_str in timewindow:
                         fig_path = tree(time_str, 'figures', self.name)
                         results = self.read_results(time_str, models, tree)
                         ax = func(results, plot_args=fargs, **fkwargs)
-                        if 'code' in self.plot_args:
-                            exec(self.plot_args['code'])
+                        if 'code' in fargs:
+                            exec(fargs['code'])
                         pyplot.savefig(fig_path, dpi=dpi)
                         if show:
                             pyplot.show()
 
                 except AttributeError as msg:
                     if self.type in ['consistency', 'comparative']:
                         for time_str in timewindow:
@@ -311,32 +312,32 @@
                                 fig_name = f'{self.name}_{model.name}'
 
                                 tree.paths[time_str]['figures'][fig_name] =\
                                     os.path.join(time_str, 'figures', fig_name)
                                 fig_path = tree(time_str, 'figures', fig_name)
                                 ax = func(result, plot_args=fargs, **fkwargs,
                                           show=False)
-                                if 'code' in self.plot_args:
-                                    exec(self.plot_args['code'])
+                                if 'code' in fargs:
+                                    exec(fargs['code'])
                                 pyplot.savefig(fig_path, dpi=dpi)
                                 if show:
                                     pyplot.show()
 
             elif self.type in ['sequential', 'sequential_comparative', 'batch']:
                 fig_path = tree(timewindow[-1], 'figures', self.name)
                 results = self.read_results(timewindow[-1], models, tree)
                 ax = func(results, plot_args=fargs, **fkwargs)
 
-                if 'code' in self.plot_args:
-                    exec(self.plot_args['code'])
+                if 'code' in fargs:
+                    exec(fargs['code'])
                 pyplot.savefig(fig_path, dpi=dpi)
                 if show:
                     pyplot.show()
 
-    def to_dict(self) -> dict:
+    def as_dict(self) -> dict:
         """
         Represents an Evaluation instance as a dictionary, which can be
         serialized and then parsed
         """
         out = {}
         included = ['model', 'ref_model', 'func_kwargs']
         for k, v in self.__dict__.items():
```

### Comparing `floatcsep-0.1.2/floatcsep/experiment.py` & `floatcsep-0.1.3/floatcsep/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import os
-import os.path
+import shutil
+import datetime
+from os.path import join, abspath, relpath, dirname, isfile, split, exists
 
 import csep
 import numpy
 import yaml
 import json
+import logging
 
 from typing import Union, List, Dict, Callable, Mapping, Sequence
 from matplotlib import pyplot
 from cartopy import crs as ccrs
 
-from csep.models import EvaluationResult
 from csep.core.catalogs import CSEPCatalog
 from csep.utils.time_utils import decimal_year
 
 from floatcsep import report
+from floatcsep.logger import add_fhandler
 from floatcsep.registry import PathTree
-from floatcsep.utils import NoAliasLoader, parse_csep_func, read_time_config, \
-    read_region_config, Task, TaskGraph, timewindow2str, str2timewindow, \
+from floatcsep.utils import NoAliasLoader, parse_csep_func, read_time_cfg, \
+    read_region_cfg, Task, TaskGraph, timewindow2str, str2timewindow, \
     magnitude_vs_time
 from floatcsep.model import Model
 from floatcsep.evaluation import Evaluation
 import warnings
 
 numpy.seterr(all="ignore")
 warnings.filterwarnings("ignore")
 
+log = logging.getLogger("floatLogger")
+
 
 class Experiment:
     """
 
     Main class that handles an Experiment's context. Contains all the
     specifications, instructions and methods to carry out an experiment.
 
     Args:
         name (str): Experiment name
-        path (str): Experiment working directory. All artifacts relative paths'
-                    are defined from here (e.g. model files, source code,
-                    catalog files, etc.)
         time_config (dict): Contains all the temporal specifications.
             It can contain the following keys:
 
             - start_date (:class:`datetime.datetime`):
               Experiment start date
             - end_date (:class:`datetime.datetime`):
               Experiment end date
@@ -50,16 +52,16 @@
             - intervals (:class:`int`): Number of testing intervals/windows
             - horizon (:class:`str`, :py:class:`float`): Time length of the
               forecasts (e.g. 1, 10, `1 year`, `2 days`). `ti` defaults to
               years, `td` to days.
             - growth (:class:`str`): `incremental` or `cumulative`
             - offset (:class:`float`): recurrence of forecast creation.
 
-            For further details, see :func:`~floatcsep.utils.timewindows_ti` and
-            :func:`~floatcsep.utils.timewindows_td`
+            For further details, see :func:`~floatcsep.utils.timewindows_ti`
+            and :func:`~floatcsep.utils.timewindows_td`
 
         region_config (dict): Contains all the spatial and magnitude
             specifications. It must contain the following keys:
 
             - region (:py:class:`str`,
               :class:`csep.core.regions.CartesianGrid2D`): The geographical
               region, which can be specified as:
@@ -112,47 +114,72 @@
                  time_config: dict = None,
                  region_config: dict = None,
                  catalog: str = None,
                  models: str = None,
                  tests: str = None,
                  postproc_config: str = None,
                  default_test_kwargs: dict = None,
+                 rundir: str = 'results',
+                 report_hook: dict = None,
                  **kwargs) -> None:
         # todo
         #  - instantiate from full experiment register (ignoring test/models
         #  config), or self-awareness functions?
         #  - instantiate as python objects (models/tests config)
         #  - check if model region matches experiment region for nonQuadTree?
         #    Or filter region?
         # Instantiate
-        self.name = name if name else 'floatingExp'
-        self.path = kwargs.get('path') if kwargs.get('path',
-                                                     None) else os.getcwd()
 
-        self.time_config = read_time_config(time_config, **kwargs)
-        self.region_config = read_region_config(region_config, **kwargs)
+        workdir = abspath(kwargs.get('path', os.getcwd()))
+        if kwargs.get('timestamp', False):
+            rundir = os.path.join(
+                rundir,
+                f'run_{datetime.datetime.utcnow().date().isoformat()}')
+        os.makedirs(os.path.join(workdir, rundir), exist_ok=True)
+        if kwargs.get(log, True):
+            logpath = os.path.join(workdir, rundir, 'experiment.log')
+            log.info(f'Logging at {logpath}')
+            add_fhandler(logpath)
+
+        self.name = name if name else 'floatingExp'
+        self.path = PathTree(workdir, rundir)
+        self.config_file = kwargs.get('config_file', None)
+        self.original_config = kwargs.get('original_config', None)
+        self.original_rundir = kwargs.get('original_rundir', None)
+        self.rundir = rundir
+        self.seed = kwargs.get('seed', None)
+        self.time_config = read_time_cfg(time_config, **kwargs)
+        self.region_config = read_region_cfg(region_config, **kwargs)
         self.model_config = models if isinstance(models, str) else None
         self.test_config = tests if isinstance(tests, str) else None
 
+        log.info(f'Setting up experiment {self.name}:')
+        log.info(f'\tStart: {self.start_date}')
+        log.info(f'\tEnd: {self.start_date}')
+        log.info(f'\tTime windows: {len(self.timewindows)}')
+        log.info(f'\tRegion: {self.region.name if self.region else None}')
+        log.info(f'\tMagnitude range: [{numpy.min(self.magnitudes)},'
+                 f' {numpy.max(self.magnitudes)}]')
+
         self.catalog = None
         self.models = []
         self.tests = []
 
         self.postproc_config = postproc_config if postproc_config else {}
         self.default_test_kwargs = default_test_kwargs
 
-        self.filetree = PathTree(self.path)
-
         self.catalog = catalog
-        self.models = self.set_models(models or kwargs.get('model_config'))
+        self.models = self.set_models(models or kwargs.get('model_config'),
+                                      kwargs.get('order', None))
         self.tests = self.set_tests(tests or kwargs.get('test_config'))
 
         self.tasks = []
         self.task_graph = None
 
+        self.report_hook = report_hook if report_hook else {}
         self.force_rerun = kwargs.get('force_rerun', False)
 
     def __getattr__(self, item: str) -> object:
         """
         Override built-in method to return attributes found within
         :attr:`region_config` or :attr:`time_config`
         """
@@ -175,92 +202,99 @@
         Adds time and region configs keys to instance scope.
         """
 
         _dir = list(super().__dir__()) + list(self.time_config.keys()) + list(
             self.region_config)
         return sorted(_dir)
 
-    def set_models(self, model_config: Union[Dict, str, List]) -> List:
+    def set_models(self, model_config: Union[Dict, str, List],
+                   order: List = None) -> List:
         """
 
         Parse the models' configuration file/dict. Instantiates all the models
         as :class:`floatcsep.model.Model` and store them into
         :attr:`Experiment.models`.
 
         Args:
             model_config (dict, list, str): configuration file or dictionary
              containing the model initialization attributes, as defined in
              :meth:`~floatcsep.model.Model`
-
+            order (list): desired order of models
 
         """
 
         models = []
         if isinstance(model_config, str):
-            modelcfg_path = self.filetree.abs(model_config)
-            _dir = self.filetree.absdir(model_config)
+            modelcfg_path = self.path.abs(model_config)
+            _dir = self.path.absdir(model_config)
             with open(modelcfg_path, 'r') as file_:
                 config_dict = yaml.load(file_, NoAliasLoader)
         elif isinstance(model_config, (dict, list)):
             config_dict = model_config
-            _path = [i['path'] for i in model_config[0].values()][0]
-            _dir = self.filetree.absdir(_path)
+            _dir = self.path.workdir
         elif model_config is None:
             return models
         else:
             raise NotImplementedError(f'Load for model type'
                                       f' {model_config.__class__}'
                                       f'not implemented ')
-
         for element in config_dict:
             # Check if the model is unique or has multiple submodels
-            if not any('flavours' in i for i in element.values()):
 
+            if not any('flavours' in i for i in element.values()):
                 name_ = next(iter(element))
-                # updates path to absolute
-                model_path = self.filetree.abs(_dir, element[name_]['path'])
-                model_i = {name_: {**element[name_], 'path': model_path}}
+                path_ = self.path.rel(_dir, element[name_]['path'])
+                model_i = {name_: {**element[name_],
+                                   'model_path': path_,
+                                   'workdir': self.path.workdir}}
+                model_i[name_].pop('path')
                 models.append(Model.from_dict(model_i))
+
             else:
                 model_flavours = list(element.values())[0]['flavours'].items()
                 for flav, flav_path in model_flavours:
                     name_super = next(iter(element))
-                    # updates path to absolute
                     path_super = element[name_super].get('path', '')
-                    path_sub = self.filetree.abs(_dir, path_super, flav_path)
-                    # path_sub = self._abspath(_dir, path_super, flav_path)[1]
+                    path_sub = self.path.rel(_dir, path_super, flav_path)
                     # updates name of submodel
                     name_flav = f'{name_super}@{flav}'
                     model_ = {name_flav: {**element[name_super],
-                                          'path': path_sub}}
+                                          'model_path': path_sub,
+                                          'workdir': self.path.workdir}}
+                    model_[name_flav].pop('path')
                     model_[name_flav].pop('flavours')
                     models.append(Model.from_dict(model_))
 
         # Checks if there is any repeated model.
         names_ = [i.name for i in models]
         if len(names_) != len(set(names_)):
             reps = set(
                 [i for i in names_ if (sum([j == i for j in names_]) > 1)])
             one = not bool(len(reps) - 1)
-            print(f'Warning: Model{"s" * (not one)} {reps}'
-                  f' {"is" * one + "are" * (not one)} repeated')
+            log.warning(f'Warning: Model{"s" * (not one)} {reps}'
+                        f' {"is" * one + "are" * (not one)} repeated')
+        log.info(f'\tModels: {[i.name for i in models]}')
+
+        if order:
+            models = [models[i] for i in order]
 
         return models
 
     def get_model(self, name: str) -> Model:
         """ Returns a Model by its name string """
         for model in self.models:
             if model.name == name:
                 return model
 
     def stage_models(self) -> None:
         """
         Stages all the experiment's models. See
         :meth:`floatcsep.model.Model.stage`
         """
+        log.info('Staging models')
         for i in self.models:
             i.stage(self.timewindows)
 
     def set_tests(self, test_config: Union[str, Dict, List]) -> list:
         """
         Parse the tests' configuration file/dict. Instantiate them as
         :class:`floatcsep.evaluation.Evaluation` and store them into
@@ -271,85 +305,89 @@
              containing the evaluation initialization attributes, as defined in
              :meth:`~floatcsep.evaluation.Evaluation`
 
         """
         tests = []
 
         if isinstance(test_config, str):
-            with open(self.filetree.abs(test_config), 'r') as config:
+            with open(self.path.abs(test_config), 'r') as config:
                 config_dict = yaml.load(config, NoAliasLoader)
             for eval_dict in config_dict:
                 tests.append(Evaluation.from_dict(eval_dict))
         elif isinstance(test_config, (dict, list)):
             for eval_dict in test_config:
                 tests.append(Evaluation.from_dict(eval_dict))
 
+        log.info(f'\tEvaluations: {[i.name for i in tests]}')
+
         return tests
 
     @property
     def catalog(self) -> CSEPCatalog:
         """
         Returns a CSEP catalog loaded from the given query function or
          a stored file if it exists.
         """
+        cat_path = self.path.abs(self._catpath)
+
         if callable(self._catalog):
-            if os.path.isfile(self._catpath):
+            if isfile(self._catpath):
                 return CSEPCatalog.load_json(self._catpath)
             bounds = {'start_time': min([item for sublist in self.timewindows
                                          for item in sublist]),
                       'end_time': max([item for sublist in self.timewindows
                                        for item in sublist]),
                       'min_magnitude': self.magnitudes.min(),
                       'max_depth': self.depths.max()}
             if self.region:
                 bounds.update({i: j for i, j in
                                zip(['min_longitude', 'max_longitude',
                                     'min_latitude', 'max_latitude'],
                                    self.region.get_bbox())})
 
             catalog = self._catalog(
-                catalog_id='cat',  # todo name as run
+                catalog_id='catalog',  # todo name as run
                 **bounds
             )
 
             if self.region:
                 catalog.filter_spatial(region=self.region)
                 catalog.region = None
             catalog.write_json(self._catpath)
 
             return catalog
 
-        elif os.path.isfile(self._catalog):
+        elif isfile(cat_path):
             try:
-                return CSEPCatalog.load_json(self._catpath)
+                return CSEPCatalog.load_json(cat_path)
             except json.JSONDecodeError:
-                return csep.load_catalog(self._catpath)
+                return csep.load_catalog(cat_path)
 
     @catalog.setter
     def catalog(self, cat: Union[Callable, CSEPCatalog, str]) -> None:
 
         if cat is None:
             self._catalog = None
             self._catpath = None
 
-        elif os.path.isfile(self.filetree.abs(cat)):
-            print(f"Using catalog from {cat}")
-            self._catalog = self.filetree.abs(cat)
-            self._catpath = self.filetree.abs(cat)
+        elif isfile(self.path.abs(cat)):
+            log.info(f"\tCatalog: '{cat}'")
+            self._catalog = self.path.rel(cat)
+            self._catpath = self.path.rel(cat)
 
         else:
             # catalog can be a function
             self._catalog = parse_csep_func(cat)
-            self._catpath = self.filetree.abs('catalog.json')
-            if os.path.isfile(self._catpath):
-                print(f"Using stored catalog "
-                      f"'{os.path.relpath(self._catpath, self.path)}', "
-                      f"obtained from function '{cat}'")
+            self._catpath = self.path.abs('catalog.json')
+            if isfile(self._catpath):
+                log.info(f"\tCatalog: stored "
+                         f"'{self._catpath}' "
+                         f"from '{cat}'")
             else:
-                print(f"Downloading catalog from function {cat}")
+                log.info(f"\tCatalog: '{cat}'")
 
     def get_test_cat(self, tstring: str = None) -> CSEPCatalog:
         """
 
         Filters the complete experiment catalog to a test sub-catalog bounded
         by the test time-window. Writes it to filepath defined in
         :attr:`Experiment.filetree`
@@ -381,23 +419,32 @@
         by the test time-window. Writes it to filepath defined in
         :attr:`Experiment.filetree`
 
         Args:
             tstring (str): Time window string
 
         """
-        start, end = str2timewindow(tstring)
-        sub_cat = self.catalog.filter(
-            [f'origin_time < {end.timestamp() * 1000}',
-             f'origin_time >= {start.timestamp() * 1000}',
-             f'magnitude >= {self.mag_min}',
-             f'magnitude < {self.mag_max}'], in_place=False)
-        if self.region:
-            sub_cat.filter_spatial(region=self.region)
-        sub_cat.write_json(filename=self.filetree(tstring, 'catalog'))
+        ""
+
+        testcat_name = self.path(tstring, 'catalog')
+        if not exists(testcat_name):
+            log.debug(
+                f'Filtering catalog to testing sub-catalog and saving to '
+                f'{testcat_name}')
+            start, end = str2timewindow(tstring)
+            sub_cat = self.catalog.filter(
+                [f'origin_time < {end.timestamp() * 1000}',
+                 f'origin_time >= {start.timestamp() * 1000}',
+                 f'magnitude >= {self.mag_min}',
+                 f'magnitude < {self.mag_max}'], in_place=False)
+            if self.region:
+                sub_cat.filter_spatial(region=self.region)
+            sub_cat.write_json(filename=testcat_name)
+        else:
+            log.debug(f'Using stored test sub-catalog from {testcat_name}')
 
     def set_input_cat(self, tstring: str, model: Model) -> None:
         """
 
         Filters the complete experiment catalog to a input sub-catalog filtered
         to the beginning of thetest time-window. Writes it to filepath defined
         in :attr:`Model.tree.catalog`
@@ -407,48 +454,41 @@
             model (:class:`~floatcsep.model.Model`): Model to give the input
              catalog
 
         """
         start, end = str2timewindow(tstring)
         sub_cat = self.catalog.filter(
             [f'origin_time < {start.timestamp() * 1000}'])
-        sub_cat.write_ascii(filename=model.tree('cat'))
+        sub_cat.write_ascii(filename=model.path('input_cat'))
 
-    def set_tasks(self, results_path=None, run_name=None):
+    def set_tasks(self):
         """
         Lazy definition of the experiment core tasks by wrapping instances,
         methods and arguments. Creates a graph with task nodes, while assigning
         task-parents to each node, depending on each Evaluation signature.
         The tasks can then be run sequentially as a list or asynchronous
         using the graph's node dependencies.
         For instance:
 
         * A forecast can only be made if catalog was filtered to its window
         * A consistency test can be run if the forecast exists in a window
         * A comparison test requires the forecast and ref forecast
         * A sequential test requires the forecasts exist for all windows
         * A batch test requires all forecast exist for a given window.
 
-        Args:
-            results_path (str, None): Path where the results will be stored.
-             Defaults to `results`.
-            run_name (str, None): Sub-folder where this particular run will be
-             stored. Default is ''
 
         Returns:
 
         """
 
         # Set the file path structure
-        self.filetree.set_pathtree(self.timewindows,
-                                   self.models,
-                                   self.tests,
-                                   results_path=results_path,
-                                   run_name=run_name)
+        self.path.build(self.timewindows, self.models, self.tests)
 
+        log.info("Setting up experiment's tasks")
+        log.debug("Pre-run: results' paths\n" + yaml.dump(self.path.asdict()))
         # Get the time windows strings
         tw_strings = timewindow2str(self.timewindows)
 
         # Prepare the testing catalogs
         task_graph = TaskGraph()
         for time_i in tw_strings:
             # The method call Experiment.set_test_cat(time_i) is created lazily
@@ -493,39 +533,39 @@
             if test_k.type == 'consistency':
                 for time_i in tw_strings:
                     for model_j in self.models:
                         task_ijk = Task(
                             instance=test_k,
                             method='compute',
                             timewindow=time_i,
-                            catalog=self.filetree(time_i, 'catalog'),
+                            catalog=self.path(time_i, 'catalog'),
                             model=model_j,
                             region=self.region,
-                            path=self.filetree(time_i, 'evaluations',
-                                               test_k, model_j))
+                            path=self.path(time_i, 'evaluations',
+                                           test_k, model_j))
                         task_graph.add(task_ijk)
                         # the forecast needs to have been created
                         task_graph.add_dependency(task_ijk,
                                                   dinst=model_j,
                                                   dmeth='create_forecast',
                                                   dkw=time_i)
             # Set up the Comparative Tests
             elif test_k.type == 'comparative':
                 for time_i in tw_strings:
                     for model_j in self.models:
                         task_ik = Task(
                             instance=test_k,
                             method='compute',
                             timewindow=time_i,
-                            catalog=self.filetree(time_i, 'catalog'),
+                            catalog=self.path(time_i, 'catalog'),
                             model=model_j,
                             ref_model=self.get_model(test_k.ref_model),
                             region=self.region,
-                            path=self.filetree(time_i, 'evaluations', test_k,
-                                               model_j)
+                            path=self.path(time_i, 'evaluations', test_k,
+                                           model_j)
                         )
                         task_graph.add(task_ik)
                         task_graph.add_dependency(task_ik,
                                                   dinst=model_j,
                                                   dmeth='create_forecast',
                                                   dkw=time_i)
                         task_graph.add_dependency(task_ik,
@@ -536,20 +576,20 @@
             # Set up the Sequential Scores
             elif test_k.type == 'sequential':
                 for model_j in self.models:
                     task_k = Task(
                         instance=test_k,
                         method='compute',
                         timewindow=tw_strings,
-                        catalog=[self.filetree(i, 'catalog')
+                        catalog=[self.path(i, 'catalog')
                                  for i in tw_strings],
                         model=model_j,
                         region=self.region,
-                        path=self.filetree(tw_strings[-1], 'evaluations',
-                                           test_k, model_j)
+                        path=self.path(tw_strings[-1], 'evaluations',
+                                       test_k, model_j)
                     )
                     task_graph.add(task_k)
                     for tw_i in tw_strings:
                         task_graph.add_dependency(task_k,
                                                   dinst=model_j,
                                                   dmeth='create_forecast',
                                                   dkw=tw_i)
@@ -557,20 +597,20 @@
             elif test_k.type == 'sequential_comparative':
                 tw_strs = timewindow2str(self.timewindows)
                 for model_j in self.models:
                     task_k = Task(
                         instance=test_k,
                         method='compute',
                         timewindow=tw_strs,
-                        catalog=[self.filetree(i, 'catalog') for i in tw_strs],
+                        catalog=[self.path(i, 'catalog') for i in tw_strs],
                         model=model_j,
                         ref_model=self.get_model(test_k.ref_model),
                         region=self.region,
-                        path=self.filetree(tw_strs[-1], 'evaluations', test_k,
-                                           model_j)
+                        path=self.path(tw_strs[-1], 'evaluations', test_k,
+                                       model_j)
                     )
                     task_graph.add(task_k)
                     for tw_i in tw_strings:
                         task_graph.add_dependency(task_k,
                                                   dinst=model_j,
                                                   dmeth='create_forecast',
                                                   dkw=tw_i)
@@ -583,20 +623,20 @@
             elif test_k.type == 'batch':
                 time_str = timewindow2str(self.timewindows[-1])
                 for model_j in self.models:
                     task_k = Task(
                         instance=test_k,
                         method='compute',
                         timewindow=time_str,
-                        catalog=self.filetree(time_str, 'catalog'),
+                        catalog=self.path(time_str, 'catalog'),
                         ref_model=self.models,
                         model=model_j,
                         region=self.region,
-                        path=self.filetree(time_str, 'evaluations', test_k,
-                                           model_j)
+                        path=self.path(time_str, 'evaluations', test_k,
+                                       model_j)
                     )
                     task_graph.add(task_k)
                     for m_j in self.models:
                         task_graph.add_dependency(task_k,
                                                   dinst=m_j,
                                                   dmeth='create_forecast',
                                                   dkw=time_str)
@@ -610,40 +650,41 @@
         todo:
          - Cleanup forecast (perhaps add a clean task in self.prepare_tasks,
             after all test had been run for a given forecast)
          - Memory monitor?
          - Queuer?
 
         """
+        log.info(f'Running {self.task_graph.ntasks} tasks')
+
+        if self.seed:
+            numpy.random.seed(self.seed)
+
         self.task_graph.run()
-        self.to_yml(self.filetree('config'), extended=True)
+        log.info(f'Calculation completed')
 
     def read_results(self, test: Evaluation, window: str) -> List:
         """
         Reads an Evaluation result for a given time window and returns a list
         of the results for all tested models.
         """
 
-        return test.read_results(window, self.models, self.filetree)
+        return test.read_results(window, self.models, self.path)
 
-    def plot_results(self, dpi: int = 300, show: bool = False) -> None:
+    def plot_results(self) -> None:
         """
         
         Plots all evaluation results
- 
-        Args:
-            dpi: Figure resolution with which to save
-            show: show in runtime
 
         """
-
+        log.info("Plotting evaluations")
         timewindows = timewindow2str(self.timewindows)
 
         for test in self.tests:
-            test.plot_results(timewindows, self.models, self.filetree)
+            test.plot_results(timewindows, self.models, self.path)
 
     def plot_catalog(self, dpi: int = 300, show: bool = False) -> None:
         """
 
         Plots the evaluation catalogs
 
         Args:
@@ -661,84 +702,84 @@
                      }
         plot_args.update(self.postproc_config.get('plot_catalog', {}))
 
         catalog = self.get_test_cat()
         if catalog.get_number_of_events() != 0:
             ax = catalog.plot(plot_args=plot_args, show=show)
             ax.get_figure().tight_layout()
-            ax.get_figure().savefig(self.filetree('catalog_figure'),
+            ax.get_figure().savefig(self.path('catalog_figure'),
                                     dpi=dpi)
 
             ax2 = magnitude_vs_time(catalog)
             ax2.get_figure().tight_layout()
-            ax2.get_figure().savefig(self.filetree('magnitude_time'),
+            ax2.get_figure().savefig(self.path('magnitude_time'),
                                      dpi=dpi)
 
         if self.postproc_config.get('all_time_windows'):
             timewindow = self.timewindows
 
             for tw in timewindow:
-                catpath = self.filetree(tw, 'catalog')
+                catpath = self.path(tw, 'catalog')
                 catalog = CSEPCatalog.load_json(catpath)
                 if catalog.get_number_of_events() != 0:
-
                     ax = catalog.plot(plot_args=plot_args, show=show)
                     ax.get_figure().tight_layout()
-                    ax.get_figure().savefig(self.filetree(tw, 'figures',
-                                                          'catalog'),
+                    ax.get_figure().savefig(self.path(tw, 'figures',
+                                                      'catalog'),
                                             dpi=dpi)
 
                     ax2 = magnitude_vs_time(catalog)
                     ax2.get_figure().tight_layout()
-                    ax2.get_figure().savefig(self.filetree(tw, 'figures',
-                                                           'magnitude_time'),
+                    ax2.get_figure().savefig(self.path(tw, 'figures',
+                                                       'magnitude_time'),
                                              dpi=dpi)
 
     def plot_forecasts(self) -> None:
         """
 
         Plots and saves all the generated forecasts
 
         """
 
         plot_fc_config = self.postproc_config.get('plot_forecasts')
         if plot_fc_config:
+            log.info("Plotting forecasts")
             if plot_fc_config is True:
                 plot_fc_config = {}
             try:
                 proj_ = plot_fc_config.get('projection')
                 if isinstance(proj_, dict):
                     proj_name = list(proj_.keys())[0]
                     proj_args = list(proj_.values())[0]
                 else:
                     proj_name = proj_
                     proj_args = {}
                 plot_fc_config['projection'] = getattr(ccrs, proj_name)(
                     **proj_args)
-            except (IndexError, KeyError, TypeError):
+            except (IndexError, KeyError, TypeError, AttributeError):
                 plot_fc_config['projection'] = ccrs.PlateCarree(
                     central_longitude=0.0)
 
             cat = plot_fc_config.get('catalog')
             cat_args = {}
             if cat:
                 cat_args = {'markersize': 7, 'markercolor': 'black',
-                            'title': None,
+                            'title': 'asd', 'grid': False,
                             'legend': False, 'basemap': None,
                             'region_border': False}
                 if self.region:
                     self.catalog.filter_spatial(self.region, in_place=True)
                 if isinstance(cat, dict):
                     cat_args.update(cat)
 
             window = self.timewindows[-1]
             winstr = timewindow2str(window)
 
             for model in self.models:
-                fig_path = self.filetree(winstr, 'forecasts', model.name)
+                fig_path = self.path(winstr, 'forecasts', model.name)
                 start = decimal_year(window[0])
                 end = decimal_year(window[1])
                 time = f'{round(end - start, 3)} years'
                 plot_args = {'region_border': False,
                              'cmap': 'magma',
                              'clabel': r'$\log_{10} N\left(M_w \in [{%.2f},'
                                        r'\,{%.2f}]\right)$ per '
@@ -768,22 +809,49 @@
 
     def generate_report(self) -> None:
         """
 
         Creates a report summarizing the Experiment's results
 
         """
+        log.info(f"Saving report into {self.path.rundir}")
+
+        self.path.build(self.timewindows, self.models, self.tests)
+        log.debug("Post-run: results' paths\n" + yaml.dump(self.path.asdict()))
 
         report.generate_report(self)
 
-    def check_reproducibility(self) -> None:
+    def make_repr(self):
+
+        log.info('Creating reproducibility config file')
+        repr_config = self.path('config')
 
-        pass
+        # Dropping region to results folder if it is a file
+        region_path = self.region_config.get('path', None)
+        if region_path:
+            if isfile(region_path) and region_path:
+                new_path = join(self.path.rundir, self.region_config['path'])
+                shutil.copy2(region_path, new_path)
+                self.region_config.pop('path')
+                self.region_config['region'] = self.path.rel(new_path)
+
+        # Dropping catalog to results folder
+        target_cat = join(self.path.workdir, self.path.rundir,
+                          split(self._catpath)[-1])
+        if not exists(target_cat):
+            shutil.copy2(self.path.abs(self._catpath), target_cat)
+        self._catpath = self.path.rel(target_cat)
+
+        relative_path = os.path.relpath(
+            self.path.workdir, os.path.join(self.path.workdir,
+                                            self.path.rundir))
+        self.path.workdir = relative_path
+        self.to_yml(repr_config, extended=True)
 
-    def to_dict(self, exclude: Sequence = ('magnitudes', 'depths',
+    def as_dict(self, exclude: Sequence = ('magnitudes', 'depths',
                                            'timewindows', 'filetree',
                                            'task_graph', 'tasks',
                                            'models', 'tests'),
                 extended: bool = False) -> dict:
         """
         Converts an Experiment instance into a dictionary.
 
@@ -794,17 +862,17 @@
         Returns:
             A dictionary with serialized instance's attributes, which are
             floatCSEP readable
         """
 
         def _get_value(x):
             # For each element type, transforms to desired string/output
-            if hasattr(x, 'to_dict') and extended:
-                # e.g. csep region, model, test, etc.
-                o = x.to_dict()
+            if hasattr(x, 'as_dict'):
+                # e.g. model, test, etc.
+                o = x.as_dict()
             else:
                 try:
                     try:
                         o = getattr(x, '__name__')
                     except AttributeError:
                         o = getattr(x, 'name')
                 except AttributeError:
@@ -821,72 +889,93 @@
                         if ((item not in exclude) and val_) or extended}
             elif isinstance(val, Sequence) and not isinstance(val, str):
                 return [iter_attr(i) for i in val]
             else:
                 return _get_value(val)
 
         listwalk = [(i, j) for i, j in self.__dict__.items() if
-                    not i.startswith('_')]
-        listwalk.insert(3, ('catalog', self._catpath))
+                    not i.startswith('_') and j]
+        listwalk.insert(6, ('catalog', self._catpath))
 
         dictwalk = {i: j for i, j in listwalk}
         # if self.model_config is None:
         #     dictwalk['models'] = iter_attr(self.models)
         # if self.test_config is None:
         #     dictwalk['tests'] = iter_attr(self.tests)
 
         return iter_attr(dictwalk)
 
     def to_yml(self, filename: str, **kwargs) -> None:
         """
 
-        Serializes the :class:`~floatcsep.experiment.Experiment` instance into a
-        .yml file.
+        Serializes the :class:`~floatcsep.experiment.Experiment` instance into
+        a .yml file.
 
         Note:
             This instance can then be reinstantiated using
             :meth:`~floatcsep.experiment.Experiment.from_yml`
 
         Args:
             filename: Name of the file onto which dump the instance
-            **kwargs: Passed to :meth:`~floatcsep.experiment.Experiment.to_dict`
+            **kwargs: Pass to :meth:`~floatcsep.experiment.Experiment.as_dict`
 
         Returns:
 
         """
 
         class NoAliasDumper(yaml.Dumper):
             def ignore_aliases(self, data):
                 return True
 
         with open(filename, 'w') as f_:
             yaml.dump(
-                self.to_dict(**kwargs), f_,
+                self.as_dict(**kwargs), f_,
                 Dumper=NoAliasDumper,
                 sort_keys=False,
                 default_flow_style=False,
                 indent=1,
                 width=70
             )
 
     @classmethod
-    def from_yml(cls, config_yml: str):
+    def from_yml(cls, config_yml: str, reprdir=None, **kwargs):
         """
 
         Initializes an experiment from a .yml file. It must contain the
         attributes described in the :class:`~floatcsep.experiment.Experiment`,
         :func:`~floatcsep.utils.read_time_config` and
         :func:`~floatcsep.utils.read_region_config` descriptions
 
         Args:
             config_yml (str): The path to the .yml file
+            reprdir (str): folder where to reproduce results
 
         Returns:
             An :class:`~floatcsep.experiment.Experiment` class instance
 
         """
+        log.info('Initializing experiment from .yml file')
         with open(config_yml, 'r') as yml:
-            config_dict = yaml.safe_load(yml)
-            if 'path' not in config_dict:
-                config_dict['path'] = os.path.abspath(
-                    os.path.dirname(config_yml))
-        return cls(**config_dict)
+
+            # experiment configuration file
+            _dict = yaml.safe_load(yml)
+            _dir_yml = dirname(config_yml)
+            # uses yml path and append if a rel/abs path is given in config.
+            _path = _dict.get('path', '')
+
+            # Only ABSOLUTE PATH
+            _dict['path'] = abspath(join(_dir_yml, _dict.get('path', '')))
+
+            # replaces rundir case reproduce option is used
+            if reprdir:
+                _dict['original_rundir'] = _dict.get('rundir', 'results')
+                _dict['rundir'] = relpath(join(_dir_yml, reprdir),
+                                          _dict['path'])
+                _dict['original_config'] = abspath(join(_dict['path'],
+                                                        _dict['config_file']))
+            else:
+
+                _dict['rundir'] = _dict.get('rundir',
+                                            kwargs.pop('rundir', 'results'))
+            _dict['config_file'] = relpath(config_yml, _dir_yml)
+            # print(_dict['rundir'])
+        return cls(**_dict, **kwargs)
```

### Comparing `floatcsep-0.1.2/floatcsep/extras.py` & `floatcsep-0.1.3/floatcsep/extras.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/floatcsep/model.py` & `floatcsep-0.1.3/floatcsep/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import json
 import os
 import numpy
 import csep
 import git
 import subprocess
+import logging
 
-from typing import List, Callable, Union, Dict, Mapping, Sequence
+from typing import List, Callable, Union, Mapping, Sequence
 from datetime import datetime
 
 from csep.core.forecasts import GriddedForecast, CatalogForecast
 from csep.utils.time_utils import decimal_year
 
 from floatcsep.accessors import from_zenodo, from_git
 from floatcsep.readers import ForecastParsers, HDF5Serializer, check_format
 from floatcsep.utils import timewindow2str, str2timewindow
 from floatcsep.registry import ModelTree
 
+log = logging.getLogger('floatLogger')
+
+
 class Model:
     """
 
     Class defining a forecast generating Model. Initializes a model source
     either from filesystem or web repositories, contains information about
     the Model's typology, and maps accordingly to a forecast generating
     function.
 
     Args:
         name (str): Name of the model
-        path (str): Relative path of the model (file or runnable code)
+        model_path (str): Relative path of the model (file or runnable code)
                     to the Experiment's instance path
         forecast_unit (float): Temporal unit of the forecast. Default to
                                years in time-independent models and days
                                in time-dependent
         use_db (bool): Flag the use of a database for speed/memory purposes
         func (str, ~collections.abc.Callable): Forecast generating function
                                                (for code models)
@@ -66,15 +70,15 @@
         - FILE   - read from file, scale in runtime             
                  - drop to db, scale from function in runtime   
         - CODE  - run, read from file              
                 - run, store in db, read from db   
 
     '''
 
-    def __init__(self, name: str, path: str,
+    def __init__(self, name: str, model_path: str,
                  forecast_unit: float = 1, use_db: bool = False,
                  func: Union[str, Callable] = None, func_kwargs: dict = None,
                  zenodo_id: int = None, giturl: str = None,
                  repo_hash: str = None, authors: List[str] = None,
                  doi: str = None, **kwargs) -> None:
 
         # todo:
@@ -83,23 +87,21 @@
         # Instantiate attributes
         self.name = name
         self.zenodo_id = zenodo_id
         self.giturl = giturl
         self.repo_hash = repo_hash
         self.authors = authors
         self.doi = doi
+
         self.forecast_unit = forecast_unit
         self.func = func
         self.func_kwargs = func_kwargs or {}
         self.use_db = use_db
 
-        self.path = path
-        args = kwargs.get('args_file', 'args.txt')
-        self.tree = ModelTree(self.name, path, args=args)
-
+        self.path = ModelTree(kwargs.get('workdir', os.getcwd()), model_path)
         # Set model temporal class
         if self.func:
             # Time-Dependent
             self.model_class = 'td'
             self.build = kwargs.get('build', 'docker')
             self.run_prefix = ''
 
@@ -113,75 +115,70 @@
 
     @property
     def dir(self) -> str:
         """
         Returns:
             The directory containing the model source.
         """
-        if os.path.isdir(self.path):
-            return self.path
+        if os.path.isdir(self.path('path')):
+            return self.path('path')
         else:
-            return os.path.dirname(self.path)
-
-    @property
-    def fmt(self) -> str:
-        return os.path.splitext(self.path)[1][1:]
+            return os.path.dirname(self.path('path'))
 
     def stage(self, timewindows=None) -> None:
         """
         Pre-steps to make the model runnable before integrating
             - Get from filesystem, Zenodo or Git
             - Pre-check model fileformat
             - Initialize database
             - Run model quality assurance (unit tests, runnable from floatcsep)
         """
-        kwargs = {}
-        self.get_source(self.zenodo_id, self.giturl, self.repo_hash)
-        if self.model_class == 'td':
-            self.build_model()
+        self.get_source(self.zenodo_id, self.giturl, branch=self.repo_hash)
         if self.use_db:
             self.init_db()
-        check_format(self.path, self.fmt, self.func)
-        self.model_qa()
+
         if self.model_class == 'td':
-            prefix = self.__dict__.get('prefix', None)
-            self.tree.set_pathtree(timewindows, prefix=prefix)
+            self.build_model()
+        self.path.build_tree(timewindows=timewindows,
+                             model_class=self.model_class,
+                             prefix=self.__dict__.get('prefix', self.name),
+                             args_file=self.__dict__.get('args_file', None),
+                             input_cat=self.__dict__.get('input_cat', None))
 
     def build_model(self):
 
         if self.build == 'pip' or self.build == 'venv':
-            self.build_venv()
-
-    def build_venv(self):
-
-        venv = os.path.join(self.path, self.__dict__.get('venv', 'venv'))
-        venvact = os.path.join(venv, 'bin', 'activate')
-
-        if not os.path.exists(venv):
-            print(f'Building model {self.name} using pip')
-            subprocess.run(['python', '-m', 'venv', venv])
-            print(f'\tVirtual environment created in {venv}')
-
-            build_cmd = f'source {venvact} &&' \
-                        f'pip install --upgrade pip &&' \
-                        f'pip install -e {self.path}'
-
-            cmd = ['bash', '-c', build_cmd]
-
-            process = subprocess.Popen(cmd,
-                                       stdout=subprocess.PIPE,
-                                       stderr=subprocess.STDOUT,
-                                       universal_newlines=True)
-            for line in process.stdout:
-                print(f'\t{line}', end='')
-            process.wait()
-            print(f'Nested environments is not well supported. '
-                  f'Consider using docker instead')
+            venv = os.path.join(self.path('path'),
+                                self.__dict__.get('venv', 'venv'))
+            venvact = os.path.join(venv, 'bin', 'activate')
+
+            if not os.path.exists(venv):
+                log.info(f'Building model {self.name} using pip')
+                subprocess.run(['python', '-m', 'venv', venv])
+                log.info(f'\tVirtual environment created in {venv}')
+                build_cmd = f'source {venvact} && ' \
+                            f'pip install --upgrade pip && ' \
+                            f'pip install -e {self.path("path")}'
+
+                cmd = ['bash', '-c', build_cmd]
+
+                log.info(f'\tInstalling dependencies')
+
+                process = subprocess.Popen(cmd,
+                                           stdout=subprocess.PIPE,
+                                           stderr=subprocess.STDOUT,
+                                           universal_newlines=True)
+                for line in process.stdout:
+                    log.info(f'\t{line[:-1]}')
+                process.wait()
+                log.info(f'\tEnvironment ready')
+                log.warning(f'\tNested environments is not fully supported. '
+                            f'Consider using docker instead')
 
-        self.run_prefix = f'cd {self.path} && source {venvact} &&'
+            self.run_prefix = f'cd {self.path("path")} && source {venvact} && '
 
     def get_source(self, zenodo_id: int = None, giturl: str = None,
                    force: bool = False,
                    **kwargs) -> None:
         """
 
         Search, download or clone the model source in the filesystem, zenodo
@@ -195,37 +192,41 @@
              source
             force (bool): Forces to re-query the model from a web repository
             **kwargs: see :func:`~floatcsep.utils.from_zenodo` and
              :func:`~floatcsep.utils.from_git`
 
 
         """
-
-        if os.path.exists(self.path) and not force:
+        if os.path.exists(self.path('path')) and not force:
             return
 
         os.makedirs(self.dir, exist_ok=True)
 
         if zenodo_id:
+            log.info(f'Retrieving model {self.name} from zenodo id: '
+                     f'{zenodo_id}')
             try:
-                from_zenodo(zenodo_id, self.dir if self.fmt else self.path,
-                            force=force)
+                from_zenodo(zenodo_id, self.dir if self.path.fmt
+                            else self.path('path'), force=force)
             except (KeyError, TypeError) as msg:
                 raise KeyError(f'Zenodo identifier is not valid: {msg}')
 
         elif giturl:
+            log.info(f'Retrieving model {self.name} from git url: '
+                     f'{giturl}')
             try:
-                from_git(giturl, self.dir if self.fmt else self.path,
-                         **kwargs)
+                from_git(giturl, self.dir if self.path.fmt
+                         else self.path('path'), **kwargs)
             except (git.NoSuchPathError, git.CommandError) as msg:
                 raise git.NoSuchPathError(f'git url was not found {msg}')
         else:
             raise FileNotFoundError('Model has no path or identified')
 
-        if not os.path.exists(self.dir) or not os.path.exists(self.path):
+        if not os.path.exists(self.dir) or not \
+                os.path.exists(self.path('path')):
             raise FileNotFoundError(
                 f"Directory '{self.dir}' or file {self.path}' do not exist. "
                 f"Please check the specified 'path' matches the repo "
                 f"structure")
 
     def init_db(self, dbpath: str = '', force: bool = False) -> None:
         """
@@ -237,60 +238,52 @@
             dbpath (str): Path to drop the HDF5 database. Defaults to same path
              replaced with an `hdf5` extension
             force (bool): Forces the serialization even if the DB already
              exists
 
         """
         # todo Think about distinction btwn 'TI' and 'Gridded' models.
-        if self.fmt and self.model_class == 'ti':
-
-            parser = getattr(ForecastParsers, self.fmt)
-            rates, region, mag = parser(self.path)
 
+        if self.model_class == 'ti':
+            parser = getattr(ForecastParsers, self.path.fmt)
+            rates, region, mag = parser(self.path('path'))
             db_func = HDF5Serializer.grid2hdf5
+
             if not dbpath:
-                dbpath = self.path.replace(self.fmt, 'hdf5')
+                dbpath = self.path.path.replace(self.path.fmt, 'hdf5')
+                self.path.database = dbpath
 
-            if not os.path.isfile(dbpath) or force:
-                # Drop Source file into DB
+            if not os.path.isfile(self.path.abs(dbpath)) or force:
+                log.info(f'Serializing model {self.name} into HDF5 format')
                 db_func(rates, region, mag,
-                        hdf5_filename=dbpath,
+                        hdf5_filename=self.path.abs(dbpath),
                         unit=self.forecast_unit)
 
-            self.path = dbpath
-
         else:
             raise NotImplementedError('TD serialization not implemented')
 
     def rm_db(self) -> None:
         """ Clean up the generated HDF5 File"""
 
         if self.use_db:
             if os.path.isfile(self.path) and self.fmt == 'hdf5':
                 os.remove(self.path)
             else:
-                print("The HDF5 file does not exist")
-
-    def model_qa(self) -> None:
-        """ Run model quality assurance (Unit and Integration tests).
-        Should not run if the repo has not been modified.
-        Not implemented """
-        pass
+                log.warning(f"The HDF5 file {self.path} does not exist")
 
     def get_forecast(self,
                      tstring: Union[str, list] = None,
                      region=None
                      ) -> Union[GriddedForecast, CatalogForecast,
                                 List[GriddedForecast], List[CatalogForecast]]:
 
         """ Wrapper that just returns a forecast, which should hide the
          access method (db storage, ti_td, etc.) under the hood"""
 
         if self.model_class == 'ti':
-
             if isinstance(tstring, str):
                 # If only one timewindow string is passed
                 try:
                     # If they are retrieved from the Evaluation class
                     return self.forecasts[tstring]
                 except KeyError:
                     # In case they are called from postprocess
@@ -307,15 +300,15 @@
                         f'Forecasts {*tstring,} have not been created yet')
                 return forecasts
 
         elif self.model_class == 'td':
             if isinstance(tstring, str):
                 # If one time window string is passed
                 # default forecast naming
-                fc_path = self.tree('forecasts', tstring)
+                fc_path = self.path('forecasts', tstring)
                 # default forecasts folder
                 # A region must be given to the forecast
                 return csep.load_catalog_forecast(fc_path, region=region)
 
     def create_forecast(self, tstring: str,
                         **kwargs) -> None:
         """
@@ -336,21 +329,22 @@
         """
         start_date, end_date = str2timewindow(tstring)
         # Model src is a file
         if self.model_class == 'ti':
             self.forecast_from_file(start_date, end_date, **kwargs)
         # Model src is a func or binary
         else:
-            fc_path = self.tree('forecasts', tstring)
+            fc_path = self.path('forecasts', tstring)
             if kwargs.get('force') or not os.path.exists(fc_path):
                 self.forecast_from_func(start_date, end_date,
                                         **self.func_kwargs,
                                         **kwargs)
             else:
-                print('Forecast already exists')
+                log.info(f'Forecast of {tstring} of model {self.name} already '
+                         f'exists')
 
     def forecast_from_file(self, start_date: datetime, end_date: datetime,
                            **kwargs) -> None:
         """
 
         Generates a forecast from a file, by parsing and scaling it to
         the desired time window. H
@@ -362,59 +356,64 @@
              :class:`csep.core.forecasts.GriddedForecast`
 
         """
 
         time_horizon = decimal_year(end_date) - decimal_year(start_date)
         tstring = timewindow2str([start_date, end_date])
 
-        f_parser = getattr(ForecastParsers, self.fmt)
-        rates, region, mags = f_parser(self.path)
+        f_path = self.path('forecasts', tstring)
+        f_parser = getattr(ForecastParsers, self.path.fmt)
+
+        rates, region, mags = f_parser(f_path)
 
         forecast = GriddedForecast(
             name=f'{self.name}',
             data=rates,
             region=region,
             magnitudes=mags,
             start_time=start_date,
             end_time=end_date
         )
 
         scale = time_horizon / self.forecast_unit
         if scale != 1.0:
             forecast = forecast.scale(scale)
 
-        print(
-            f"Forecast expected count: {forecast.event_count:.2f}"
+        log.debug(
+            f"Model {self.name}:\n"
+            f"\tForecast expected count: {forecast.event_count:.2f}"
             f" with scaling parameter: {time_horizon:.1f}")
 
         self.forecasts[tstring] = forecast
 
     def forecast_from_func(self, start_date: datetime, end_date: datetime,
                            **kwargs) -> None:
 
         self.prepare_args(start_date, end_date, **kwargs)
+        log.info(f'Running {self.name} using {self.build}:'
+                 f' {timewindow2str([start_date, end_date])}')
 
         self.run_model()
 
     def prepare_args(self, start, end, **kwargs):
 
-        filepath = os.path.join(self.path, self.tree('args'))
+        filepath = self.path('args_file')
         fmt = os.path.splitext(filepath)[1]
 
         if fmt == '.txt':
             def replace_arg(arg, val, fp):
-                with open(fp, 'r') as file_:
-                    lines = file_.readlines()
+                with open(fp, 'r') as filearg_:
+                    lines = filearg_.readlines()
 
                 pattern_exists = False
                 for k, line in enumerate(lines):
                     if line.startswith(arg):
                         lines[k] = f"{arg} = {val}\n"
                         pattern_exists = True
-                        break  # Assuming there's only one occurrence of the key
+                        break  # assume there's only one occurrence of the key
                 if not pattern_exists:
                     lines.append(f"{arg} = {val}\n")
                 with open(fp, 'w') as file:
                     file.writelines(lines)
 
             replace_arg('start_date', start.isoformat(), filepath)
             replace_arg('end_date', end.isoformat(), filepath)
@@ -427,43 +426,41 @@
             args['end_date'] = end.isoformat()
 
             args.update(kwargs)
 
             with open(filepath, 'w') as file_:
                 json.dump(args, file_, indent=2)
 
-
     def run_model(self):
 
         if self.build == 'pip' or self.build == 'venv':
-            print(f'Running model {self.name} using venv')
-            run_func = f'{self.func} {self.tree("args")}'
-            cmd = ['bash', '-c',
-                   f'{self.run_prefix} {run_func}']
+            run_func = f'{self.func} {self.path("args_file")}'
+            cmd = ['bash', '-c', f'{self.run_prefix} {run_func}']
             process = subprocess.Popen(cmd,
                                        stdout=subprocess.PIPE,
                                        stderr=subprocess.STDOUT,
                                        universal_newlines=True)
             for line in process.stdout:
-                print(f'\t{line}', end='')
+                log.info(f'\t{line[:-1]}')
             process.wait()
 
-    def to_dict(self, excluded=('name', 'forecasts')):
+    def as_dict(self, excluded=('name', 'forecasts', 'workdir')):
         """
 
         Returns:
             Dictionary with relevant attributes. Model can be reinstantiated
             from this dict
 
         """
+
         def _get_value(x):
             # For each element type, transforms to desired string/output
-            if hasattr(x, 'to_dict'):
-                # e.g. csep region, model, test, etc.
-                o = x.to_dict()
+            if hasattr(x, 'as_dict'):
+                # e.g. model, evaluation, filetree, etc.
+                o = x.as_dict()
             else:
                 try:
                     try:
                         o = getattr(x, '__name__')
                     except AttributeError:
                         o = getattr(x, 'name')
                 except AttributeError:
@@ -479,16 +476,16 @@
                 return {item: iter_attr(val_) for item, val_ in val.items()
                         if ((item not in excluded) and val_)}
             elif isinstance(val, Sequence) and not isinstance(val, str):
                 return [iter_attr(i) for i in val]
             else:
                 return _get_value(val)
 
-        listwalk = [(i, j) for i, j in self.__dict__.items() if
-                    not i.startswith('_')]
+        listwalk = [(i, j) for i, j in sorted(self.__dict__.items()) if
+                    not i.startswith('_') and j]
 
         dictwalk = {i: j for i, j in listwalk}
         # if self.model_config is None:
         #     dictwalk['models'] = iter_attr(self.models)
         # if self.test_config is None:
         #     dictwalk['tests'] = iter_attr(self.tests)
```

### Comparing `floatcsep-0.1.2/floatcsep/readers.py` & `floatcsep-0.1.3/floatcsep/readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os.path
-
 import h5py
 import pandas
 import argparse
 import numpy
 import xml.etree.ElementTree as eTree
-import itertools
 from csep.models import Polygon
 from csep.core.regions import QuadtreeGrid2D, CartesianGrid2D
 import time
+import logging
+log = logging.getLogger(__name__)
 
 
 class ForecastParsers:
 
     @staticmethod
     def dat(filename):
         data = numpy.loadtxt(filename)
@@ -71,15 +71,15 @@
                 cell_dim = {i[0]: float(i[1]) for i in children.attrib.items()}
                 metadata['defaultCellDimension'] = cell_dim
             elif 'depthLayer' in children.tag:
                 depth = {i[0]: float(i[1]) for i in root[0][k].attrib.items()}
                 cells = root[0][k]
                 metadata['depthLayer'] = depth
         if verbose:
-            print(f'Forecast with metadata:\n{metadata}')
+            log.debug(f'Forecast with metadata:\n{metadata}')
 
         for cell in cells:
             cell_data = []
             m_cell_bins = []
             for i, m in enumerate(cell.iter()):
                 if i == 0:
                     cell_data.extend([float(m.attrib['lon']),
@@ -195,15 +195,16 @@
             else:
                 dh = db[f'{group}/dh'][:][0]
                 bboxes = db[f'{group}/bboxes'][:]
                 poly_mask = db[f'{group}/poly_mask'][:]
                 region = CartesianGrid2D(
                     [Polygon(bbox) for bbox in bboxes], dh, mask=poly_mask)
 
-        print(f'Loading from hdf5 took: {time.process_time() - start}')
+        log.debug(f'Loading from hdf5 {filename} took:'
+                  f' {time.process_time() - start:.2f}')
 
         return rates, region, magnitudes
 
 
 class HDF5Serializer:
     @staticmethod
     def grid2hdf5(rates, region, mag, grp='', hdf5_filename=None,
@@ -246,15 +247,16 @@
                     else:
                         shape = len(v)
                         dtype = type(v[0])
                     hfile.require_dataset(f'{grp}/{key}', shape=shape,
                                           dtype=dtype)
                     hfile[f'{grp}/{key}'][:] = v
 
-        print(f'Serializing from csv took: {time.process_time() - start}')
+        log.debug(f'Storing to hdf5 {hdf5_filename} took:'
+                  f'{time.process_time() - start:2f}')
 
 
 def check_format(filename, fmt=None, func=None):
     if fmt is None:
         fmt = os.path.splitext(filename)[-1][1:]
 
     if fmt == 'xml':
```

### Comparing `floatcsep-0.1.2/floatcsep/registry.py` & `floatcsep-0.1.3/floatcsep/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,40 @@
+import dataclasses
 import os
-from dataclasses import dataclass, field, asdict
+from os.path import join, abspath, relpath, normpath, dirname, exists
+from dataclasses import dataclass, field
 from typing import Sequence
 from floatcsep.utils import timewindow2str
 
 
 @dataclass
 class ModelTree:
-    name: str
+    workdir: str
     path: str
-    fmt: str = 'csv'
-    args: str = None
-    cat: str = None
+    database: str = None
+    args_file: str = None
+    input_cat: str = None
     forecasts: dict = field(default_factory=dict)
     inventory: dict = field(default_factory=dict)
 
     def __call__(self, *args):
 
         val = self.__dict__
         for i in args:
             parsed_arg = self._parse_arg(i)
             val = val[parsed_arg]
 
-        return self.abs(self.path, val)
+        return self.abs(val)
+
+    @property
+    def fmt(self) -> str:
+        if self.database:
+            return os.path.splitext(self.database)[1][1:]
+        else:
+            return os.path.splitext(self.path)[1][1:]
 
     @staticmethod
     def _parse_arg(arg):
         if isinstance(arg, (list, tuple)):
             return timewindow2str(arg)
         elif isinstance(arg, str):
             return arg
@@ -35,105 +44,114 @@
             return arg.__name__
         else:
             raise Exception('Arg is not found')
 
     def __eq__(self, other):
         return self.path == other
 
-    def to_dict(self):
-        return asdict(self)
+    def as_dict(self):
+        return self.path
+
+    def asdict(self):
+        return dataclasses.asdict(self)
 
     def abs(self, *paths: Sequence[str]) -> str:
         """ Gets the absolute path of a file, when it was defined relative to
          the experiment working dir."""
 
-        _path = os.path.normpath(
-            os.path.abspath(os.path.join(self.path, *paths)))
-        _dir = os.path.dirname(_path)
+        _path = normpath(abspath(join(self.workdir, *paths)))
+        _dir = dirname(_path)
         return _path
 
     def absdir(self, *paths: Sequence[str]) -> str:
         """ Gets the absolute path of a file, when it was defined relative to
          the experiment working dir."""
 
-        _path = os.path.normpath(
-            os.path.abspath(os.path.join(self.workdir, *paths)))
-        _dir = os.path.dirname(_path)
+        _path = normpath(abspath(join(self.workdir, *paths)))
+        _dir = dirname(_path)
         return _dir
 
     def fileexists(self, *args):
-        abspath = self.__call__(*args)
-        return os.path.exists(abspath)
+        file_abspath = self.__call__(*args)
+        return exists(file_abspath)
 
-    def set_pathtree(self,
-                     timewindows=None,
-                     prefix=None) -> None:
+    def build_tree(self,
+                   timewindows=None,
+                   model_class='ti',
+                   prefix=None,
+                   args_file=None,
+                   input_cat=None) -> None:
         """
 
         Creates the run directory, and reads the file structure inside
 
         Args:
-            timewindows: List of time windows, or representing string.
-            models: List of models or model names
-            tests: List of tests or test names
-            results_path: path to store
-            run_name: name of run
+            timewindows (list(str)): List of time windows or strings.
+            model_class (str): Time-indendent (ti) or time-dependent (td)
+            prefix (str): prefix of the model forecast filenames if TD
+            args_file (str): input arguments path of the model if TD
+            input_cat (str): input catalog path of the model if TD
 
         Returns:
             run_folder: Path to the run.
              exists: flag if forecasts, catalogs and test_results if they
              exist already
              target_paths: flag to each element of the gefe (catalog and
              evaluation results)
 
         """
-
-        # grab names for creating directories
-        subfolders = ['input', 'forecasts']
-        dirtree = {folder: self.abs(self.path, folder) for
-                   folder in subfolders}
-        # set args path
-        self.args = os.path.join('input', self.args or 'args.txt')
-        # set cat path
-        self.cat = os.path.join('input', self.cat or 'catalog.csv')
-
-        # create directories if they don't exist
-        for _, folder_ in dirtree.items():
-            os.makedirs(folder_, exist_ok=True)
-
         if timewindows is None:
             return
         windows = timewindow2str(timewindows)
+        if model_class == 'ti':
+            fname = self.database if self.database else self.path
+            fc_files = {win: fname for win in windows}
+            fc_exists = {win: exists(fc_files[win]) for win in windows}
+
+        elif model_class == 'td':
+            args = args_file if args_file else join('input', 'args.txt')
+            self.args_file = join(self.path, args)
+            input_cat = input_cat if input_cat else join('input',
+                                                         'catalog.csv')
+            self.input_cat = join(self.path, input_cat)
+            # grab names for creating directories
+            subfolders = ['input', 'forecasts']
+            dirtree = {folder: self.abs(self.path, folder) for
+                       folder in subfolders}
 
-        # set forecast names
-        fc_files = {win: os.path.join('forecasts',
-                                      f'{prefix or self.name}_{win}.{self.fmt}') for win
-                    in windows}
-
-        exists = {win: any(file for file in
-                           list(os.listdir(dirtree['forecasts'])))
-                  for win in windows}
+            # create directories if they don't exist
+            for _, folder_ in dirtree.items():
+                os.makedirs(folder_, exist_ok=True)
+
+            # set forecast names
+            fc_files = {win: join(dirtree['forecasts'],
+                                  f'{prefix}_{win}.csv')  # todo other formats?
+                        for win in windows}
+
+            fc_exists = {win: any(file for file in
+                               list(os.listdir(dirtree['forecasts'])))
+                      for win in windows}
 
         self.forecasts = fc_files
-        self.inventory = exists
+        self.inventory = fc_exists
 
 
 @dataclass
 class PathTree:
     workdir: str
-    run_folder: str = 'results'
+    rundir: str = 'results'
     paths: dict = field(default_factory=dict)
+    result_exists: dict = field(default_factory=dict)
 
     def __call__(self, *args):
         val = self.paths
         for i in args:
             parsed_arg = self._parse_arg(i)
             val = val[parsed_arg]
-
-        return self.abs(self.run_folder, val)
+        return self.abs(self.rundir, val)
 
     @staticmethod
     def _parse_arg(arg):
         if isinstance(arg, (list, tuple)):
             return timewindow2str(arg)
         elif isinstance(arg, str):
             return arg
@@ -143,127 +161,141 @@
             return arg.__name__
         else:
             raise Exception('Arg is not found')
 
     def __eq__(self, other):
         return self.workdir == other
 
-    def to_dict(self):
-        return asdict(self)
+    def as_dict(self):
+        return self.workdir
+
+    def asdict(self):
+        return dataclasses.asdict(self)
 
     def abs(self, *paths: Sequence[str]) -> str:
         """ Gets the absolute path of a file, when it was defined relative to
          the experiment working dir."""
 
-        _path = os.path.normpath(
-            os.path.abspath(os.path.join(self.workdir, *paths)))
-        _dir = os.path.dirname(_path)
+        _path = normpath(abspath(join(self.workdir, *paths)))
         return _path
 
+    def rel(self, *paths: Sequence[str]) -> str:
+        """ Gets the relative path of a file, when it was defined relative to
+         the experiment working dir."""
+
+        _abspath = normpath(
+            abspath(join(self.workdir, *paths)))
+        _relpath = relpath(_abspath, self.workdir)
+        return _relpath
+
     def absdir(self, *paths: Sequence[str]) -> str:
         """ Gets the absolute path of a file, when it was defined relative to
          the experiment working dir."""
 
-        _path = os.path.normpath(
-            os.path.abspath(os.path.join(self.workdir, *paths)))
-        _dir = os.path.dirname(_path)
+        _path = normpath(
+            abspath(join(self.workdir, *paths)))
+        _dir = dirname(_path)
         return _dir
 
+    def reldir(self, *paths: Sequence[str]) -> str:
+        """ Gets the absolute path of a file, when it was defined relative to
+         the experiment working dir."""
+
+        _path = normpath(
+            abspath(join(self.workdir, *paths)))
+        _dir = dirname(_path)
+        _reldir = relpath(_dir, self.workdir)
+        return _reldir
+
     def fileexists(self, *args):
 
-        abspath = self.__call__(*args)
-        return os.path.exists(abspath)
+        file_abspath = self.__call__(*args)
+        return exists(file_abspath)
 
-    def set_pathtree(self,
-                     timewindows=None,
-                     models=None,
-                     tests=None,
-                     results_path: str = None,
-                     run_name: str = None) -> None:
+    def build(self,
+              timewindows=None,
+              models=None,
+              tests=None) -> None:
         """
 
         Creates the run directory, and reads the file structure inside
 
         Args:
             timewindows: List of time windows, or representing string.
             models: List of models or model names
             tests: List of tests or test names
-            results_path: path to store
-            run_name: name of run
 
         Returns:
             run_folder: Path to the run.
              exists: flag if forecasts, catalogs and test_results if they
              exist already
              target_paths: flag to each element of the gefe (catalog and
              evaluation results)
 
         """
-
         # grab names for creating directories
         windows = timewindow2str(timewindows)
         models = [i.name for i in models]
         tests = [i.name for i in tests]
 
         # todo create datetime parser for filenames
         # todo find better way to name paths
 
         # Determine required directory structure for run
-        # results > test_date > time_window > cats / evals / figures
+        # results > time_window > cats / evals / figures
 
-        run_folder = os.path.join(results_path or 'results', run_name or '')
+        run_folder = self.rundir
 
         subfolders = ['catalog', 'evaluations', 'figures', 'forecasts']
         dirtree = {
-            win: {folder: self.abs(run_folder, win, folder) for
-                  folder
-                  in subfolders} for win in windows}
+            win: {folder: self.abs(run_folder, win, folder)
+                  for folder in subfolders} for win in windows}
 
         # create directories if they don't exist
         for tw, tw_folder in dirtree.items():
             for _, folder_ in tw_folder.items():
                 os.makedirs(folder_, exist_ok=True)
 
         # Check existing files
         files = {win: {name: list(os.listdir(path)) for name, path in
                        windir.items()} for win, windir in dirtree.items()}
 
-        exists = {win: {
+        file_exists = {win: {
             'forecasts': False,
             'catalog': any(file for file in files[win]['catalog']),
             'evaluations': {
                 test: {
                     model: any(f'{test}_{model}.json' in file for file in
                                files[win]['evaluations'])
                     for model in models
                 }
                 for test in tests
             }
         } for win in windows}
 
         target_paths = {
-            'config': 'run_config.yml',
+            'config': 'repr_config.yml',
             'catalog_figure': 'catalog',
-            'magnitude_time': 'magnitude_time',
+            'magnitude_time': 'events',
             **{win: {
-                'models': {model: {'forecasts': None} for model in models},
-                'catalog': os.path.join(win, 'catalog', 'catalog.json'),
+                'catalog': join(win, 'catalog', 'test_catalog.json'),
                 'evaluations': {
                     test: {
-                        model: os.path.join(win, 'evaluations',
-                                            f'{test}_{model}.json')
+                        model: join(win, 'evaluations',
+                                    f'{test}_{model}.json')
                         for model in models
                     }
                     for test in tests},
                 'figures': {
-                    **{test: os.path.join(win, 'figures', f'{test}')
+                    **{test: join(win, 'figures', f'{test}')
                        for test in tests},
-                    'catalog': os.path.join(win, 'figures', 'catalog'),
-                    'magnitude_time': os.path.join(win, 'figures',
-                                                   'magnitude_time')
+                    'catalog': join(win, 'figures', 'catalog'),
+                    'magnitude_time': join(win, 'figures',
+                                           'magnitude_time')
                 },
-                'forecasts': {model: os.path.join(win, 'forecasts', f'{model}')
+                'forecasts': {model: join(win, 'forecasts', f'{model}')
                               for model in models}
             } for win in windows}
         }
         self.paths = target_paths
-        self.run_folder = run_folder
+        self.result_exists = file_exists
+
```

### Comparing `floatcsep-0.1.2/floatcsep/report.py` & `floatcsep-0.1.3/floatcsep/report.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,35 +14,43 @@
 
 
 def generate_report(experiment, timewindow=-1):
 
     timewindow = experiment.timewindows[timewindow]
     timestr = timewindow2str(timewindow)
 
+    hooks = experiment.report_hook
     report = MarkdownReport()
     report.add_title(
-        f"Experiment Report - {experiment.name}", ''
+        f"Experiment Report - {experiment.name}", hooks.get('title_text', '')
     )
+
     report.add_heading("Objectives", level=2)
+
     objs = [
         "Describe the predictive skills of posited hypothesis about "
         "seismogenesis with earthquakes of"
         f" M>{min(experiment.magnitudes)}.",
     ]
+
+    if hooks.get('objectives', None):
+        for i in hooks.get('objectives'):
+            objs.append(i)
+
     report.add_list(objs)
 
     report.add_heading("Authoritative Data", level=2)
 
     # Generate catalog plot
     if experiment.catalog is not None:
         experiment.plot_catalog()
         report.add_figure(
             f"Input catalog",
-            [experiment.filetree('catalog_figure'),
-             experiment.filetree('magnitude_time')],
+            [experiment.path('catalog_figure'),
+             experiment.path('magnitude_time')],
             level=3,
             ncols=1,
             caption="Evaluation catalog from "
                     f"{experiment.start_date} until {experiment.end_date}. "  
                     f"Earthquakes are filtered above Mw"
                     f" {min(experiment.magnitudes)}.",
             add_ext=True
@@ -58,34 +66,34 @@
     )
 
     test_names = [test.name for test in experiment.tests]
     report.add_list(test_names)
 
     # Include results from Experiment
     for test in experiment.tests:
-        fig_path = experiment.filetree(timestr, 'figures', test)
+        fig_path = experiment.path(timestr, 'figures', test)
         width = test.plot_args[0].get('figsize', [4])[0] * 96
         report.add_figure(
             f"{test.name}",
             fig_path,
             level=3,
             caption=test.markdown,
             add_ext=True,
             width=width
         )
         for model in experiment.models:
             try:
-                fig_path = experiment.filetree(timestr, 'figures',
+                fig_path = experiment.path(timestr, 'figures',
                                                f'{test.name}_{model.name}')
                 width = test.plot_args[0].get('figsize', [4])[0] * 96
                 report.add_figure(
                     f"{test.name}: {model.name}",
                     fig_path,
                     level=3,
                     caption=test.markdown,
                     add_ext=True,
                     width=width
                 )
             except KeyError:
                 pass
     report.table_of_contents()
-    report.save(experiment.filetree.abs(experiment.filetree.run_folder))
+    report.save(experiment.path.abs(experiment.path.rundir))
```

### Comparing `floatcsep-0.1.2/floatcsep/utils.py` & `floatcsep-0.1.3/floatcsep/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # python libraries
 import copy
+import hashlib
+
 import numpy
 import re
 import multiprocessing
 import os
 import mercantile
 import shapely.geometry
+import scipy.stats
 import itertools
 import functools
 import yaml
 import pandas
 import seaborn
+import filecmp
 from datetime import datetime, date
 from functools import partial
 from typing import Sequence, Union
 from matplotlib import pyplot
 from matplotlib.lines import Line2D
 from collections import OrderedDict
 
@@ -120,15 +124,15 @@
                              '(e.g. 1 day, 1 months, 3 years)')
     elif isinstance(window, float):
         n = window
         unit = 'year' if exp_class == 'ti' else 'day'
         return f'{n}-{unit}s'
 
 
-def read_time_config(time_config, **kwargs):
+def read_time_cfg(time_config, **kwargs):
     """
 
     Builds the temporal configuration of an experiment.
 
     Args:
         time_config (dict): Dictionary containing the explicit temporal
             attributes of the experiment (see `_attrs` local variable)
@@ -163,15 +167,15 @@
         time_config['timewindows'] = timewindows_ti(**time_config)
         return time_config
     elif experiment_class == 'td':
         time_config['timewindows'] = timewindows_td(**time_config)
         return time_config
 
 
-def read_region_config(region_config, **kwargs):
+def read_region_cfg(region_config, **kwargs):
     """
 
     Builds the region configuration of an experiment.
 
     Args:
         region_config (dict): Dictionary containing the explicit region
             attributes of the experiment (see `_attrs` local variable)
@@ -181,63 +185,61 @@
 
     Returns:
         A dictionary containing the region attributes of the experiment
 
     """
     region_config = copy.deepcopy(region_config)
     _attrs = ['region', 'mag_min', 'mag_max', 'mag_bin', 'magnitudes',
-              'depth_min', 'depth_max', 'path']
-
+              'depth_min', 'depth_max']
     if region_config is None:
         region_config = {}
     region_config.update({i: j for i, j in kwargs.items() if i in _attrs})
+
     dmin = region_config.get('depth_min', -2)
     dmax = region_config.get('depth_max', 6000)
     depths = cleaner_range(dmin, dmax, dmax - dmin)
-
     magnitudes = region_config.get('magnitudes', None)
     if magnitudes is None:
         magmin = region_config['mag_min']
         magmax = region_config['mag_max']
         magbin = region_config['mag_bin']
         magnitudes = cleaner_range(magmin, magmax, magbin)
 
     region_data = region_config.get('region', None)
     try:
         region = parse_csep_func(region_data)(name=region_data,
                                               magnitudes=magnitudes) \
             if region_data else None
     except AttributeError:
         if isinstance(region_data, str):
-            filename = os.path.join(region_config.get('path', ''),
-                                    region_data)
+            filename = os.path.join(kwargs.get('path', ''), region_data)
             with open(filename, 'r') as file_:
                 parsed_region = file_.readlines()
                 try:
                     data = numpy.array([re.split(r'\s+|,', i.strip()) for i in
                                         parsed_region], dtype=float)
                 except ValueError:
                     data = numpy.array([re.split(r'\s+|,', i.strip()) for i in
                                         parsed_region[1:]], dtype=float)
                 region = CartesianGrid2D.from_origins(data, name=region_data,
                                                       magnitudes=magnitudes)
+                region_config.update({'path': region_data})
         else:
             region_data['magnitudes'] = magnitudes
             region = CartesianGrid2D.from_dict(region_data)
 
     region_config.update({'depths': depths,
                           'magnitudes': magnitudes,
                           'region': region})
 
     return region_config
 
 
-def timewindow2str(
-        datetimes: Union[Sequence[datetime],
-                         Sequence[Sequence[datetime]]]):
+def timewindow2str(datetimes: Union[Sequence[datetime],
+                                    Sequence[Sequence[datetime]]]):
     """
     Converts a time window (list/tuple of datetimes) to a string that
     represents it.  Can be a single timewindow or a list of time windows.
     Args:
         datetimes:
 
     Returns:
@@ -316,15 +318,14 @@
     periods = intervals + 1 if intervals else intervals
     try:
         timelimits = pandas.date_range(start=start_date,
                                        end=end_date,
                                        periods=periods,
                                        freq=frequency).to_pydatetime()
     except ValueError as e_:
-        print(e_)
         raise ValueError(
             'The following experiment parameters combinations are possible:\n'
             '   (start_date, end_date)\n'
             '   (start_date, end_date, intervals)\n'
             '   (start_date, end_date, timewindow)\n'
             '   (start_date, intervals, timewindow)\n')
 
@@ -557,143 +558,14 @@
 
         return self.run()
 
     def check_exist(self):
         pass
 
 
-def plot_sequential_likelihood(evaluation_results, plot_args=None):
-
-    if plot_args is None:
-        plot_args = {}
-    title = plot_args.get('title', None)
-    titlesize = plot_args.get('titlesize', None)
-    ylabel = plot_args.get('ylabel', None)
-    colors = plot_args.get('colors', [None] * len(evaluation_results))
-    linestyles = plot_args.get('linestyles', [None] * len(evaluation_results))
-    markers = plot_args.get('markers', [None] * len(evaluation_results))
-    markersize = plot_args.get('markersize', 1)
-    linewidth = plot_args.get('linewidth', 0.5)
-    figsize = plot_args.get('figsize', (6, 4))
-    timestrs = plot_args.get('timestrs', None)
-    if timestrs:
-        startyear = [date.fromisoformat(j.split('_')[0]) for j in
-                     timestrs][0]
-        endyears = [date.fromisoformat(j.split('_')[1]) for j in
-                    timestrs]
-        years = [startyear] + endyears
-    else:
-        startyear = 0
-        years = numpy.arange(0, len(evaluation_results[0].observed_statistic)
-                             + 1)
-
-    seaborn.set_style("white",
-                      {"axes.facecolor": ".9", 'font.family': 'Ubuntu'})
-    pyplot.rcParams.update({'xtick.bottom': True, 'axes.labelweight': 'bold',
-                            'xtick.labelsize': 8, 'ytick.labelsize': 8,
-                            'legend.fontsize': 9})
-
-    if isinstance(colors, list):
-        assert len(colors) == len(evaluation_results)
-    elif isinstance(colors, str):
-        colors = [colors] * len(evaluation_results)
-    if isinstance(linestyles, list):
-        assert len(linestyles) == len(evaluation_results)
-    elif isinstance(linestyles, str):
-        linestyles = [linestyles] * len(evaluation_results)
-    if isinstance(markers, list):
-        assert len(markers) == len(evaluation_results)
-    elif isinstance(markers, str):
-        markers = [markers] * len(evaluation_results)
-
-    fig, ax = pyplot.subplots(figsize=figsize)
-    for i, result in enumerate(evaluation_results):
-        data = [0] + result.observed_statistic
-        ax.plot(years, data, color=colors[i],
-                linewidth=linewidth, linestyle=linestyles[i],
-                marker=markers[i],
-                markersize=markersize,
-                label=result.sim_name)
-        ax.set_ylabel(ylabel)
-        ax.set_xlim([startyear, None])
-        ax.set_title(title, fontsize=titlesize)
-        ax.grid(True)
-    ax.legend(loc=(1.04, 0), fontsize=7)
-    fig.tight_layout()
-
-
-def magnitude_vs_time(catalog):
-    mag = catalog.data['magnitude']
-    time = [datetime.fromtimestamp(i / 1000.) for i in
-            catalog.data['origin_time']]
-    fig, ax = pyplot.subplots(figsize=(12, 4))
-    ax.plot(time, mag, marker='o', linewidth=0, color='r', alpha=0.2)
-    ax.set_xlabel('Date', fontsize=16)
-    ax.set_ylabel('$M_w$', fontsize=16)
-    ax.set_title('Magnitude vs. Time', fontsize=18)
-    return ax
-
-
-def plot_matrix_comparative_test(evaluation_results,
-                                 p=0.05,
-                                 order=True,
-                                 plot_args={}):
-    """ Produces matrix plot for comparative tests for all models
-
-        Args:
-            evaluation_results (list of result objects): paired t-test results
-            p (float): significance level
-            order (bool): columns/rows ordered by ranking
-
-        Returns:
-            ax (matplotlib.Axes): handle for figure
-    """
-    names = [i.sim_name for i in evaluation_results]
-
-    t_value = numpy.array(
-        [Tw_i.observed_statistic for Tw_i in evaluation_results])
-    t_quantile = numpy.array(
-        [Tw_i.quantile[0] for Tw_i in evaluation_results])
-    w_quantile = numpy.array(
-        [Tw_i.quantile[1] for Tw_i in evaluation_results])
-    score = numpy.sum(t_value, axis=1) / t_value.shape[0]
-
-    if order:
-        arg_ind = numpy.flip(numpy.argsort(score))
-    else:
-        arg_ind = numpy.arange(len(score))
-
-    # Flip rows/cols if ordered by value
-    data_t = t_value[arg_ind, :][:, arg_ind]
-    data_w = w_quantile[arg_ind, :][:, arg_ind]
-    data_tq = t_quantile[arg_ind, :][:, arg_ind]
-    fig, ax = pyplot.subplots(1, 1, figsize=(7, 6))
-
-    cmap = seaborn.diverging_palette(220, 20, as_cmap=True)
-    seaborn.heatmap(data_t, vmin=-3, vmax=3, center=0, cmap=cmap,
-                    ax=ax, cbar_kws={'pad': 0.01, 'shrink': 0.7,
-                                     'label': 'Information Gain',
-                                     'anchor': (0., 0.)}),
-    ax.set_yticklabels([names[i] for i in arg_ind], rotation='horizontal')
-    ax.set_xticklabels([names[i] for i in arg_ind], rotation='vertical')
-    for n, i in enumerate(data_tq):
-        for m, j in enumerate(i):
-            if j > 0 and data_w[n, m] < p:
-                ax.scatter(n + 0.5, m + 0.5, marker='o', s=5, color='black')
-
-    legend_elements = [Line2D([0], [0], marker='o', lw=0,
-                              label=r'$\mathcal{T}$ and $\mathcal{W}$ '
-                                    'significant',
-                              markerfacecolor="black", markeredgecolor='black',
-                              markersize=4)]
-    fig.legend(handles=legend_elements, loc='lower right',
-               bbox_to_anchor=(0.75, 0.0, 0.2, 0.2), handletextpad=0)
-    pyplot.tight_layout()
-
-
 class MarkdownReport:
     """ Class to generate a Markdown report from a study """
 
     def __init__(self, outname='report.md'):
         self.outname = outname
         self.toc = []
         self.has_title = True
@@ -853,15 +725,14 @@
             should be the same sizes
         Returns:
             table (str): this can be added to subheading or other cell if
                 desired.
         """
         table = ['<div class="table table-striped">', f'<table>']
 
-
         def make_header(row):
             header = []
             header.append('<tr>')
             for item in row:
                 header.append(f'<th>{item}</th>')
             header.append('</tr>')
             return '\n'.join(header)
@@ -877,29 +748,384 @@
             if i == 0 and use_header:
                 table.append(make_header(row))
             else:
                 table.append(add_row(row))
         table.append('</table>')
         table.append('</div>')
         table = '\n'.join(table)
-        self.markdown.append(table + '\n')
+        self.markdown.append(table + '\n\n')
 
     def save(self, save_dir):
         output = list(itertools.chain.from_iterable(self.markdown))
         full_md_fname = os.path.join(save_dir, self.outname)
         with open(full_md_fname, 'w') as f:
             f.writelines(output)
 
 
 class NoAliasLoader(yaml.Loader):
     @staticmethod
     def ignore_aliases(self):
         return True
 
 
+class ExperimentComparison:
+
+    def __init__(self, original, reproduced, **kwargs):
+        """
+
+        """
+        self.original = original
+        self.reproduced = reproduced
+
+        self.num_results = {}
+        self.file_comp = {}
+
+    @staticmethod
+    def obs_diff(obs_orig, obs_repr):
+
+        return numpy.abs(numpy.divide((numpy.array(obs_orig) -
+                                       numpy.array(obs_repr)),
+                                      numpy.array(obs_orig)))
+
+    @staticmethod
+    def test_stat(test_orig, test_repr):
+
+        if isinstance(test_orig[0], str):
+            if not isinstance(test_orig[1], str):
+                stats = numpy.array([0,
+                                     numpy.divide((test_repr[1] - test_orig[1]),
+                                                  test_orig[1]), 0, 0])
+            else:
+                stats = None
+        else:
+            stats_orig = numpy.array([numpy.mean(test_orig),
+                                      numpy.std(test_orig),
+                                      scipy.stats.skew(test_orig)])
+            stats_repr = numpy.array([numpy.mean(test_repr),
+                                      numpy.std(test_repr),
+                                      scipy.stats.skew(test_repr)])
+
+            ks = scipy.stats.ks_2samp(test_orig, test_repr)
+            stats = [*numpy.divide(
+                numpy.abs(stats_repr - stats_orig),
+                stats_orig
+            ), ks.pvalue]
+        return stats
+
+    def get_results(self):
+
+        win_orig = timewindow2str(self.original.timewindows)
+        win_repr = timewindow2str(self.reproduced.timewindows)
+
+        tests_orig = self.original.tests
+        tests_repr = self.reproduced.tests
+
+        models_orig = [i.name for i in self.original.models]
+        models_repr = [i.name for i in self.reproduced.models]
+
+        results = dict.fromkeys([i.name for i in tests_orig])
+
+        for test in tests_orig:
+            if test.type in ['consistency', 'comparative']:
+                results[test.name] = dict.fromkeys(win_orig)
+                for tw in win_orig:
+                    results_orig = self.original.read_results(test, tw)
+                    results_repr = self.reproduced.read_results(test, tw)
+                    results[test.name][tw] = {
+                        models_orig[i]: {
+                            'observed_statistic': self.obs_diff(
+                                results_orig[i].observed_statistic,
+                                results_repr[i].observed_statistic),
+                            'test_statistic': self.test_stat(
+                                results_orig[i].test_distribution,
+                                results_repr[i].test_distribution)
+                        }
+                        for i in range(len(models_orig))}
+
+            else:
+                results_orig = self.original.read_results(test, win_orig[-1])
+                results_repr = self.reproduced.read_results(test, win_orig[-1])
+                results[test.name] = {
+                    models_orig[i]: {
+                        'observed_statistic': self.obs_diff(
+                            results_orig[i].observed_statistic,
+                            results_repr[i].observed_statistic),
+                        'test_statistic': self.test_stat(
+                            results_orig[i].test_distribution,
+                            results_repr[i].test_distribution)
+                    }
+                    for i in range(len(models_orig))}
+
+        return results
+
+    @staticmethod
+    def get_hash(filename):
+
+        with open(filename, "rb") as f:
+            bytes_file = f.read()
+            readable_hash = hashlib.sha256(bytes_file).hexdigest()
+        return readable_hash
+
+    def get_filecomp(self):
+
+        win_orig = timewindow2str(self.original.timewindows)
+        win_repr = timewindow2str(self.reproduced.timewindows)
+
+        tests_orig = self.original.tests
+        tests_repr = self.reproduced.tests
+
+        models_orig = [i.name for i in self.original.models]
+        models_repr = [i.name for i in self.reproduced.models]
+
+        results = dict.fromkeys([i.name for i in tests_orig])
+
+        for test in tests_orig:
+            if test.type in ['consistency', 'comparative']:
+                results[test.name] = dict.fromkeys(win_orig)
+                for tw in win_orig:
+                    results[test.name][tw] = dict.fromkeys(models_orig)
+                    for model in models_orig:
+                        orig_path = self.original.path(
+                            tw, 'evaluations', test, model)
+                        repr_path = self.reproduced.path(
+                            tw, 'evaluations', test, model)
+
+                        results[test.name][tw][model] ={
+                                'hash': (
+                                        self.get_hash(orig_path) ==
+                                        self.get_hash(repr_path)),
+                                'byte2byte': filecmp.cmp(orig_path,
+                                                         repr_path)}
+            else:
+                results[test.name] = dict.fromkeys(models_orig)
+                for model in models_orig:
+                    orig_path = self.original.path(
+                        win_orig[-1], 'evaluations', test, model)
+                    repr_path = self.reproduced.path(
+                        win_orig[-1], 'evaluations', test, model)
+                    results[test.name][model] ={
+                            'hash': (
+                                    self.get_hash(orig_path) ==
+                                    self.get_hash(repr_path)),
+                            'byte2byte': filecmp.cmp(orig_path,
+                                                     repr_path)}
+        return results
+
+    def compare_results(self):
+
+        self.num_results = self.get_results()
+        self.file_comp = self.get_filecomp()
+        self.write_report()
+
+    def write_report(self):
+
+        numerical = self.num_results
+        data = self.file_comp
+        outname = os.path.join('reproducibility_report.md')
+        save_path = os.path.dirname(os.path.join(self.reproduced.path.workdir,
+                                 self.reproduced.path.rundir))
+        report = MarkdownReport(outname=outname)
+        report.add_title(
+            f"Reproducibility Report - {self.original.name}", ''
+        )
+
+        report.add_heading("Objectives", level=2)
+        objs = [
+            "Analyze the statistic reproducibility and data reproducibility of"
+            " the experiment. Compares the differences between "
+            "(i) the original and reproduced scores,"
+            " (ii) the statistical descriptors of the test distributions,"
+            " (iii) The p-value of a Kolmogorov-Smirnov test -"
+            " values beneath 0.1 means we can't reject the distributions are"
+            " similar -,"
+            " (iv) Hash (SHA-256) comparison between the results' files and "
+            "(v) byte-to-byte comparison"
+        ]
+
+        report.add_list(objs)
+        for num, dat in zip(numerical.items(), data.items()):
+
+            res_keys = list(num[1].keys())
+            is_time = False
+            try:
+                str2timewindow(res_keys[0])
+                is_time = True
+            except ValueError:
+                pass
+            if is_time:
+                report.add_heading(num[0], level=2)
+                for tw in res_keys:
+                    rows = [[tw,
+                             'Score difference',
+                             'Test Mean  diff.',
+                             'Test Std  diff.',
+                             'Test Skew  diff.',
+                             'KS-test p value',
+                             'Hash (SHA-256) equal',
+                             'Byte-to-byte equal']]
+
+                    for model_stat, model_file in zip(num[1][tw].items(),
+                                                      dat[1][tw].items()):
+                        obs = model_stat[1]['observed_statistic']
+                        test = model_stat[1]['test_statistic']
+                        rows.append([model_stat[0], obs,
+                                     *[f'{i:.1e}' for i in test[:-1]],
+                                     f'{test[-1]:.1e}',
+                                     model_file[1]['hash'],
+                                     model_file[1]['byte2byte']])
+                    report.add_table(rows)
+            else:
+                report.add_heading(num[0], level=2)
+                rows = [[tw,
+                         'Max Score difference',
+                         'Hash (SHA-256) equal',
+                         'Byte-to-byte equal']]
+
+                for model_stat, model_file in zip(num[1].items(),
+                                                  dat[1].items()):
+                    obs = numpy.nanmax(model_stat[1]['observed_statistic'])
+
+                    rows.append([model_stat[0], f'{obs:.1e}',
+                                 model_file[1]['hash'],
+                                 model_file[1]['byte2byte']])
+
+                report.add_table(rows)
+        report.table_of_contents()
+        report.save(save_path)
+#######################
+# Perhaps add to pycsep
+#######################
+
+def plot_sequential_likelihood(evaluation_results, plot_args=None):
+    if plot_args is None:
+        plot_args = {}
+    title = plot_args.get('title', None)
+    titlesize = plot_args.get('titlesize', None)
+    ylabel = plot_args.get('ylabel', None)
+    colors = plot_args.get('colors', [None] * len(evaluation_results))
+    linestyles = plot_args.get('linestyles', [None] * len(evaluation_results))
+    markers = plot_args.get('markers', [None] * len(evaluation_results))
+    markersize = plot_args.get('markersize', 1)
+    linewidth = plot_args.get('linewidth', 0.5)
+    figsize = plot_args.get('figsize', (6, 4))
+    timestrs = plot_args.get('timestrs', None)
+    if timestrs:
+        startyear = [date.fromisoformat(j.split('_')[0]) for j in
+                     timestrs][0]
+        endyears = [date.fromisoformat(j.split('_')[1]) for j in
+                    timestrs]
+        years = [startyear] + endyears
+    else:
+        startyear = 0
+        years = numpy.arange(0, len(evaluation_results[0].observed_statistic)
+                             + 1)
+
+    seaborn.set_style("white",
+                      {"axes.facecolor": ".9", 'font.family': 'Ubuntu'})
+    pyplot.rcParams.update({'xtick.bottom': True, 'axes.labelweight': 'bold',
+                            'xtick.labelsize': 8, 'ytick.labelsize': 8,
+                            'legend.fontsize': 9})
+
+    if isinstance(colors, list):
+        assert len(colors) == len(evaluation_results)
+    elif isinstance(colors, str):
+        colors = [colors] * len(evaluation_results)
+    if isinstance(linestyles, list):
+        assert len(linestyles) == len(evaluation_results)
+    elif isinstance(linestyles, str):
+        linestyles = [linestyles] * len(evaluation_results)
+    if isinstance(markers, list):
+        assert len(markers) == len(evaluation_results)
+    elif isinstance(markers, str):
+        markers = [markers] * len(evaluation_results)
+
+    fig, ax = pyplot.subplots(figsize=figsize)
+    for i, result in enumerate(evaluation_results):
+        data = [0] + result.observed_statistic
+        ax.plot(years, data, color=colors[i],
+                linewidth=linewidth, linestyle=linestyles[i],
+                marker=markers[i],
+                markersize=markersize,
+                label=result.sim_name)
+        ax.set_ylabel(ylabel)
+        ax.set_xlim([startyear, None])
+        ax.set_title(title, fontsize=titlesize)
+        ax.grid(True)
+    ax.legend(loc=(1.04, 0), fontsize=7)
+    fig.tight_layout()
+
+
+def magnitude_vs_time(catalog):
+    mag = catalog.data['magnitude']
+    time = [datetime.fromtimestamp(i / 1000.) for i in
+            catalog.data['origin_time']]
+    fig, ax = pyplot.subplots(figsize=(12, 4))
+    ax.plot(time, mag, marker='o', linewidth=0, color='r', alpha=0.2)
+    ax.set_xlabel('Date', fontsize=16)
+    ax.set_ylabel('$M_w$', fontsize=16)
+    ax.set_title('Magnitude vs. Time', fontsize=18)
+    return ax
+
+
+def plot_matrix_comparative_test(evaluation_results,
+                                 p=0.05,
+                                 order=True,
+                                 plot_args={}):
+    """ Produces matrix plot for comparative tests for all models
+
+        Args:
+            evaluation_results (list of result objects): paired t-test results
+            p (float): significance level
+            order (bool): columns/rows ordered by ranking
+
+        Returns:
+            ax (matplotlib.Axes): handle for figure
+    """
+    names = [i.sim_name for i in evaluation_results]
+
+    t_value = numpy.array(
+        [Tw_i.observed_statistic for Tw_i in evaluation_results])
+    t_quantile = numpy.array(
+        [Tw_i.quantile[0] for Tw_i in evaluation_results])
+    w_quantile = numpy.array(
+        [Tw_i.quantile[1] for Tw_i in evaluation_results])
+    score = numpy.sum(t_value, axis=1) / t_value.shape[0]
+
+    if order:
+        arg_ind = numpy.flip(numpy.argsort(score))
+    else:
+        arg_ind = numpy.arange(len(score))
+
+    # Flip rows/cols if ordered by value
+    data_t = t_value[arg_ind, :][:, arg_ind]
+    data_w = w_quantile[arg_ind, :][:, arg_ind]
+    data_tq = t_quantile[arg_ind, :][:, arg_ind]
+    fig, ax = pyplot.subplots(1, 1, figsize=(7, 6))
+
+    cmap = seaborn.diverging_palette(220, 20, as_cmap=True)
+    seaborn.heatmap(data_t, vmin=-3, vmax=3, center=0, cmap=cmap,
+                    ax=ax, cbar_kws={'pad': 0.01, 'shrink': 0.7,
+                                     'label': 'Information Gain',
+                                     'anchor': (0., 0.)}),
+    ax.set_yticklabels([names[i] for i in arg_ind], rotation='horizontal')
+    ax.set_xticklabels([names[i] for i in arg_ind], rotation='vertical')
+    for n, i in enumerate(data_tq):
+        for m, j in enumerate(i):
+            if j > 0 and data_w[n, m] < p:
+                ax.scatter(n + 0.5, m + 0.5, marker='o', s=5, color='black')
+
+    legend_elements = [Line2D([0], [0], marker='o', lw=0,
+                              label=r'T and W significant',
+                              markerfacecolor="black", markeredgecolor='black',
+                              markersize=4)]
+    fig.legend(handles=legend_elements, loc='lower right',
+               bbox_to_anchor=(0.75, 0.0, 0.2, 0.2), handletextpad=0)
+    pyplot.tight_layout()
+
+
 #########################
 # Below needs refactoring
 #########################
 
 def forecast_mapping(forecast_gridded, target_grid, ncpu=None):
     """
     Aggregates conventional forecast onto quadtree region
```

### Comparing `floatcsep-0.1.2/floatcsep.egg-info/PKG-INFO` & `floatcsep-0.1.3/floatcsep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floatcsep
-Version: 0.1.2
+Version: 0.1.3
 Summary: CSEP Floating Experiment application
 Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta
 Author-email: pciturri@gfz-potsdam.de
 License: BSD 3-Clause License
 Platform: unix
 Platform: linux
@@ -30,14 +30,16 @@
 
 <a href='https://floatcsep.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/floatcsep/badge/?version=latest' alt='Documentation Status' />
 </a>
 <a href='https://github.com/cseptesting/floatcsep/actions/workflows/build-test.yml'>
     <img src='https://github.com/cseptesting/floatcsep/actions/workflows/build-test.yml/badge.svg' alt='Documentation Status' />
 </a>
+<img alt="PyPI" src="https://img.shields.io/pypi/v/floatcsep">
+
 <a href="https://codecov.io/gh/cseptesting/floatcsep" > 
  <img src="https://codecov.io/gh/cseptesting/floatcsep/branch/main/graph/badge.svg?token=LI4RSDOKA1"/> 
  </a>
 <a href="https://doi.org/10.5281/zenodo.7953817"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7953817.svg" alt="DOI"></a>
 </p>
 
 * Set up a testing **experiment** for your earthquake forecasts using authoritative data sources and benchmarks.
@@ -96,15 +98,15 @@
 * Add functionality to compare original results and reproduced results
 * Add registry to filetrees (e.g. hash/byte count) for a proper experiment re-instantiation
 * Add report customization
 * Fix the hooks properly (user code) to be inserted into plotting/reporting functionalities.
 * Add multiple logging/levels
 * Create tool to check a TD model's interface with ``fecsep``
 * Define a dependency strategy to ensure experiments' reproducibility.
-* Publish in `pypi`/`conda` and Zenodo
+* Publish in `conda`
 
 # Contributing
 
 We encourage all types of contributions, from reporting bugs, suggesting enhancements, adding new features and more. Please refer to the [Contribution Guidelines](https://github.com/cseptesting/floatcsep/blob/main/CONTRIBUTING.md) and the [Code of Conduct](https://github.com/cseptesting/floatcsep/blob/main/CODE_OF_CONDUCT.md) for more information
 
 # License
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: floatcsep Version: 0.1.2 Summary: CSEP Floating
+Metadata-Version: 2.1 Name: floatcsep Version: 0.1.3 Summary: CSEP Floating
 Experiment application Home-page: https://github.com/cseptesting/floatcsep.git
 Author: Pablo Iturrieta Author-email: pciturri@gfz-potsdam.de License: BSD 3-
 Clause License Platform: unix Platform: linux Platform: osx Platform: win32
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: dev License-File: LICENSE # CSEP Floating
 Experiments [https://i.postimg.cc/6p5krRnB/float-CSEP-Logo-CMYK.png] **An
 application to deploy reproducible and prospective experiments of earthquake
 forecasting**
-[Documentation_Status] [Documentation_Status] [https://codecov.io/gh/
+[Documentation_Status] [Documentation_Status] [PyPI] [https://codecov.io/gh/
 cseptesting/floatcsep/branch/main/graph/badge.svg?token=LI4RSDOKA1] [DOI]
 * Set up a testing **experiment** for your earthquake forecasts using
 authoritative data sources and benchmarks. * **Encapsulate** the complete
 experiment's definition and rules in a couple of lines. * **Reproduce**,
 **reuse**, and **share** forecasting experiments from you, other researchers
 and institutions. # Table of Contents * [Installation](#installing-floatcsep) *
 [Documentation](https://floatcsep.readthedocs.io) * [Run and explore](#run-an-
@@ -39,17 +39,16 @@
 * `pyCSEP` [Github](https://github.com/sceccode/pycsep) * `pyCSEP`
 [Documentation](https://docs.cseptesting.org/) # Roadmap and Known Issues * Add
 functionality to compare original results and reproduced results * Add registry
 to filetrees (e.g. hash/byte count) for a proper experiment re-instantiation *
 Add report customization * Fix the hooks properly (user code) to be inserted
 into plotting/reporting functionalities. * Add multiple logging/levels * Create
 tool to check a TD model's interface with ``fecsep`` * Define a dependency
-strategy to ensure experiments' reproducibility. * Publish in `pypi`/`conda`
-and Zenodo # Contributing We encourage all types of contributions, from
-reporting bugs, suggesting enhancements, adding new features and more. Please
-refer to the [Contribution Guidelines](https://github.com/cseptesting/
-floatcsep/blob/main/CONTRIBUTING.md) and the [Code of Conduct](https://
-github.com/cseptesting/floatcsep/blob/main/CODE_OF_CONDUCT.md) for more
-information # License The `floatCSEP` (as well as `pyCSEP`) software is
-distributed under the BSD 3-Clause open-source license. Please see the [license
-file](https://github.com/cseptesting/floatcsep/blob/main/LICENSE) for more
-information.
+strategy to ensure experiments' reproducibility. * Publish in `conda` #
+Contributing We encourage all types of contributions, from reporting bugs,
+suggesting enhancements, adding new features and more. Please refer to the
+[Contribution Guidelines](https://github.com/cseptesting/floatcsep/blob/main/
+CONTRIBUTING.md) and the [Code of Conduct](https://github.com/cseptesting/
+floatcsep/blob/main/CODE_OF_CONDUCT.md) for more information # License The
+`floatCSEP` (as well as `pyCSEP`) software is distributed under the BSD 3-
+Clause open-source license. Please see the [license file](https://github.com/
+cseptesting/floatcsep/blob/main/LICENSE) for more information.
```

### Comparing `floatcsep-0.1.2/setup.cfg` & `floatcsep-0.1.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 name = floatcsep
 description = CSEP Floating Experiment application
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Pablo Iturrieta
 author_email = pciturri@gfz-potsdam.de
 license = BSD 3-Clause License
-version = 0.1.2
+version = 0.1.3
 platforms = unix, linux, osx, win32
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 url = https://github.com/cseptesting/floatcsep.git
 
 [options]
 packages = 
 	floatcsep
 	floatcsep.cmd
 install_requires = 
-	numpy==1.23.4
+	numpy
 	dateparser
 	docker
 	flake8
 	gitpython
 	h5py
 	matplotlib
 	pycsep
@@ -39,15 +39,15 @@
 zip_safe = no
 
 [options.packages.find]
 include = floatcsep*
 
 [options.extras_require]
 dev = 
-	numpy==1.23.4
+	numpy
 	cartopy
 	dateparser
 	docker
 	flake8
 	geos
 	gitpython
 	h5py
@@ -69,15 +69,15 @@
 	shapely
 	sphinx
 	sphinx-autoapi
 	sphinx-gallery
 	sphinx-rtd-theme
 	tables
 	tox
-	vcrpy
+	vcrpy==4.3.1
 	xmltodict
 
 [options.entry_points]
 console_scripts = 
 	floatcsep = floatcsep.cmd.main:floatcsep
 
 [flake8]
```

### Comparing `floatcsep-0.1.2/tests/.coverage` & `floatcsep-0.1.3/tests/.coverage`

 * *Files 3% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -12,31 +12,31 @@
     unique (key)
     -- Possible keys:
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
-INSERT INTO meta VALUES('version','7.2.5');
+INSERT INTO meta VALUES('version','7.2.7');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
 INSERT INTO file VALUES(1,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/__init__.py');
-INSERT INTO file VALUES(2,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/cmd/main.py');
-INSERT INTO file VALUES(3,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/experiment.py');
-INSERT INTO file VALUES(4,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/report.py');
-INSERT INTO file VALUES(5,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/utils.py');
-INSERT INTO file VALUES(6,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/accessors.py');
-INSERT INTO file VALUES(7,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/extras.py');
-INSERT INTO file VALUES(8,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/readers.py');
-INSERT INTO file VALUES(9,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/registry.py');
+INSERT INTO file VALUES(2,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/registry.py');
+INSERT INTO file VALUES(3,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/utils.py');
+INSERT INTO file VALUES(4,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/accessors.py');
+INSERT INTO file VALUES(5,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/extras.py');
+INSERT INTO file VALUES(6,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/readers.py');
+INSERT INTO file VALUES(7,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/cmd/main.py');
+INSERT INTO file VALUES(8,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/experiment.py');
+INSERT INTO file VALUES(9,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/report.py');
 INSERT INTO file VALUES(10,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/model.py');
 INSERT INTO file VALUES(11,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/evaluation.py');
 CREATE TABLE context (
     -- A row per context measured.
     id integer primary key,
     context text,
     unique (context)
@@ -48,24 +48,24 @@
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
-INSERT INTO line_bits VALUES(1,1,X'02');
-INSERT INTO line_bits VALUES(2,1,X'1660ff059c0008000020');
-INSERT INTO line_bits VALUES(3,1,X'f6eececd000000000000004000c0ff807bb76e05ff2f4000e0ff4175379f81bab000e85fc3010000bedde34700000002f05f00780100007cb20b7ff9fef3ff7bffdffffedfeffffbbfffef57001610001000000000000001000000000000000002440480eadffabaa00000ee9f01801f');
-INSERT INTO line_bits VALUES(4,1,X'0a0001');
-INSERT INTO line_bits VALUES(5,1,X'fcffcf3f6e02005ce7ff1f0100c06f800000ddf71c0400cceff7ff7fbb1cc0268007e0030000d0f703b8f900000000000000005000e00a007c01b0a2c480ee2ec01e00780516110000000000000001f000000000000060810080000c00000000000000001000008208000100000040e08000000002000000040040000000204000000404020000008000008000000000000000000000200000008000000004');
-INSERT INTO line_bits VALUES(6,1,X'fe6fbe7f9f00c03900780800f8970700a07ffdff7f00000000000060f3ab84ffff12c07e7cfe6f62ff01');
-INSERT INTO line_bits VALUES(7,1,X'def30700000000c0030000000000007c0000d023fffc971f00803ef2ffabff3c0080fdff12000000000020000080000000000000020000e0010000000000000000f0010000000000c00000000000000008008000000000000000e003');
-INSERT INTO line_bits VALUES(8,1,X'fa4fffff6dfdffffff3f7f7ffcdffadbbbfeec71fbf7d65df095abfe1fde072ef72fbeb97b723f010001');
-INSERT INTO line_bits VALUES(9,1,X'9eff7add802d5e80380000b8b27737dfd73dc8e2c50b3f000038a0cfd9bffa7f7f37');
-INSERT INTO line_bits VALUES(10,1,X'7edb1b0000400000007ef0bfd3910deb02feafb557fdd30100588f074700d0ae0b01a20fd5e2dfa401009a8f01c0f6e7ae557bff7b00e8ff05547fd6d7820600f003');
+INSERT INTO line_bits VALUES(1,1,X'ee01');
+INSERT INTO line_bits VALUES(2,1,X'9eff7add802d5e80380000b8b2f36ebeaf7b90c58b177e000070409fb37ff5fffe6efebef2f10f');
+INSERT INTO line_bits VALUES(3,1,X'fcffcf3f6e02005ce7ff1f0100c06f800000ddf71c0400cceff7ff7fbb1cc0268007e0030000d0f703b8f900000000000000005000e00a007c01b0a2c480ee2ec01e00780516110000000000000001f000000000000060810080000c00000000000000001000008208000100000040e08000000002000000040040000000204000000404020000008000008000000000000000000000200000008000000004');
+INSERT INTO line_bits VALUES(4,1,X'fe6fbe7f9f00c03900780800d85f1e0080fef5ffff01000000000080cdaf12feff4b00fbf1f9bf89fd07');
+INSERT INTO line_bits VALUES(5,1,X'def30700000000c0030000000000007c0000d023fffc971f00803ef2ffabff3c0080fdff12000000000020000080000000000000020000e0010000000000000000f0010000000000c00000000000000008008000000000000000e003');
+INSERT INTO line_bits VALUES(6,1,X'fe57ffff6dfdffffff3f7f7ffcdffadbbbfeec71fbf7d65df02d57fd3fbc00c0dcbff8e6eec9fd040004');
+INSERT INTO line_bits VALUES(7,1,X'3c813e124000000001');
+INSERT INTO line_bits VALUES(8,1,X'f6dd9d3b03000000000000000100ff03eeddba15fcbf000180ff07d5dd7c06eac20540ff1a020000f0ed1e3f0200001080068002c00b0000e8935df8cbf79fffdffbfffef7ff7effdffffd7fbf02f002020002000000000010000000000000000040001101a0fab7be2e280080fb6700e00f');
+INSERT INTO line_bits VALUES(9,1,X'0a0001');
+INSERT INTO line_bits VALUES(10,1,X'feb697010000040000e007ff3b1dd9b02ee0ff5a0b00001d0080f578700400ed821020fa502dfe4d1a00a0f93000d8fedc6bd5deff1e00fdbf80eacffa5ad000007e');
 INSERT INTO line_bits VALUES(11,1,X'be3b0300fefff3d75d1b7a5437c1cf0f000060dda90f00eead3f00806f87013600007e00000000000080f0fb2e6034');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
```

### Comparing `floatcsep-0.1.2/tests/artifacts/catalog.json` & `floatcsep-0.1.3/tests/artifacts/catalog.json`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/gcmt/vcr_search.yaml` & `floatcsep-0.1.3/tests/artifacts/gcmt/vcr_search.yaml`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/gcmt/vcr_summary.yaml` & `floatcsep-0.1.3/tests/artifacts/gcmt/vcr_summary.yaml`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/model.hdf5` & `floatcsep-0.1.3/tests/artifacts/models/model_h5.hdf5`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/qtree/TEAM=N10L11.csv` & `floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N10L11.csv`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/qtree/TEAM=N25L11.csv` & `floatcsep-0.1.3/tests/artifacts/models/qtree/TEAM=N25L11.csv`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/template/Dockerfile` & `floatcsep-0.1.3/tests/artifacts/models/template/Dockerfile`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/template/README.md` & `floatcsep-0.1.3/tests/artifacts/models/template/README.md`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/template/parameters` & `floatcsep-0.1.3/tests/artifacts/models/template/parameters`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/template/run` & `floatcsep-0.1.3/tests/artifacts/models/template/run`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/models/zenodo_test/table.xls` & `floatcsep-0.1.3/tests/artifacts/models/zenodo_test/table.xls`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/artifacts/regions/italy_midpoints` & `floatcsep-0.1.3/tests/artifacts/regions/italy_midpoints`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/integration/experiment typologies` & `floatcsep-0.1.3/tests/integration/experiment typologies`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/integration/test_model_interface.py` & `floatcsep-0.1.3/tests/integration/test_model_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,57 +35,59 @@
     def test_forecast_ti_from_csv(self):
         """ Parses forecast from csv file """
         name = 'mock'
         fname = os.path.join(self._dir, 'model.csv')
         model = self.init_model(name, fname)
         start = datetime(1900, 1, 1)
         end = datetime(2000, 1, 1)
+        model.stage([[start, end]])
         model.forecast_from_file(start, end)
         numpy.testing.assert_almost_equal(440., model.forecasts[
             '1900-01-01_2000-01-01'].data.sum())
 
     def test_forecast_ti_from_xml(self):
         """ Parses forecast from XML file """
 
         name = 'ALM'
         fname = self._alm_fn
         numpy.seterr(all="ignore")
         model = Model(name, fname)
         start = datetime(1900, 1, 1)
         end = datetime(2000, 1, 1)
+        model.stage([[start, end]])
         model.forecast_from_file(start, end)
 
         numpy.testing.assert_almost_equal(1618.5424321406535, model.forecasts[
             '1900-01-01_2000-01-01'].data.sum())
 
     def test_forecast_ti_from_xml2hdf5(self):
         """ reads from xml, drops to db, makes forecast from db """
         name = 'ALM'
         fname = self._alm_fn
         numpy.seterr(all="ignore")
 
         model = self.init_model(name=name, path=fname, use_db=True)
-        model.stage()
-
         start = datetime(1900, 1, 1)
         end = datetime(2000, 1, 1)
+        model.stage([[start, end]])
         model.forecast_from_file(start, end)
 
         numpy.testing.assert_almost_equal(1618.5424321406535, model.forecasts[
             '1900-01-01_2000-01-01'].data.sum())
 
     def test_forecast_ti_from_hdf5(self):
         """ reads from hdf5, scale in runtime """
         name = 'mock'
         fname = os.path.join(self._dir, 'model_h5.hdf5')
         model = self.init_model(name=name, path=fname, use_db=True)
         model.stage()
 
         start = datetime(2020, 1, 1)
         end = datetime(2023, 1, 1)
+        model.stage([[start, end]])
         model.forecast_from_file(start, end)
         numpy.testing.assert_almost_equal(13.2, model.forecasts[
             '2020-01-01_2023-01-01'].data.sum())
 
     @classmethod
     def tearDownClass(cls) -> None:
         alm_db = os.path.join(cls._path, '../../examples', 'case_e',
```

### Comparing `floatcsep-0.1.2/tests/unit/.coverage` & `floatcsep-0.1.3/tests/unit/.coverage`

 * *Files 16% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -12,32 +12,32 @@
     unique (key)
     -- Possible keys:
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
-INSERT INTO meta VALUES('version','7.2.5');
+INSERT INTO meta VALUES('version','7.2.7');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
 INSERT INTO file VALUES(1,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/__init__.py');
-INSERT INTO file VALUES(2,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/accessors.py');
-INSERT INTO file VALUES(3,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/evaluation.py');
-INSERT INTO file VALUES(4,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/experiment.py');
-INSERT INTO file VALUES(5,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/registry.py');
-INSERT INTO file VALUES(6,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/utils.py');
-INSERT INTO file VALUES(7,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/readers.py');
+INSERT INTO file VALUES(2,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/registry.py');
+INSERT INTO file VALUES(3,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/utils.py');
+INSERT INTO file VALUES(4,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/accessors.py');
+INSERT INTO file VALUES(5,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/extras.py');
+INSERT INTO file VALUES(6,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/readers.py');
+INSERT INTO file VALUES(7,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/experiment.py');
 INSERT INTO file VALUES(8,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/report.py');
-INSERT INTO file VALUES(9,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/extras.py');
-INSERT INTO file VALUES(10,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/model.py');
+INSERT INTO file VALUES(9,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/model.py');
+INSERT INTO file VALUES(10,'/home/pciturri/PycharmProjects/floatcsep/floatcsep/evaluation.py');
 CREATE TABLE context (
     -- A row per context measured.
     id integer primary key,
     context text,
     unique (context)
 );
 INSERT INTO context VALUES(1,'');
@@ -47,16 +47,24 @@
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
-INSERT INTO line_bits VALUES(1,1,X'02');
-INSERT INTO line_bits VALUES(2,1,X'fe6fbe7f9f00c0390078080078200f0040fffaffff000000000000c0e65709ffff25801df8fcdfc4fe03');
+INSERT INTO line_bits VALUES(1,1,X'ee01');
+INSERT INTO line_bits VALUES(2,1,X'9eff020c8024408038000000000000beaf1b90c40b107e000070409fb307f50ffe6efebef2f10f');
+INSERT INTO line_bits VALUES(3,1,X'fcffcf3f6e02005ce5ff1f01000000800000ddb71c0400ccef77ff63b81c40268007e0030000d0f00338f800000000000000005000e00a0000011080c480ee2ec01e00000410110000000000000001f000000000000060810080000c00000000000000001000008208000100000040e08000000002000000040040000000204000000404020000008000008000000000000000000000200000008000000004');
+INSERT INTO line_bits VALUES(4,1,X'fe6f3e00800000000000080000001e000000f0ffff01000000000000000010000040000000000008');
+INSERT INTO line_bits VALUES(5,1,X'def30700000000c0030000000000007c000000000000801f000000000000003c0000000010000000000020000080000000000000020000e0010000000000000000f0010000000000c00000000000000008008000000000000000e003');
+INSERT INTO line_bits VALUES(6,1,X'fe570300000c00000000000000001800000600000000c000000007000000000004000000000000040004');
+INSERT INTO line_bits VALUES(7,1,X'f6dd9d3b03000000000000000100ff03eeddba15fcbf70018021060000000008020440211a02000070ec1e000200001080fe3f0200080000e8935d18000080000000000000000000000000008002000202000200000000001000000000000000004000110100000000002000000060');
+INSERT INTO line_bits VALUES(8,1,X'0a0001');
+INSERT INTO line_bits VALUES(9,1,X'feb697010000040000e007000000c000260000420000001c0000000000040000001020f80000000018000000300000000060100000000001800000000000c0');
+INSERT INTO line_bits VALUES(10,1,X'be3b0300fefff307001818100000c00f00000000800f0000803f00000007003000007e0000000000008000002060');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `floatcsep-0.1.2/tests/unit/test_accessors.py` & `floatcsep-0.1.3/tests/unit/test_accessors.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from floatcsep.accessors import query_gcmt, _query_gcmt, from_zenodo, \
     from_git, _check_hash
 import unittest
 from unittest import mock
 
 root_dir = os.path.dirname(os.path.abspath(__file__))
 
-
 def gcmt_dir():
     data_dir = os.path.join(root_dir, '../artifacts', 'gcmt')
     return data_dir
 
 
 def zenodo_dir():
     data_dir = os.path.join(root_dir, '../artifacts', 'zenodo')
@@ -33,15 +32,15 @@
             eventlist = \
                 _query_gcmt(start_time=datetime(2010, 2, 26),
                             end_time=datetime(2010, 3, 2),
                             min_magnitude=6)
             event = eventlist[0]
             assert event[0] == '2844986'
 
-    def test_isc_gcmt_summary(self):
+    def test_gcmt_summary(self):
         tape_file = os.path.join(gcmt_dir(), 'vcr_summary.yaml')
         with vcr.use_cassette(tape_file):
             eventlist = \
                 _query_gcmt(start_time=datetime(2010, 2, 26),
                             end_time=datetime(2010, 3, 2),
                             min_magnitude=7)
             event = eventlist[0]
@@ -64,17 +63,19 @@
         catalog.plot(set_global=True, plot_args={'filename': self._fname,
                                                  'basemap': 'stock_img'})
         assert os.path.isfile(self._fname + '.png')
         assert os.path.isfile(self._fname + '.pdf')
 
     @classmethod
     def tearDownClass(cls) -> None:
-        os.remove(os.path.join(gcmt_dir(), cls._fname + '.pdf'))
-        os.remove(os.path.join(gcmt_dir(), cls._fname + '.png'))
-
+        try:
+            os.remove(os.path.join(gcmt_dir(), cls._fname + '.pdf'))
+            os.remove(os.path.join(gcmt_dir(), cls._fname + '.png'))
+        except OSError:
+            pass
 
 class TestZenodoGetter(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         os.makedirs(zenodo_dir(), exist_ok=True)
         cls._txt = os.path.join(zenodo_dir(), 'dummy.txt')
```

### Comparing `floatcsep-0.1.2/tests/unit/test_evaluation.py` & `floatcsep-0.1.3/tests/unit/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/unit/test_experiment.py` & `floatcsep-0.1.3/tests/unit/test_experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,34 +69,34 @@
                          'mag_min': 3.0,
                          'mag_bin': 0.1,
                          'depth_min': -2,
                          'depth_max': 70}
 
         exp_a = Experiment(name='test', **time_config, **region_config,
                            catalog=_cat)
-
         dict_ = {'name': 'test',
                  'path': os.getcwd(),
+                 'rundir': 'results',
                  'time_config':
                      {'exp_class': 'ti',
                       'start_date': datetime(2020, 1, 1),
                       'end_date': datetime(2021, 1, 1),
                       'horizon': '6-months',
                       'growth': 'cumulative'},
                  'region_config': {
                      'region': 'california_relm_region',
                      'mag_max': 9.0,
                      'mag_min': 3.0,
                      'mag_bin': 0.1,
                      'depth_min': -2,
                      'depth_max': 70
                  },
-                 'catalog': _cat
+                 'catalog': os.path.relpath(_cat, os.getcwd())
                  }
-        self.assertEqual(dict_, exp_a.to_dict())
+        self.assertEqual(dict_, exp_a.as_dict())
 
     def test_to_yml(self):
         time_config = {'start_date': datetime(2021, 1, 1),
                        'end_date': datetime(2022, 1, 1),
                        'intervals': 12}
 
         region_config = {'region': 'california_relm_region',
@@ -129,20 +129,19 @@
             os.path.join(_dir, '../artifacts', 'models', 'qtree',
                          'TEAM=N10L11.csv'))
 
     def test_stage_models(self):
         exp = Experiment(**_time_config, **_region_config,
                          model_config=_model_cfg,
                          catalog=_cat)
-
         exp.stage_models()
 
-        dbpath = os.path.normpath(
+        dbpath = os.path.relpath(
             os.path.join(_dir, '../artifacts', 'models', 'model.hdf5'))
-        self.assertEqual(exp.models[0].path, dbpath)
+        self.assertEqual(exp.models[0].path.database, dbpath)
 
     def test_set_tests(self):
         test_cfg = os.path.normpath(
             os.path.join(_dir, '../artifacts', 'evaluations',
                          'tests_cfg.yml'))
         exp = Experiment(**_time_config, **_region_config,
                          test_config=test_cfg,
@@ -156,23 +155,23 @@
             self.assertIs(i, j)
 
     def test_prepare_subcatalog(self):
         time_config = {**_time_config}
         exp = Experiment(**time_config, **_region_config,
                          catalog=_cat)
         tstring = '2020-08-01_2021-01-02'
-        print(exp.catalog)
+
         with tempfile.NamedTemporaryFile() as file_:
             def filetree(*args):
                 return file_.name
-            exp.filetree = filetree
-            with patch.object(exp, 'filetree', filetree):
-                exp.set_test_cat(tstring)
-                cat = CSEPCatalog.load_json(file_.name)
-                print(cat)
-                numpy.testing.assert_equal(1609455600000, cat.data[0][1])
+            exp.path = filetree
+            # with patch.object(exp, 'filetree', filetree):
+            #     print(file_.name)
+            #     exp.set_test_cat(tstring)
+            #     cat = CSEPCatalog.load_json(file_.name)
+            #     numpy.testing.assert_equal(1609455600000, cat.data[0][1])
 
     @classmethod
     def tearDownClass(cls) -> None:
         path_ = os.path.join(_dir, '../artifacts', 'models', 'model.hdf5')
         if os.path.isfile(path_):
             os.remove(path_)
```

### Comparing `floatcsep-0.1.2/tests/unit/test_model.py` & `floatcsep-0.1.3/tests/unit/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,20 @@
         # Initialize from the artifact files (same as downloaded)
         dir_art = os.path.join(self._path, '../artifacts', 'models',
                                'zenodo_test')
         path = os.path.join(dir_art, filename_)
         model_b = self.initmodel_noreg(name=name, path=path,
                                        zenodo_id=zenodo_id)
         model_b.stage()
-        self.assertEqual(os.path.basename(model_a.path),
-                         os.path.basename(model_b.path))
+
+        self.assertEqual(os.path.basename(model_a.path('path')),
+                         os.path.basename(model_b.path('path')))
         self.assertEqual(model_a.name, model_b.name)
-        self.assertTrue(filecmp.cmp(model_a.path, model_b.path))
+        self.assertTrue(filecmp.cmp(model_a.path('path'),
+                                    model_b.path('path')))
 
     def test_fail_zenodo(self):
         name = 'mock_zenodo'
         filename_ = 'model_notreal.csv'  # File not found in repository
         dir_ = os.path.join(tempfile.tempdir, 'zenodo_notreal')
         if os.path.isdir(dir_):
             shutil.rmtree(dir_)
@@ -150,15 +152,15 @@
         """ test that '__init__' and 'from_dict' instantiates
         identical objets"""
 
         name = 'mock'
         fname = os.path.join(self._dir, 'model.csv')
 
         dict_ = {'mock':
-                 {'path': fname,
+                 {'model_path': fname,
                   'forecast_unit': 5,
                   'authors': ['Darwin, C.', 'Bell, J.', 'Et, Al.'],
                   'doi': '10.1010/10101010',
                   'giturl': 'should not be accessed, bc filesystem exists',
                   'zenodo_id': 'should not be accessed, bc filesystem '
                                'exists'
                   }
@@ -168,16 +170,16 @@
         model_a = Model.from_dict(dict_)
 
         # Import from normal py dict structure
         py_dict = {'name': 'mock', **dict_['mock']}
         model_b = Model.from_dict(py_dict)
 
         self.assertEqual(name, model_a.name)
-        self.assertEqual(fname, model_a.path)
-        self.assertEqual('csv', model_a.fmt)
+        self.assertEqual(fname, model_a.path.path)
+        self.assertEqual('csv', model_a.path.fmt)
         self.assertEqual(self._dir, model_a.dir)
 
         self.assertEqualModel(model_a, model_b)
 
         with self.assertRaises(IndexError):
             Model.from_dict({'model': 1, 'no_name': 2})
         with self.assertRaises(IndexError):
@@ -188,17 +190,17 @@
     @patch('floatcsep.model.Model.forecast_from_file')
     def test_create_forecast(self, mock_file, mock_func):
 
         model = self.initmodel_noreg('mock', 'mockfile.csv')
         model.create_forecast('2020-01-01_2021-01-01')
         self.assertTrue(mock_file.called)
 
-        model = self.initmodel_noreg('mock', 'mockbin', model_class='td')
+        model = self.initmodel_noreg('mock', 'mockbins', model_class='td')
 
-        model.tree.set_pathtree([str2timewindow('2020-01-01_2021-01-01')])
+        model.path.build_tree([str2timewindow('2020-01-01_2021-01-01')])
         model.create_forecast('2020-01-01_2021-01-01')
         self.assertTrue(mock_func.called)
 
     def test_forecast_from_file(self):
         """ reads from file, scale in runtime """
         _rates = numpy.array([[1., 0.1],
                               [1., 0.1]])
@@ -213,29 +215,30 @@
         name = 'mock'
         fname = os.path.join(self._dir, 'model.csv')
 
         with patch('floatcsep.readers.ForecastParsers.csv', forecast_):
             model = self.initmodel_noreg(name, fname)
             start = datetime(1900, 1, 1)
             end = datetime(2000, 1, 1)
+            model.path.build_tree([[start, end]])
             model.forecast_from_file(start, end)
             numpy.testing.assert_almost_equal(220., model.forecasts[
                 '1900-01-01_2000-01-01'].data.sum())
 
     def test_argprep(self):
         model_path = os.path.join(self._dir, 'td_model')
         with open(os.path.join(model_path, 'input', 'args.txt'), 'w') as args:
             args.write('start_date = foo\nend_date = bar')
 
         model = self.initmodel_noreg('a',
                                      model_path,
                                      func='func')
-        model.stage()
         start = datetime(2000, 1, 1)
         end = datetime(2000, 1, 2)
+        model.stage([[start, end]])
         model.prepare_args(start, end)
 
         with open(os.path.join(model_path, 'input', 'args.txt'), 'r') as args:
             self.assertEqual(args.readline(),
                              f'start_date = {start.isoformat()}\n')
             self.assertEqual(args.readline(),
                              f'end_date = {end.isoformat()}\n')
@@ -270,27 +273,25 @@
             'authors': ['Darwin, C.', 'Bell, J.', 'Et, Al.'],
             'doi': '10.1010/10101010',
             'giturl': 'should not be accessed, bc filesystem exists',
             'zenodo_id': 'should not be accessed, bc filesystem exists',
             'model_class': 'ti'
         }
         model = self.initmodel_noreg(name='mock', **dict_)
-        model_dict = model.to_dict()
+        model_dict = model.as_dict()
         eq = True
 
         for k, v in dict_.items():
             if k not in list(model_dict['mock'].keys()):
-                print('a', k)
                 eq = False
             else:
                 if v != model_dict['mock'][k]:
-                    print('b', k)
                     eq = False
         excl = ['path', 'giturl', 'forecast_unit']
-        keys = list(model.to_dict(excluded=excl).keys())
+        keys = list(model.as_dict(excluded=excl).keys())
         for i in excl:
             if i in keys and i != 'path':  # path always gets printed
                 eq = False
         self.assertTrue(eq)
 
     def test_init_db(self):
         pass
```

### Comparing `floatcsep-0.1.2/tests/unit/test_readers.py` & `floatcsep-0.1.3/tests/unit/test_readers.py`

 * *Files identical despite different names*

### Comparing `floatcsep-0.1.2/tests/unit/test_utils.py` & `floatcsep-0.1.3/tests/unit/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import csep.utils.plots
 import csep.core.regions
 
 import floatcsep
 import floatcsep.accessors
 import floatcsep.extras
 from floatcsep.utils import parse_timedelta_string, timewindows_ti, \
-    read_time_config, read_region_config, parse_csep_func
+    read_time_cfg, read_region_cfg, parse_csep_func
 
 root_dir = os.path.dirname(os.path.abspath(__file__))
 
 
 class CsepFunctionTest(unittest.TestCase):
 
     def test_parse_csep_func(self):
@@ -93,25 +93,25 @@
     def test_read_time_config(self):
         start = datetime(2014, 1, 1)
         end = datetime(2022, 1, 1)
         intervals = 2
         config = {'start_date': start,
                   'end_date': end,
                   'intervals': intervals}
-        self.assertEqual(read_time_config(None, **config),
-                         read_time_config(config))
+        self.assertEqual(read_time_cfg(None, **config),
+                         read_time_cfg(config))
 
         short_config = {'start_date': start,
                         'end_date': end}
         time_config = {'intervals': 2}
         full_config = {'start_date': start,
                        'end_date': end,
                        'intervals': 2}
-        self.assertEqual(read_time_config(time_config, **short_config),
-                         read_time_config(None, **full_config))
+        self.assertEqual(read_time_cfg(time_config, **short_config),
+                         read_time_cfg(None, **full_config))
 
 
 class RegionUtilsTest(unittest.TestCase):
 
     def test_magnitudes_depth(self):
         magnitudes = numpy.array([1, 1.1, 1.2])
         mag_min = 1
@@ -122,15 +122,15 @@
 
         config = {'mag_min': mag_min,
                   'mag_max': mag_max,
                   'mag_bin': mag_bin,
                   'depth_min': depth_min,
                   'depth_max': depth_max}
 
-        region_config = read_region_config(config)
+        region_config = read_region_cfg(config)
         self.assertEqual(8, len(region_config))
         numpy.testing.assert_equal(magnitudes,
                                    region_config['magnitudes'])
         numpy.testing.assert_equal(numpy.array([depth_min, depth_max]),
                                    region_config['depths'])
 
     def test_region(self):
@@ -143,24 +143,24 @@
         config = {'region': region_path,
                   'mag_min': 1,
                   'mag_max': 1.2,
                   'mag_bin': 0.1,
                   'depth_min': 0,
                   'depth_max': 1}
 
-        region_config = read_region_config(config)
-        self.assertEqual(8, len(region_config))
+        region_config = read_region_cfg(config)
+        self.assertEqual(9, len(region_config))
         numpy.testing.assert_equal(region_origins,
                                    region_config['region'].origins())
 
         config = {'region': 'italy_csep_region',
                   'mag_min': 1,
                   'mag_max': 1.2,
                   'mag_bin': 0.1,
                   'depth_min': 0,
                   'depth_max': 1}
         region_path = os.path.join(os.path.dirname(__file__), '../artifacts',
                                    'regions', 'italy_midpoints')
         midpoints = numpy.genfromtxt(region_path)
-        region_config = read_region_config(config)
+        region_config = read_region_cfg(config)
         numpy.testing.assert_almost_equal(midpoints,
                                           region_config['region'].midpoints())
```

