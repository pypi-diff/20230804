# Comparing `tmp/flydra_analysis-0.7.14.tar.gz` & `tmp/flydra_analysis-0.7.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flydra_analysis-0.7.14.tar", last modified: Tue Sep 14 07:02:22 2021, max compression
+gzip compressed data, was "flydra_analysis-0.7.15.tar", last modified: Fri Aug  4 07:53:23 2023, max compression
```

## Comparing `flydra_analysis-0.7.14.tar` & `flydra_analysis-0.7.15.tar`

### file list

```diff
@@ -1,184 +1,131 @@
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:22.127265 flydra_analysis-0.7.14/
--rw-rw-rw-   0        0        0      138 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/.gitignore
--rw-rw-rw-   0        0        0     4275 2021-09-14 07:02:22.127265 flydra_analysis-0.7.14/PKG-INFO
--rw-rw-rw-   0        0        0     3901 2021-09-14 00:03:57.000000 flydra_analysis-0.7.14/README.md
--rw-rw-rw-   0        0        0      292 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/application-flydra-h5.sharedmimeinfo
--rw-rw-rw-   0        0        0      114 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra-plot-timeseries-2d-3d.mime
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:21.936540 flydra_analysis-0.7.14/flydra_analysis/
--rw-rw-rw-   0        0        0        0 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:22.049426 flydra_analysis-0.7.14/flydra_analysis/a2/
--rw-rw-rw-   0        0        0      383 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/Makefile.kalmanize
--rw-rw-rw-   0        0        0        2 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/__init__.py
--rw-rw-rw-   0        0        0     3495 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/aggdraw_coord_shifter.py
--rw-rw-rw-   0        0        0     1233 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/analysis_options.py
--rw-rw-rw-   0        0        0     5407 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/auto_discover_movies.py
--rw-rw-rw-   0        0        0     4738 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/auto_discover_ufmfs.py
--rw-rw-rw-   0        0        0    13611 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/benu.py
--rw-rw-rw-   0        0        0    14778 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/benu_colormaps.py
--rw-rw-rw-   0        0        0    10308 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/calculate_reprojection_errors.py
--rw-rw-rw-   0        0        0     2295 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/calculate_skipped_frames.py
--rw-rw-rw-   0        0        0    17064 2021-09-13 23:46:16.000000 flydra_analysis-0.7.14/flydra_analysis/a2/calibration_align_gui.py
--rw-rw-rw-   0        0        0      982 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/calibration_to_xml.py
--rw-rw-rw-   0        0        0     2301 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/check_clock_sync.py
--rw-rw-rw-   0        0        0     7987 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/check_frame_skip.py
--rw-rw-rw-   0        0        0     3505 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/check_mainbrain_h5_contiguity.py
--rw-rw-rw-   0        0        0     6354 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/conditions.py
--rw-rw-rw-   0        0        0      484 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/conditions2.py
--rw-rw-rw-   0        0        0    16010 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/conditions_draw.py
--rw-rw-rw-   0        0        0   105309 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/core_analysis.py
--rw-rw-rw-   0        0        0    17916 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/data2smoothed.py
--rw-rw-rw-   0        0        0     9885 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/densities.py
--rw-rw-rw-   0        0        0     5605 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/experiment_layout.py
--rw-rw-rw-   0        0        0     4123 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/find_equiv_obj_id.py
--rw-rw-rw-   0        0        0     2123 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/find_long_trajectories.py
--rw-rw-rw-   0        0        0     1609 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/flydra_images_export.py
--rw-rw-rw-   0        0        0     8616 2020-12-11 21:55:42.000000 flydra_analysis-0.7.14/flydra_analysis/a2/flydra_scons.py
--rw-rw-rw-   0        0        0      978 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/flydra_textlog2csv.py
--rw-rw-rw-   0        0        0     6335 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/flypos.py
--rw-rw-rw-   0        0        0     3310 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/get_2D_image_latency.py
--rw-rw-rw-   0        0        0     4453 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/get_2D_image_latency_plot.py
--rw-rw-rw-   0        0        0     2240 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/get_clock_sync.py
--rw-rw-rw-   0        0        0     5101 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/h5_info.py
--rw-rw-rw-   0        0        0     5906 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/h5_shorten.py
--rw-rw-rw-   0        0        0    48711 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/image_based_orientation.py
--rw-rw-rw-   0        0        0    16700 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/kdmovie_saver.py
--rw-rw-rw-   0        0        0     1248 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/kdmovie_saver_default_path.kmp
--rw-rw-rw-   0        0        0    53259 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/kdviewer.py
--rw-rw-rw-   0        0        0     2710 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/lsprofcalltree.py
--rw-rw-rw-   0        0        0     1361 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/misc.py
--rw-rw-rw-   0        0        0       45 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/missing_value_error.py
--rw-rw-rw-   0        0        0    37419 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/montage_ufmfs.py
--rw-rw-rw-   0        0        0    50431 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/orientation_ekf_fitter.py
--rw-rw-rw-   0        0        0     9963 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/orientation_ekf_plot.py
--rw-rw-rw-   0        0        0    10025 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/overlay_kalman_movie.py
--rw-rw-rw-   0        0        0     1639 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_calibration_input.py
--rw-rw-rw-   0        0        0      669 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_camera_positions.py
--rw-rw-rw-   0        0        0    25968 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_kalman_2d.py
--rw-rw-rw-   0        0        0      599 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_skipped_frames.py
--rw-rw-rw-   0        0        0     2513 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_summary.py
--rw-rw-rw-   0        0        0    24537 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_timeseries.py
--rw-rw-rw-   0        0        0    27896 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_timeseries_2d_3d.py
--rw-rw-rw-   0        0        0    15014 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/plot_top_view.py
--rw-rw-rw-   0        0        0     4751 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/pos_ori2fu.py
--rw-rw-rw-   0        0        0      180 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/print_kalmanize_makefile_location.py
--rw-rw-rw-   0        0        0      961 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/print_reprojection_error.py
--rw-rw-rw-   0        0        0     5340 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/ransac.py
--rw-rw-rw-   0        0        0    16133 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/retrack_movies.py
--rw-rw-rw-   0        0        0    11956 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/retrack_reuse_data_association.py
--rw-rw-rw-   0        0        0     2196 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/revert_schema12_to_schema11.py
--rw-rw-rw-   0        0        0     7326 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/rosbag2flydrah5.py
--rw-rw-rw-   0        0        0      794 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_bowl.xml
--rw-rw-rw-   0        0        0     3716 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_calibration.xml
--rw-rw-rw-   0        0        0     3360 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_calibration_water.xml
--rw-rw-rw-   0        0        0 17292460 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_datafile-v0.4.28.h5
--rw-rw-rw-   0        0        0  1967744 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_datafile-v0.4.28.h5.retracked.h5
--rw-rw-rw-   0        0        0   286952 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_datafile.h5.spreadh5
--rw-rw-rw-   0        0        0    75544 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_kalman_trajectories.h5
--rw-rw-rw-   0        0        0      178 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_one_meter_cylinder_arena.xml
--rw-rw-rw-   0        0        0      399 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/a2/sample_stim_cubic_arena.xml
--rw-rw-rw-   0        0        0    55668 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/save_movies_overlay.py
--rw-rw-rw-   0        0        0      960 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/stim_plugins.py
--rw-rw-rw-   0        0        0     1136 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/stimulus_positions.py
--rw-rw-rw-   0        0        0     1747 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/tables_tools.py
--rw-rw-rw-   0        0        0     3390 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/trajectory_filtering.py
--rw-rw-rw-   0        0        0    11636 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/ufmf_tools.py
--rw-rw-rw-   0        0        0    10485 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/a2/utils.py
--rw-rw-rw-   0        0        0     7029 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/water_surface_align.py
--rw-rw-rw-   0        0        0    25329 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/a2/xml_stimulus.py
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:22.077812 flydra_analysis-0.7.14/flydra_analysis/analysis/
--rw-rw-rw-   0        0        0    34589 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/PQmath.py
--rw-rw-rw-   0        0        0        0 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/__init__.py
--rw-rw-rw-   0        0        0     8855 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/caching_movie_opener.py
--rw-rw-rw-   0        0        0    89478 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/calc_forces.py
--rw-rw-rw-   0        0        0     2004 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/cam_params_play.py
--rw-rw-rw-   0        0        0     2810 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/circstats.py
--rw-rw-rw-   0        0        0      748 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/copy_data_files.sh
--rw-rw-rw-   0        0        0      550 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/copy_data_files_local.sh
--rw-rw-rw-   0        0        0      105 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/create_movie.sh
--rw-rw-rw-   0        0        0     8132 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_convert_to_mat.py
--rw-rw-rw-   0        0        0     4698 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_filter_kalman_data.py
--rw-rw-rw-   0        0        0    16144 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_generate_recalibration.py
--rw-rw-rw-   0        0        0     3160 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_plot_clock_drift.py
--rw-rw-rw-   0        0        0     9690 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_plot_kalman_2d_histogram.py
--rw-rw-rw-   0        0        0      906 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_print_camera_summary.py
--rw-rw-rw-   0        0        0     1891 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_convert_table_add_point_id.py
--rw-rw-rw-   0        0        0     4864 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/hzgeom.py
--rw-rw-rw-   0        0        0      517 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/move_data_files_local.sh
--rw-rw-rw-   0        0        0     1515 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/pqmath_angular_velocity_quaternion_play.py
--rw-rw-rw-   0        0        0     6265 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/reconstruct_orientation.py
--rw-rw-rw-   0        0        0    28159 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/result_utils.py
--rw-rw-rw-   0        0        0     3698 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/save_as_flydra_hdf5.py
--rw-rw-rw-   0        0        0     2874 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/setup_analysis_dir.sh
--rw-rw-rw-   0        0        0     1444 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/smdfile.py
--rw-rw-rw-   0        0        0     2004 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/smooth_position.m
--rw-rw-rw-   0        0        0      573 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/smooth_position_micro_demo.py
--rw-rw-rw-   0        0        0      193 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/test_smooth.m
--rw-rw-rw-   0        0        0     4639 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/analysis/test_smooth_orientation.py
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:22.094823 flydra_analysis-0.7.14/flydra_analysis/autogenerated/
--rw-rw-rw-   0        0        0  1963909 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/data2smoothed.mat
--rw-rw-rw-   0        0        0   286952 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/datafile2d.spreadh5
--rw-rw-rw-   0        0        0  1256466 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/kalmanized.h5
--rw-rw-rw-   0        0        0    25256 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/mpl_markersize.png
--rw-rw-rw-   0        0        0   384161 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/plot_kalman_2d.png
--rw-rw-rw-   0        0        0   151462 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/plot_timeseries_2d.png
--rw-rw-rw-   0        0        0   222753 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/plot_timeseries_2d_3d.png
--rw-rw-rw-   0        0        0   139169 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/flydra_analysis/autogenerated/plot_timeseries_2d_with_spread.png
--rw-rw-rw-   0        0        0     8052 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/generate_fake_calibration.py
--rw-rw-rw-   0        0        0     1853 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/image_compare.py
--rw-rw-rw-   0        0        0    43090 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/kalmanize.py
--rw-rw-rw-   0        0        0      726 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/mpl_markersize.py
--rw-rw-rw-   0        0        0     3627 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/offline_data_save.py
--rw-rw-rw-   0        0        0     3755 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/talign.py
--rw-rw-rw-   0        0        0    14612 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/test_commands.py
--rw-rw-rw-   0        0        0     8264 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/flydra_analysis/test_geom.py
--rw-rw-rw-   0        0        0    19759 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_analysis/test_reconstruction.py
--rw-rw-rw-   0        0        0       53 2021-09-14 06:11:57.000000 flydra_analysis-0.7.14/flydra_analysis/version.py
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:21.948539 flydra_analysis-0.7.14/flydra_analysis.egg-info/
--rw-rw-rw-   0        0        0     4275 2021-09-14 07:02:21.000000 flydra_analysis-0.7.14/flydra_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7002 2021-09-14 07:02:21.000000 flydra_analysis-0.7.14/flydra_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-14 07:02:21.000000 flydra_analysis-0.7.14/flydra_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4250 2021-09-14 07:02:21.000000 flydra_analysis-0.7.14/flydra_analysis.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2021-09-14 07:02:21.000000 flydra_analysis-0.7.14/flydra_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   290554 2021-09-14 07:02:21.000000 flydra_analysis-0.7.14/flydra_fastfinder_help.c
--rw-rw-rw-   0        0        0     2096 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/flydra_fastfinder_help.pyx
--rw-rw-rw-   0        0        0      158 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/pyproject.toml
--rw-rw-rw-   0        0        0      174 2021-09-14 06:39:24.000000 flydra_analysis-0.7.14/requirements.txt
--rw-rw-rw-   0        0        0      210 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/run_tests.sh
--rw-rw-rw-   0        0        0      795 2021-09-14 07:02:22.131264 flydra_analysis-0.7.14/setup.cfg
--rw-rw-rw-   0        0        0     6916 2021-09-14 06:11:57.000000 flydra_analysis-0.7.14/setup.py
--rw-rw-rw-   0        0        0      612 2020-04-08 16:40:27.000000 flydra_analysis-0.7.14/stdeb.cfg
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:22.102129 flydra_analysis-0.7.14/tests/
-drwxrwxrwx   0        0        0        0 2021-09-14 07:02:22.126266 flydra_analysis-0.7.14/tests/sample_calibration/
--rw-rw-rw-   0        0        0      245 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/Cst.dat
--rw-rw-rw-   0        0        0      975 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/Pmatrices.dat
--rw-rw-rw-   0        0        0      735 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/Pst.dat
--rw-rw-rw-   0        0        0       40 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/Res.dat
--rw-rw-rw-   0        0        0      202 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename1.cal
--rw-rw-rw-   0        0        0      337 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename1.rad
--rw-rw-rw-   0        0        0      199 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename2.cal
--rw-rw-rw-   0        0        0      337 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename2.rad
--rw-rw-rw-   0        0        0      201 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename3.cal
--rw-rw-rw-   0        0        0      337 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename3.rad
--rw-rw-rw-   0        0        0      204 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename4.cal
--rw-rw-rw-   0        0        0      336 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename4.rad
--rw-rw-rw-   0        0        0      202 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename5.cal
--rw-rw-rw-   0        0        0      337 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/basename5.rad
--rw-rw-rw-   0        0        0       12 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/calibration_units.txt
--rw-rw-rw-   0        0        0    57178 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/cam1.points4cal.dat
--rw-rw-rw-   0        0        0    46782 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/cam2.points4cal.dat
--rw-rw-rw-   0        0        0    51528 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/cam3.points4cal.dat
--rw-rw-rw-   0        0        0    57178 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/cam4.points4cal.dat
--rw-rw-rw-   0        0        0    27120 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/cam5.points4cal.dat
--rw-rw-rw-   0        0        0      195 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/camera1.Pmat.cal
--rw-rw-rw-   0        0        0      195 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/camera2.Pmat.cal
--rw-rw-rw-   0        0        0      195 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/camera3.Pmat.cal
--rw-rw-rw-   0        0        0      195 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/camera4.Pmat.cal
--rw-rw-rw-   0        0        0      195 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/camera5.Pmat.cal
--rw-rw-rw-   0        0        0       35 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/sample_calibration/camera_order.txt
--rw-rw-rw-   0        0        0     1333 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/tests/test_calculate_reprojection_errors.py
--rw-rw-rw-   0        0        0     1845 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/test_calibration_realignment.py
--rw-rw-rw-   0        0        0      947 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/test_export_flydra_hdf5.py
--rw-rw-rw-   0        0        0     1670 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/test_previously_failing.py
--rw-rw-rw-   0        0        0     5527 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/tests/test_pymvg.py
--rw-rw-rw-   0        0        0     3862 2021-07-18 07:01:45.000000 flydra_analysis-0.7.14/tests/test_reconstruct.py
--rw-rw-rw-   0        0        0      549 2020-04-06 16:08:04.000000 flydra_analysis-0.7.14/tests/test_result_utils.py
+drwxr-xr-x   0 andrew     (504) staff       (20)        0 2023-08-04 07:53:23.218318 flydra_analysis-0.7.15/
+-rw-r--r--   0 andrew     (504) staff       (20)       35 2023-08-04 07:52:02.000000 flydra_analysis-0.7.15/MANIFEST.in
+-rw-r--r--   0 andrew     (504) staff       (20)      522 2023-08-04 07:53:23.218067 flydra_analysis-0.7.15/PKG-INFO
+-rw-r--r--   0 andrew     (504) staff       (20)      205 2023-08-04 07:52:02.000000 flydra_analysis-0.7.15/README.md
+drwxr-xr-x   0 andrew     (504) staff       (20)        0 2023-08-04 07:53:23.165675 flydra_analysis-0.7.15/flydra_analysis/
+-rw-r--r--   0 andrew     (504) staff       (20)        0 2018-12-05 14:59:22.000000 flydra_analysis-0.7.15/flydra_analysis/__init__.py
+drwxr-xr-x   0 andrew     (504) staff       (20)        0 2023-08-04 07:53:23.210083 flydra_analysis-0.7.15/flydra_analysis/a2/
+-rw-r--r--   0 andrew     (504) staff       (20)      383 2018-12-05 14:59:22.000000 flydra_analysis-0.7.15/flydra_analysis/a2/Makefile.kalmanize
+-rw-r--r--   0 andrew     (504) staff       (20)        2 2018-12-05 14:59:22.000000 flydra_analysis-0.7.15/flydra_analysis/a2/__init__.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3495 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/aggdraw_coord_shifter.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1233 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/analysis_options.py
+-rw-r--r--   0 andrew     (504) staff       (20)     5407 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/auto_discover_movies.py
+-rw-r--r--   0 andrew     (504) staff       (20)     4738 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/auto_discover_ufmfs.py
+-rw-r--r--   0 andrew     (504) staff       (20)    13611 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/benu.py
+-rw-r--r--   0 andrew     (504) staff       (20)    14778 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/benu_colormaps.py
+-rw-r--r--   0 andrew     (504) staff       (20)    10308 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/calculate_reprojection_errors.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2295 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/calculate_skipped_frames.py
+-rwxr-xr-x   0 andrew     (504) staff       (20)    17064 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/calibration_align_gui.py
+-rw-r--r--   0 andrew     (504) staff       (20)      982 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/calibration_to_xml.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2301 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/check_clock_sync.py
+-rw-r--r--   0 andrew     (504) staff       (20)     7987 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/check_frame_skip.py
+-rwxr-xr-x   0 andrew     (504) staff       (20)     3505 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/check_mainbrain_h5_contiguity.py
+-rw-r--r--   0 andrew     (504) staff       (20)     6354 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/conditions.py
+-rw-r--r--   0 andrew     (504) staff       (20)      484 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/conditions2.py
+-rw-r--r--   0 andrew     (504) staff       (20)    16010 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/conditions_draw.py
+-rw-r--r--   0 andrew     (504) staff       (20)   105205 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/a2/core_analysis.py
+-rw-r--r--   0 andrew     (504) staff       (20)    17916 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/data2smoothed.py
+-rw-r--r--   0 andrew     (504) staff       (20)     9885 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/densities.py
+-rw-r--r--   0 andrew     (504) staff       (20)     5605 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/experiment_layout.py
+-rw-r--r--   0 andrew     (504) staff       (20)     4123 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/find_equiv_obj_id.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2123 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/find_long_trajectories.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1609 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/flydra_images_export.py
+-rwxr-xr-x   0 andrew     (504) staff       (20)     8616 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/flydra_scons.py
+-rw-r--r--   0 andrew     (504) staff       (20)      978 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/flydra_textlog2csv.py
+-rw-r--r--   0 andrew     (504) staff       (20)     6335 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/flypos.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3310 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/get_2D_image_latency.py
+-rw-r--r--   0 andrew     (504) staff       (20)     4453 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/get_2D_image_latency_plot.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2240 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/get_clock_sync.py
+-rw-r--r--   0 andrew     (504) staff       (20)     5101 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/h5_info.py
+-rw-r--r--   0 andrew     (504) staff       (20)     5906 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/h5_shorten.py
+-rw-r--r--   0 andrew     (504) staff       (20)    48719 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/a2/image_based_orientation.py
+-rw-r--r--   0 andrew     (504) staff       (20)    16700 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/kdmovie_saver.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1248 2018-12-05 14:59:22.000000 flydra_analysis-0.7.15/flydra_analysis/a2/kdmovie_saver_default_path.kmp
+-rw-r--r--   0 andrew     (504) staff       (20)    53263 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/a2/kdviewer.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2710 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/lsprofcalltree.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1361 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/misc.py
+-rw-r--r--   0 andrew     (504) staff       (20)       45 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/missing_value_error.py
+-rw-r--r--   0 andrew     (504) staff       (20)    37419 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/montage_ufmfs.py
+-rw-r--r--   0 andrew     (504) staff       (20)    50439 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/a2/orientation_ekf_fitter.py
+-rw-r--r--   0 andrew     (504) staff       (20)     9965 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/a2/orientation_ekf_plot.py
+-rw-r--r--   0 andrew     (504) staff       (20)    10025 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/overlay_kalman_movie.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1639 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_calibration_input.py
+-rw-r--r--   0 andrew     (504) staff       (20)      669 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_camera_positions.py
+-rw-r--r--   0 andrew     (504) staff       (20)    25968 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_kalman_2d.py
+-rw-r--r--   0 andrew     (504) staff       (20)      599 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_skipped_frames.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2513 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_summary.py
+-rw-r--r--   0 andrew     (504) staff       (20)    24537 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_timeseries.py
+-rw-r--r--   0 andrew     (504) staff       (20)    27896 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_timeseries_2d_3d.py
+-rw-r--r--   0 andrew     (504) staff       (20)    15014 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/plot_top_view.py
+-rw-r--r--   0 andrew     (504) staff       (20)     4751 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/pos_ori2fu.py
+-rw-r--r--   0 andrew     (504) staff       (20)      180 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/print_kalmanize_makefile_location.py
+-rw-r--r--   0 andrew     (504) staff       (20)      961 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/print_reprojection_error.py
+-rw-r--r--   0 andrew     (504) staff       (20)     5340 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/ransac.py
+-rw-r--r--   0 andrew     (504) staff       (20)    16133 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/retrack_movies.py
+-rw-r--r--   0 andrew     (504) staff       (20)    11956 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/retrack_reuse_data_association.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2196 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/revert_schema12_to_schema11.py
+-rw-r--r--   0 andrew     (504) staff       (20)     7326 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/rosbag2flydrah5.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3716 2018-12-05 14:59:22.000000 flydra_analysis-0.7.15/flydra_analysis/a2/sample_calibration.xml
+-rw-r--r--   0 andrew     (504) staff       (20) 17292460 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/flydra_analysis/a2/sample_datafile-v0.4.28.h5
+-rw-r--r--   0 andrew     (504) staff       (20)  1967744 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/flydra_analysis/a2/sample_datafile-v0.4.28.h5.retracked.h5
+-rw-r--r--   0 andrew     (504) staff       (20)    75544 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/flydra_analysis/a2/sample_kalman_trajectories.h5
+-rw-r--r--   0 andrew     (504) staff       (20)    55668 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/save_movies_overlay.py
+-rw-r--r--   0 andrew     (504) staff       (20)      960 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/stim_plugins.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1136 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/stimulus_positions.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1747 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/tables_tools.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3390 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/trajectory_filtering.py
+-rw-r--r--   0 andrew     (504) staff       (20)    11636 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/ufmf_tools.py
+-rw-r--r--   0 andrew     (504) staff       (20)    10489 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/a2/utils.py
+-rw-r--r--   0 andrew     (504) staff       (20)     7037 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/a2/water_surface_align.py
+-rw-r--r--   0 andrew     (504) staff       (20)    25329 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/a2/xml_stimulus.py
+drwxr-xr-x   0 andrew     (504) staff       (20)        0 2023-08-04 07:53:23.215246 flydra_analysis-0.7.15/flydra_analysis/analysis/
+-rw-r--r--   0 andrew     (504) staff       (20)    34589 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/PQmath.py
+-rw-r--r--   0 andrew     (504) staff       (20)        0 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/__init__.py
+-rw-r--r--   0 andrew     (504) staff       (20)     8855 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/caching_movie_opener.py
+-rw-r--r--   0 andrew     (504) staff       (20)    89478 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/calc_forces.py
+-rwxr-xr-x   0 andrew     (504) staff       (20)     2004 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/cam_params_play.py
+-rw-r--r--   0 andrew     (504) staff       (20)     2810 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/circstats.py
+-rw-r--r--   0 andrew     (504) staff       (20)     8132 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_convert_to_mat.py
+-rw-r--r--   0 andrew     (504) staff       (20)     4698 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_filter_kalman_data.py
+-rw-r--r--   0 andrew     (504) staff       (20)    16063 2023-07-15 11:47:20.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_generate_recalibration.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3160 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_plot_clock_drift.py
+-rw-r--r--   0 andrew     (504) staff       (20)     9690 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_plot_kalman_2d_histogram.py
+-rw-r--r--   0 andrew     (504) staff       (20)      906 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_print_camera_summary.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1891 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_convert_table_add_point_id.py
+-rw-r--r--   0 andrew     (504) staff       (20)     4864 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/hzgeom.py
+-rwxr-xr-x   0 andrew     (504) staff       (20)     1515 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/pqmath_angular_velocity_quaternion_play.py
+-rw-r--r--   0 andrew     (504) staff       (20)     6267 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/reconstruct_orientation.py
+-rw-r--r--   0 andrew     (504) staff       (20)    28159 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/result_utils.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3698 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/save_as_flydra_hdf5.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1444 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/smdfile.py
+-rw-r--r--   0 andrew     (504) staff       (20)      573 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/smooth_position_micro_demo.py
+-rw-r--r--   0 andrew     (504) staff       (20)     4583 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/analysis/test_smooth_orientation.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1857 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/image_compare.py
+-rw-r--r--   0 andrew     (504) staff       (20)    43092 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/kalmanize.py
+-rw-r--r--   0 andrew     (504) staff       (20)      726 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/mpl_markersize.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3627 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/offline_data_save.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3763 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/talign.py
+-rw-r--r--   0 andrew     (504) staff       (20)    14473 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_analysis/test_commands.py
+-rw-r--r--   0 andrew     (504) staff       (20)     8264 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/test_geom.py
+-rw-r--r--   0 andrew     (504) staff       (20)    19759 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/flydra_analysis/test_reconstruction.py
+-rw-r--r--   0 andrew     (504) staff       (20)       59 2023-08-04 07:52:02.000000 flydra_analysis-0.7.15/flydra_analysis/version.py
+drwxr-xr-x   0 andrew     (504) staff       (20)        0 2023-08-04 07:53:23.167171 flydra_analysis-0.7.15/flydra_analysis.egg-info/
+-rw-r--r--   0 andrew     (504) staff       (20)      522 2023-08-04 07:53:23.000000 flydra_analysis-0.7.15/flydra_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (504) staff       (20)     4863 2023-08-04 07:53:23.000000 flydra_analysis-0.7.15/flydra_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (504) staff       (20)        1 2023-08-04 07:53:23.000000 flydra_analysis-0.7.15/flydra_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (504) staff       (20)     4249 2023-08-04 07:53:23.000000 flydra_analysis-0.7.15/flydra_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 andrew     (504) staff       (20)      262 2023-08-04 07:53:23.000000 flydra_analysis-0.7.15/flydra_analysis.egg-info/requires.txt
+-rw-r--r--   0 andrew     (504) staff       (20)       39 2023-08-04 07:53:23.000000 flydra_analysis-0.7.15/flydra_analysis.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (504) staff       (20)   431171 2023-08-04 07:53:22.000000 flydra_analysis-0.7.15/flydra_fastfinder_help.c
+-rw-r--r--   0 andrew     (504) staff       (20)     2100 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/flydra_fastfinder_help.pyx
+-rw-r--r--   0 andrew     (504) staff       (20)     6523 2023-08-04 07:52:02.000000 flydra_analysis-0.7.15/pyproject.toml
+-rw-r--r--   0 andrew     (504) staff       (20)       38 2023-08-04 07:53:23.218414 flydra_analysis-0.7.15/setup.cfg
+-rw-r--r--   0 andrew     (504) staff       (20)      379 2023-07-26 07:22:51.000000 flydra_analysis-0.7.15/setup.py
+drwxr-xr-x   0 andrew     (504) staff       (20)        0 2023-08-04 07:53:23.217728 flydra_analysis-0.7.15/tests/
+-rw-r--r--   0 andrew     (504) staff       (20)     1333 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/tests/test_calculate_reprojection_errors.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1845 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/tests/test_calibration_realignment.py
+-rw-r--r--   0 andrew     (504) staff       (20)      947 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/tests/test_export_flydra_hdf5.py
+-rw-r--r--   0 andrew     (504) staff       (20)     1670 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/tests/test_previously_failing.py
+-rw-r--r--   0 andrew     (504) staff       (20)     5527 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/tests/test_pymvg.py
+-rw-r--r--   0 andrew     (504) staff       (20)     3862 2021-03-28 06:13:39.000000 flydra_analysis-0.7.15/tests/test_reconstruct.py
+-rw-r--r--   0 andrew     (504) staff       (20)      549 2018-12-05 14:59:23.000000 flydra_analysis-0.7.15/tests/test_result_utils.py
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/aggdraw_coord_shifter.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/aggdraw_coord_shifter.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/analysis_options.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/analysis_options.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/auto_discover_movies.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/auto_discover_movies.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/auto_discover_ufmfs.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/auto_discover_ufmfs.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/benu.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/benu.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/benu_colormaps.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/benu_colormaps.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/calculate_reprojection_errors.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/calculate_reprojection_errors.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/calculate_skipped_frames.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/calculate_skipped_frames.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/calibration_align_gui.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/calibration_align_gui.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/calibration_to_xml.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/calibration_to_xml.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/check_clock_sync.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/check_clock_sync.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/check_frame_skip.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/check_frame_skip.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/check_mainbrain_h5_contiguity.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/check_mainbrain_h5_contiguity.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/conditions.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/conditions.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/conditions_draw.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/conditions_draw.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/core_analysis.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/core_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 import cgtypes  # cgkit 1.x
 
 import weakref
 import warnings, tempfile
 import unittest
 from distutils.version import StrictVersion
 import pkg_resources
-from nose.plugins.attrib import attr as nose_attr  # ubuntu: apt-get install python-nose
-
+import pytest
 
 def add_arguments_to_parser(parser):
     return add_options_to_parser(parser, is_argparse=True)
 
 
 def add_options_to_parser(parser, is_argparse=False):
     if is_argparse:
@@ -219,15 +218,15 @@
     elif 0:
         # take qth point
         return x[::q]
     else:
         # simple averaging
         xtrimlen = int(math.ceil(len(x) / q)) * q
         lendiff = xtrimlen - len(x)
-        xtrim = numpy.zeros((xtrimlen,), dtype=numpy.float)
+        xtrim = numpy.zeros((xtrimlen,), dtype=numpy.float64)
         xtrim[: len(x)] = x
 
         all = []
         for i in range(q):
             all.append(xtrim[i::q])
         mysum = numpy.sum(numpy.array(all), axis=0)
         result = numpy.zeros_like(mysum)
@@ -353,18 +352,18 @@
         fend,
     )
     frames = numpy.arange(fstart, fend + 1, dtype=np.int64)
     if frames.dtype != obs_frames.dtype:
         warnings.warn("searchsorted is probably very slow because of different dtypes")
     idx = frames.searchsorted(obs_frames)
 
-    x = np.nan * numpy.ones(frames.shape, dtype=numpy.float)
-    y = np.nan * numpy.ones(frames.shape, dtype=numpy.float)
-    z = np.nan * numpy.ones(frames.shape, dtype=numpy.float)
-    R = np.nan * numpy.ones((frames.shape[0], 3, 3), dtype=numpy.float)
+    x = np.nan * numpy.ones(frames.shape, dtype=numpy.float64)
+    y = np.nan * numpy.ones(frames.shape, dtype=numpy.float64)
+    z = np.nan * numpy.ones(frames.shape, dtype=numpy.float64)
+    R = np.nan * numpy.ones((frames.shape[0], 3, 3), dtype=numpy.float64)
     obj_id_array = numpy.ma.masked_array(
         numpy.empty(frames.shape, dtype=numpy.uint32),
         mask=numpy.ones(frames.shape, dtype=numpy.bool_),
     )
 
     x[idx] = orig_rows["x"]
     y[idx] = orig_rows["y"]
@@ -642,15 +641,15 @@
 
     Returns
     -------
     directions : Nx3 array
        directions above with sign chosen to minimize cost
     """
     if (up_dir is None) and (elevation_up_bias_degrees != 0):
-        # up_dir = np.array([0,0,1],dtype=np.float)
+        # up_dir = np.array([0,0,1],dtype=np.float64)
         raise ValueError("up_dir must be specified. " "(Hint: --up-dir='0,0,1')")
     D2R = np.pi / 180
 
     if DEBUG:
         frames = rows["frame"]
         if 1:
             cond1 = (128125 < frames) & (frames < 128140)
@@ -1828,15 +1827,15 @@
             self.keep_references.append(
                 data_file
             )  # prevent from garbage collection with weakref
 
         is_mat_file = check_is_mat_file(data_file)
 
         if up_dir is not None:
-            up_dir = np.array(up_dir, dtype=np.float)
+            up_dir = np.array(up_dir, dtype=np.float64)
 
         if is_mat_file:
             # We ignore use_kalman_smoothing -- always smoothed
             if 0:
                 kalman_rows = matfile2rows(data_file, obj_id)
             elif 0:
                 kalman_rows = LazyRecArrayMimic(data_file, obj_id)
@@ -2367,15 +2366,15 @@
             h5file.close()
             del self._smooth_cache.open_cache_h5files[fname]
 
     def __del__(self):
         self.close()
 
 
-@nose_attr("known_fail")
+@pytest.mark.xfail
 def test_choose_orientations():
     #                             8     9     10   11  12 13   14   15     16     17     18  19 20
     x = np.array(
         [
             0,
             1,
             2,
@@ -2503,27 +2502,27 @@
         for data_file, is_mat_file in zip(self.data_files, self.is_mat_files):
             if not is_mat_file:
                 data_file.close()
 
     def failUnless(self, value):
         assert not value, "test failed"
 
-    @nose_attr("known_fail")
+    @pytest.mark.xfail
     def test_fast_startstopidx_on_sorted_array_scalar(self):
         sorted_array = numpy.arange(10)
         for value in [-1, 0, 2, 5, 6, 11]:
             idx_fast_start, idx_fast_stop = fast_startstopidx_on_sorted_array(
                 sorted_array, value
             )
             idx_slow = numpy.nonzero(sorted_array == value)[0]
             idx_fast = numpy.arange(idx_fast_start, idx_fast_stop)
             self.failUnless(idx_fast.shape == idx_slow.shape)
             self.failUnless(numpy.allclose(idx_fast, idx_slow))
 
-    @nose_attr("known_fail")
+    @pytest.mark.xfail
     def test_fast_startstopidx_on_sorted_array_1d(self):
         sorted_array = numpy.arange(10)
         values = [-1, 0, 2, 5, 6, 11]
 
         idx_fast_start, idx_fast_stop = fast_startstopidx_on_sorted_array(
             sorted_array, values
         )
@@ -2557,15 +2556,15 @@
                 except NoObjectIDError:
                     pass
                 else:
                     raise RuntimeError(
                         "We should not get here - a " "NoObjectIDError should be raised"
                     )
 
-    @nose_attr("known_fail")
+    @pytest.mark.xfail
     def test_smooth(self):
         if not hasattr(self, "data_files"):
             # XXX why do I have to do this? Shouldn't nose do this?
             self.setUp()
         for i in range(len(self.data_files)):
             yield self.check_smooth, i
 
@@ -2632,15 +2631,15 @@
                 orig = numpy.array(orig)
                 smooth = numpy.array(smooth)
                 dist = numpy.sqrt(numpy.sum((orig - smooth) ** 2, axis=1))
                 mean_dist = numpy.mean(dist)
                 # print 'mean_dist',mean_dist
                 assert mean_dist < 1.0  # should certainly be less than 1 meter!
 
-    @nose_attr("known_fail")
+    @pytest.mark.xfail
     def test_CachingAnalyzer_load_data1(self):
         if not hasattr(self, "data_files"):
             # XXX why do I have to do this? Shouldn't nose do this?
             self.setUp()
         for i in range(len(self.data_files)):
             yield self.check_load_data1, i
 
@@ -2689,15 +2688,15 @@
                     )
                 filt = numpy.array(filt)
                 smooth = numpy.array(smooth)
                 dist = numpy.sqrt(numpy.sum((filt - smooth) ** 2, axis=1))
                 mean_dist = numpy.mean(dist)
                 assert mean_dist < 0.1
 
-    @nose_attr("known_fail")
+    @pytest.mark.xfail
     def test_CachingAnalyzer_calculate_trajectory_metrics(self):
         for data_file, test_obj_ids, is_mat_file, fps, model in zip(
             self.data_files,
             self.test_obj_ids_list,
             self.is_mat_files,
             self.fps,
             self.dynamic_model,
@@ -2725,15 +2724,15 @@
                     # if rows are missing in original kalman data, we
                     # can interpolate here:
 
                     ## print ("len(results['X_kalmanized']),len(rows),obj_id",
                     ##        len(results['X_kalmanized']),len(rows),obj_id)
                     assert len(results["X_kalmanized"]) == len(rows)
 
-    @nose_attr("known_fail")
+    @pytest.mark.xfail
     def test_CachingAnalyzer_load_data2(self):
         if not hasattr(self, "data_files"):
             # XXX why do I have to do this? Shouldn't nose do this?
             self.setUp()
         for i in range(len(self.data_files)):
             # for smooth in [True,False]:
             for smooth in [False, True]:
@@ -2760,21 +2759,21 @@
         ##        rows['obj_id'], test_obj_ids)
         assert numpy.allclose(rows["obj_id"], test_obj_ids)
         # print
 
 
 if 1:
 
-    @nose_attr("known_fail")
+    @pytest.mark.xfail
     def test_choose_orientations2():
         x = numpy.linspace(0, 1000, 10)
         y = numpy.ones_like(x)
         z = numpy.ones_like(x)
         rows = np.recarray(
-            x.shape, dtype=[("x", np.float), ("y", np.float), ("z", np.float)]
+            x.shape, dtype=[("x", np.float64), ("y", np.float64), ("z", np.float64)]
         )
         rows["x"] = x
         rows["y"] = y
         rows["z"] = z
         directions = np.zeros((len(x), 3))
         directions[:, 0] = np.random.randn(len(x))
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/data2smoothed.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/data2smoothed.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/densities.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/densities.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/experiment_layout.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/experiment_layout.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/find_equiv_obj_id.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/find_equiv_obj_id.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/find_long_trajectories.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/find_long_trajectories.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/flydra_images_export.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/flydra_images_export.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/flydra_scons.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/flydra_scons.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/flydra_textlog2csv.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/flydra_textlog2csv.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/flypos.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/flypos.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/get_2D_image_latency.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/get_2D_image_latency.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/get_2D_image_latency_plot.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/get_2D_image_latency_plot.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/get_clock_sync.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/get_clock_sync.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/h5_info.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/h5_info.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/h5_shorten.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/h5_shorten.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/image_based_orientation.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/image_based_orientation.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,15 +591,15 @@
 
                     com_coords = np.array(com_coords)
                     if do_rts_smoothing:
                         # Perform RTS smoothing on center-of-mass coordinates.
 
                         # Find first good datum.
                         fgnz = np.nonzero(~np.isnan(com_coords[:, 0]))
-                        com_coords_smooth = np.empty(com_coords.shape, dtype=np.float)
+                        com_coords_smooth = np.empty(com_coords.shape, dtype=np.float64)
                         com_coords_smooth.fill(np.nan)
 
                         if len(fgnz[0]):
                             first_good = fgnz[0][0]
 
                             RTS_com_coords = com_coords[first_good:, :]
 
@@ -608,25 +608,25 @@
                             A = np.array(
                                 [
                                     [1, 0, dt, 0],  # process update
                                     [0, 1, 0, dt],
                                     [0, 0, 1, 0],
                                     [0, 0, 0, 1],
                                 ],
-                                dtype=np.float,
+                                dtype=np.float64,
                             )
                             C = np.array(
                                 [[1, 0, 0, 0], [0, 1, 0, 0]],  # observation matrix
-                                dtype=np.float,
+                                dtype=np.float64,
                             )
                             Q = 0.1 * np.eye(4)  # process noise
                             R = 1.0 * np.eye(2)  # observation noise
                             initx = np.array(
                                 [RTS_com_coords[0, 0], RTS_com_coords[0, 1], 0, 0],
-                                dtype=np.float,
+                                dtype=np.float64,
                             )
                             initV = 2 * np.eye(4)
                             initV[0, 0] = 0.1
                             initV[1, 1] = 0.1
                             y = RTS_com_coords
                             xsmooth, Vsmooth = adskalman.adskalman.kalman_smoother(
                                 y, A, C, Q, R, initx, initV
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/kdmovie_saver.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/kdmovie_saver.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/kdmovie_saver_default_path.kmp` & `flydra_analysis-0.7.15/flydra_analysis/a2/kdmovie_saver_default_path.kmp`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/kdviewer.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/kdviewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         "kalman",
         "observations",
     ]  # kalman means smoothed or filtered, depending on use_kalman_smoothing
 
     all_max_vel = 0.0
 
     if up_dir is not None:
-        up_dir = np.array(up_dir, dtype=np.float)
+        up_dir = np.array(up_dir, dtype=np.float64)
         assert up_dir.shape == (3,)
 
     if link_all_simultaneous_objs:
         allsave = []
 
     if not use_kalman_smoothing:
         if options.dynamic_model is not None:
@@ -868,15 +868,15 @@
                 or options.highlight_stop is not None
             ):
                 highlight = np.ones(rows["frame"].shape, dtype=np.bool)
                 if options.highlight_start is not None:
                     highlight &= rows["frame"] >= options.highlight_start
                 if options.highlight_stop is not None:
                     highlight &= rows["frame"] <= options.highlight_stop
-                pd.point_data.scalars = highlight.astype(np.float)
+                pd.point_data.scalars = highlight.astype(np.float64)
             actors.append(a)
             actor2obj_id[a] = obj_id
 
             if verts_directions is not None and (
                 options.smooth_orientations or options.body_axis
             ):
                 smoothed_ori_verts = numpy.vstack(
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/lsprofcalltree.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/lsprofcalltree.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/misc.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/misc.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/montage_ufmfs.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/montage_ufmfs.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/orientation_ekf_fitter.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/orientation_ekf_fitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,17 +564,17 @@
                     save_cols["frame"] = []
                     for camn in camn_list:
                         save_cols["dist%d" % camn] = []
                         save_cols["used%d" % camn] = []
                         save_cols["theta%d" % camn] = []
 
                     # NxM array with rows being frames and cols being cameras
-                    slopes = np.ones((n_frames, n_cams), dtype=np.float)
-                    x0ds = np.ones((n_frames, n_cams), dtype=np.float)
-                    y0ds = np.ones((n_frames, n_cams), dtype=np.float)
+                    slopes = np.ones((n_frames, n_cams), dtype=np.float64)
+                    x0ds = np.ones((n_frames, n_cams), dtype=np.float64)
+                    y0ds = np.ones((n_frames, n_cams), dtype=np.float64)
                     for j, camn in enumerate(camn_list):
 
                         slopes_by_frame = slopes_by_camn_by_frame[camn]
                         x0d_by_frame = x0d_by_camn_by_frame[camn]
                         y0d_by_frame = y0d_by_camn_by_frame[camn]
 
                         for frame_idx, absolute_frame_number in enumerate(frame_range):
@@ -586,15 +586,15 @@
                                 absolute_frame_number, np.nan
                             )
                             y0ds[frame_idx, j] = y0d_by_frame.get(
                                 absolute_frame_number, np.nan
                             )
 
                         if options.show:
-                            frf = np.array(frame_range, dtype=np.float)
+                            frf = np.array(frame_range, dtype=np.float64)
                             min_frame_range = min(np.min(frf), min_frame_range)
                             max_frame_range = max(np.max(frf), max_frame_range)
 
                             ax1.plot(
                                 frame_range,
                                 slope2modpi(slopes[:, j]),
                                 ".",
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/orientation_ekf_plot.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/orientation_ekf_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                     camns.append(camn)
             for camn in camns:
                 label = camn2cam_id.get(camn, "camn%d" % camn)
                 theta = rows["theta%d" % camn]
                 used = rows["used%d" % camn]
                 dist = rows["dist%d" % camn]
 
-                frf = np.array(frame, dtype=np.float)
+                frf = np.array(frame, dtype=np.float64)
                 min_frame_range = min(np.min(frf), min_frame_range)
                 max_frame_range = max(np.max(frf), max_frame_range)
 
                 (line,) = ax1.plot(frame, theta * R2D, "o", mew=0, ms=2.0, label=label)
                 c = line.get_color()
                 ax2.plot(
                     frame[used], dist[used] * R2D, "o", color=c, mew=0, label=label
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/overlay_kalman_movie.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/overlay_kalman_movie.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_calibration_input.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_calibration_input.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_camera_positions.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_camera_positions.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_kalman_2d.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_kalman_2d.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_skipped_frames.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_skipped_frames.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_summary.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_summary.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_timeseries.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_timeseries.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_timeseries_2d_3d.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_timeseries_2d_3d.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/plot_top_view.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/plot_top_view.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/pos_ori2fu.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/pos_ori2fu.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/print_reprojection_error.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/print_reprojection_error.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/ransac.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/ransac.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/retrack_movies.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/retrack_movies.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/retrack_reuse_data_association.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/retrack_reuse_data_association.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/revert_schema12_to_schema11.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/revert_schema12_to_schema11.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/rosbag2flydrah5.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/rosbag2flydrah5.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/sample_calibration.xml` & `flydra_analysis-0.7.15/flydra_analysis/a2/sample_calibration.xml`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/sample_datafile-v0.4.28.h5` & `flydra_analysis-0.7.15/flydra_analysis/a2/sample_datafile-v0.4.28.h5`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/sample_datafile-v0.4.28.h5.retracked.h5` & `flydra_analysis-0.7.15/flydra_analysis/a2/sample_datafile-v0.4.28.h5.retracked.h5`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/sample_kalman_trajectories.h5` & `flydra_analysis-0.7.15/flydra_analysis/a2/sample_kalman_trajectories.h5`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/save_movies_overlay.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/save_movies_overlay.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/stim_plugins.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/stim_plugins.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/stimulus_positions.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/stimulus_positions.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/tables_tools.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/tables_tools.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/trajectory_filtering.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/trajectory_filtering.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/ufmf_tools.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/ufmf_tools.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/utils.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
     def get_idx_of_equal(self, testvals, missing_ok=False):
 
         # XXX should test dtype of testvals and self.values and call
         # appropriate helper function.
 
         return flydra_fastfinder_help.get_first_idx_double(
-            self.values.astype(np.float),
-            np.asanyarray(testvals).astype(np.float),
+            self.values.astype(np.float64),
+            np.asanyarray(testvals).astype(np.float64),
             missing_ok=missing_ok,
         )
 
     def get_idx_of_equal_slow(self, testvals):
         """performs fast search for vector
 
         Fails unless there is one and only one equal value in the
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/water_surface_align.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/water_surface_align.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     np_out = np.dot(m_np, point1)
     assert np.allclose(np_out, point1_out)
 
 
 class PlaneModelHelper:
     def fit(self, data):
         # http://stackoverflow.com/a/10904220/1633026
-        data = np.array(data, dtype=np.float)
+        data = np.array(data, dtype=np.float64)
         assert data.ndim == 2
         assert data.shape[1] == 3
         nrows = len(data)
         G = np.empty((nrows, 4))
         G[:, :3] = data
         G[:, 3] = 1.0
         u, d, vt = svd(G, full_matrices=True)
@@ -111,15 +111,15 @@
     x = np.concatenate(x)
     y = np.concatenate(y)
     z = np.concatenate(z)
 
     recon = Reconstructor(cal_source=data_file)
     extra["kresults"].close()  # close file
 
-    data = np.empty((len(x), 3), dtype=np.float)
+    data = np.empty((len(x), 3), dtype=np.float64)
     data[:, 0] = x
     data[:, 1] = y
     data[:, 2] = z
 
     # calculate plane-of-best fit ------------
 
     helper = PlaneModelHelper()
@@ -138,25 +138,25 @@
         k = 100
         t = np.mean([np.std(x), np.std(y), np.std(z)])
         d = 100
         plane_params = ransac.ransac(data, helper, n, k, t, d, debug=False)
 
     # Calculate rotation matrix from plane-of-best-fit to z==0 --------
     orig_normal = norm(plane_params[:3])
-    new_normal = np.array([0, 0, 1], dtype=np.float)
+    new_normal = np.array([0, 0, 1], dtype=np.float64)
     rot_axis = norm(np.cross(orig_normal, new_normal))
     cos_angle = np.dot(orig_normal, new_normal)
     angle = np.arccos(cos_angle)
     q = cgtypes.quat().fromAngleAxis(angle, rot_axis)
     m = q.toMat3()
     R = cgmat2np(m)
 
     # Calculate aligned data without translation -----------------
     s = 1.0
-    t = np.array([0, 0, 0], dtype=np.float)
+    t = np.array([0, 0, 0], dtype=np.float64)
 
     aligned_data = align.align_points(s, R, t, data.T).T
 
     # Calculate aligned data so that mean point is origin -----------------
     t = -np.mean(aligned_data[:, :3], axis=0)
     aligned_data = align.align_points(s, R, t, data.T).T
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/a2/xml_stimulus.py` & `flydra_analysis-0.7.15/flydra_analysis/a2/xml_stimulus.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/PQmath.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/PQmath.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/caching_movie_opener.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/caching_movie_opener.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/calc_forces.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/calc_forces.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/cam_params_play.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/cam_params_play.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/circstats.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/circstats.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_convert_to_mat.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_convert_to_mat.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_filter_kalman_data.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_filter_kalman_data.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_generate_recalibration.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_generate_recalibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,27 +310,27 @@
             [creconstructor.get_camera_center(cam_id)[:, 0] for cam_id in cam_ids]
         )
         flydra_core.reconstruct.save_ascii_matrix(
             cam_centers, os.path.join(calib_dir, "original_cam_centers.dat")
         )
 
     intrinsics_reconstructor = options.undistort_intrinsics_reconstructor
-    if intrinsics_reconstructor and os.path.exists(intrinsics_reconstructor):
+    if intrinsics_reconstructor:
         tdir = tempfile.mkdtemp()
         reconstructor = flydra_core.reconstruct.Reconstructor(
             cal_source=intrinsics_reconstructor
         )
         for i, cam_id in enumerate(cam_ids):
             fname = os.path.join(tdir, "%s.rad" % cam_id)
             scc = reconstructor.get_SingleCameraCalibration(cam_id)
             scc.helper.save_to_rad_file(fname)
             cam_calibrations.append(fname)
 
     intrinsics_yaml = options.undistort_intrinsics_yaml
-    if intrinsics_yaml and os.path.exists(intrinsics_yaml):
+    if intrinsics_yaml:
         for cam_id in cam_ids:
             fname = os.path.join(intrinsics_yaml, "%s.yaml" % cam_id)
             cam_calibrations.append(fname)
 
     undo_radial_distortion = len(cam_calibrations) == len(cam_ids)
 
     mcsc = MultiCamSelfCal(calib_dir)
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_plot_clock_drift.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_plot_clock_drift.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_plot_kalman_2d_histogram.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_plot_kalman_2d_histogram.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_analysis_print_camera_summary.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_analysis_print_camera_summary.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/flydra_convert_table_add_point_id.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/flydra_convert_table_add_point_id.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/hzgeom.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/hzgeom.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/pqmath_angular_velocity_quaternion_play.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/pqmath_angular_velocity_quaternion_play.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/reconstruct_orientation.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/reconstruct_orientation.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             # print 'line3d_by_frame[frame]',line3d_by_frame[frame]
 
             L = line3d_by_frame[frame]
             if L is None:
                 L = (nan, nan, nan, nan, nan, nan)
 
             fXl.append([frame] + list(X_by_frame[frame]) + list(L))
-        fXl = numpy.array(fXl, dtype=numpy.float)
+        fXl = numpy.array(fXl, dtype=numpy.float64)
         return fXl
     else:
         return line3d_by_frame
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/result_utils.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/result_utils.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/save_as_flydra_hdf5.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/save_as_flydra_hdf5.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/smdfile.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/smdfile.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/smooth_position_micro_demo.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/smooth_position_micro_demo.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/analysis/test_smooth_orientation.py` & `flydra_analysis-0.7.15/flydra_analysis/analysis/test_smooth_orientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     ObjectiveFunctionQuats,
     QuatSeq,
     orientation_to_quat,
     quat_to_orient,
     CachingObjectiveFunctionQuats,
     QuatSmoother,
 )
-import nose
 
 
 class TestPQmath:
     def setUp(self):
         D2R = np.pi / 180.0
 
         fps = 200.0
@@ -124,10 +123,7 @@
         Qsmooth_cache = QuatSmoother(frames_per_second=self.fps).smooth_quats(
             self.Q, objective_func_name="CachingObjectiveFunctionQuats",
         )
 
         for i, (qs, qc) in enumerate(zip(Qsmooth_slow, Qsmooth_cache)):
             assert qs == qc
 
-
-if __name__ == "__main__":
-    nose.main()
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/image_compare.py` & `flydra_analysis-0.7.15/flydra_analysis/image_compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     if im1.shape != im2.shape:
         raise ValueError("images have different shape")
     if np.allclose(im1, im2):
         # identical -- no more testing needed
         return True
 
     # maybe-3D absolute difference image
-    di = abs(im1.astype(np.float) - im2.astype(np.float))
+    di = abs(im1.astype(np.float64) - im2.astype(np.float64))
 
     # ensure 2D
     if di.ndim == 3:
         # flatten
         di2d = np.mean(di, axis=2)
     else:
         di2d = di
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/kalmanize.py` & `flydra_analysis-0.7.15/flydra_analysis/kalmanize.py`

 * *Files 1% similar despite different names*

```diff
@@ -886,15 +886,15 @@
 
         camn_order = np.array(camn_order)
         cam_id_array = np.array(cam_ids)
 
         N_cams = len(camn_order)
         N_frames = len(accum_frame_spread_fno)
 
-        all_timestamps = np.empty((N_frames, N_cams), dtype=np.float)
+        all_timestamps = np.empty((N_frames, N_cams), dtype=np.float64)
         all_timestamps.fill(np.nan)
         for i, (timestamps, camns) in enumerate(
             zip(accum_frame_all_timestamps, accum_frame_all_camns)
         ):
 
             for j, camn in enumerate(camn_order):
                 try:
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/mpl_markersize.py` & `flydra_analysis-0.7.15/flydra_analysis/mpl_markersize.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/offline_data_save.py` & `flydra_analysis-0.7.15/flydra_analysis/offline_data_save.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/talign.py` & `flydra_analysis-0.7.15/flydra_analysis/talign.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,33 +73,33 @@
         qy = cgtypes.quat().fromAngleAxis(self.r_y * D2R, cgtypes.vec3(0, 1, 0))
         qz = cgtypes.quat().fromAngleAxis(self.r_z * D2R, cgtypes.vec3(0, 0, 1))
         Rx = cgmat2np(qx.toMat3())
         Ry = cgmat2np(qy.toMat3())
         Rz = cgmat2np(qz.toMat3())
         R = np.dot(Rx, np.dot(Ry, Rz))
 
-        t = np.array([self.tx, self.ty, self.tz], np.float)
+        t = np.array([self.tx, self.ty, self.tz], np.float64)
         s = self.s
 
-        T = np.zeros((4, 4), dtype=np.float)
+        T = np.zeros((4, 4), dtype=np.float64)
         T[:3, :3] = s * R
         T[:3, 3] = t
         T[3, 3] = 1.0
 
         # convert bool to -1 or 1
         fx = fy = fz = 1
         if self.flip_x:
             fx = -1
         if self.flip_y:
             fy = -1
         if self.flip_z:
             fz = -1
 
         flip = np.array(
-            [[fx, 0, 0, 0], [0, fy, 0, 0], [0, 0, fz, 0], [0, 0, 0, 1]], dtype=np.float
+            [[fx, 0, 0, 0], [0, fy, 0, 0], [0, 0, fz, 0], [0, 0, 0, 1]], dtype=np.float64
         )
         T = np.dot(flip, T)
         # T = np.dot(T,flip)
         return T
 
     def as_dict(self):
         qx = cgtypes.quat().fromAngleAxis(self.r_x * D2R, cgtypes.vec3(1, 0, 0))
@@ -115,15 +115,15 @@
         if self.flip_x:
             fx = -1
         if self.flip_y:
             fy = -1
         if self.flip_z:
             fz = -1
 
-        flip = np.array([[fx, 0, 0], [0, fy, 0], [0, 0, fz]], dtype=np.float)
+        flip = np.array([[fx, 0, 0], [0, fy, 0], [0, 0, fz]], dtype=np.float64)
         _R = np.dot(flip, _R)
 
         s = float(self.s)
         t = map(float, [self.tx, self.ty, self.tz])
         R = []
         for row in _R:
             R.append(map(float, [i for i in row]))
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/test_commands.py` & `flydra_analysis-0.7.15/flydra_analysis/test_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from __future__ import print_function
 from __future__ import absolute_import
 import pkg_resources
 import os, subprocess, tempfile, shutil, sys, warnings
 import numpy as np
 import scipy.misc
 from optparse import OptionParser
-import nose
 from . import image_compare
-from nose.plugins.attrib import attr as nose_attr
+import pytest
 
 AUTOGEN_DIR = os.path.join(os.path.split(__file__)[0], "autogenerated")
 GALLERY_PATH = os.path.join(
     os.path.split(__file__)[0], "..", "flydra-sphinx-docs", "gallery.rst"
 )
 
 DATAFILE2D = pkg_resources.resource_filename(
@@ -192,26 +191,24 @@
 ===============
 
 %(command_gallery)s
 
 """
 
 
-@nose_attr("slow_command")
-@nose_attr("known_fail")
+@pytest.mark.skip
 def test_image_generating_commands():
     suffix = ""
     prefix = "flydra-test-"
     tmpdir = tempfile.mkdtemp(suffix, prefix)
     for info in image_info:
         yield check_command, "check", info, tmpdir
 
 
-@nose_attr("slow_command")
-@nose_attr("known_fail")
+@pytest.mark.skip
 def test_commands():
     suffix = ""
     prefix = "flydra-test-"
     tmpdir = tempfile.mkdtemp(suffix, prefix)
     for info in command_info:
         yield check_command, "check", info, tmpdir
 
@@ -459,12 +456,12 @@
 
     parser = OptionParser(usage)
     parser.add_option("--generate", action="store_true", default=False)
     (options, args) = parser.parse_args()
     if options.generate:
         generate()
     else:
-        nose.main()  # how to limit to just this module?
+        raise NotImplementedError
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `flydra_analysis-0.7.14/flydra_analysis/test_geom.py` & `flydra_analysis-0.7.15/flydra_analysis/test_geom.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis/test_reconstruction.py` & `flydra_analysis-0.7.15/flydra_analysis/test_reconstruction.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/flydra_analysis.egg-info/entry_points.txt` & `flydra_analysis-0.7.15/flydra_analysis.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,8 +50,7 @@
 [flydra_analysis.kdviewer.plugins]
 default = flydra_analysis.a2.conditions_draw:default
 hum07 = flydra_analysis.a2.conditions_draw:hum07
 mama07 = flydra_analysis.a2.conditions_draw:mama07
 mama20080414 = flydra_analysis.a2.conditions_draw:mama20080414
 mama20080501 = flydra_analysis.a2.conditions_draw:mama20080501
 wt0803 = flydra_analysis.a2.conditions_draw:wt0803
-
```

### Comparing `flydra_analysis-0.7.14/flydra_fastfinder_help.c` & `flydra_analysis-0.7.15/flydra_fastfinder_help.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,60 @@
-/* Generated by Cython 0.29.20 */
+/* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\Users\\drand\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python38\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\Users\\drand\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python38\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\Users\\drand\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python38\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\Users\\drand\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python38\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\Users\\drand\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python38\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "/private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "C:\\Users\\drand\\AppData\\Local\\Packages\\PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0\\LocalCache\\local-packages\\Python38\\site-packages\\numpy\\core\\include"
+            "/private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/core/include"
         ],
         "name": "flydra_fastfinder_help",
         "sources": [
             "flydra_fastfinder_help.pyx"
         ]
     },
     "module_name": "flydra_fastfinder_help"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_20"
-#define CYTHON_HEX_VERSION 0x001D14F0
-#define CYTHON_FUTURE_DIVISION 0
+#define CYTHON_ABI "3_0_0"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000F0
+#define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -51,30 +65,34 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -91,35 +109,167 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-#elif defined(PYSTON_VERSION)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #undef CYTHON_USE_ASYNC_SLOTS
+  #define CYTHON_USE_ASYNC_SLOTS 0
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
+  #endif
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
@@ -134,54 +284,55 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -191,35 +342,68 @@
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
-  #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -237,78 +421,128 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
   #elif defined(_MSC_VER)
@@ -316,93 +550,225 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return result;
+    }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -425,74 +791,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
+#else
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define CYTHON_PEP393_ENABLED 1
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #else
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
+  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -513,16 +971,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -533,46 +997,46 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
-#endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
@@ -584,16 +1048,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -608,35 +1074,44 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__flydra_fastfinder_help
 #define __PYX_HAVE_API__flydra_fastfinder_help
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
+
+    /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
+    
 #include "numpy/arrayobject.h"
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
-
-    /* NumPy API declarations from "numpy/__init__.pxd" */
-    
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -697,54 +1172,111 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -758,15 +1290,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -823,31 +1355,27 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif defined(_Complex_I)
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -857,22 +1385,23 @@
   #endif
 #endif
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "flydra_fastfinder_help.pyx",
-  "__init__.pxd",
+  "__init__.cython-30.pxd",
   "type.pxd",
 };
+/* #### Code section: utility_code_proto_before_types ### */
 /* BufferFormatStructs.proto */
-#define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
   struct __Pyx_StructField_* fields;
   size_t size;
   size_t arraysize[8];
@@ -899,355 +1428,506 @@
   int is_complex;
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
+/* #### Code section: numeric_typedefs ### */
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":690
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":691
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":692
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":693
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":697
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":698
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":699
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":700
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":704
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":705
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":714
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":715
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":716
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":718
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":719
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":720
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":722
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":723
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":725
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":726
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":727
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
+/* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
 #else
     typedef struct { float real, imag; } __pyx_t_float_complex;
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< double > __pyx_t_double_complex;
   #else
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":729
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":730
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":731
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":733
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* IsLittleEndian.proto */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
 
 /* BufferFormatCheck.proto */
@@ -1264,14 +1944,31 @@
 static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
     __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
 static void __Pyx_ZeroBuffer(Py_buffer* buf);
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1292,197 +1989,264 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* BufferFallbackError.proto */
 static void __Pyx_RaiseBufferFallbackError(void);
 
 #define __Pyx_BufPtrStrided1d(type, buf, i0, s0) (type)((char*)buf + i0 * s0)
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif
-
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+#endif
+#endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+/* TypeImport.proto */
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
+};
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+/* Import.proto */
+static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
+
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+/* ImportFrom.proto */
+static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
 
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
+
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+    PyCMethodObject func;
 #endif
-
-/* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
-};
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
 #endif
-
-/* Import.proto */
-static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
-
-/* ImportFrom.proto */
-static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* BufferStructDeclare.proto */
 typedef struct {
@@ -1503,19 +2267,18 @@
     static void __Pyx_ReleaseBuffer(Py_buffer *view);
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+/* GCCDiagnostics.proto */
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
@@ -1532,15 +2295,15 @@
     #define __Pyx_SET_CIMAG(z,y) ((z).imag(y))
 #else
     #define __Pyx_SET_CREAL(z,x) __Pyx_CREAL(z) = (x)
     #define __Pyx_SET_CIMAG(z,y) __Pyx_CIMAG(z) = (y)
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
     #define __Pyx_c_neg_float(a)     (-(a))
   #ifdef __cplusplus
@@ -1570,15 +2333,15 @@
     #if 1
         static CYTHON_INLINE float __Pyx_c_abs_float(__pyx_t_float_complex);
         static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_pow_float(__pyx_t_float_complex, __pyx_t_float_complex);
     #endif
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_double(a, b)   ((a)==(b))
     #define __Pyx_c_sum_double(a, b)  ((a)+(b))
     #define __Pyx_c_diff_double(a, b) ((a)-(b))
     #define __Pyx_c_prod_double(a, b) ((a)*(b))
     #define __Pyx_c_quot_double(a, b) ((a)/(b))
     #define __Pyx_c_neg_double(a)     (-(a))
   #ifdef __cplusplus
@@ -1610,1217 +2373,799 @@
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
 
-/* Module declarations from 'cpython.buffer' */
-
-/* Module declarations from 'libc.string' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from 'libc.stdio' */
+/* Module declarations from "libc.stdio" */
 
-/* Module declarations from '__builtin__' */
+/* Module declarations from "__builtin__" */
 
-/* Module declarations from 'cpython.type' */
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+/* Module declarations from "cpython.type" */
 
-/* Module declarations from 'cpython' */
+/* Module declarations from "cpython" */
 
-/* Module declarations from 'cpython.object' */
+/* Module declarations from "cpython.object" */
 
-/* Module declarations from 'cpython.ref' */
+/* Module declarations from "cpython.ref" */
 
-/* Module declarations from 'cpython.mem' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
-static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
-static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_generic = 0;
-static PyTypeObject *__pyx_ptype_5numpy_number = 0;
-static PyTypeObject *__pyx_ptype_5numpy_integer = 0;
-static PyTypeObject *__pyx_ptype_5numpy_signedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_unsignedinteger = 0;
-static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
-static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
-static PyTypeObject *__pyx_ptype_5numpy_character = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
+/* Module declarations from "cython" */
 
-/* Module declarations from 'cython' */
-
-/* Module declarations from 'flydra_fastfinder_help' */
-static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
+/* Module declarations from "flydra_fastfinder_help" */
+/* #### Code section: typeinfo ### */
+static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, __PYX_IS_UNSIGNED(long) ? 'U' : 'I', __PYX_IS_UNSIGNED(long), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "flydra_fastfinder_help"
 extern int __pyx_module_is_main_flydra_fastfinder_help;
 int __pyx_module_is_main_flydra_fastfinder_help = 0;
 
-/* Implementation of 'flydra_fastfinder_help' */
+/* Implementation of "flydra_fastfinder_help" */
+/* #### Code section: global_var ### */
+static PyObject *__pyx_builtin_AssertionError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ImportError;
+/* #### Code section: string_decls ### */
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_j[] = "j";
+static const char __pyx_k__3[] = "*";
+static const char __pyx_k__4[] = ".";
+static const char __pyx_k__8[] = "?";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_any[] = "any";
-static const char __pyx_k_int[] = "int";
 static const char __pyx_k_hmax[] = "hmax";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_nmax[] = "nmax";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_found[] = "found";
+static const char __pyx_k_int64[] = "int64";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_needles[] = "needles";
 static const char __pyx_k_haystack[] = "haystack";
 static const char __pyx_k_missing_ok[] = "missing_ok";
 static const char __pyx_k_ImportError[] = "ImportError";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_needle_found[] = "needle_found";
+static const char __pyx_k_AssertionError[] = "AssertionError";
 static const char __pyx_k_MissingValueError[] = "MissingValueError";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_get_first_idx_long[] = "get_first_idx_long";
 static const char __pyx_k_get_first_idx_double[] = "get_first_idx_double";
 static const char __pyx_k_flydra_fastfinder_help[] = "flydra_fastfinder_help";
 static const char __pyx_k_flydra_fastfinder_help_pyx[] = "flydra_fastfinder_help.pyx";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_flydra_analysis_a2_missing_value[] = "flydra_analysis.a2.missing_value_error";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_some_of_your_needles_were_not_fo[] = "some of your needles were not found";
-static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_n_s_MissingValueError;
-static PyObject *__pyx_n_s_any;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_flydra_analysis_a2_missing_value;
-static PyObject *__pyx_n_s_flydra_fastfinder_help;
-static PyObject *__pyx_kp_s_flydra_fastfinder_help_pyx;
-static PyObject *__pyx_n_s_found;
-static PyObject *__pyx_n_s_get_first_idx_double;
-static PyObject *__pyx_n_s_get_first_idx_long;
-static PyObject *__pyx_n_s_haystack;
-static PyObject *__pyx_n_s_hmax;
-static PyObject *__pyx_n_s_i;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_int;
-static PyObject *__pyx_n_s_j;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_missing_ok;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_needle_found;
-static PyObject *__pyx_n_s_needles;
-static PyObject *__pyx_n_s_nmax;
-static PyObject *__pyx_n_s_np;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
-static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_kp_s_some_of_your_needles_were_not_fo;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_zeros;
+/* #### Code section: decls ### */
 static PyObject *__pyx_pf_22flydra_fastfinder_help_get_first_idx_long(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_haystack, PyArrayObject *__pyx_v_needles, int __pyx_v_missing_ok); /* proto */
 static PyObject *__pyx_pf_22flydra_fastfinder_help_2get_first_idx_double(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_haystack, PyArrayObject *__pyx_v_needles, int __pyx_v_missing_ok); /* proto */
-static PyObject *__pyx_int_neg_1;
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__5;
-static PyObject *__pyx_codeobj__4;
-static PyObject *__pyx_codeobj__6;
-/* Late includes */
-
-/* "flydra_fastfinder_help.pyx":10
- * 
- * @cython.boundscheck(False) # turn of bounds-checking for entire function
- * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
- * 
- *     # TODO: implementation that does binary search on pre-sorted
- */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_5numpy_dtype;
+  PyTypeObject *__pyx_ptype_5numpy_flatiter;
+  PyTypeObject *__pyx_ptype_5numpy_broadcast;
+  PyTypeObject *__pyx_ptype_5numpy_ndarray;
+  PyTypeObject *__pyx_ptype_5numpy_generic;
+  PyTypeObject *__pyx_ptype_5numpy_number;
+  PyTypeObject *__pyx_ptype_5numpy_integer;
+  PyTypeObject *__pyx_ptype_5numpy_signedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_unsignedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_inexact;
+  PyTypeObject *__pyx_ptype_5numpy_floating;
+  PyTypeObject *__pyx_ptype_5numpy_complexfloating;
+  PyTypeObject *__pyx_ptype_5numpy_flexible;
+  PyTypeObject *__pyx_ptype_5numpy_character;
+  PyTypeObject *__pyx_ptype_5numpy_ufunc;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyObject *__pyx_n_s_AssertionError;
+  PyObject *__pyx_n_s_ImportError;
+  PyObject *__pyx_n_s_MissingValueError;
+  PyObject *__pyx_n_s__3;
+  PyObject *__pyx_kp_u__4;
+  PyObject *__pyx_n_s__8;
+  PyObject *__pyx_n_s_any;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_dtype;
+  PyObject *__pyx_n_s_flydra_analysis_a2_missing_value;
+  PyObject *__pyx_n_s_flydra_fastfinder_help;
+  PyObject *__pyx_kp_s_flydra_fastfinder_help_pyx;
+  PyObject *__pyx_n_s_found;
+  PyObject *__pyx_n_s_get_first_idx_double;
+  PyObject *__pyx_n_s_get_first_idx_long;
+  PyObject *__pyx_n_s_haystack;
+  PyObject *__pyx_n_s_hmax;
+  PyObject *__pyx_n_s_i;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_int64;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_n_s_j;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_missing_ok;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_needle_found;
+  PyObject *__pyx_n_s_needles;
+  PyObject *__pyx_n_s_nmax;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
+  PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_n_s_range;
+  PyObject *__pyx_kp_s_some_of_your_needles_were_not_fo;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_zeros;
+  PyObject *__pyx_int_neg_1;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_codeobj__6;
+  PyObject *__pyx_codeobj__7;
+} __pyx_mstate;
 
-/* Python wrapper */
-static PyObject *__pyx_pw_22flydra_fastfinder_help_1get_first_idx_long(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_22flydra_fastfinder_help_1get_first_idx_long = {"get_first_idx_long", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22flydra_fastfinder_help_1get_first_idx_long, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_22flydra_fastfinder_help_1get_first_idx_long(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyArrayObject *__pyx_v_haystack = 0;
-  PyArrayObject *__pyx_v_needles = 0;
-  int __pyx_v_missing_ok;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("get_first_idx_long (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_haystack,&__pyx_n_s_needles,&__pyx_n_s_missing_ok,0};
-    PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_haystack)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_needles)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("get_first_idx_long", 0, 2, 3, 1); __PYX_ERR(0, 10, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_missing_ok);
-          if (value) { values[2] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_first_idx_long") < 0)) __PYX_ERR(0, 10, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_haystack = ((PyArrayObject *)values[0]);
-    __pyx_v_needles = ((PyArrayObject *)values[1]);
-    if (values[2]) {
-      __pyx_v_missing_ok = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_missing_ok == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
-    } else {
-      __pyx_v_missing_ok = ((int)0);
-    }
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_first_idx_long", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 10, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_long", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_haystack), __pyx_ptype_5numpy_ndarray, 1, "haystack", 0))) __PYX_ERR(0, 10, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_needles), __pyx_ptype_5numpy_ndarray, 1, "needles", 0))) __PYX_ERR(0, 10, __pyx_L1_error)
-  __pyx_r = __pyx_pf_22flydra_fastfinder_help_get_first_idx_long(__pyx_self, __pyx_v_haystack, __pyx_v_needles, __pyx_v_missing_ok);
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
 
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
 
-static PyObject *__pyx_pf_22flydra_fastfinder_help_get_first_idx_long(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_haystack, PyArrayObject *__pyx_v_needles, int __pyx_v_missing_ok) {
-  long __pyx_v_hmax;
-  long __pyx_v_nmax;
-  long __pyx_v_i;
-  long __pyx_v_j;
-  int __pyx_v_needle_found;
-  PyArrayObject *__pyx_v_found = 0;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_found;
-  __Pyx_Buffer __pyx_pybuffer_found;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_haystack;
-  __Pyx_Buffer __pyx_pybuffer_haystack;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_needles;
-  __Pyx_Buffer __pyx_pybuffer_needles;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyArrayObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  long __pyx_t_11;
-  long __pyx_t_12;
-  long __pyx_t_13;
-  long __pyx_t_14;
-  long __pyx_t_15;
-  long __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  Py_ssize_t __pyx_t_18;
-  int __pyx_t_19;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_first_idx_long", 0);
-  __pyx_pybuffer_found.pybuffer.buf = NULL;
-  __pyx_pybuffer_found.refcount = 0;
-  __pyx_pybuffernd_found.data = NULL;
-  __pyx_pybuffernd_found.rcbuffer = &__pyx_pybuffer_found;
-  __pyx_pybuffer_haystack.pybuffer.buf = NULL;
-  __pyx_pybuffer_haystack.refcount = 0;
-  __pyx_pybuffernd_haystack.data = NULL;
-  __pyx_pybuffernd_haystack.rcbuffer = &__pyx_pybuffer_haystack;
-  __pyx_pybuffer_needles.pybuffer.buf = NULL;
-  __pyx_pybuffer_needles.refcount = 0;
-  __pyx_pybuffernd_needles.data = NULL;
-  __pyx_pybuffernd_needles.rcbuffer = &__pyx_pybuffer_needles;
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer, (PyObject*)__pyx_v_haystack, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 10, __pyx_L1_error)
-  }
-  __pyx_pybuffernd_haystack.diminfo[0].strides = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_haystack.diminfo[0].shape = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.shape[0];
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_needles.rcbuffer->pybuffer, (PyObject*)__pyx_v_needles, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 10, __pyx_L1_error)
-  }
-  __pyx_pybuffernd_needles.diminfo[0].strides = __pyx_pybuffernd_needles.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_needles.diminfo[0].shape = __pyx_pybuffernd_needles.rcbuffer->pybuffer.shape[0];
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
 
-  /* "flydra_fastfinder_help.pyx":15
- *     # haystack
- * 
- *     assert haystack.ndim==1             # <<<<<<<<<<<<<<
- *     assert needles.ndim==1
- * 
- */
-  #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
-    if (unlikely(!((__pyx_v_haystack->nd == 1) != 0))) {
-      PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 15, __pyx_L1_error)
-    }
-  }
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
-
-  /* "flydra_fastfinder_help.pyx":16
- * 
- *     assert haystack.ndim==1
- *     assert needles.ndim==1             # <<<<<<<<<<<<<<
- * 
- *     cdef long hmax = haystack.shape[0]
- */
-  #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
-    if (unlikely(!((__pyx_v_needles->nd == 1) != 0))) {
-      PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 16, __pyx_L1_error)
-    }
-  }
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
-
-  /* "flydra_fastfinder_help.pyx":18
- *     assert needles.ndim==1
- * 
- *     cdef long hmax = haystack.shape[0]             # <<<<<<<<<<<<<<
- *     cdef long nmax = needles.shape[0]
- *     cdef long i,j
- */
-  __pyx_v_hmax = (__pyx_v_haystack->dimensions[0]);
-
-  /* "flydra_fastfinder_help.pyx":19
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_dtype);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_generic);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_number);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_integer);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_inexact);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_floating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flexible);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_character);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_AssertionError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MissingValueError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__4);
+  Py_CLEAR(clear_module_state->__pyx_n_s__8);
+  Py_CLEAR(clear_module_state->__pyx_n_s_any);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
+  Py_CLEAR(clear_module_state->__pyx_n_s_flydra_analysis_a2_missing_value);
+  Py_CLEAR(clear_module_state->__pyx_n_s_flydra_fastfinder_help);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_flydra_fastfinder_help_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_found);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_first_idx_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_first_idx_long);
+  Py_CLEAR(clear_module_state->__pyx_n_s_haystack);
+  Py_CLEAR(clear_module_state->__pyx_n_s_hmax);
+  Py_CLEAR(clear_module_state->__pyx_n_s_i);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_int64);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_n_s_j);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_missing_ok);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_needle_found);
+  Py_CLEAR(clear_module_state->__pyx_n_s_needles);
+  Py_CLEAR(clear_module_state->__pyx_n_s_nmax);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_numpy_core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_some_of_your_needles_were_not_fo);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_zeros);
+  Py_CLEAR(clear_module_state->__pyx_int_neg_1);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_dtype);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_generic);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_number);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_integer);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_inexact);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_floating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flexible);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_character);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_AssertionError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MissingValueError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__4);
+  Py_VISIT(traverse_module_state->__pyx_n_s__8);
+  Py_VISIT(traverse_module_state->__pyx_n_s_any);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
+  Py_VISIT(traverse_module_state->__pyx_n_s_flydra_analysis_a2_missing_value);
+  Py_VISIT(traverse_module_state->__pyx_n_s_flydra_fastfinder_help);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_flydra_fastfinder_help_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_found);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_first_idx_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_first_idx_long);
+  Py_VISIT(traverse_module_state->__pyx_n_s_haystack);
+  Py_VISIT(traverse_module_state->__pyx_n_s_hmax);
+  Py_VISIT(traverse_module_state->__pyx_n_s_i);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_int64);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_n_s_j);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_missing_ok);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_needle_found);
+  Py_VISIT(traverse_module_state->__pyx_n_s_needles);
+  Py_VISIT(traverse_module_state->__pyx_n_s_nmax);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_numpy_core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_some_of_your_needles_were_not_fo);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_zeros);
+  Py_VISIT(traverse_module_state->__pyx_int_neg_1);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_5numpy_dtype __pyx_mstate_global->__pyx_ptype_5numpy_dtype
+#define __pyx_ptype_5numpy_flatiter __pyx_mstate_global->__pyx_ptype_5numpy_flatiter
+#define __pyx_ptype_5numpy_broadcast __pyx_mstate_global->__pyx_ptype_5numpy_broadcast
+#define __pyx_ptype_5numpy_ndarray __pyx_mstate_global->__pyx_ptype_5numpy_ndarray
+#define __pyx_ptype_5numpy_generic __pyx_mstate_global->__pyx_ptype_5numpy_generic
+#define __pyx_ptype_5numpy_number __pyx_mstate_global->__pyx_ptype_5numpy_number
+#define __pyx_ptype_5numpy_integer __pyx_mstate_global->__pyx_ptype_5numpy_integer
+#define __pyx_ptype_5numpy_signedinteger __pyx_mstate_global->__pyx_ptype_5numpy_signedinteger
+#define __pyx_ptype_5numpy_unsignedinteger __pyx_mstate_global->__pyx_ptype_5numpy_unsignedinteger
+#define __pyx_ptype_5numpy_inexact __pyx_mstate_global->__pyx_ptype_5numpy_inexact
+#define __pyx_ptype_5numpy_floating __pyx_mstate_global->__pyx_ptype_5numpy_floating
+#define __pyx_ptype_5numpy_complexfloating __pyx_mstate_global->__pyx_ptype_5numpy_complexfloating
+#define __pyx_ptype_5numpy_flexible __pyx_mstate_global->__pyx_ptype_5numpy_flexible
+#define __pyx_ptype_5numpy_character __pyx_mstate_global->__pyx_ptype_5numpy_character
+#define __pyx_ptype_5numpy_ufunc __pyx_mstate_global->__pyx_ptype_5numpy_ufunc
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_n_s_AssertionError __pyx_mstate_global->__pyx_n_s_AssertionError
+#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
+#define __pyx_n_s_MissingValueError __pyx_mstate_global->__pyx_n_s_MissingValueError
+#define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
+#define __pyx_n_s__8 __pyx_mstate_global->__pyx_n_s__8
+#define __pyx_n_s_any __pyx_mstate_global->__pyx_n_s_any
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
+#define __pyx_n_s_flydra_analysis_a2_missing_value __pyx_mstate_global->__pyx_n_s_flydra_analysis_a2_missing_value
+#define __pyx_n_s_flydra_fastfinder_help __pyx_mstate_global->__pyx_n_s_flydra_fastfinder_help
+#define __pyx_kp_s_flydra_fastfinder_help_pyx __pyx_mstate_global->__pyx_kp_s_flydra_fastfinder_help_pyx
+#define __pyx_n_s_found __pyx_mstate_global->__pyx_n_s_found
+#define __pyx_n_s_get_first_idx_double __pyx_mstate_global->__pyx_n_s_get_first_idx_double
+#define __pyx_n_s_get_first_idx_long __pyx_mstate_global->__pyx_n_s_get_first_idx_long
+#define __pyx_n_s_haystack __pyx_mstate_global->__pyx_n_s_haystack
+#define __pyx_n_s_hmax __pyx_mstate_global->__pyx_n_s_hmax
+#define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_int64 __pyx_mstate_global->__pyx_n_s_int64
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_n_s_j __pyx_mstate_global->__pyx_n_s_j
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_missing_ok __pyx_mstate_global->__pyx_n_s_missing_ok
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_needle_found __pyx_mstate_global->__pyx_n_s_needle_found
+#define __pyx_n_s_needles __pyx_mstate_global->__pyx_n_s_needles
+#define __pyx_n_s_nmax __pyx_mstate_global->__pyx_n_s_nmax
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_kp_s_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_s_numpy_core_multiarray_failed_to
+#define __pyx_kp_s_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_s_numpy_core_umath_failed_to_impor
+#define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_kp_s_some_of_your_needles_were_not_fo __pyx_mstate_global->__pyx_kp_s_some_of_your_needles_were_not_fo
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_zeros __pyx_mstate_global->__pyx_n_s_zeros
+#define __pyx_int_neg_1 __pyx_mstate_global->__pyx_int_neg_1
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
+#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
+/* #### Code section: module_code ### */
+
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":245
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
+  PyObject *__pyx_r;
+
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":248
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
- *     cdef long hmax = haystack.shape[0]
- *     cdef long nmax = needles.shape[0]             # <<<<<<<<<<<<<<
- *     cdef long i,j
- *     cdef int needle_found
+ *         @property
  */
-  __pyx_v_nmax = (__pyx_v_needles->dimensions[0]);
+  __pyx_r = PyArray_BASE(__pyx_v_self);
+  goto __pyx_L0;
 
-  /* "flydra_fastfinder_help.pyx":24
- *     cdef np.ndarray[long, ndim=1] found
- * 
- *     found = np.zeros( (needles.shape[0],) , dtype=np.int)             # <<<<<<<<<<<<<<
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":245
  * 
- *     for i in range(nmax):
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_needles->dimensions[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 24, __pyx_L1_error)
-  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
-    __pyx_t_7 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
-    if (unlikely(__pyx_t_7 < 0)) {
-      PyErr_Fetch(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
-      if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_v_found, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
-        Py_XDECREF(__pyx_t_8); Py_XDECREF(__pyx_t_9); Py_XDECREF(__pyx_t_10);
-        __Pyx_RaiseBufferFallbackError();
-      } else {
-        PyErr_Restore(__pyx_t_8, __pyx_t_9, __pyx_t_10);
-      }
-      __pyx_t_8 = __pyx_t_9 = __pyx_t_10 = 0;
-    }
-    __pyx_pybuffernd_found.diminfo[0].strides = __pyx_pybuffernd_found.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_found.diminfo[0].shape = __pyx_pybuffernd_found.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 24, __pyx_L1_error)
-  }
-  __pyx_t_6 = 0;
-  __pyx_v_found = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
 
-  /* "flydra_fastfinder_help.pyx":26
- *     found = np.zeros( (needles.shape[0],) , dtype=np.int)
- * 
- *     for i in range(nmax):             # <<<<<<<<<<<<<<
- *         needle_found = 0
- *         for j in range(hmax):
- */
-  __pyx_t_11 = __pyx_v_nmax;
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
-    __pyx_v_i = __pyx_t_13;
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
 
-    /* "flydra_fastfinder_help.pyx":27
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":251
  * 
- *     for i in range(nmax):
- *         needle_found = 0             # <<<<<<<<<<<<<<
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:
- */
-    __pyx_v_needle_found = 0;
-
-    /* "flydra_fastfinder_help.pyx":28
- *     for i in range(nmax):
- *         needle_found = 0
- *         for j in range(hmax):             # <<<<<<<<<<<<<<
- *             if haystack[j]==needles[i]:
- *                 needle_found=1
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
  */
-    __pyx_t_14 = __pyx_v_hmax;
-    __pyx_t_15 = __pyx_t_14;
-    for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
-      __pyx_v_j = __pyx_t_16;
 
-      /* "flydra_fastfinder_help.pyx":29
- *         needle_found = 0
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
- *                 needle_found=1
- *                 break
- */
-      __pyx_t_17 = __pyx_v_j;
-      if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_haystack.diminfo[0].shape;
-      __pyx_t_18 = __pyx_v_i;
-      if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_needles.diminfo[0].shape;
-      __pyx_t_19 = (((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_haystack.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_haystack.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_needles.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_needles.diminfo[0].strides))) != 0);
-      if (__pyx_t_19) {
-
-        /* "flydra_fastfinder_help.pyx":30
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:
- *                 needle_found=1             # <<<<<<<<<<<<<<
- *                 break
- *         if needle_found:
- */
-        __pyx_v_needle_found = 1;
-
-        /* "flydra_fastfinder_help.pyx":31
- *             if haystack[j]==needles[i]:
- *                 needle_found=1
- *                 break             # <<<<<<<<<<<<<<
- *         if needle_found:
- *             found[i] = j
- */
-        goto __pyx_L6_break;
-
-        /* "flydra_fastfinder_help.pyx":29
- *         needle_found = 0
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
- *                 needle_found=1
- *                 break
- */
-      }
-    }
-    __pyx_L6_break:;
-
-    /* "flydra_fastfinder_help.pyx":32
- *                 needle_found=1
- *                 break
- *         if needle_found:             # <<<<<<<<<<<<<<
- *             found[i] = j
- *         else:
- */
-    __pyx_t_19 = (__pyx_v_needle_found != 0);
-    if (__pyx_t_19) {
-
-      /* "flydra_fastfinder_help.pyx":33
- *                 break
- *         if needle_found:
- *             found[i] = j             # <<<<<<<<<<<<<<
- *         else:
- *             found[i] = -1
- */
-      __pyx_t_18 = __pyx_v_i;
-      if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_found.diminfo[0].shape;
-      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_found.diminfo[0].strides) = __pyx_v_j;
-
-      /* "flydra_fastfinder_help.pyx":32
- *                 needle_found=1
- *                 break
- *         if needle_found:             # <<<<<<<<<<<<<<
- *             found[i] = j
- *         else:
- */
-      goto __pyx_L8;
-    }
-
-    /* "flydra_fastfinder_help.pyx":35
- *             found[i] = j
- *         else:
- *             found[i] = -1             # <<<<<<<<<<<<<<
- * 
- *     if not missing_ok:
- */
-    /*else*/ {
-      __pyx_t_17 = __pyx_v_i;
-      if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_found.diminfo[0].shape;
-      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_found.diminfo[0].strides) = -1L;
-    }
-    __pyx_L8:;
-  }
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
+  PyArray_Descr *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyArray_Descr *__pyx_t_1;
+  __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "flydra_fastfinder_help.pyx":37
- *             found[i] = -1
- * 
- *     if not missing_ok:             # <<<<<<<<<<<<<<
- *         if np.any(found==-1):
- *             raise MissingValueError('some of your needles were not found')
- */
-  __pyx_t_19 = ((!(__pyx_v_missing_ok != 0)) != 0);
-  if (__pyx_t_19) {
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":254
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
+  __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
+  __pyx_r = ((PyArray_Descr *)__pyx_t_1);
+  goto __pyx_L0;
 
-    /* "flydra_fastfinder_help.pyx":38
- * 
- *     if not missing_ok:
- *         if np.any(found==-1):             # <<<<<<<<<<<<<<
- *             raise MissingValueError('some of your needles were not found')
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":251
  * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_any); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyObject_RichCompare(((PyObject *)__pyx_v_found), __pyx_int_neg_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 38, __pyx_L1_error)
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_2);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_19 < 0)) __PYX_ERR(0, 38, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(__pyx_t_19)) {
 
-      /* "flydra_fastfinder_help.pyx":39
- *     if not missing_ok:
- *         if np.any(found==-1):
- *             raise MissingValueError('some of your needles were not found')             # <<<<<<<<<<<<<<
- * 
- *     return found
- */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MissingValueError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-        if (likely(__pyx_t_3)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-          __Pyx_INCREF(__pyx_t_3);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_1, function);
-        }
-      }
-      __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_some_of_your_needles_were_not_fo) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_some_of_your_needles_were_not_fo);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 39, __pyx_L1_error)
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
 
-      /* "flydra_fastfinder_help.pyx":38
- * 
- *     if not missing_ok:
- *         if np.any(found==-1):             # <<<<<<<<<<<<<<
- *             raise MissingValueError('some of your needles were not found')
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":257
  * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
  */
-    }
 
-    /* "flydra_fastfinder_help.pyx":37
- *             found[i] = -1
- * 
- *     if not missing_ok:             # <<<<<<<<<<<<<<
- *         if np.any(found==-1):
- *             raise MissingValueError('some of your needles were not found')
- */
-  }
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
+  int __pyx_r;
 
-  /* "flydra_fastfinder_help.pyx":41
- *             raise MissingValueError('some of your needles were not found')
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":260
+ *             """Returns the number of dimensions in the array.
+ *             """
+ *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
- *     return found             # <<<<<<<<<<<<<<
- * 
- * @cython.boundscheck(False) # turn of bounds-checking for entire function
+ *         @property
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_found));
-  __pyx_r = ((PyObject *)__pyx_v_found);
+  __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "flydra_fastfinder_help.pyx":10
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":257
  * 
- * @cython.boundscheck(False) # turn of bounds-checking for entire function
- * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
- * 
- *     # TODO: implementation that does binary search on pre-sorted
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
  */
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
-  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_long", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  goto __pyx_L2;
   __pyx_L0:;
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_found);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "flydra_fastfinder_help.pyx":44
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":263
  * 
- * @cython.boundscheck(False) # turn of bounds-checking for entire function
- * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
- * 
- *     # TODO: implementation that does binary search on pre-sorted
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_22flydra_fastfinder_help_3get_first_idx_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_22flydra_fastfinder_help_3get_first_idx_double = {"get_first_idx_double", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22flydra_fastfinder_help_3get_first_idx_double, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_22flydra_fastfinder_help_3get_first_idx_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  PyArrayObject *__pyx_v_haystack = 0;
-  PyArrayObject *__pyx_v_needles = 0;
-  int __pyx_v_missing_ok;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("get_first_idx_double (wrapper)", 0);
-  {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_haystack,&__pyx_n_s_needles,&__pyx_n_s_missing_ok,0};
-    PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
-      Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
-        case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_haystack)) != 0)) kw_args--;
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_needles)) != 0)) kw_args--;
-        else {
-          __Pyx_RaiseArgtupleInvalid("get_first_idx_double", 0, 2, 3, 1); __PYX_ERR(0, 44, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_missing_ok);
-          if (value) { values[2] = value; kw_args--; }
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_first_idx_double") < 0)) __PYX_ERR(0, 44, __pyx_L3_error)
-      }
-    } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-        break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-    }
-    __pyx_v_haystack = ((PyArrayObject *)values[0]);
-    __pyx_v_needles = ((PyArrayObject *)values[1]);
-    if (values[2]) {
-      __pyx_v_missing_ok = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_missing_ok == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
-    } else {
-      __pyx_v_missing_ok = ((int)0);
-    }
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_first_idx_double", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 44, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_haystack), __pyx_ptype_5numpy_ndarray, 1, "haystack", 0))) __PYX_ERR(0, 44, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_needles), __pyx_ptype_5numpy_ndarray, 1, "needles", 0))) __PYX_ERR(0, 44, __pyx_L1_error)
-  __pyx_r = __pyx_pf_22flydra_fastfinder_help_2get_first_idx_double(__pyx_self, __pyx_v_haystack, __pyx_v_needles, __pyx_v_missing_ok);
-
-  /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_22flydra_fastfinder_help_2get_first_idx_double(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_haystack, PyArrayObject *__pyx_v_needles, int __pyx_v_missing_ok) {
-  long __pyx_v_hmax;
-  long __pyx_v_nmax;
-  long __pyx_v_i;
-  long __pyx_v_j;
-  int __pyx_v_needle_found;
-  PyArrayObject *__pyx_v_found = 0;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_found;
-  __Pyx_Buffer __pyx_pybuffer_found;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_haystack;
-  __Pyx_Buffer __pyx_pybuffer_haystack;
-  __Pyx_LocalBuf_ND __pyx_pybuffernd_needles;
-  __Pyx_Buffer __pyx_pybuffer_needles;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  PyArrayObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  PyObject *__pyx_t_10 = NULL;
-  long __pyx_t_11;
-  long __pyx_t_12;
-  long __pyx_t_13;
-  long __pyx_t_14;
-  long __pyx_t_15;
-  long __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  Py_ssize_t __pyx_t_18;
-  int __pyx_t_19;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_first_idx_double", 0);
-  __pyx_pybuffer_found.pybuffer.buf = NULL;
-  __pyx_pybuffer_found.refcount = 0;
-  __pyx_pybuffernd_found.data = NULL;
-  __pyx_pybuffernd_found.rcbuffer = &__pyx_pybuffer_found;
-  __pyx_pybuffer_haystack.pybuffer.buf = NULL;
-  __pyx_pybuffer_haystack.refcount = 0;
-  __pyx_pybuffernd_haystack.data = NULL;
-  __pyx_pybuffernd_haystack.rcbuffer = &__pyx_pybuffer_haystack;
-  __pyx_pybuffer_needles.pybuffer.buf = NULL;
-  __pyx_pybuffer_needles.refcount = 0;
-  __pyx_pybuffernd_needles.data = NULL;
-  __pyx_pybuffernd_needles.rcbuffer = &__pyx_pybuffer_needles;
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer, (PyObject*)__pyx_v_haystack, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 44, __pyx_L1_error)
-  }
-  __pyx_pybuffernd_haystack.diminfo[0].strides = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_haystack.diminfo[0].shape = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.shape[0];
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_needles.rcbuffer->pybuffer, (PyObject*)__pyx_v_needles, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 44, __pyx_L1_error)
-  }
-  __pyx_pybuffernd_needles.diminfo[0].strides = __pyx_pybuffernd_needles.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_needles.diminfo[0].shape = __pyx_pybuffernd_needles.rcbuffer->pybuffer.shape[0];
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
 
-  /* "flydra_fastfinder_help.pyx":49
- *     # haystack
- * 
- *     assert haystack.ndim==1             # <<<<<<<<<<<<<<
- *     assert needles.ndim==1
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":268
+ *             Can return NULL for 0-dimensional arrays.
+ *             """
+ *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
+ *         @property
  */
-  #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
-    if (unlikely(!((__pyx_v_haystack->nd == 1) != 0))) {
-      PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 49, __pyx_L1_error)
-    }
-  }
-  #endif
+  __pyx_r = PyArray_DIMS(__pyx_v_self);
+  goto __pyx_L0;
 
-  /* "flydra_fastfinder_help.pyx":50
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":263
  * 
- *     assert haystack.ndim==1
- *     assert needles.ndim==1             # <<<<<<<<<<<<<<
- * 
- *     cdef long hmax = haystack.shape[0]
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
  */
-  #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
-    if (unlikely(!((__pyx_v_needles->nd == 1) != 0))) {
-      PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(0, 50, __pyx_L1_error)
-    }
-  }
-  #endif
 
-  /* "flydra_fastfinder_help.pyx":52
- *     assert needles.ndim==1
- * 
- *     cdef long hmax = haystack.shape[0]             # <<<<<<<<<<<<<<
- *     cdef long nmax = needles.shape[0]
- *     cdef long i,j
- */
-  __pyx_v_hmax = (__pyx_v_haystack->dimensions[0]);
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
 
-  /* "flydra_fastfinder_help.pyx":53
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":271
  * 
- *     cdef long hmax = haystack.shape[0]
- *     cdef long nmax = needles.shape[0]             # <<<<<<<<<<<<<<
- *     cdef long i,j
- *     cdef int needle_found
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
  */
-  __pyx_v_nmax = (__pyx_v_needles->dimensions[0]);
 
-  /* "flydra_fastfinder_help.pyx":58
- *     cdef np.ndarray[long, ndim=1] found
- * 
- *     found = np.zeros( (needles.shape[0],) , dtype=np.int)             # <<<<<<<<<<<<<<
- * 
- *     for i in range(nmax):
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_needles->dimensions[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
-  __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 58, __pyx_L1_error)
-  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
-  {
-    __Pyx_BufFmt_StackElem __pyx_stack[1];
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
-    __pyx_t_7 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
-    if (unlikely(__pyx_t_7 < 0)) {
-      PyErr_Fetch(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
-      if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_v_found, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
-        Py_XDECREF(__pyx_t_8); Py_XDECREF(__pyx_t_9); Py_XDECREF(__pyx_t_10);
-        __Pyx_RaiseBufferFallbackError();
-      } else {
-        PyErr_Restore(__pyx_t_8, __pyx_t_9, __pyx_t_10);
-      }
-      __pyx_t_8 = __pyx_t_9 = __pyx_t_10 = 0;
-    }
-    __pyx_pybuffernd_found.diminfo[0].strides = __pyx_pybuffernd_found.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_found.diminfo[0].shape = __pyx_pybuffernd_found.rcbuffer->pybuffer.shape[0];
-    if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
-  }
-  __pyx_t_6 = 0;
-  __pyx_v_found = ((PyArrayObject *)__pyx_t_5);
-  __pyx_t_5 = 0;
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
 
-  /* "flydra_fastfinder_help.pyx":60
- *     found = np.zeros( (needles.shape[0],) , dtype=np.int)
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":275
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ *             """
+ *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
- *     for i in range(nmax):             # <<<<<<<<<<<<<<
- *         needle_found = 0
- *         for j in range(hmax):
+ *         @property
  */
-  __pyx_t_11 = __pyx_v_nmax;
-  __pyx_t_12 = __pyx_t_11;
-  for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
-    __pyx_v_i = __pyx_t_13;
+  __pyx_r = PyArray_STRIDES(__pyx_v_self);
+  goto __pyx_L0;
 
-    /* "flydra_fastfinder_help.pyx":61
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":271
  * 
- *     for i in range(nmax):
- *         needle_found = 0             # <<<<<<<<<<<<<<
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:
- */
-    __pyx_v_needle_found = 0;
-
-    /* "flydra_fastfinder_help.pyx":62
- *     for i in range(nmax):
- *         needle_found = 0
- *         for j in range(hmax):             # <<<<<<<<<<<<<<
- *             if haystack[j]==needles[i]:
- *                 needle_found=1
- */
-    __pyx_t_14 = __pyx_v_hmax;
-    __pyx_t_15 = __pyx_t_14;
-    for (__pyx_t_16 = 0; __pyx_t_16 < __pyx_t_15; __pyx_t_16+=1) {
-      __pyx_v_j = __pyx_t_16;
-
-      /* "flydra_fastfinder_help.pyx":63
- *         needle_found = 0
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
- *                 needle_found=1
- *                 break
- */
-      __pyx_t_17 = __pyx_v_j;
-      if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_haystack.diminfo[0].shape;
-      __pyx_t_18 = __pyx_v_i;
-      if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_needles.diminfo[0].shape;
-      __pyx_t_19 = (((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_haystack.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_haystack.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_needles.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_needles.diminfo[0].strides))) != 0);
-      if (__pyx_t_19) {
-
-        /* "flydra_fastfinder_help.pyx":64
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:
- *                 needle_found=1             # <<<<<<<<<<<<<<
- *                 break
- *         if needle_found:
- */
-        __pyx_v_needle_found = 1;
-
-        /* "flydra_fastfinder_help.pyx":65
- *             if haystack[j]==needles[i]:
- *                 needle_found=1
- *                 break             # <<<<<<<<<<<<<<
- *         if needle_found:
- *             found[i] = j
- */
-        goto __pyx_L6_break;
-
-        /* "flydra_fastfinder_help.pyx":63
- *         needle_found = 0
- *         for j in range(hmax):
- *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
- *                 needle_found=1
- *                 break
- */
-      }
-    }
-    __pyx_L6_break:;
-
-    /* "flydra_fastfinder_help.pyx":66
- *                 needle_found=1
- *                 break
- *         if needle_found:             # <<<<<<<<<<<<<<
- *             found[i] = j
- *         else:
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
  */
-    __pyx_t_19 = (__pyx_v_needle_found != 0);
-    if (__pyx_t_19) {
 
-      /* "flydra_fastfinder_help.pyx":67
- *                 break
- *         if needle_found:
- *             found[i] = j             # <<<<<<<<<<<<<<
- *         else:
- *             found[i] = -1
- */
-      __pyx_t_18 = __pyx_v_i;
-      if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_found.diminfo[0].shape;
-      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_found.diminfo[0].strides) = __pyx_v_j;
-
-      /* "flydra_fastfinder_help.pyx":66
- *                 needle_found=1
- *                 break
- *         if needle_found:             # <<<<<<<<<<<<<<
- *             found[i] = j
- *         else:
- */
-      goto __pyx_L8;
-    }
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
 
-    /* "flydra_fastfinder_help.pyx":69
- *             found[i] = j
- *         else:
- *             found[i] = -1             # <<<<<<<<<<<<<<
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":278
  * 
- *     if not missing_ok:
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
  */
-    /*else*/ {
-      __pyx_t_17 = __pyx_v_i;
-      if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_found.diminfo[0].shape;
-      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_found.diminfo[0].strides) = -1L;
-    }
-    __pyx_L8:;
-  }
 
-  /* "flydra_fastfinder_help.pyx":71
- *             found[i] = -1
- * 
- *     if not missing_ok:             # <<<<<<<<<<<<<<
- *         if np.any(found==-1):
- *             raise MissingValueError('some of your needles were not found')
- */
-  __pyx_t_19 = ((!(__pyx_v_missing_ok != 0)) != 0);
-  if (__pyx_t_19) {
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
+  npy_intp __pyx_r;
 
-    /* "flydra_fastfinder_help.pyx":72
- * 
- *     if not missing_ok:
- *         if np.any(found==-1):             # <<<<<<<<<<<<<<
- *             raise MissingValueError('some of your needles were not found')
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":281
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
+ *         @property
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_any); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = PyObject_RichCompare(((PyObject *)__pyx_v_found), __pyx_int_neg_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __pyx_t_2 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_2)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_2);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_19 < 0)) __PYX_ERR(0, 72, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(__pyx_t_19)) {
+  __pyx_r = PyArray_SIZE(__pyx_v_self);
+  goto __pyx_L0;
 
-      /* "flydra_fastfinder_help.pyx":73
- *     if not missing_ok:
- *         if np.any(found==-1):
- *             raise MissingValueError('some of your needles were not found')             # <<<<<<<<<<<<<<
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":278
  * 
- *     return found
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MissingValueError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
-        if (likely(__pyx_t_3)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-          __Pyx_INCREF(__pyx_t_3);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_1, function);
-        }
-      }
-      __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_kp_s_some_of_your_needles_were_not_fo) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_kp_s_some_of_your_needles_were_not_fo);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 73, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 73, __pyx_L1_error)
 
-      /* "flydra_fastfinder_help.pyx":72
- * 
- *     if not missing_ok:
- *         if np.any(found==-1):             # <<<<<<<<<<<<<<
- *             raise MissingValueError('some of your needles were not found')
- * 
- */
-    }
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
 
-    /* "flydra_fastfinder_help.pyx":71
- *             found[i] = -1
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":284
  * 
- *     if not missing_ok:             # <<<<<<<<<<<<<<
- *         if np.any(found==-1):
- *             raise MissingValueError('some of your needles were not found')
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
  */
-  }
 
-  /* "flydra_fastfinder_help.pyx":75
- *             raise MissingValueError('some of your needles were not found')
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
+  char *__pyx_r;
+
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":290
+ *             of `PyArray_DATA()` instead, which returns a 'void*'.
+ *             """
+ *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
- *     return found             # <<<<<<<<<<<<<<
+ *     ctypedef unsigned char      npy_bool
  */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_found));
-  __pyx_r = ((PyObject *)__pyx_v_found);
+  __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "flydra_fastfinder_help.pyx":44
- * 
- * @cython.boundscheck(False) # turn of bounds-checking for entire function
- * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":284
  * 
- *     # TODO: implementation that does binary search on pre-sorted
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
-    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
-  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  goto __pyx_L2;
   __pyx_L0:;
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
-  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
-  __pyx_L2:;
-  __Pyx_XDECREF((PyObject *)__pyx_v_found);
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":735
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2829,29 +3174,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2862,15 +3207,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":738
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2879,29 +3224,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2912,15 +3257,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":741
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2929,29 +3274,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2962,15 +3307,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":744
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2979,29 +3324,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3012,15 +3357,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":747
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3029,29 +3374,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3062,212 +3407,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":750
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
-  __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
+  __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":931
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":935
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
-  __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
+  __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":938
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":937
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":939
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":943
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3283,15 +3628,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3299,84 +3644,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 984, __pyx_L3_error)
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":946
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 985, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 947, __pyx_L5_except_error)
+      __PYX_ERR(1, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":943
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3391,15 +3736,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":949
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3415,15 +3760,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3431,84 +3776,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 990, __pyx_L3_error)
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":952
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 991, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 953, __pyx_L5_except_error)
+      __PYX_ERR(1, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":949
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3523,15 +3868,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":955
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3547,15 +3892,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":956
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3563,84 +3908,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 957, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 996, __pyx_L3_error)
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":958
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 958, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 997, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":959
+      /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
- * cdef extern from *:
+ * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 959, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 959, __pyx_L5_except_error)
+      __PYX_ERR(1, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":955
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3655,338 +4000,1489 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":969
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":969
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":984
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":984
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":999
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":999
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1009
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1009
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1016
+/* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1020
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1016
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-static PyMethodDef __pyx_methods[] = {
-  {0, 0, 0, 0}
-};
+/* "flydra_fastfinder_help.pyx":9
+ * # see also FastFinder class in flydra_analysis.a2.utils
+ * 
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):
+ * 
+ */
 
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_flydra_fastfinder_help(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_flydra_fastfinder_help},
-  {0, NULL}
-};
+/* Python wrapper */
+static PyObject *__pyx_pw_22flydra_fastfinder_help_1get_first_idx_long(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_22flydra_fastfinder_help_1get_first_idx_long = {"get_first_idx_long", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_22flydra_fastfinder_help_1get_first_idx_long, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_22flydra_fastfinder_help_1get_first_idx_long(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyArrayObject *__pyx_v_haystack = 0;
+  PyArrayObject *__pyx_v_needles = 0;
+  int __pyx_v_missing_ok;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_first_idx_long (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_haystack,&__pyx_n_s_needles,&__pyx_n_s_missing_ok,0};
+    PyObject* values[3] = {0,0,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_haystack)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_needles)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("get_first_idx_long", 0, 2, 3, 1); __PYX_ERR(0, 9, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_missing_ok);
+          if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_first_idx_long") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_haystack = ((PyArrayObject *)values[0]);
+    __pyx_v_needles = ((PyArrayObject *)values[1]);
+    if (values[2]) {
+      __pyx_v_missing_ok = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_missing_ok == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 10, __pyx_L3_error)
+    } else {
+      __pyx_v_missing_ok = ((int)((int)0));
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("get_first_idx_long", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 9, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_long", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_haystack), __pyx_ptype_5numpy_ndarray, 1, "haystack", 0))) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_needles), __pyx_ptype_5numpy_ndarray, 1, "needles", 0))) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_r = __pyx_pf_22flydra_fastfinder_help_get_first_idx_long(__pyx_self, __pyx_v_haystack, __pyx_v_needles, __pyx_v_missing_ok);
 
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "flydra_fastfinder_help",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_22flydra_fastfinder_help_get_first_idx_long(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_haystack, PyArrayObject *__pyx_v_needles, int __pyx_v_missing_ok) {
+  long __pyx_v_hmax;
+  long __pyx_v_nmax;
+  long __pyx_v_i;
+  long __pyx_v_j;
+  int __pyx_v_needle_found;
+  PyArrayObject *__pyx_v_found = 0;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_found;
+  __Pyx_Buffer __pyx_pybuffer_found;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_haystack;
+  __Pyx_Buffer __pyx_pybuffer_haystack;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_needles;
+  __Pyx_Buffer __pyx_pybuffer_needles;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_t_2;
+  npy_intp *__pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyArrayObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  long __pyx_t_13;
+  long __pyx_t_14;
+  long __pyx_t_15;
+  long __pyx_t_16;
+  long __pyx_t_17;
+  long __pyx_t_18;
+  Py_ssize_t __pyx_t_19;
+  Py_ssize_t __pyx_t_20;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_first_idx_long", 0);
+  __pyx_pybuffer_found.pybuffer.buf = NULL;
+  __pyx_pybuffer_found.refcount = 0;
+  __pyx_pybuffernd_found.data = NULL;
+  __pyx_pybuffernd_found.rcbuffer = &__pyx_pybuffer_found;
+  __pyx_pybuffer_haystack.pybuffer.buf = NULL;
+  __pyx_pybuffer_haystack.refcount = 0;
+  __pyx_pybuffernd_haystack.data = NULL;
+  __pyx_pybuffernd_haystack.rcbuffer = &__pyx_pybuffer_haystack;
+  __pyx_pybuffer_needles.pybuffer.buf = NULL;
+  __pyx_pybuffer_needles.refcount = 0;
+  __pyx_pybuffernd_needles.data = NULL;
+  __pyx_pybuffernd_needles.rcbuffer = &__pyx_pybuffer_needles;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer, (PyObject*)__pyx_v_haystack, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_haystack.diminfo[0].strides = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_haystack.diminfo[0].shape = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.shape[0];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_needles.rcbuffer->pybuffer, (PyObject*)__pyx_v_needles, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_needles.diminfo[0].strides = __pyx_pybuffernd_needles.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_needles.diminfo[0].shape = __pyx_pybuffernd_needles.rcbuffer->pybuffer.shape[0];
+
+  /* "flydra_fastfinder_help.pyx":15
+ *     # haystack
+ * 
+ *     assert haystack.ndim==1             # <<<<<<<<<<<<<<
+ *     assert needles.ndim==1
+ * 
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(((PyArrayObject *)__pyx_v_haystack)); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_2 = (__pyx_t_1 == 1);
+    if (unlikely(!__pyx_t_2)) {
+      __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
+      __PYX_ERR(0, 15, __pyx_L1_error)
+    }
+  }
   #else
-    -1, /* m_size */
+  if ((1)); else __PYX_ERR(0, 15, __pyx_L1_error)
   #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
+
+  /* "flydra_fastfinder_help.pyx":16
+ * 
+ *     assert haystack.ndim==1
+ *     assert needles.ndim==1             # <<<<<<<<<<<<<<
+ * 
+ *     cdef long hmax = haystack.shape[0]
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(((PyArrayObject *)__pyx_v_needles)); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L1_error)
+    __pyx_t_2 = (__pyx_t_1 == 1);
+    if (unlikely(!__pyx_t_2)) {
+      __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
+      __PYX_ERR(0, 16, __pyx_L1_error)
+    }
+  }
   #else
-    NULL, /* m_reload */
+  if ((1)); else __PYX_ERR(0, 16, __pyx_L1_error)
   #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
+
+  /* "flydra_fastfinder_help.pyx":18
+ *     assert needles.ndim==1
+ * 
+ *     cdef long hmax = haystack.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef long nmax = needles.shape[0]
+ *     cdef long i,j
+ */
+  __pyx_t_3 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_haystack)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_v_hmax = (__pyx_t_3[0]);
+
+  /* "flydra_fastfinder_help.pyx":19
+ * 
+ *     cdef long hmax = haystack.shape[0]
+ *     cdef long nmax = needles.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef long i,j
+ *     cdef int needle_found
+ */
+  __pyx_t_3 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_needles)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_v_nmax = (__pyx_t_3[0]);
+
+  /* "flydra_fastfinder_help.pyx":24
+ *     cdef np.ndarray[long, ndim=1] found
+ * 
+ *     found = np.zeros( (needles.shape[0],) , dtype=np.int64)             # <<<<<<<<<<<<<<
+ * 
+ *     for i in range(nmax):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_needles)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int64); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_9 = ((PyArrayObject *)__pyx_t_8);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
+    __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
+    if (unlikely(__pyx_t_1 < 0)) {
+      PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
+      if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_v_found, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+        Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
+        __Pyx_RaiseBufferFallbackError();
+      } else {
+        PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
+      }
+      __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
+    }
+    __pyx_pybuffernd_found.diminfo[0].strides = __pyx_pybuffernd_found.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_found.diminfo[0].shape = __pyx_pybuffernd_found.rcbuffer->pybuffer.shape[0];
+    if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 24, __pyx_L1_error)
+  }
+  __pyx_t_9 = 0;
+  __pyx_v_found = ((PyArrayObject *)__pyx_t_8);
+  __pyx_t_8 = 0;
+
+  /* "flydra_fastfinder_help.pyx":26
+ *     found = np.zeros( (needles.shape[0],) , dtype=np.int64)
+ * 
+ *     for i in range(nmax):             # <<<<<<<<<<<<<<
+ *         needle_found = 0
+ *         for j in range(hmax):
+ */
+  __pyx_t_13 = __pyx_v_nmax;
+  __pyx_t_14 = __pyx_t_13;
+  for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
+    __pyx_v_i = __pyx_t_15;
+
+    /* "flydra_fastfinder_help.pyx":27
+ * 
+ *     for i in range(nmax):
+ *         needle_found = 0             # <<<<<<<<<<<<<<
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:
+ */
+    __pyx_v_needle_found = 0;
+
+    /* "flydra_fastfinder_help.pyx":28
+ *     for i in range(nmax):
+ *         needle_found = 0
+ *         for j in range(hmax):             # <<<<<<<<<<<<<<
+ *             if haystack[j]==needles[i]:
+ *                 needle_found=1
+ */
+    __pyx_t_16 = __pyx_v_hmax;
+    __pyx_t_17 = __pyx_t_16;
+    for (__pyx_t_18 = 0; __pyx_t_18 < __pyx_t_17; __pyx_t_18+=1) {
+      __pyx_v_j = __pyx_t_18;
+
+      /* "flydra_fastfinder_help.pyx":29
+ *         needle_found = 0
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
+ *                 needle_found=1
+ *                 break
+ */
+      __pyx_t_19 = __pyx_v_j;
+      if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_haystack.diminfo[0].shape;
+      __pyx_t_20 = __pyx_v_i;
+      if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_needles.diminfo[0].shape;
+      __pyx_t_2 = ((*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_haystack.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_haystack.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_needles.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_needles.diminfo[0].strides)));
+      if (__pyx_t_2) {
+
+        /* "flydra_fastfinder_help.pyx":30
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:
+ *                 needle_found=1             # <<<<<<<<<<<<<<
+ *                 break
+ *         if needle_found:
+ */
+        __pyx_v_needle_found = 1;
+
+        /* "flydra_fastfinder_help.pyx":31
+ *             if haystack[j]==needles[i]:
+ *                 needle_found=1
+ *                 break             # <<<<<<<<<<<<<<
+ *         if needle_found:
+ *             found[i] = j
+ */
+        goto __pyx_L6_break;
+
+        /* "flydra_fastfinder_help.pyx":29
+ *         needle_found = 0
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
+ *                 needle_found=1
+ *                 break
+ */
+      }
+    }
+    __pyx_L6_break:;
+
+    /* "flydra_fastfinder_help.pyx":32
+ *                 needle_found=1
+ *                 break
+ *         if needle_found:             # <<<<<<<<<<<<<<
+ *             found[i] = j
+ *         else:
+ */
+    __pyx_t_2 = (__pyx_v_needle_found != 0);
+    if (__pyx_t_2) {
+
+      /* "flydra_fastfinder_help.pyx":33
+ *                 break
+ *         if needle_found:
+ *             found[i] = j             # <<<<<<<<<<<<<<
+ *         else:
+ *             found[i] = -1
+ */
+      __pyx_t_20 = __pyx_v_i;
+      if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_found.diminfo[0].shape;
+      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_found.diminfo[0].strides) = __pyx_v_j;
+
+      /* "flydra_fastfinder_help.pyx":32
+ *                 needle_found=1
+ *                 break
+ *         if needle_found:             # <<<<<<<<<<<<<<
+ *             found[i] = j
+ *         else:
+ */
+      goto __pyx_L8;
+    }
+
+    /* "flydra_fastfinder_help.pyx":35
+ *             found[i] = j
+ *         else:
+ *             found[i] = -1             # <<<<<<<<<<<<<<
+ * 
+ *     if not missing_ok:
+ */
+    /*else*/ {
+      __pyx_t_20 = __pyx_v_i;
+      if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_found.diminfo[0].shape;
+      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_found.diminfo[0].strides) = -1L;
+    }
+    __pyx_L8:;
+  }
+
+  /* "flydra_fastfinder_help.pyx":37
+ *             found[i] = -1
+ * 
+ *     if not missing_ok:             # <<<<<<<<<<<<<<
+ *         if np.any(found==-1):
+ *             raise MissingValueError('some of your needles were not found')
+ */
+  __pyx_t_2 = (!(__pyx_v_missing_ok != 0));
+  if (__pyx_t_2) {
+
+    /* "flydra_fastfinder_help.pyx":38
+ * 
+ *     if not missing_ok:
+ *         if np.any(found==-1):             # <<<<<<<<<<<<<<
+ *             raise MissingValueError('some of your needles were not found')
+ * 
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 38, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_any); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 38, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_found), __pyx_int_neg_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 38, __pyx_L1_error)
+    __pyx_t_5 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_6};
+      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 38, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    }
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 38, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(__pyx_t_2)) {
+
+      /* "flydra_fastfinder_help.pyx":39
+ *     if not missing_ok:
+ *         if np.any(found==-1):
+ *             raise MissingValueError('some of your needles were not found')             # <<<<<<<<<<<<<<
+ * 
+ *     return found
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MissingValueError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_6 = NULL;
+      __pyx_t_1 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __pyx_t_1 = 1;
+        }
+      }
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_s_some_of_your_needles_were_not_fo};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 39, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(0, 39, __pyx_L1_error)
+
+      /* "flydra_fastfinder_help.pyx":38
+ * 
+ *     if not missing_ok:
+ *         if np.any(found==-1):             # <<<<<<<<<<<<<<
+ *             raise MissingValueError('some of your needles were not found')
+ * 
+ */
+    }
+
+    /* "flydra_fastfinder_help.pyx":37
+ *             found[i] = -1
+ * 
+ *     if not missing_ok:             # <<<<<<<<<<<<<<
+ *         if np.any(found==-1):
+ *             raise MissingValueError('some of your needles were not found')
+ */
+  }
+
+  /* "flydra_fastfinder_help.pyx":41
+ *             raise MissingValueError('some of your needles were not found')
+ * 
+ *     return found             # <<<<<<<<<<<<<<
+ * 
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF((PyObject *)__pyx_v_found);
+  __pyx_r = ((PyObject *)__pyx_v_found);
+  goto __pyx_L0;
+
+  /* "flydra_fastfinder_help.pyx":9
+ * # see also FastFinder class in flydra_analysis.a2.utils
+ * 
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_long", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_found);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "flydra_fastfinder_help.pyx":43
+ *     return found
+ * 
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_22flydra_fastfinder_help_3get_first_idx_double(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_22flydra_fastfinder_help_3get_first_idx_double = {"get_first_idx_double", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_22flydra_fastfinder_help_3get_first_idx_double, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_22flydra_fastfinder_help_3get_first_idx_double(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyArrayObject *__pyx_v_haystack = 0;
+  PyArrayObject *__pyx_v_needles = 0;
+  int __pyx_v_missing_ok;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("get_first_idx_double (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_haystack,&__pyx_n_s_needles,&__pyx_n_s_missing_ok,0};
+    PyObject* values[3] = {0,0,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_haystack)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_needles)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("get_first_idx_double", 0, 2, 3, 1); __PYX_ERR(0, 43, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_missing_ok);
+          if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_first_idx_double") < 0)) __PYX_ERR(0, 43, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_haystack = ((PyArrayObject *)values[0]);
+    __pyx_v_needles = ((PyArrayObject *)values[1]);
+    if (values[2]) {
+      __pyx_v_missing_ok = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_missing_ok == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L3_error)
+    } else {
+      __pyx_v_missing_ok = ((int)((int)0));
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("get_first_idx_double", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 43, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_haystack), __pyx_ptype_5numpy_ndarray, 1, "haystack", 0))) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_needles), __pyx_ptype_5numpy_ndarray, 1, "needles", 0))) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_r = __pyx_pf_22flydra_fastfinder_help_2get_first_idx_double(__pyx_self, __pyx_v_haystack, __pyx_v_needles, __pyx_v_missing_ok);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_22flydra_fastfinder_help_2get_first_idx_double(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_haystack, PyArrayObject *__pyx_v_needles, int __pyx_v_missing_ok) {
+  long __pyx_v_hmax;
+  long __pyx_v_nmax;
+  long __pyx_v_i;
+  long __pyx_v_j;
+  int __pyx_v_needle_found;
+  PyArrayObject *__pyx_v_found = 0;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_found;
+  __Pyx_Buffer __pyx_pybuffer_found;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_haystack;
+  __Pyx_Buffer __pyx_pybuffer_haystack;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_needles;
+  __Pyx_Buffer __pyx_pybuffer_needles;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_t_2;
+  npy_intp *__pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyArrayObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  long __pyx_t_13;
+  long __pyx_t_14;
+  long __pyx_t_15;
+  long __pyx_t_16;
+  long __pyx_t_17;
+  long __pyx_t_18;
+  Py_ssize_t __pyx_t_19;
+  Py_ssize_t __pyx_t_20;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("get_first_idx_double", 0);
+  __pyx_pybuffer_found.pybuffer.buf = NULL;
+  __pyx_pybuffer_found.refcount = 0;
+  __pyx_pybuffernd_found.data = NULL;
+  __pyx_pybuffernd_found.rcbuffer = &__pyx_pybuffer_found;
+  __pyx_pybuffer_haystack.pybuffer.buf = NULL;
+  __pyx_pybuffer_haystack.refcount = 0;
+  __pyx_pybuffernd_haystack.data = NULL;
+  __pyx_pybuffernd_haystack.rcbuffer = &__pyx_pybuffer_haystack;
+  __pyx_pybuffer_needles.pybuffer.buf = NULL;
+  __pyx_pybuffer_needles.refcount = 0;
+  __pyx_pybuffernd_needles.data = NULL;
+  __pyx_pybuffernd_needles.rcbuffer = &__pyx_pybuffer_needles;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer, (PyObject*)__pyx_v_haystack, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_haystack.diminfo[0].strides = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_haystack.diminfo[0].shape = __pyx_pybuffernd_haystack.rcbuffer->pybuffer.shape[0];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_needles.rcbuffer->pybuffer, (PyObject*)__pyx_v_needles, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_needles.diminfo[0].strides = __pyx_pybuffernd_needles.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_needles.diminfo[0].shape = __pyx_pybuffernd_needles.rcbuffer->pybuffer.shape[0];
+
+  /* "flydra_fastfinder_help.pyx":49
+ *     # haystack
+ * 
+ *     assert haystack.ndim==1             # <<<<<<<<<<<<<<
+ *     assert needles.ndim==1
+ * 
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(((PyArrayObject *)__pyx_v_haystack)); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_2 = (__pyx_t_1 == 1);
+    if (unlikely(!__pyx_t_2)) {
+      __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
+      __PYX_ERR(0, 49, __pyx_L1_error)
+    }
+  }
+  #else
+  if ((1)); else __PYX_ERR(0, 49, __pyx_L1_error)
+  #endif
+
+  /* "flydra_fastfinder_help.pyx":50
+ * 
+ *     assert haystack.ndim==1
+ *     assert needles.ndim==1             # <<<<<<<<<<<<<<
+ * 
+ *     cdef long hmax = haystack.shape[0]
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    __pyx_t_1 = __pyx_f_5numpy_7ndarray_4ndim_ndim(((PyArrayObject *)__pyx_v_needles)); if (unlikely(__pyx_t_1 == ((int)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L1_error)
+    __pyx_t_2 = (__pyx_t_1 == 1);
+    if (unlikely(!__pyx_t_2)) {
+      __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
+      __PYX_ERR(0, 50, __pyx_L1_error)
+    }
+  }
+  #else
+  if ((1)); else __PYX_ERR(0, 50, __pyx_L1_error)
+  #endif
+
+  /* "flydra_fastfinder_help.pyx":52
+ *     assert needles.ndim==1
+ * 
+ *     cdef long hmax = haystack.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef long nmax = needles.shape[0]
+ *     cdef long i,j
+ */
+  __pyx_t_3 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_haystack)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_v_hmax = (__pyx_t_3[0]);
+
+  /* "flydra_fastfinder_help.pyx":53
+ * 
+ *     cdef long hmax = haystack.shape[0]
+ *     cdef long nmax = needles.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef long i,j
+ *     cdef int needle_found
+ */
+  __pyx_t_3 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_needles)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_v_nmax = (__pyx_t_3[0]);
+
+  /* "flydra_fastfinder_help.pyx":58
+ *     cdef np.ndarray[long, ndim=1] found
+ * 
+ *     found = np.zeros( (needles.shape[0],) , dtype=np.int64)             # <<<<<<<<<<<<<<
+ * 
+ *     for i in range(nmax):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_needles)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_np); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_int64); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_9 = ((PyArrayObject *)__pyx_t_8);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
+    __pyx_t_1 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack);
+    if (unlikely(__pyx_t_1 < 0)) {
+      PyErr_Fetch(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
+      if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_found.rcbuffer->pybuffer, (PyObject*)__pyx_v_found, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+        Py_XDECREF(__pyx_t_10); Py_XDECREF(__pyx_t_11); Py_XDECREF(__pyx_t_12);
+        __Pyx_RaiseBufferFallbackError();
+      } else {
+        PyErr_Restore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
+      }
+      __pyx_t_10 = __pyx_t_11 = __pyx_t_12 = 0;
+    }
+    __pyx_pybuffernd_found.diminfo[0].strides = __pyx_pybuffernd_found.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_found.diminfo[0].shape = __pyx_pybuffernd_found.rcbuffer->pybuffer.shape[0];
+    if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 58, __pyx_L1_error)
+  }
+  __pyx_t_9 = 0;
+  __pyx_v_found = ((PyArrayObject *)__pyx_t_8);
+  __pyx_t_8 = 0;
+
+  /* "flydra_fastfinder_help.pyx":60
+ *     found = np.zeros( (needles.shape[0],) , dtype=np.int64)
+ * 
+ *     for i in range(nmax):             # <<<<<<<<<<<<<<
+ *         needle_found = 0
+ *         for j in range(hmax):
+ */
+  __pyx_t_13 = __pyx_v_nmax;
+  __pyx_t_14 = __pyx_t_13;
+  for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
+    __pyx_v_i = __pyx_t_15;
+
+    /* "flydra_fastfinder_help.pyx":61
+ * 
+ *     for i in range(nmax):
+ *         needle_found = 0             # <<<<<<<<<<<<<<
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:
+ */
+    __pyx_v_needle_found = 0;
+
+    /* "flydra_fastfinder_help.pyx":62
+ *     for i in range(nmax):
+ *         needle_found = 0
+ *         for j in range(hmax):             # <<<<<<<<<<<<<<
+ *             if haystack[j]==needles[i]:
+ *                 needle_found=1
+ */
+    __pyx_t_16 = __pyx_v_hmax;
+    __pyx_t_17 = __pyx_t_16;
+    for (__pyx_t_18 = 0; __pyx_t_18 < __pyx_t_17; __pyx_t_18+=1) {
+      __pyx_v_j = __pyx_t_18;
+
+      /* "flydra_fastfinder_help.pyx":63
+ *         needle_found = 0
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
+ *                 needle_found=1
+ *                 break
+ */
+      __pyx_t_19 = __pyx_v_j;
+      if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_haystack.diminfo[0].shape;
+      __pyx_t_20 = __pyx_v_i;
+      if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_needles.diminfo[0].shape;
+      __pyx_t_2 = ((*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_haystack.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_haystack.diminfo[0].strides)) == (*__Pyx_BufPtrStrided1d(double *, __pyx_pybuffernd_needles.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_needles.diminfo[0].strides)));
+      if (__pyx_t_2) {
+
+        /* "flydra_fastfinder_help.pyx":64
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:
+ *                 needle_found=1             # <<<<<<<<<<<<<<
+ *                 break
+ *         if needle_found:
+ */
+        __pyx_v_needle_found = 1;
+
+        /* "flydra_fastfinder_help.pyx":65
+ *             if haystack[j]==needles[i]:
+ *                 needle_found=1
+ *                 break             # <<<<<<<<<<<<<<
+ *         if needle_found:
+ *             found[i] = j
+ */
+        goto __pyx_L6_break;
+
+        /* "flydra_fastfinder_help.pyx":63
+ *         needle_found = 0
+ *         for j in range(hmax):
+ *             if haystack[j]==needles[i]:             # <<<<<<<<<<<<<<
+ *                 needle_found=1
+ *                 break
+ */
+      }
+    }
+    __pyx_L6_break:;
+
+    /* "flydra_fastfinder_help.pyx":66
+ *                 needle_found=1
+ *                 break
+ *         if needle_found:             # <<<<<<<<<<<<<<
+ *             found[i] = j
+ *         else:
+ */
+    __pyx_t_2 = (__pyx_v_needle_found != 0);
+    if (__pyx_t_2) {
+
+      /* "flydra_fastfinder_help.pyx":67
+ *                 break
+ *         if needle_found:
+ *             found[i] = j             # <<<<<<<<<<<<<<
+ *         else:
+ *             found[i] = -1
+ */
+      __pyx_t_20 = __pyx_v_i;
+      if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_found.diminfo[0].shape;
+      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_found.diminfo[0].strides) = __pyx_v_j;
+
+      /* "flydra_fastfinder_help.pyx":66
+ *                 needle_found=1
+ *                 break
+ *         if needle_found:             # <<<<<<<<<<<<<<
+ *             found[i] = j
+ *         else:
+ */
+      goto __pyx_L8;
+    }
+
+    /* "flydra_fastfinder_help.pyx":69
+ *             found[i] = j
+ *         else:
+ *             found[i] = -1             # <<<<<<<<<<<<<<
+ * 
+ *     if not missing_ok:
+ */
+    /*else*/ {
+      __pyx_t_20 = __pyx_v_i;
+      if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_pybuffernd_found.diminfo[0].shape;
+      *__Pyx_BufPtrStrided1d(long *, __pyx_pybuffernd_found.rcbuffer->pybuffer.buf, __pyx_t_20, __pyx_pybuffernd_found.diminfo[0].strides) = -1L;
+    }
+    __pyx_L8:;
+  }
+
+  /* "flydra_fastfinder_help.pyx":71
+ *             found[i] = -1
+ * 
+ *     if not missing_ok:             # <<<<<<<<<<<<<<
+ *         if np.any(found==-1):
+ *             raise MissingValueError('some of your needles were not found')
+ */
+  __pyx_t_2 = (!(__pyx_v_missing_ok != 0));
+  if (__pyx_t_2) {
+
+    /* "flydra_fastfinder_help.pyx":72
+ * 
+ *     if not missing_ok:
+ *         if np.any(found==-1):             # <<<<<<<<<<<<<<
+ *             raise MissingValueError('some of your needles were not found')
+ * 
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_any); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = PyObject_RichCompare(((PyObject *)__pyx_v_found), __pyx_int_neg_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
+    __pyx_t_5 = NULL;
+    __pyx_t_1 = 0;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+        __pyx_t_1 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_6};
+      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 72, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    }
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 72, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(__pyx_t_2)) {
+
+      /* "flydra_fastfinder_help.pyx":73
+ *     if not missing_ok:
+ *         if np.any(found==-1):
+ *             raise MissingValueError('some of your needles were not found')             # <<<<<<<<<<<<<<
+ * 
+ *     return found
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MissingValueError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_6 = NULL;
+      __pyx_t_1 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_6)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_6);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __pyx_t_1 = 1;
+        }
+      }
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_s_some_of_your_needles_were_not_fo};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_1, 1+__pyx_t_1);
+        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 73, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(0, 73, __pyx_L1_error)
+
+      /* "flydra_fastfinder_help.pyx":72
+ * 
+ *     if not missing_ok:
+ *         if np.any(found==-1):             # <<<<<<<<<<<<<<
+ *             raise MissingValueError('some of your needles were not found')
+ * 
+ */
+    }
+
+    /* "flydra_fastfinder_help.pyx":71
+ *             found[i] = -1
+ * 
+ *     if not missing_ok:             # <<<<<<<<<<<<<<
+ *         if np.any(found==-1):
+ *             raise MissingValueError('some of your needles were not found')
+ */
+  }
+
+  /* "flydra_fastfinder_help.pyx":75
+ *             raise MissingValueError('some of your needles were not found')
+ * 
+ *     return found             # <<<<<<<<<<<<<<
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF((PyObject *)__pyx_v_found);
+  __pyx_r = ((PyObject *)__pyx_v_found);
+  goto __pyx_L0;
+
+  /* "flydra_fastfinder_help.pyx":43
+ *     return found
+ * 
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("flydra_fastfinder_help.get_first_idx_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_found.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_haystack.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_needles.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_found);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyMethodDef __pyx_methods[] = {
+  {0, 0, 0, 0}
+};
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_n_s_MissingValueError, __pyx_k_MissingValueError, sizeof(__pyx_k_MissingValueError), 0, 0, 1, 1},
-  {&__pyx_n_s_any, __pyx_k_any, sizeof(__pyx_k_any), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_flydra_analysis_a2_missing_value, __pyx_k_flydra_analysis_a2_missing_value, sizeof(__pyx_k_flydra_analysis_a2_missing_value), 0, 0, 1, 1},
-  {&__pyx_n_s_flydra_fastfinder_help, __pyx_k_flydra_fastfinder_help, sizeof(__pyx_k_flydra_fastfinder_help), 0, 0, 1, 1},
-  {&__pyx_kp_s_flydra_fastfinder_help_pyx, __pyx_k_flydra_fastfinder_help_pyx, sizeof(__pyx_k_flydra_fastfinder_help_pyx), 0, 0, 1, 0},
-  {&__pyx_n_s_found, __pyx_k_found, sizeof(__pyx_k_found), 0, 0, 1, 1},
-  {&__pyx_n_s_get_first_idx_double, __pyx_k_get_first_idx_double, sizeof(__pyx_k_get_first_idx_double), 0, 0, 1, 1},
-  {&__pyx_n_s_get_first_idx_long, __pyx_k_get_first_idx_long, sizeof(__pyx_k_get_first_idx_long), 0, 0, 1, 1},
-  {&__pyx_n_s_haystack, __pyx_k_haystack, sizeof(__pyx_k_haystack), 0, 0, 1, 1},
-  {&__pyx_n_s_hmax, __pyx_k_hmax, sizeof(__pyx_k_hmax), 0, 0, 1, 1},
-  {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
-  {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_missing_ok, __pyx_k_missing_ok, sizeof(__pyx_k_missing_ok), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_needle_found, __pyx_k_needle_found, sizeof(__pyx_k_needle_found), 0, 0, 1, 1},
-  {&__pyx_n_s_needles, __pyx_k_needles, sizeof(__pyx_k_needles), 0, 0, 1, 1},
-  {&__pyx_n_s_nmax, __pyx_k_nmax, sizeof(__pyx_k_nmax), 0, 0, 1, 1},
-  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
-  {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_kp_s_some_of_your_needles_were_not_fo, __pyx_k_some_of_your_needles_were_not_fo, sizeof(__pyx_k_some_of_your_needles_were_not_fo), 0, 0, 1, 0},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_AssertionError, __pyx_k_AssertionError, sizeof(__pyx_k_AssertionError), 0, 0, 1, 1},
+    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+    {&__pyx_n_s_MissingValueError, __pyx_k_MissingValueError, sizeof(__pyx_k_MissingValueError), 0, 0, 1, 1},
+    {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
+    {&__pyx_n_s__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 0, 1, 1},
+    {&__pyx_n_s_any, __pyx_k_any, sizeof(__pyx_k_any), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+    {&__pyx_n_s_flydra_analysis_a2_missing_value, __pyx_k_flydra_analysis_a2_missing_value, sizeof(__pyx_k_flydra_analysis_a2_missing_value), 0, 0, 1, 1},
+    {&__pyx_n_s_flydra_fastfinder_help, __pyx_k_flydra_fastfinder_help, sizeof(__pyx_k_flydra_fastfinder_help), 0, 0, 1, 1},
+    {&__pyx_kp_s_flydra_fastfinder_help_pyx, __pyx_k_flydra_fastfinder_help_pyx, sizeof(__pyx_k_flydra_fastfinder_help_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_found, __pyx_k_found, sizeof(__pyx_k_found), 0, 0, 1, 1},
+    {&__pyx_n_s_get_first_idx_double, __pyx_k_get_first_idx_double, sizeof(__pyx_k_get_first_idx_double), 0, 0, 1, 1},
+    {&__pyx_n_s_get_first_idx_long, __pyx_k_get_first_idx_long, sizeof(__pyx_k_get_first_idx_long), 0, 0, 1, 1},
+    {&__pyx_n_s_haystack, __pyx_k_haystack, sizeof(__pyx_k_haystack), 0, 0, 1, 1},
+    {&__pyx_n_s_hmax, __pyx_k_hmax, sizeof(__pyx_k_hmax), 0, 0, 1, 1},
+    {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_missing_ok, __pyx_k_missing_ok, sizeof(__pyx_k_missing_ok), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_needle_found, __pyx_k_needle_found, sizeof(__pyx_k_needle_found), 0, 0, 1, 1},
+    {&__pyx_n_s_needles, __pyx_k_needles, sizeof(__pyx_k_needles), 0, 0, 1, 1},
+    {&__pyx_n_s_nmax, __pyx_k_nmax, sizeof(__pyx_k_nmax), 0, 0, 1, 1},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
+    {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
+    {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_kp_s_some_of_your_needles_were_not_fo, __pyx_k_some_of_your_needles_were_not_fo, sizeof(__pyx_k_some_of_your_needles_were_not_fo), 0, 0, 1, 0},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 15, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 26, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 947, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 986, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 947, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../../../../../private/var/folders/8r/wczrm19j599_qsgyft707_wh0000gr/T/build-env-q90son3f/lib/python3.8/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 953, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 992, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "flydra_fastfinder_help.pyx":10
+  /* "flydra_fastfinder_help.pyx":9
+ * # see also FastFinder class in flydra_analysis.a2.utils
  * 
- * @cython.boundscheck(False) # turn of bounds-checking for entire function
- * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):
  * 
- *     # TODO: implementation that does binary search on pre-sorted
  */
-  __pyx_tuple__3 = PyTuple_Pack(9, __pyx_n_s_haystack, __pyx_n_s_needles, __pyx_n_s_missing_ok, __pyx_n_s_hmax, __pyx_n_s_nmax, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_needle_found, __pyx_n_s_found); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_flydra_fastfinder_help_pyx, __pyx_n_s_get_first_idx_long, 10, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(9, __pyx_n_s_haystack, __pyx_n_s_needles, __pyx_n_s_missing_ok, __pyx_n_s_hmax, __pyx_n_s_nmax, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_needle_found, __pyx_n_s_found); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_flydra_fastfinder_help_pyx, __pyx_n_s_get_first_idx_long, 9, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 9, __pyx_L1_error)
 
-  /* "flydra_fastfinder_help.pyx":44
+  /* "flydra_fastfinder_help.pyx":43
+ *     return found
  * 
- * @cython.boundscheck(False) # turn of bounds-checking for entire function
- * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):
  * 
- *     # TODO: implementation that does binary search on pre-sorted
  */
-  __pyx_tuple__5 = PyTuple_Pack(9, __pyx_n_s_haystack, __pyx_n_s_needles, __pyx_n_s_missing_ok, __pyx_n_s_hmax, __pyx_n_s_nmax, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_needle_found, __pyx_n_s_found); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_flydra_fastfinder_help_pyx, __pyx_n_s_get_first_idx_double, 44, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_flydra_fastfinder_help_pyx, __pyx_n_s_get_first_idx_double, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  /* NumpyImportArray.init */
+  /*
+ * Cython has automatically inserted a call to _import_array since
+ * you didn't include one when you cimported numpy. To disable this
+ * add the line
+ *   <void>numpy._import_array
+ */
+#ifdef NPY_FEATURE_VERSION
+#if !NO_IMPORT_ARRAY
+if (unlikely(_import_array() == -1)) {
+    PyErr_SetString(PyExc_ImportError, "numpy.core.multiarray failed to import "
+    "(auto-generated because you didn't call 'numpy.import_array()' after cimporting numpy; "
+    "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
+}
+#endif
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  return 0;
+  __pyx_L1_error:;
+  return -1;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -4030,55 +5526,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 812, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 814, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 816, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 818, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 820, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 822, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 824, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 828, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 830, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 868, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -4097,14 +5579,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_flydra_fastfinder_help(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_flydra_fastfinder_help},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "flydra_fastfinder_help",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -4147,42 +5678,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -4190,29 +5735,63 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_flydra_fastfinder_help(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'flydra_fastfinder_help' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("flydra_fastfinder_help", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to flydra_fastfinder_help pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -4223,187 +5802,220 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("flydra_fastfinder_help", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_flydra_fastfinder_help) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "flydra_fastfinder_help")) {
-      if (unlikely(PyDict_SetItemString(modules, "flydra_fastfinder_help", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "flydra_fastfinder_help", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "flydra_fastfinder_help.pyx":1
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "flydra_fastfinder_help.pyx":5
  * 
  * import cython
  * from flydra_analysis.a2.missing_value_error import MissingValueError             # <<<<<<<<<<<<<<
  * 
  * # see also FastFinder class in flydra_analysis.a2.utils
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_MissingValueError);
   __Pyx_GIVEREF(__pyx_n_s_MissingValueError);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_MissingValueError);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_flydra_analysis_a2_missing_value, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_MissingValueError);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_flydra_analysis_a2_missing_value, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_MissingValueError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_MissingValueError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MissingValueError, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MissingValueError, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "flydra_fastfinder_help.pyx":10
  * 
  * @cython.boundscheck(False) # turn of bounds-checking for entire function
  * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
  * 
  *     # TODO: implementation that does binary search on pre-sorted
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22flydra_fastfinder_help_1get_first_idx_long, NULL, __pyx_n_s_flydra_fastfinder_help); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(((int)0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
+  /* "flydra_fastfinder_help.pyx":9
+ * # see also FastFinder class in flydra_analysis.a2.utils
+ * 
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_long(np.ndarray[long, ndim=1] haystack, np.ndarray[long, ndim=1] needles, int missing_ok=0):
+ * 
+ */
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_first_idx_long, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_22flydra_fastfinder_help_1get_first_idx_long, 0, __pyx_n_s_get_first_idx_long, NULL, __pyx_n_s_flydra_fastfinder_help, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_first_idx_long, __pyx_t_3) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "flydra_fastfinder_help.pyx":44
  * 
  * @cython.boundscheck(False) # turn of bounds-checking for entire function
  * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):             # <<<<<<<<<<<<<<
  * 
  *     # TODO: implementation that does binary search on pre-sorted
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22flydra_fastfinder_help_3get_first_idx_double, NULL, __pyx_n_s_flydra_fastfinder_help); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_first_idx_double, __pyx_t_2) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(((int)0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
 
-  /* "flydra_fastfinder_help.pyx":1
- * import numpy as np             # <<<<<<<<<<<<<<
- * cimport numpy as np
+  /* "flydra_fastfinder_help.pyx":43
+ *     return found
+ * 
+ * @cython.boundscheck(False) # turn of bounds-checking for entire function             # <<<<<<<<<<<<<<
+ * def get_first_idx_double(np.ndarray[double, ndim=1] haystack, np.ndarray[double, ndim=1] needles, int missing_ok=0):
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_22flydra_fastfinder_help_3get_first_idx_double, 0, __pyx_n_s_get_first_idx_double, NULL, __pyx_n_s_flydra_fastfinder_help, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_first_idx_double, __pyx_t_3) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "../../../../AppData/Local/Packages/PythonSoftwareFoundation.Python.3.8_qbz5n2kfra8p0/LocalCache/local-packages/Python38/site-packages/numpy/__init__.pxd":1016
- * 
+  /* "flydra_fastfinder_help.pyx":1
+ * import numpy as np             # <<<<<<<<<<<<<<
+ * cimport numpy as np
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
- *     """
- *     returns the unit part of the dtype for a numpy datetime64 object.
  */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init flydra_fastfinder_help", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init flydra_fastfinder_help");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -4415,42 +6027,729 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -4486,25 +6785,37 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
@@ -4530,19 +6841,20 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
@@ -4573,44 +6885,51 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
         if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
         #endif
     }
     else {
         if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
@@ -4693,15 +7012,15 @@
     case 'd': return (is_complex ? "'complex double'" : "'double'");
     case 'g': return (is_complex ? "'complex long double'" : "'long double'");
     case 'T': return "a struct";
     case 'O': return "Python object";
     case 'P': return "a pointer";
     case 's': case 'p': return "a string";
     case 0: return "end";
-    default: return "unparseable format string";
+    default: return "unparsable format string";
   }
 }
 static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return 2;
     case 'i': case 'I': case 'l': case 'L': return 4;
@@ -4743,15 +7062,16 @@
 typedef struct { char c; float x; } __Pyx_st_float;
 typedef struct { char c; double x; } __Pyx_st_double;
 typedef struct { char c; long double x; } __Pyx_st_longdouble;
 typedef struct { char c; void *x; } __Pyx_st_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
@@ -4775,15 +7095,16 @@
 typedef struct { float x; char c; } __Pyx_pad_float;
 typedef struct { double x; char c; } __Pyx_pad_double;
 typedef struct { long double x; char c; } __Pyx_pad_longdouble;
 typedef struct { void *x; char c; } __Pyx_pad_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
@@ -5209,14 +7530,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -5227,78 +7556,42 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* PyObjectCall */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
 /* ExtTypeTest */
   static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    __Pyx_TypeName obj_type_name;
+    __Pyx_TypeName type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    type_name = __Pyx_PyType_GetName(type);
+    PyErr_Format(PyExc_TypeError,
+                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
+                 obj_type_name, type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
     return 0;
 }
 
 /* BufferFallbackError */
   static void __Pyx_RaiseBufferFallbackError(void) {
   PyErr_SetString(PyExc_ValueError,
      "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
 }
 
-/* PyCFunctionFastCall */
-  #if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
 /* PyFunctionFastCall */
-  #if CYTHON_FAST_PYCALL
+  #if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -5319,15 +7612,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -5335,15 +7627,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -5406,44 +7698,14 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
-
-/* PyObjectCall2Args */
-  static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
 
 /* PyObjectCallMethO */
   #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
@@ -5457,440 +7719,158 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallOneArg */
-  #if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+/* PyObjectFastCall */
+  static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
     PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
-    }
-#endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
-#endif
-        }
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
-}
-#else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
     return result;
 }
-#endif
-
-/* PyErrFetchRestore */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* RaiseException */
-  #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
-#if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
-        }
-    }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
-}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
 #else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
-                }
+        if (PyCFunction_Check(func))
+#endif
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
             }
         }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
             }
         }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
     }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
+#endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
         } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
-    }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
         }
-#endif
     }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
-}
-#endif
-
-/* GetTopmostException */
-  #if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
     }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
     #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
     #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* PyErrExceptionMatches */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
-/* GetException */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
     }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
     #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
-#ifdef Py_LIMITED_API
+    Py_ssize_t itemsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
-#ifndef Py_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
-            "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -5898,135 +7878,1419 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* Import */
   static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, empty_dict, empty_dict, from_list, level);
+            #else
+            module = PyImport_ImportModuleLevelObject(
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+  #if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__3;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
 /* ImportFrom */
   static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
     PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
     if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        const char* module_name_str = 0;
+        PyObject* module_name = 0;
+        PyObject* module_dot = 0;
+        PyObject* full_name = 0;
+        PyErr_Clear();
+        module_name_str = PyModule_GetName(module);
+        if (unlikely(!module_name_str)) { goto modbad; }
+        module_name = PyUnicode_FromString(module_name_str);
+        if (unlikely(!module_name)) { goto modbad; }
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__4);
+        if (unlikely(!module_dot)) { goto modbad; }
+        full_name = PyUnicode_Concat(module_dot, name);
+        if (unlikely(!full_name)) { goto modbad; }
+        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+        {
+            PyObject *modules = PyImport_GetModuleDict();
+            if (unlikely(!modules))
+                goto modbad;
+            value = PyObject_GetItem(modules, full_name);
+        }
+        #else
+        value = PyImport_GetModule(full_name);
+        #endif
+      modbad:
+        Py_XDECREF(full_name);
+        Py_XDECREF(module_dot);
+        Py_XDECREF(module_name);
+    }
+    if (unlikely(!value)) {
         PyErr_Format(PyExc_ImportError,
         #if PY_MAJOR_VERSION < 3
             "cannot import name %.230s", PyString_AS_STRING(name));
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
+/* FixUpExtensionType */
+  #if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
+    }
+#endif
+    return 0;
+}
+#endif
+
+/* FetchSharedCythonModule */
+  static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+  static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+  #if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -6096,84 +9360,118 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -6181,19 +9479,25 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    __Pyx_TypeName obj_type_name;
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+                 "'" __Pyx_FMT_TYPENAME "' does not have the buffer interface",
+                 obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
@@ -6224,78 +9528,16 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value) {
-    const Py_intptr_t neg_one = (Py_intptr_t) ((Py_intptr_t) 0 - (Py_intptr_t) 1), const_zero = (Py_intptr_t) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(Py_intptr_t) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(Py_intptr_t) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(Py_intptr_t),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -6307,15 +9549,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -6415,15 +9657,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -6441,15 +9683,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -6461,15 +9703,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -6569,15 +9811,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -6596,181 +9838,265 @@
             return z;
         }
     #endif
 #endif
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -6783,183 +10109,343 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -6972,19 +10458,34 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
+/* FormatTypeName */
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__8));
+    }
+    return name;
+}
+#endif
+
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -6997,14 +10498,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -7021,19 +10538,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -7074,56 +10591,88 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  #if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
+static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -7177,15 +10726,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -7206,30 +10755,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -7287,21 +10840,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -7336,16 +10887,41 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `flydra_analysis-0.7.14/flydra_fastfinder_help.pyx` & `flydra_analysis-0.7.15/flydra_fastfinder_help.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     cdef long hmax = haystack.shape[0]
     cdef long nmax = needles.shape[0]
     cdef long i,j
     cdef int needle_found
     cdef np.ndarray[long, ndim=1] found
 
-    found = np.zeros( (needles.shape[0],) , dtype=np.int)
+    found = np.zeros( (needles.shape[0],) , dtype=np.int64)
 
     for i in range(nmax):
         needle_found = 0
         for j in range(hmax):
             if haystack[j]==needles[i]:
                 needle_found=1
                 break
@@ -51,15 +51,15 @@
 
     cdef long hmax = haystack.shape[0]
     cdef long nmax = needles.shape[0]
     cdef long i,j
     cdef int needle_found
     cdef np.ndarray[long, ndim=1] found
 
-    found = np.zeros( (needles.shape[0],) , dtype=np.int)
+    found = np.zeros( (needles.shape[0],) , dtype=np.int64)
 
     for i in range(nmax):
         needle_found = 0
         for j in range(hmax):
             if haystack[j]==needles[i]:
                 needle_found=1
                 break
```

### Comparing `flydra_analysis-0.7.14/setup.py` & `flydra_analysis-0.7.15/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,137 @@
-import sys
-from setuptools import setup, find_packages
-from distutils.core import Extension  # actually monkey-patched by setuptools
-from Cython.Build import cythonize
-
-import numpy as np
-
-from io import open
-from os import path
-
-# read the contents of your README file
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
-    long_description = f.read()
-
-ext_modules = []
-
-ext_modules.append(
-    Extension(
-        name="flydra_fastfinder_help",
-        sources=["flydra_fastfinder_help.pyx"],
-        include_dirs=[np.get_include()],
-    )
-)
-
-setup(
-    name="flydra_analysis",
-    version="0.7.14",  # keep in sync with flydra_analysis/version.py
-    author="Andrew Straw",
-    author_email="strawman@astraw.com",
-    url="https://github.com/strawlab/flydra",
-    description="flydra analysis tools",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    packages=find_packages(),
-    test_suite="nose.collector",
-    ext_modules=cythonize(ext_modules),
-    setup_requires=["setuptools_git >= 0.3",],
-    entry_points={
-        "console_scripts": [
-            # analysis - re-kalmanize
-            "flydra_kalmanize = flydra_analysis.kalmanize:main",
-            # analysis - ufmf care and feeding
-            "flydra_analysis_auto_discover_ufmfs = flydra_analysis.a2.auto_discover_ufmfs:main",
-            "flydra_analysis_montage_ufmfs = flydra_analysis.a2.montage_ufmfs:main",
-            "flydra_analysis_retrack_movies = flydra_analysis.a2.retrack_movies:main",
-            # analysis - generate movies with tracking overlays (uses fmfs or ufmfs)
-            "flydra_analysis_overlay_kalman_movie = flydra_analysis.a2.overlay_kalman_movie:main",
-            # analysis - .h5 file care and feeding
-            "flydra_analysis_check_sync = flydra_analysis.kalmanize:check_sync",
-            "flydra_analysis_print_h5_info = flydra_analysis.a2.h5_info:cmdline",
-            "flydra_analysis_filter_kalman_data = flydra_analysis.analysis.flydra_analysis_filter_kalman_data:main",
-            "flydra_analysis_h5_shorten = flydra_analysis.a2.h5_shorten:main",
-            "flydra_analysis_check_mainbrain_h5_contiguity = flydra_analysis.a2.check_mainbrain_h5_contiguity:main",
-            "flydra_analysis_get_clock_sync = flydra_analysis.a2.get_clock_sync:main",
-            "flydra_analysis_get_2D_image_latency = flydra_analysis.a2.get_2D_image_latency:main",
-            "flydra_analysis_get_2D_image_latency_plot = flydra_analysis.a2.get_2D_image_latency_plot:main",
-            # timestamp conversion
-            "flydra_analysis_frame2timestamp = flydra_analysis.analysis.result_utils:frame2timestamp_command",
-            "flydra_analysis_timestamp2frame = flydra_analysis.analysis.result_utils:timestamp2frame_command",
-            # analysis - not yet classified
-            "flydra_analysis_convert_to_mat = flydra_analysis.analysis.flydra_analysis_convert_to_mat:main",
-            "flydra_analysis_plot_clock_drift = flydra_analysis.analysis.flydra_analysis_plot_clock_drift:main",
-            "flydra_analysis_plot_kalman_2d = flydra_analysis.a2.plot_kalman_2d:main",
-            "flydra_analysis_plot_summary = flydra_analysis.a2.plot_summary:main",
-            "flydra_analysis_plot_timeseries_2d_3d = flydra_analysis.a2.plot_timeseries_2d_3d:main",
-            "flydra_analysis_plot_timeseries_3d = flydra_analysis.a2.plot_timeseries:main",
-            "flydra_analysis_plot_top_view = flydra_analysis.a2.plot_top_view:main",
-            "flydra_analysis_print_camera_summary = flydra_analysis.analysis.flydra_analysis_print_camera_summary:main",
-            "flydra_analysis_save_movies_overlay = flydra_analysis.a2.save_movies_overlay:main",
-            "flydra_images_export = flydra_analysis.a2.flydra_images_export:main",
-            "kdviewer = flydra_analysis.a2.kdviewer:main",
-            "kdmovie_saver = flydra_analysis.a2.kdmovie_saver:main",
-            "flydra_analysis_data2smoothed = flydra_analysis.a2.data2smoothed:main",
-            "flydra_analysis_export_flydra_hdf5 = flydra_analysis.a2.data2smoothed:export_flydra_hdf5",
-            "flydra_textlog2csv = flydra_analysis.a2.flydra_textlog2csv:main",
-            "flydra_analysis_print_kalmanize_makefile_location = flydra_analysis.a2.print_kalmanize_makefile_location:main",
-            "flydra_analysis_calculate_reprojection_errors = flydra_analysis.a2.calculate_reprojection_errors:main",
-            "flydra_analysis_retrack_reuse_data_association = flydra_analysis.a2.retrack_reuse_data_association:main",
-            "flydra_analysis_calculate_skipped_frames = flydra_analysis.a2.calculate_skipped_frames:main",
-            "flydra_analysis_plot_skipped_frames = flydra_analysis.a2.plot_skipped_frames:main",
-            # analysis - image based orientation
-            "flydra_analysis_image_based_orientation = flydra_analysis.a2.image_based_orientation:main",
-            "flydra_analysis_orientation_ekf_fitter = flydra_analysis.a2.orientation_ekf_fitter:main",
-            "flydra_analysis_orientation_ekf_plot = flydra_analysis.a2.orientation_ekf_plot:main",
-            "flydra_analysis_orientation_is_fit = flydra_analysis.a2.orientation_ekf_fitter:is_orientation_fit_sysexit",
-            # camera calibration
-            "flydra_analysis_calibration_align_gui = flydra_analysis.a2.calibration_align_gui:main",
-            "flydra_analysis_generate_recalibration = flydra_analysis.analysis.flydra_analysis_generate_recalibration:main",
-            "flydra_analysis_plot_calibration_input = flydra_analysis.a2.plot_calibration_input:main",
-            "flydra_analysis_calibration_to_xml = flydra_analysis.a2.calibration_to_xml:main",
-            "flydra_analysis_water_surface_align = flydra_analysis.a2.water_surface_align:main",
-            "flydra_analysis_plot_camera_positions = flydra_analysis.a2.plot_camera_positions:main",
-            # ROS pointcloud stuff
-            "flydra_analysis_rosbag2flydrah5 = flydra_analysis.a2.rosbag2flydrah5:main",
-            # testing
-            "flydra_test_commands = flydra_analysis.test_commands:main",
-        ],
-        "flydra_analysis.kdviewer.plugins": [
-            "default = flydra_analysis.a2.conditions_draw:default",
-            "mama07 = flydra_analysis.a2.conditions_draw:mama07",
-            "mama20080414 = flydra_analysis.a2.conditions_draw:mama20080414",
-            "mama20080501 = flydra_analysis.a2.conditions_draw:mama20080501",
-            "hum07 = flydra_analysis.a2.conditions_draw:hum07",
-            "wt0803 = flydra_analysis.a2.conditions_draw:wt0803",
-        ],
-    },
-    package_data={
-        "flydra_analysis.a2": [
-            "kdmovie_saver_default_path.kmp",
-            "sample_*.h5",
-            "sample_*.mat",
-            "sample_calibration.xml",
-            "Makefile.kalmanize",
-        ],
-    },
-)
+[project]
+name = "flydra_analysis"
+version = "0.7.15"                     # keep in sync with flydra_analysis/version.py
+description = "fflydra analysis tools"
+readme = "README.md"
+requires-python = ">= 3.8"
+#license.file = "LICENSE-MIT" and "LICENSE-APACHE"
+authors = [{ name = "Andrew Straw", email = "strawman@astraw.com" }]
+maintainers = [{ name = "Andrew Straw", email = "strawman@astraw.com" }]
+
+urls.homepage = "https://github.com/strawlab/flydra"
+
+dependencies = [
+    "setuptools >= 44.1",
+    "numpy >= 1.19",
+    "cython>=0.26",
+
+    "cgkit1 >= 1.3.0",
+    "flydra_core",
+    "imageio",
+    "pytest",
+    "pycairo",
+    "matplotlib",
+    "multicamselfcal >= 0.2.1",
+    "pymvg >= 2.1.0",
+    "progressbar",
+    "motmot.FlyMovieFormat",
+    "motmot.ufmf",
+    "motmot.imops",
+    "h5py",
+    "pandas",
+    "traits",
+    "traitsui",
+    "pillow",
+    "aggdraw",
+    "PyYAML",
+    "sympy",
+    "cherrypy",
+]
+
+[project.scripts]
+# analysis - re-kalmanize
+flydra_kalmanize = "flydra_analysis.kalmanize:main"
+# analysis - ufmf care and feeding
+flydra_analysis_auto_discover_ufmfs = "flydra_analysis.a2.auto_discover_ufmfs:main"
+flydra_analysis_montage_ufmfs = "flydra_analysis.a2.montage_ufmfs:main"
+flydra_analysis_retrack_movies = "flydra_analysis.a2.retrack_movies:main"
+# analysis - generate movies with tracking overlays (uses fmfs or ufmfs)
+flydra_analysis_overlay_kalman_movie = "flydra_analysis.a2.overlay_kalman_movie:main"
+# analysis - .h5 file care and feeding
+flydra_analysis_check_sync = "flydra_analysis.kalmanize:check_sync"
+flydra_analysis_print_h5_info = "flydra_analysis.a2.h5_info:cmdline"
+flydra_analysis_filter_kalman_data = "flydra_analysis.analysis.flydra_analysis_filter_kalman_data:main"
+flydra_analysis_h5_shorten = "flydra_analysis.a2.h5_shorten:main"
+flydra_analysis_check_mainbrain_h5_contiguity = "flydra_analysis.a2.check_mainbrain_h5_contiguity:main"
+flydra_analysis_get_clock_sync = "flydra_analysis.a2.get_clock_sync:main"
+flydra_analysis_get_2D_image_latency = "flydra_analysis.a2.get_2D_image_latency:main"
+flydra_analysis_get_2D_image_latency_plot = "flydra_analysis.a2.get_2D_image_latency_plot:main"
+# timestamp conversion
+flydra_analysis_frame2timestamp = "flydra_analysis.analysis.result_utils:frame2timestamp_command"
+flydra_analysis_timestamp2frame = "flydra_analysis.analysis.result_utils:timestamp2frame_command"
+# analysis - not yet classified
+flydra_analysis_convert_to_mat = "flydra_analysis.analysis.flydra_analysis_convert_to_mat:main"
+flydra_analysis_plot_clock_drift = "flydra_analysis.analysis.flydra_analysis_plot_clock_drift:main"
+flydra_analysis_plot_kalman_2d = "flydra_analysis.a2.plot_kalman_2d:main"
+flydra_analysis_plot_summary = "flydra_analysis.a2.plot_summary:main"
+flydra_analysis_plot_timeseries_2d_3d = "flydra_analysis.a2.plot_timeseries_2d_3d:main"
+flydra_analysis_plot_timeseries_3d = "flydra_analysis.a2.plot_timeseries:main"
+flydra_analysis_plot_top_view = "flydra_analysis.a2.plot_top_view:main"
+flydra_analysis_print_camera_summary = "flydra_analysis.analysis.flydra_analysis_print_camera_summary:main"
+flydra_analysis_save_movies_overlay = "flydra_analysis.a2.save_movies_overlay:main"
+flydra_images_export = "flydra_analysis.a2.flydra_images_export:main"
+kdviewer = "flydra_analysis.a2.kdviewer:main"
+kdmovie_saver = "flydra_analysis.a2.kdmovie_saver:main"
+flydra_analysis_data2smoothed = "flydra_analysis.a2.data2smoothed:main"
+flydra_analysis_export_flydra_hdf5 = "flydra_analysis.a2.data2smoothed:export_flydra_hdf5"
+flydra_textlog2csv = "flydra_analysis.a2.flydra_textlog2csv:main"
+flydra_analysis_print_kalmanize_makefile_location = "flydra_analysis.a2.print_kalmanize_makefile_location:main"
+flydra_analysis_calculate_reprojection_errors = "flydra_analysis.a2.calculate_reprojection_errors:main"
+flydra_analysis_retrack_reuse_data_association = "flydra_analysis.a2.retrack_reuse_data_association:main"
+flydra_analysis_calculate_skipped_frames = "flydra_analysis.a2.calculate_skipped_frames:main"
+flydra_analysis_plot_skipped_frames = "flydra_analysis.a2.plot_skipped_frames:main"
+# analysis - image based orientation
+flydra_analysis_image_based_orientation = "flydra_analysis.a2.image_based_orientation:main"
+flydra_analysis_orientation_ekf_fitter = "flydra_analysis.a2.orientation_ekf_fitter:main"
+flydra_analysis_orientation_ekf_plot = "flydra_analysis.a2.orientation_ekf_plot:main"
+flydra_analysis_orientation_is_fit = "flydra_analysis.a2.orientation_ekf_fitter:is_orientation_fit_sysexit"
+# camera calibration
+flydra_analysis_calibration_align_gui = "flydra_analysis.a2.calibration_align_gui:main"
+flydra_analysis_generate_recalibration = "flydra_analysis.analysis.flydra_analysis_generate_recalibration:main"
+flydra_analysis_plot_calibration_input = "flydra_analysis.a2.plot_calibration_input:main"
+flydra_analysis_calibration_to_xml = "flydra_analysis.a2.calibration_to_xml:main"
+flydra_analysis_water_surface_align = "flydra_analysis.a2.water_surface_align:main"
+flydra_analysis_plot_camera_positions = "flydra_analysis.a2.plot_camera_positions:main"
+# ROS pointcloud stuff
+flydra_analysis_rosbag2flydrah5 = "flydra_analysis.a2.rosbag2flydrah5:main"
+# testing
+flydra_test_commands = "flydra_analysis.test_commands:main"
+
+[project.entry-points."flydra_analysis.kdviewer.plugins"]
+default = "flydra_analysis.a2.conditions_draw:default"
+mama07 = "flydra_analysis.a2.conditions_draw:mama07"
+mama20080414 = "flydra_analysis.a2.conditions_draw:mama20080414"
+mama20080501 = "flydra_analysis.a2.conditions_draw:mama20080501"
+hum07 = "flydra_analysis.a2.conditions_draw:hum07"
+wt0803 = "flydra_analysis.a2.conditions_draw:wt0803"
+
+[build-system]
+# following advice in https://stackoverflow.com/a/66479252
+requires = ["setuptools >= 61", "cython >= 0.29", "numpy"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+include-package-data = false
+
+[tool.setuptools.package-data]
+"flydra_analysis.a2" = [
+    "kdmovie_saver_default_path.kmp",
+    "sample_*.h5",
+    "sample_calibration.xml",
+    "Makefile.kalmanize",
+]
+
+[tool.pytest.ini_options]
+addopts = ["--doctest-modules", "--doctest-ignore-import-errors"]
+python_files = [
+    "flydra_analysis/talign.py",
+    "flydra_analysis/test_geom.py",
+    "flydra_analysis/a2/core_analysis.py",
+    "flydra_analysis/a2/utils.py",
+    "flydra_analysis/a2/benu.py",
+    "flydra_analysis/a2/pos_ori2fu.py",
+    "flydra_analysis/analysis/circstats.py",
+    "flydra_analysis/analysis/result_utils.py",
+    "flydra_analysis/analysis/PQmath.py",
+    "flydra_analysis/analysis/calc_forces.py",
+]
```

### Comparing `flydra_analysis-0.7.14/tests/test_calculate_reprojection_errors.py` & `flydra_analysis-0.7.15/tests/test_calculate_reprojection_errors.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/tests/test_calibration_realignment.py` & `flydra_analysis-0.7.15/tests/test_calibration_realignment.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/tests/test_export_flydra_hdf5.py` & `flydra_analysis-0.7.15/tests/test_export_flydra_hdf5.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/tests/test_previously_failing.py` & `flydra_analysis-0.7.15/tests/test_previously_failing.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/tests/test_pymvg.py` & `flydra_analysis-0.7.15/tests/test_pymvg.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/tests/test_reconstruct.py` & `flydra_analysis-0.7.15/tests/test_reconstruct.py`

 * *Files identical despite different names*

### Comparing `flydra_analysis-0.7.14/tests/test_result_utils.py` & `flydra_analysis-0.7.15/tests/test_result_utils.py`

 * *Files identical despite different names*

