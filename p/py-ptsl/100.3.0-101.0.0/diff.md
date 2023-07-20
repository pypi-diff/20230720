# Comparing `tmp/py_ptsl-100.3.0.tar.gz` & `tmp/py_ptsl-101.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ptsl-100.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_ptsl-101.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_ptsl-100.3.0.tar` & `py_ptsl-101.0.0.tar`

### file list

```diff
@@ -1,80 +1,83 @@
--rw-r--r--   0        0        0     1498 2023-07-18 02:51:28.789213 py_ptsl-100.3.0/LICENSE
--rw-r--r--   0        0        0     2270 2023-07-18 02:51:28.789213 py_ptsl-100.3.0/README.md
--rw-r--r--   0        0        0    53243 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/PTSL_pb2.py
--rw-r--r--   0        0        0    74192 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/PTSL_pb2.pyi
--rw-r--r--   0        0        0     4008 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/PTSL_pb2_grpc.py
--rw-r--r--   0        0        0     1075 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/__init__.py
--rw-r--r--   0        0        0    11768 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/client.py
--rw-r--r--   0        0        0    29726 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/engine.py
--rw-r--r--   0        0        0     1416 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/errors.py
--rw-r--r--   0        0        0     3654 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/__init__.py
--rw-r--r--   0        0        0       80 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/authorize_connection.py
--rw-r--r--   0        0        0       66 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/clear.py
--rw-r--r--   0        0        0       73 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/clear_special.py
--rw-r--r--   0        0        0       73 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/close_session.py
--rw-r--r--   0        0        0       76 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/consolidate_clip.py
--rw-r--r--   0        0        0       65 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/copy.py
--rw-r--r--   0        0        0       72 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/copy_special.py
--rw-r--r--   0        0        0       87 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/create_fades_based_on_preset.py
--rw-r--r--   0        0        0       74 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/create_session.py
--rw-r--r--   0        0        0       64 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/cut.py
--rw-r--r--   0        0        0       71 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/cut_special.py
--rw-r--r--   0        0        0       79 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/export_clips_as_files.py
--rw-r--r--   0        0        0       70 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/export_mix.py
--rw-r--r--   0        0        0       89 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/export_selected_tracks_as_aaf_omf.py
--rw-r--r--   0        0        0      300 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/export_session_info_as_text.py
--rw-r--r--   0        0        0       92 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/extend_selection_to_target_tracks.py
--rw-r--r--   0        0        0       81 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_dyamic_properties.py
--rw-r--r--   0        0        0       76 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_file_location.py
--rw-r--r--   0        0        0      695 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_playback_mode.py
--rw-r--r--   0        0        0       75 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_ptsl_version.py
--rw-r--r--   0        0        0       74 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_record_mode.py
--rw-r--r--   0        0        0       82 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_audio_format.py
--rw-r--r--   0        0        0       92 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_audio_rate_pull_settings.py
--rw-r--r--   0        0        0       79 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_bit_depth.py
--rw-r--r--   0        0        0       85 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_feet_frames_rate.py
--rw-r--r--   0        0        0      537 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_interleaved_state.py
--rw-r--r--   0        0        0       77 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_length.py
--rw-r--r--   0        0        0       75 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_name.py
--rw-r--r--   0        0        0       75 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_path.py
--rw-r--r--   0        0        0      631 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_sample_rate.py
--rw-r--r--   0        0        0       80 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_start_time.py
--rw-r--r--   0        0        0       83 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_time_code_rate.py
--rw-r--r--   0        0        0       92 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_session_video_rate_pull_settings.py
--rw-r--r--   0        0        0       74 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_task_status.py
--rw-r--r--   0        0        0      774 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_track_list.py
--rw-r--r--   0        0        0       78 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_transport_armed.py
--rw-r--r--   0        0        0       78 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/get_transport_state.py
--rw-r--r--   0        0        0       75 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/host_ready_check.py
--rw-r--r--   0        0        0       69 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/import_command.py
--rw-r--r--   0        0        0      127 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/memory_locations.py
--rw-r--r--   0        0        0       72 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/open_session.py
--rw-r--r--   0        0        0     2771 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/operation.py
--rw-r--r--   0        0        0       66 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/paste.py
--rw-r--r--   0        0        0       73 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/paste_special.py
--rw-r--r--   0        0        0       89 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/refresh_all_modified_audio_files.py
--rw-r--r--   0        0        0       84 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/refresh_target_audio_files.py
--rw-r--r--   0        0        0       79 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/register_connection.py
--rw-r--r--   0        0        0       79 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/rename_selected_clip.py
--rw-r--r--   0        0        0       77 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/rename_target_clip.py
--rw-r--r--   0        0        0       78 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/rename_target_track.py
--rw-r--r--   0        0        0       72 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/save_session.py
--rw-r--r--   0        0        0       74 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/save_session_as.py
--rw-r--r--   0        0        0       82 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/select_all_clips_on_track.py
--rw-r--r--   0        0        0       76 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_playback_mode.py
--rw-r--r--   0        0        0       74 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_record_mode.py
--rw-r--r--   0        0        0       82 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_audio_format.py
--rw-r--r--   0        0        0       92 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_audio_rate_pull_settings.py
--rw-r--r--   0        0        0       79 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_bit_depth.py
--rw-r--r--   0        0        0       85 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_feet_frames_rate.py
--rw-r--r--   0        0        0       87 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_interleaved_state.py
--rw-r--r--   0        0        0       77 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_length.py
--rw-r--r--   0        0        0       80 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_start_time.py
--rw-r--r--   0        0        0       83 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_time_code_rate.py
--rw-r--r--   0        0        0       92 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/set_session_video_rate_pull_settings.py
--rw-r--r--   0        0        0       65 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/spot.py
--rw-r--r--   0        0        0      212 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/toggle_play_state.py
--rw-r--r--   0        0        0       76 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/ops/trim_to_selection.py
--rw-r--r--   0        0        0     4947 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/ptsl/util.py
--rw-r--r--   0        0        0     1759 2023-07-18 02:51:28.793213 py_ptsl-100.3.0/pyproject.toml
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 py_ptsl-100.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/LICENSE
+-rw-r--r--   0        0        0     2270 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/README.md
+-rw-r--r--   0        0        0    53243 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/PTSL_pb2.py
+-rw-r--r--   0        0        0    74192 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/PTSL_pb2.pyi
+-rw-r--r--   0        0        0     4008 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/PTSL_pb2_grpc.py
+-rw-r--r--   0        0        0     1075 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/__init__.py
+-rw-r--r--   0        0        0     3926 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/builders/create_session_builder.py
+-rw-r--r--   0        0        0     4277 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/builders/export_text_builder.py
+-rw-r--r--   0        0        0     4611 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/builders/import_builder.py
+-rw-r--r--   0        0        0    11768 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/client.py
+-rw-r--r--   0        0        0    25162 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/engine.py
+-rw-r--r--   0        0        0     1416 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/errors.py
+-rw-r--r--   0        0        0     3654 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/__init__.py
+-rw-r--r--   0        0        0       80 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/authorize_connection.py
+-rw-r--r--   0        0        0       66 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/clear.py
+-rw-r--r--   0        0        0       73 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/clear_special.py
+-rw-r--r--   0        0        0       73 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/close_session.py
+-rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/consolidate_clip.py
+-rw-r--r--   0        0        0       65 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/copy.py
+-rw-r--r--   0        0        0       72 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/copy_special.py
+-rw-r--r--   0        0        0       87 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/create_fades_based_on_preset.py
+-rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/create_session.py
+-rw-r--r--   0        0        0       64 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/cut.py
+-rw-r--r--   0        0        0       71 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/cut_special.py
+-rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_clips_as_files.py
+-rw-r--r--   0        0        0       70 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_mix.py
+-rw-r--r--   0        0        0       89 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_selected_tracks_as_aaf_omf.py
+-rw-r--r--   0        0        0      300 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_session_info_as_text.py
+-rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/extend_selection_to_target_tracks.py
+-rw-r--r--   0        0        0       81 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_dyamic_properties.py
+-rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_file_location.py
+-rw-r--r--   0        0        0      695 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_playback_mode.py
+-rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_ptsl_version.py
+-rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_record_mode.py
+-rw-r--r--   0        0        0       82 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_audio_format.py
+-rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_audio_rate_pull_settings.py
+-rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_bit_depth.py
+-rw-r--r--   0        0        0       85 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_feet_frames_rate.py
+-rw-r--r--   0        0        0      537 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_interleaved_state.py
+-rw-r--r--   0        0        0       77 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_length.py
+-rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_name.py
+-rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_path.py
+-rw-r--r--   0        0        0      631 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_sample_rate.py
+-rw-r--r--   0        0        0       80 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_start_time.py
+-rw-r--r--   0        0        0       83 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_time_code_rate.py
+-rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_video_rate_pull_settings.py
+-rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_task_status.py
+-rw-r--r--   0        0        0      774 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_track_list.py
+-rw-r--r--   0        0        0       78 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_transport_armed.py
+-rw-r--r--   0        0        0       78 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_transport_state.py
+-rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/host_ready_check.py
+-rw-r--r--   0        0        0       69 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/import_command.py
+-rw-r--r--   0        0        0      127 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/memory_locations.py
+-rw-r--r--   0        0        0       72 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/open_session.py
+-rw-r--r--   0        0        0     2771 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/operation.py
+-rw-r--r--   0        0        0       66 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/paste.py
+-rw-r--r--   0        0        0       73 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/paste_special.py
+-rw-r--r--   0        0        0       89 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/refresh_all_modified_audio_files.py
+-rw-r--r--   0        0        0       84 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/refresh_target_audio_files.py
+-rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/register_connection.py
+-rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/rename_selected_clip.py
+-rw-r--r--   0        0        0       77 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/rename_target_clip.py
+-rw-r--r--   0        0        0       78 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/rename_target_track.py
+-rw-r--r--   0        0        0       72 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/save_session.py
+-rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/save_session_as.py
+-rw-r--r--   0        0        0       82 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/select_all_clips_on_track.py
+-rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_playback_mode.py
+-rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_record_mode.py
+-rw-r--r--   0        0        0       82 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_audio_format.py
+-rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_audio_rate_pull_settings.py
+-rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_bit_depth.py
+-rw-r--r--   0        0        0       85 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_feet_frames_rate.py
+-rw-r--r--   0        0        0       87 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_interleaved_state.py
+-rw-r--r--   0        0        0       77 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_length.py
+-rw-r--r--   0        0        0       80 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_start_time.py
+-rw-r--r--   0        0        0       83 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_time_code_rate.py
+-rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_video_rate_pull_settings.py
+-rw-r--r--   0        0        0       65 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/spot.py
+-rw-r--r--   0        0        0      212 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/toggle_play_state.py
+-rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/trim_to_selection.py
+-rw-r--r--   0        0        0     4821 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/util.py
+-rw-r--r--   0        0        0     1759 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 py_ptsl-101.0.0/PKG-INFO
```

### Comparing `py_ptsl-100.3.0/LICENSE` & `py_ptsl-101.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/README.md` & `py_ptsl-101.0.0/README.md`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/PTSL_pb2.py` & `py_ptsl-101.0.0/ptsl/PTSL_pb2.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/PTSL_pb2.pyi` & `py_ptsl-101.0.0/ptsl/PTSL_pb2.pyi`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/PTSL_pb2_grpc.py` & `py_ptsl-101.0.0/ptsl/PTSL_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/__init__.py` & `py_ptsl-101.0.0/ptsl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
 """
 
 from .client import Client
 from .engine import Engine, open_engine
 from .errors import CommandError
 
-__version__ = '100.3.0'
+__version__ = '101.0.0'
```

### Comparing `py_ptsl-100.3.0/ptsl/client.py` & `py_ptsl-101.0.0/ptsl/client.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/errors.py` & `py_ptsl-101.0.0/ptsl/errors.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/ops/__init__.py` & `py_ptsl-101.0.0/ptsl/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/ops/get_playback_mode.py` & `py_ptsl-101.0.0/ptsl/ops/get_playback_mode.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/ops/get_session_interleaved_state.py` & `py_ptsl-101.0.0/ptsl/ops/get_session_interleaved_state.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/ops/get_session_sample_rate.py` & `py_ptsl-101.0.0/ptsl/ops/get_session_sample_rate.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/ops/get_track_list.py` & `py_ptsl-101.0.0/ptsl/ops/get_track_list.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/ops/operation.py` & `py_ptsl-101.0.0/ptsl/ops/operation.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/ptsl/util.py` & `py_ptsl-101.0.0/ptsl/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 """
 ptsl Utilities - Utility functions for working with types
 """
 
-from typing import Tuple, Optional
+from typing import Tuple, Optional, Dict
 from fractions import Fraction
-import os.path
 
 import ptsl.PTSL_pb2 as pt
 from ptsl.PTSL_pb2 import SessionTimeCodeRate, SessionFeetFramesRate, \
     SessionRatePull, SampleRate
 
 
 def timecode_info(
         session_rate: 'SessionTimeCodeRate'
-        ) -> Tuple[Fraction, bool]:
+) -> Tuple[Fraction, bool]:
     """
     For the given :class:`~ptsl.PTSL_pb2.SessionTimeCodeRate` enumeration
     value, returns a library-agnostic description that can be used for time
     arithmetic.
 
     The first element in the return :class:`tuple` is the duration of a frame
     in the given ``session_rate`` as a fractional number of seconds. The
     second element is a `bool` which is `True` if the ``session_rate`` is
     drop-frame.
 
     :param session_rate: The session rate value.
     :returns: a Tuple of (`frame duration`, `is drop frame`)
     """
-    map_dict = {
+    map_dict: Dict[pt.SessionTimeCodeRate, Tuple[int, int, bool]] = {
         pt.STCR_Fps120: (120, 1, False),
         pt.STCR_Fps120Drop: (120, 1, True),
         pt.STCR_Fps11988: (120_000, 1001, False),
         pt.STCR_Fps11988Drop: (120_000, 1001, True),
         pt.STCR_Fps100: (100, 1, False),
         pt.STCR_Fps60: (60, 1, False),
         pt.STCR_Fps60Drop: (60, 1, True),
@@ -47,15 +46,15 @@
         pt.STCR_Fps25: (25, 1, False),
         pt.STCR_Fps24: (24, 1, False),
         pt.STCR_Fps23976: (24000, 1001, False)
     }
     assert session_rate in map_dict.keys(), \
         "session_rate (%i) not recognized" % session_rate
 
-    val = map_dict.get(session_rate)
+    val = map_dict[session_rate]
     return (Fraction(val[0], val[1]), val[2])
 
 
 def feet_frames_info(feet_frames_rate: 'SessionFeetFramesRate') -> Fraction:
     """
     For the given :class:`~ptsl.PTSL_pb2.SessionFeetFramesRate` enumeration
     value, returns a library-agnostic description that can be used for time
@@ -72,26 +71,47 @@
     }
     assert feet_frames_rate in map_dict.keys(), \
         "feet_frames_rate (%i) not recognized" % feet_frames_rate
 
     return Fraction(*map_dict.get(feet_frames_rate))
 
 
+def sample_rate_enum(sample_rate: Optional[int]) -> 'SampleRate':
+    """
+    Get the symbolic sample rate from the `SampleRate` enum from
+    an integer.
+
+    .. note:: A `sample_rate` not in the enumeration will be returned
+        as `SR_None`
+    """
+    map_dict = {
+        192000: pt.SR_192000,
+        176400: pt.SR_176400,
+        96000: pt.SR_96000,
+        88200: pt.SR_88200,
+        48000: pt.SR_48000,
+        44100: pt.SR_44100,
+        None: pt.SR_None
+    }
+    return map_dict.get(sample_rate, pt.SR_None)
+
+
 def sample_rate_info(sample_rate: 'SampleRate') -> Optional[int]:
     """
     Get the sample rate for a :class:`~ptsl.PTSL_pb2.SampleRate` as an
     integer.
 
     .. note:: The :attr:`~ptsl.PTSL_pb2.SampleRate.SR_None` value will be
         returned as a `None`
     """
     map_dict = {
         pt.SR_192000: 192000,
         pt.SR_176400: 176400,
         pt.SR_96000: 96000,
+        pt.SR_88200: 88200,
         pt.SR_48000: 48000,
         pt.SR_44100: 44100,
         pt.SR_None: None
     }
     return map_dict[sample_rate]
 
 
@@ -119,34 +139,8 @@
         pt.SRP_Up4: (1, 0),
         pt.SRP_Up4Up01: (1, 1),
         pt.SRP_Up4Down01: (1, -1),
     }
     assert rate_pull in map_dict.keys(), \
         "rate_pull (%i) not recgonized" % rate_pull
 
-    return map_dict.get(rate_pull)
-
-
-def macos_to_patform_path(macos_path: str) -> str:
-    """
-    Converts a colon-delimited MacOS Classic path
-    into a native path on the current platform.
-    """
-
-    components = macos_path.split(":")
-    components = ["Volumes"] + components
-    return os.path.join(*components)
-
-# def native_to_macos_path(path: str) -> str:
-#     """
-#     Converts a path in the current platform's native
-#     format to a colon-delimited MacOS Classic path.
-#
-#     :param path: A native path. Must be normalized and
-#     absolute.
-#     """
-#     components = []
-#     head = path
-#     while head != "":
-#         head, tail = os.path.split(head)
-#         components = [tail] + components
-# FIXME: Finish this
+    return map_dict[rate_pull]
```

### Comparing `py_ptsl-100.3.0/pyproject.toml` & `py_ptsl-101.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_ptsl-100.3.0/PKG-INFO` & `py_ptsl-101.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ptsl
-Version: 100.3.0
+Version: 101.0.0
 Summary: Native Python PTSL (Pro Tools Scripting Library) RPC interface
 Keywords: pro tools,scripting,grpc,automation,avid
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

