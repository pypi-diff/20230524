# Comparing `tmp/dtscalibration-1.2.0.tar.gz` & `tmp/dtscalibration-2.0.0.tar.gz`

## Comparing `dtscalibration-1.2.0.tar` & `dtscalibration-2.0.0.tar`

### file list

```diff
@@ -1,156 +1,155 @@
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.bumpversion.cfg
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.coveragerc
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.editorconfig
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.readthedocs.yml
--rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.style.yapf
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.zenodo.json
--rw-r--r--   0        0        0    10057 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/CITATION.cff
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/MANIFEST.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/_config.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/authors.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/changelog.rst
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/contributing.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/index.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/installation.rst
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/learn_by_examples.rst
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/nb_examples_to_docs.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/readme.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/requirements.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/usage.rst
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.DataStore.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.check_dims.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.check_timestep_allclose.rst
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.get_netcdf_encoding.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.merge_double_ended.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.open_datastore.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.open_mf_datastore.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_accuracy.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_location_residuals_double_ended.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_residuals_reference_sections.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_residuals_reference_sections_single.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.plot_sigma_report.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_apsensing_files.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_sensornet_files.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_sensortran_files.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.read_silixa_files.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.shift_double_ended.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/api/dtscalibration.suggest_cable_shift_double_ended.rst
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/01Load_xml_measurement_files.ipynb
--rw-r--r--   0        0        0    11008 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/03Define_sections.ipynb
--rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/04Calculate_variance_Stokes.ipynb
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/05Calibrate_single_ols.ipynb
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/06Calibrate_double_ols.ipynb
--rw-r--r--   0        0        0    11287 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/07Calibrate_single_wls.ipynb
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/08Calibrate_double_wls.ipynb
--rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/09Import_timeseries.ipynb
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/10Align_double_ended_measurements.ipynb
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/11Merge_single_measurements_into_double.ipynb
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/12Datastore_from_numpy_arrays.ipynb
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/13Fixed_parameter_calibration.ipynb
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/14Lossy_splices.ipynb
--rw-r--r--   0        0        0     7531 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/15Matching_sections.ipynb
--rw-r--r--   0        0        0    15828 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/16Averaging_temperatures.ipynb
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/A2Load_sensornet_files.ipynb
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/A3Load_ap_sensing_files.ipynb
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/notebooks/A4Load_sensortran_files.ipynb
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/docs/reference/index.rst
--rw-r--r--   0        0        0    63280 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/Added uncertainty from fixing parameters.pdf
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/README.md
--rw-r--r--   0        0        0   133564 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/temperature_variance_from_stokes.pdf
--rw-r--r--   0        0        0  1407624 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/conference presentations/EGU2019_poster_dtscalibration.pdf
--rw-r--r--   0        0        0  2086568 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/__init__.py
--rw-r--r--   0        0        0    51325 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/calibrate_utils.py
--rw-r--r--   0        0        0   241203 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/datastore.py
--rw-r--r--   0        0        0    12525 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/datastore_utils.py
--rw-r--r--   0        0        0    60445 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/io.py
--rwxr-xr-x   0        0        0    24378 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/src/dtscalibration/plot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/test_datastore.py
--rw-r--r--   0        0        0   116952 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/test_dtscalibration.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/test_examples.py
--rw-r--r--   0        0        0   677982 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
--rw-r--r--   0        0        0   678035 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
--rw-r--r--   0        0        0   678009 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
--rwxr-xr-x   0        0        0   171342 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112245510.xml
--rwxr-xr-x   0        0        0   171341 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112746818.xml
--rwxr-xr-x   0        0        0   171310 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921113248085.xml
--rwxr-xr-x   0        0        0   129624 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014052498.xml
--rwxr-xr-x   0        0        0   129585 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014057119.xml
--rwxr-xr-x   0        0        0   129431 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014101652.xml
--rwxr-xr-x   0        0        0   129452 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014106243.xml
--rwxr-xr-x   0        0        0   129559 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014110917.xml
--rwxr-xr-x   0        0        0   129482 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014115480.xml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_ended2/info.txt
--rw-r--r--   0        0        0   436539 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
--rw-r--r--   0        0        0   436736 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
--rw-r--r--   0        0        0   436525 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
--rw-r--r--   0        0        0   436669 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
--rw-r--r--   0        0        0   436527 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
--rw-r--r--   0        0        0   436478 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
--rw-r--r--   0        0        0   436371 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
--rw-r--r--   0        0        0   436475 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
--rw-r--r--   0        0        0   436421 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
--rw-r--r--   0        0        0   436359 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
--rw-r--r--   0        0        0   436400 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
--rw-r--r--   0        0        0   436238 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
--rwxr-xr-x   0        0        0    20057 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
--rwxr-xr-x   0        0        0    20028 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
--rwxr-xr-x   0        0        0    20086 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
--rw-r--r--   0        0        0    47136 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
--rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
--rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
--rw-r--r--   0        0        0    47107 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
--rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
--rw-r--r--   0        0        0    64983 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
--rw-r--r--   0        0        0    65031 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
--rw-r--r--   0        0        0    65017 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
--rw-r--r--   0        0        0    65058 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
--rw-r--r--   0        0        0    65029 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
--rw-r--r--   0        0        0    65043 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
--rw-r--r--   0        0        0    65018 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
--rw-r--r--   0        0        0    48160 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
--rw-r--r--   0        0        0    48206 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
--rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
--rw-r--r--   0        0        0    48174 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
--rw-r--r--   0        0        0    48163 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
--rw-r--r--   0        0        0   126331 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
--rw-r--r--   0        0        0   126323 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
--rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
--rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
--rw-r--r--   0        0        0   164764 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
--rw-r--r--   0        0        0   164730 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
--rw-r--r--   0        0        0   164757 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
--rw-r--r--   0        0        0   164679 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
--rw-r--r--   0        0        0   164785 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
--rw-r--r--   0        0        0   164691 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
--rw-r--r--   0        0        0   164784 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
--rw-r--r--   0        0        0   215137 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
--rw-r--r--   0        0        0   215082 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
--rw-r--r--   0        0        0   215091 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
--rw-r--r--   0        0        0   215114 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
--rw-r--r--   0        0        0   215119 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
--rw-r--r--   0        0        0   286652 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
--rwxr-xr-x   0        0        0    88932 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132202074.xml
--rwxr-xr-x   0        0        0    88936 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132232903.xml
--rwxr-xr-x   0        0        0    88888 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132303723.xml
--rw-r--r--   0        0        0   166974 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/double_ended.zip
--rw-r--r--   0        0        0   255063 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/double_ended2.zip
--rw-r--r--   0        0        0  1508174 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/double_single_ended.zip
--rw-r--r--   0        0        0   260862 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/silixa_v4.5.zip
--rw-r--r--   0        0        0    78779 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/tests/data/zipped data/single_ended.zip
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/.gitignore
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/AUTHORS.rst
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/LICENSE
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/README.rst
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 dtscalibration-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/.coveragerc
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/.editorconfig
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/.style.yapf
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/.zenodo.json
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/CITATION.cff
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/_config.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/authors.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/contributing.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/index.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/installation.rst
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/learn_by_examples.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/nb_examples_to_docs.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/readme.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/usage.rst
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.DataStore.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.check_dims.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.check_timestep_allclose.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.get_netcdf_encoding.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.merge_double_ended.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.open_datastore.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.open_mf_datastore.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.plot_accuracy.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.plot_location_residuals_double_ended.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.plot_residuals_reference_sections.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.plot_residuals_reference_sections_single.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.plot_sigma_report.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.read_apsensing_files.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.read_sensornet_files.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.read_sensortran_files.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.read_silixa_files.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.shift_double_ended.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/api/dtscalibration.suggest_cable_shift_double_ended.rst
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/01Load_xml_measurement_files.ipynb
+-rw-r--r--   0        0        0    11090 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/03Define_sections.ipynb
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/04Calculate_variance_Stokes.ipynb
+-rw-r--r--   0        0        0     9932 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/07Calibrate_single_ended.ipynb
+-rw-r--r--   0        0        0    16708 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/08Calibrate_double_ended.ipynb
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/09Import_timeseries.ipynb
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/10Align_double_ended_measurements.ipynb
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/11Merge_single_measurements_into_double.ipynb
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/12Datastore_from_numpy_arrays.ipynb
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/13Fixed_parameter_calibration.ipynb
+-rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/14Lossy_splices.ipynb
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/15Matching_sections.ipynb
+-rw-r--r--   0        0        0    15898 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/16Averaging_temperatures.ipynb
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/17Temperature_uncertainty_single_ended.ipynb
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/A2Load_sensornet_files.ipynb
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/A3Load_ap_sensing_files.ipynb
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/notebooks/A4Load_sensortran_files.ipynb
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/docs/reference/index.rst
+-rw-r--r--   0        0        0    63280 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/examples/Added uncertainty from fixing parameters.pdf
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/examples/README.md
+-rw-r--r--   0        0        0   133564 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/examples/temperature_variance_from_stokes.pdf
+-rw-r--r--   0        0        0  1407624 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/examples/conference presentations/EGU2019_poster_dtscalibration.pdf
+-rw-r--r--   0        0        0  2086568 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/src/dtscalibration/__init__.py
+-rw-r--r--   0        0        0    50487 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/src/dtscalibration/calibrate_utils.py
+-rw-r--r--   0        0        0   265508 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/src/dtscalibration/datastore.py
+-rw-r--r--   0        0        0    12525 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/src/dtscalibration/datastore_utils.py
+-rw-r--r--   0        0        0    62926 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/src/dtscalibration/io.py
+-rwxr-xr-x   0        0        0    24378 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/src/dtscalibration/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/test_datastore.py
+-rw-r--r--   0        0        0   110455 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/test_dtscalibration.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/test_examples.py
+-rw-r--r--   0        0        0   677982 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml
+-rw-r--r--   0        0        0   678035 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml
+-rw-r--r--   0        0        0   678009 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml
+-rwxr-xr-x   0        0        0   171342 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended/channel 1_20170921112245510.xml
+-rwxr-xr-x   0        0        0   171341 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended/channel 1_20170921112746818.xml
+-rwxr-xr-x   0        0        0   171310 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended/channel 1_20170921113248085.xml
+-rwxr-xr-x   0        0        0   129624 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014052498.xml
+-rwxr-xr-x   0        0        0   129585 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014057119.xml
+-rwxr-xr-x   0        0        0   129431 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014101652.xml
+-rwxr-xr-x   0        0        0   129452 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014106243.xml
+-rwxr-xr-x   0        0        0   129559 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014110917.xml
+-rwxr-xr-x   0        0        0   129482 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014115480.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_ended2/info.txt
+-rw-r--r--   0        0        0   436539 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml
+-rw-r--r--   0        0        0   436736 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml
+-rw-r--r--   0        0        0   436525 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml
+-rw-r--r--   0        0        0   436669 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml
+-rw-r--r--   0        0        0   436527 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml
+-rw-r--r--   0        0        0   436478 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml
+-rw-r--r--   0        0        0   436371 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml
+-rw-r--r--   0        0        0   436475 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml
+-rw-r--r--   0        0        0   436421 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml
+-rw-r--r--   0        0        0   436359 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml
+-rw-r--r--   0        0        0   436400 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml
+-rw-r--r--   0        0        0   436238 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml
+-rwxr-xr-x   0        0        0    20057 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv
+-rwxr-xr-x   0        0        0    20028 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv
+-rwxr-xr-x   0        0        0    20086 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv
+-rw-r--r--   0        0        0    47136 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf
+-rw-r--r--   0        0        0    47126 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf
+-rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf
+-rw-r--r--   0        0        0    47107 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf
+-rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf
+-rw-r--r--   0        0        0    64983 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf
+-rw-r--r--   0        0        0    65031 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf
+-rw-r--r--   0        0        0    65017 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf
+-rw-r--r--   0        0        0    65058 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf
+-rw-r--r--   0        0        0    65029 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf
+-rw-r--r--   0        0        0    65043 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf
+-rw-r--r--   0        0        0    65018 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf
+-rw-r--r--   0        0        0    48160 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf
+-rw-r--r--   0        0        0    48206 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf
+-rw-r--r--   0        0        0    48196 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf
+-rw-r--r--   0        0        0    48174 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf
+-rw-r--r--   0        0        0    48163 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf
+-rw-r--r--   0        0        0   126331 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf
+-rw-r--r--   0        0        0   126323 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat
+-rw-r--r--   0        0        0    96176 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat
+-rw-r--r--   0        0        0    92832 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat
+-rw-r--r--   0        0        0   164764 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml
+-rw-r--r--   0        0        0   164730 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml
+-rw-r--r--   0        0        0   164757 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml
+-rw-r--r--   0        0        0   164679 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml
+-rw-r--r--   0        0        0   164785 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml
+-rw-r--r--   0        0        0   164691 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml
+-rw-r--r--   0        0        0   164784 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml
+-rw-r--r--   0        0        0   215137 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml
+-rw-r--r--   0        0        0   215082 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml
+-rw-r--r--   0        0        0   215091 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml
+-rw-r--r--   0        0        0   215114 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml
+-rw-r--r--   0        0        0   215119 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml
+-rw-r--r--   0        0        0   286652 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml
+-rwxr-xr-x   0        0        0    88932 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/single_ended/channel 2_20180504132202074.xml
+-rwxr-xr-x   0        0        0    88936 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/single_ended/channel 2_20180504132232903.xml
+-rwxr-xr-x   0        0        0    88888 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/single_ended/channel 2_20180504132303723.xml
+-rw-r--r--   0        0        0   166974 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/zipped data/double_ended.zip
+-rw-r--r--   0        0        0   255063 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/zipped data/double_ended2.zip
+-rw-r--r--   0        0        0  1508174 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/zipped data/double_single_ended.zip
+-rw-r--r--   0        0        0   260862 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/zipped data/silixa_v4.5.zip
+-rw-r--r--   0        0        0    78779 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/tests/data/zipped data/single_ended.zip
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/.gitignore
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/README.rst
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 dtscalibration-2.0.0/PKG-INFO
```

### Comparing `dtscalibration-1.2.0/.style.yapf` & `dtscalibration-2.0.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/.zenodo.json` & `dtscalibration-2.0.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/CHANGELOG.rst` & `dtscalibration-2.0.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 
 Changelog
 =========
-[1.2.0] (13-03-2023)
 
+2.0.0 (2023-05-24)
+------------------
+
+* Faster approach on error propagation. As alternative to computational intensive Monte Carlo runs.
+* Refractored some of the indexing logic of the calibration routines.
+* Rewritten single-ended and double-ended example notebooks.
+* Removed support for OLS calibration, as with minor extra efforts WLS could be used, which has significant benefits.
+
+1.2.0 (2023-03-13)
+------------------
 Bugfixes
 
 * Fixed deprecated np.float and np.int
 
 Other
 
 * Moved project build system & scripts to hatch.
```

### Comparing `dtscalibration-1.2.0/CITATION.cff` & `dtscalibration-2.0.0/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,9 @@
   - calibration
   - Python
 cff-version: "1.0.3"
 doi: "10.5281/zenodo.1410097"
 license: "BSD-3-Clause"
 repository-code: "https://github.com/dtscalibration/python-dts-calibration"
 title: "Python distributed temperature sensing calibration"
-version: "v1.2.0"
+version: "v2.0.0"
 url: "https://python-dts-calibration.readthedocs.io"
```

### Comparing `dtscalibration-1.2.0/CONTRIBUTING.rst` & `dtscalibration-2.0.0/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
 4. Activate your desired development environment (e.g., a python venv or conda environment), and install the package in editable mode, with the dev dependencies::
 
-    pip install -e .[dev]
+    pip install -e ".[dev]"
+
 
 4. When you're done making changes, make sure the code follows the right style, that all tests pass, and that the docs build with the following commands::
 
     hatch run format
     hatch run test
     hatch run docs:build
```

### Comparing `dtscalibration-1.2.0/MANIFEST.in` & `dtscalibration-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/docs/conf.py` & `dtscalibration-2.0.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 source_suffix = ['.rst', '.md']
 master_doc = 'index'
 project = 'dtscalibration'
 year = str(date.today().year)
 author = 'Bas des Tombe and Bart Schilperoort'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '1.2.0'
+version = release = '2.0.0'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/dtscalibration/python-dts-calibration/issues'
               '/%s', '#'),
     'pr': ('https://github.com/dtscalibration/python-dts-calibration/pull/%s',
```

### Comparing `dtscalibration-1.2.0/docs/learn_by_examples.rst` & `dtscalibration-2.0.0/docs/learn_by_examples.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/docs/nb_examples_to_docs.py` & `dtscalibration-2.0.0/docs/nb_examples_to_docs.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/docs/api/dtscalibration.DataStore.rst` & `dtscalibration-2.0.0/docs/api/dtscalibration.DataStore.rst`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/docs/notebooks/01Load_xml_measurement_files.ipynb` & `dtscalibration-2.0.0/docs/notebooks/01Load_xml_measurement_files.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977813852813853%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(0, \'filepath = os.path.join("..", "..", "tests", "data", '*

 * *            '"double_ended2")\\n\')], delete: [0]}}, 4: {\'source\': {insert: [(1, \'filepathlist '*

 * *            '= sorted(glob.glob(os.path.join(filepath, "*.xml")))\\n\')], delete: [1]}}, 6: '*

 * *            '{\'source\': [\'ds = read_silixa_files(directory=filepath, timezone_netcdf="UTC", '*

 * *            'file_ext="*.xml")\']}}'}*

```diff
@@ -51,15 +51,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:48.304776Z",
                     "iopub.status.idle": "2022-04-06T08:08:48.308162Z",
                     "shell.execute_reply": "2022-04-06T08:08:48.307655Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
                 "print(filepath)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -69,15 +69,15 @@
                     "iopub.status.idle": "2022-04-06T08:08:48.335864Z",
                     "shell.execute_reply": "2022-04-06T08:08:48.335260Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# Bonus: Just to show which files are in the folder\n",
-                "filepathlist = sorted(glob.glob(os.path.join(filepath, '*.xml')))\n",
+                "filepathlist = sorted(glob.glob(os.path.join(filepath, \"*.xml\")))\n",
                 "filenamelist = [os.path.basename(path) for path in filepathlist]\n",
                 "\n",
                 "for fn in filenamelist:\n",
                 "    print(fn)"
             ]
         },
         {
@@ -96,17 +96,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:48.337960Z",
                     "iopub.status.idle": "2022-04-06T08:08:48.648874Z",
                     "shell.execute_reply": "2022-04-06T08:08:48.648058Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds = read_silixa_files(directory=filepath,\n",
-                "                       timezone_netcdf='UTC',\n",
-                "                       file_ext='*.xml')"
+                "ds = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The object tries to gather as much metadata from the measurement files as possible (temporal and spatial coordinates, filenames, temperature probes measurements). All other configuration settings are loaded from the first files and stored as attributes of the `DataStore`."
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb` & `dtscalibration-2.0.0/docs/notebooks/02Common_DataStore_functions_slice_mean_max_std_resample.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946846382783883%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(0, \'filepath = os.path.join("..", "..", "tests", "data", '*

 * *            '"single_ended")\\n\'), (2, \'ds = read_silixa_files(directory=filepath, '*

 * *            'timezone_netcdf="UTC", file_ext="*.xml")\')], delete: [5, 4, 3, 2, 0]}}, 5: '*

 * *            '{\'source\': [\'ds["st"]  # is the data stored, presented as a DataArray\']}, 6: '*

 * *            '{\'source\': [\'ds["tmp"].plot(figsize=(12, 8));\']}, 8: {\'source\': [\'ds_min = '*

 * *            'ds.mean(\\n\', \'    dim="t […]*

```diff
@@ -48,20 +48,17 @@
                     "iopub.status.busy": "2022-04-06T08:08:58.947893Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.145387Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.144710Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'single_ended')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"single_ended\")\n",
                 "\n",
-                "ds = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')"
+                "ds = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 0 Access the data\n",
@@ -77,15 +74,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.170926Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.201341Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.200765Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds['st']  # is the data stored, presented as a DataArray"
+                "ds[\"st\"]  # is the data stored, presented as a DataArray"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -93,15 +90,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.203591Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.265177Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.264679Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds['tmp'].plot(figsize=(12, 8));"
+                "ds[\"tmp\"].plot(figsize=(12, 8));"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 1 mean, min, max\n",
@@ -121,15 +118,17 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.267493Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.273319Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.272886Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds_min = ds.mean(dim='time', keep_attrs=True)  # take the minimum of all data variables (e.g., Stokes, Temperature) along the time dimension"
+                "ds_min = ds.mean(\n",
+                "    dim=\"time\", keep_attrs=True\n",
+                ")  # take the minimum of all data variables (e.g., Stokes, Temperature) along the time dimension"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -137,15 +136,17 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.275507Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.279270Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.278851Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds_max = ds.max(dim='x', keep_attrs=True)  # Take the maximum of all data variables (e.g., Stokes, Temperature) along the x dimension"
+                "ds_max = ds.max(\n",
+                "    dim=\"x\", keep_attrs=True\n",
+                ")  # Take the maximum of all data variables (e.g., Stokes, Temperature) along the x dimension"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -153,15 +154,17 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.281321Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.287525Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.286991Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds_std = ds.std(dim='time', keep_attrs=True)  # Calculate the standard deviation along the time dimension"
+                "ds_std = ds.std(\n",
+                "    dim=\"time\", keep_attrs=True\n",
+                ")  # Calculate the standard deviation along the time dimension"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 2 Selecting\n",
@@ -177,15 +180,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.289877Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.293824Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.293152Z"
                 }
             },
             "outputs": [],
             "source": [
-                "section = slice(20., 35.)\n",
+                "section = slice(20.0, 35.0)\n",
                 "section_of_interest = ds.sel(x=section)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -194,15 +197,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.295850Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.299802Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.299282Z"
                 }
             },
             "outputs": [],
             "source": [
-                "section_of_interest_max = section_of_interest.max(dim='x')"
+                "section_of_interest_max = section_of_interest.max(dim=\"x\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "What if you would like to have the measurement at approximately $x=20$ m?"
@@ -217,15 +220,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.301950Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.306081Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.305484Z"
                 }
             },
             "outputs": [],
             "source": [
-                "point_of_interest = ds.sel(x=20., method='nearest')"
+                "point_of_interest = ds.sel(x=20.0, method=\"nearest\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 3 Selecting by index\n",
@@ -282,15 +285,15 @@
                     "iopub.status.busy": "2022-04-06T08:08:59.320029Z",
                     "iopub.status.idle": "2022-04-06T08:08:59.341833Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.341341Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds_resampled = ds.resample_datastore(how='mean', time=\"47S\")"
+                "ds_resampled = ds.resample_datastore(how=\"mean\", time=\"47S\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## 5 Upsample / Interpolation (length and time dimension)\n",
@@ -307,16 +310,16 @@
                     "iopub.status.idle": "2022-04-06T08:08:59.353186Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.352734Z"
                 }
             },
             "outputs": [],
             "source": [
                 "x_old = ds.x.data\n",
-                "x_new = x_old[:-1] + 0.05 # no extrapolation\n",
-                "ds_xinterped = ds.interp(coords={'x': x_new})"
+                "x_new = x_old[:-1] + 0.05  # no extrapolation\n",
+                "ds_xinterped = ds.interp(coords={\"x\": x_new})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can do the same in the time dimension"
@@ -332,17 +335,18 @@
                     "iopub.status.idle": "2022-04-06T08:08:59.371585Z",
                     "shell.execute_reply": "2022-04-06T08:08:59.371063Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
+                "\n",
                 "time_old = ds.time.data\n",
-                "time_new = time_old + np.timedelta64(10, 's')\n",
-                "ds_tinterped = ds.interp(coords={'time': time_new})"
+                "time_new = time_old + np.timedelta64(10, \"s\")\n",
+                "ds_tinterped = ds.interp(coords={\"time\": time_new})"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/03Define_sections.ipynb` & `dtscalibration-2.0.0/docs/notebooks/03Define_sections.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974826388888889%*

 * *Differences: {"'cells'": '{2: {\'source\': [\'filepath = os.path.join("..", "..", "tests", "data", '*

 * *            '"double_ended2")\\n\', \'ds = read_silixa_files(directory=filepath, '*

 * *            'timezone_netcdf="UTC", file_ext="*.xml")\']}, 4: {\'source\': {insert: [(0, '*

 * *            "'print(ds.timeseries_keys)  # list the available timeseeries\\n')], delete: [0]}}, 8: "*

 * *            '{\'source\': {insert: [(1, \'    "probe1Temperature": [slice(7.5, 17.0), slice(70.0, '*

 * *            '80.0)],  # cold bath\\n\'), (2, \'   […]*

```diff
@@ -35,19 +35,16 @@
                     "iopub.status.busy": "2022-04-06T08:09:09.855138Z",
                     "iopub.status.idle": "2022-04-06T08:09:10.207557Z",
                     "shell.execute_reply": "2022-04-06T08:09:10.204867Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
-                "ds = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')"
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
+                "ds = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "First we have a look at which temperature timeseries are available for calibration. Therefore we access `ds.data_vars` and we find `probe1Temperature` and `probe2Temperature` that refer to the temperature measurement timeseries of the two probes attached to the Ultima.\n",
@@ -64,15 +61,15 @@
                     "iopub.status.busy": "2022-04-06T08:09:10.210555Z",
                     "iopub.status.idle": "2022-04-06T08:09:10.276848Z",
                     "shell.execute_reply": "2022-04-06T08:09:10.275933Z"
                 }
             },
             "outputs": [],
             "source": [
-                "print(ds.timeseries_keys)    # list the available timeseeries\n",
+                "print(ds.timeseries_keys)  # list the available timeseeries\n",
                 "ds.probe1Temperature.plot(figsize=(12, 8));  # plot one of the timeseries"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -112,17 +109,17 @@
                     "iopub.status.idle": "2022-04-06T08:09:10.306041Z",
                     "shell.execute_reply": "2022-04-06T08:09:10.305366Z"
                 }
             },
             "outputs": [],
             "source": [
                 "sections = {\n",
-                "    'probe1Temperature': [slice(7.5, 17.), slice(70., 80.)],  # cold bath\n",
-                "    'probe2Temperature': [slice(24., 34.), slice(85., 95.)],  # warm bath\n",
-                "    }\n",
+                "    \"probe1Temperature\": [slice(7.5, 17.0), slice(70.0, 80.0)],  # cold bath\n",
+                "    \"probe2Temperature\": [slice(24.0, 34.0), slice(85.0, 95.0)],  # warm bath\n",
+                "}\n",
                 "ds.sections = sections"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/04Calculate_variance_Stokes.ipynb` & `dtscalibration-2.0.0/docs/notebooks/04Calculate_variance_Stokes.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961778846153846%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(3, \'warnings.simplefilter("ignore")  # Hide warnings to '*

 * *            "avoid clutter in the notebook\\n'), (7, '\\n')], delete: [3]}}, 3: {'source': "*

 * *            '{insert: [(0, \'filepath = os.path.join("..", "..", "tests", "data", '*

 * *            '"double_ended2")\\n\'), (2, \'ds = read_silixa_files(directory=filepath, '*

 * *            'timezone_netcdf="UTC", file_ext="*.xml")\')], delete: [5, 4, 3, 2, 0]}}, 5: '*

 * *            '{\'source\': {insert: [(1, \'    "probe1Tem […]*

```diff
@@ -28,18 +28,19 @@
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import warnings\n",
                 "\n",
-                "warnings.simplefilter('ignore')  # Hide warnings to avoid clutter in the notebook\n",
+                "warnings.simplefilter(\"ignore\")  # Hide warnings to avoid clutter in the notebook\n",
                 "\n",
                 "from dtscalibration import read_silixa_files\n",
                 "from matplotlib import pyplot as plt\n",
+                "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -48,20 +49,17 @@
                     "iopub.status.busy": "2022-04-06T08:09:22.074288Z",
                     "iopub.status.idle": "2022-04-06T08:09:22.384442Z",
                     "shell.execute_reply": "2022-04-06T08:09:22.383910Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
                 "\n",
-                "ds = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')"
+                "ds = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "And we define the sections as we learned from the previous notebook. Sections are required to calculate the variance in the Stokes."
@@ -77,17 +75,17 @@
                     "iopub.status.idle": "2022-04-06T08:09:22.407332Z",
                     "shell.execute_reply": "2022-04-06T08:09:22.406738Z"
                 }
             },
             "outputs": [],
             "source": [
                 "sections = {\n",
-                "    'probe1Temperature': [slice(7.5, 17.), slice(70., 80.)],  # cold bath\n",
-                "    'probe2Temperature': [slice(24., 34.), slice(85., 95.)],  # warm bath\n",
-                "    }\n",
+                "    \"probe1Temperature\": [slice(7.5, 17.0), slice(70.0, 80.0)],  # cold bath\n",
+                "    \"probe2Temperature\": [slice(24.0, 34.0), slice(85.0, 95.0)],  # warm bath\n",
+                "}\n",
                 "ds.sections = sections"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -118,17 +116,21 @@
                     "iopub.status.busy": "2022-04-06T08:09:22.409845Z",
                     "iopub.status.idle": "2022-04-06T08:09:22.633926Z",
                     "shell.execute_reply": "2022-04-06T08:09:22.633317Z"
                 }
             },
             "outputs": [],
             "source": [
-                "I_var, residuals = ds.variance_stokes_constant(st_label='st')\n",
-                "print(\"The variance of the Stokes signal along the reference sections \"\n",
-                "      \"is approximately {:.2f} on a {:.1f} sec acquisition time\".format(I_var, ds.userAcquisitionTimeFW.data[0]))"
+                "I_var, residuals = ds.variance_stokes_constant(st_label=\"st\")\n",
+                "print(\n",
+                "    \"The variance of the Stokes signal along the reference sections \"\n",
+                "    \"is approximately {:.2f} on a {:.1f} sec acquisition time\".format(\n",
+                "        I_var, ds.userAcquisitionTimeFW.data[0]\n",
+                "    )\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -139,22 +141,23 @@
                 }
             },
             "outputs": [],
             "source": [
                 "from dtscalibration import plot\n",
                 "\n",
                 "fig_handle = plot.plot_residuals_reference_sections(\n",
-                "        residuals,\n",
-                "        sections,\n",
-                "        title='Distribution of the noise in the Stokes signal',\n",
-                "        plot_avg_std=I_var ** 0.5,\n",
-                "        plot_names=True,\n",
-                "        robust=True,\n",
-                "        units='',\n",
-                "        method='single')"
+                "    residuals,\n",
+                "    sections,\n",
+                "    title=\"Distribution of the noise in the Stokes signal\",\n",
+                "    plot_avg_std=I_var**0.5,\n",
+                "    plot_names=True,\n",
+                "    robust=True,\n",
+                "    units=\"\",\n",
+                "    method=\"single\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The residuals should be normally distributed and independent from previous time steps and other points along the cable. If you observe patterns in the residuals plot (above), it might be caused by:\n",
@@ -177,15 +180,15 @@
             "outputs": [],
             "source": [
                 "import scipy\n",
                 "import numpy as np\n",
                 "\n",
                 "sigma = residuals.std()\n",
                 "mean = residuals.mean()\n",
-                "x = np.linspace(mean - 3*sigma, mean + 3*sigma, 100)\n",
+                "x = np.linspace(mean - 3 * sigma, mean + 3 * sigma, 100)\n",
                 "approximated_normal_fit = scipy.stats.norm.pdf(x, mean, sigma)\n",
                 "residuals.plot.hist(bins=50, figsize=(12, 8), density=True)\n",
                 "plt.plot(x, approximated_normal_fit);"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/05Calibrate_single_ols.ipynb` & `dtscalibration-2.0.0/docs/notebooks/A2Load_sensornet_files.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8307486631016043%*

 * *Differences: {"'cells'": "{0: {'source': ['# A2. Loading sensornet files\\n', 'This example loads sensornet "*

 * *            "files. Both single-ended and double-ended measurements are supported.']}, 2: "*

 * *            "{'source': ['The example data files are located in "*

 * *            "`./python-dts-calibration/tests/data`.']}, 3: {'metadata': {'execution': "*

 * *            "{'iopub.execute_input': '2022-04-06T08:12:19.821193Z', 'iopub.status.busy': "*

 * *            "'2022-04-06T08:12:19.820976Z', 'iopub.status.idle': '2022-04-06T0 […]*

```diff
@@ -1,142 +1,152 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# 5. Calibration of single-ended measurement with OLS"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Use WLS instead. See `examples/notebooks/07Calibrate_single_wls.ipynb`.\n",
-                "\n",
-                "A double ended calibration is performed with Ordinary Least Squares. Over all timesteps simultaneous. $\\gamma$ and $\\alpha$ remain constant, while $C$ varies over time. The weights are considered equal here and no variance or confidence interval is calculated.\n",
-                "\n",
-                "Note that the internal reference section can not be used since there is a connector between the internal and external fiber and therefore the integrated differential attenuation cannot be considered to be linear anymore."
+                "# A2. Loading sensornet files\n",
+                "This example loads sensornet files. Both single-ended and double-ended measurements are supported."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:35.393302Z",
-                    "iopub.status.busy": "2022-04-06T08:09:35.392875Z",
-                    "iopub.status.idle": "2022-04-06T08:09:37.461713Z",
-                    "shell.execute_reply": "2022-04-06T08:09:37.461135Z"
+                    "iopub.execute_input": "2022-04-06T08:12:18.017157Z",
+                    "iopub.status.busy": "2022-04-06T08:12:18.016166Z",
+                    "iopub.status.idle": "2022-04-06T08:12:19.818415Z",
+                    "shell.execute_reply": "2022-04-06T08:12:19.817618Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
+                "import glob\n",
                 "\n",
-                "from dtscalibration import read_silixa_files\n",
-                "import matplotlib.pyplot as plt\n",
-                "\n",
-                "%matplotlib inline"
+                "from dtscalibration import read_sensornet_files"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The example data files are located in `./python-dts-calibration/tests/data`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:37.464466Z",
-                    "iopub.status.busy": "2022-04-06T08:09:37.464071Z",
-                    "iopub.status.idle": "2022-04-06T08:09:37.689220Z",
-                    "shell.execute_reply": "2022-04-06T08:09:37.688535Z"
+                    "iopub.execute_input": "2022-04-06T08:12:19.821193Z",
+                    "iopub.status.busy": "2022-04-06T08:12:19.820976Z",
+                    "iopub.status.idle": "2022-04-06T08:12:19.825091Z",
+                    "shell.execute_reply": "2022-04-06T08:12:19.824478Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'single_ended')\n",
-                "\n",
-                "ds = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')\n",
-                "\n",
-                "ds100 = ds.sel(x=slice(-30, 101))  # only calibrate parts of the fiber, in meters\n",
-                "sections = {\n",
-                "            'probe1Temperature':    [slice(20, 25.5)],  # warm bath\n",
-                "            'probe2Temperature':    [slice(5.5, 15.5)],  # cold bath\n",
-                "            }\n",
-                "ds100.sections = sections"
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"sensornet_oryx_v3.7\")\n",
+                "print(filepath)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:37.717941Z",
-                    "iopub.status.busy": "2022-04-06T08:09:37.717519Z",
-                    "iopub.status.idle": "2022-04-06T08:09:37.722731Z",
-                    "shell.execute_reply": "2022-04-06T08:09:37.721982Z"
+                    "iopub.execute_input": "2022-04-06T08:12:19.862591Z",
+                    "iopub.status.busy": "2022-04-06T08:12:19.862218Z",
+                    "iopub.status.idle": "2022-04-06T08:12:19.868228Z",
+                    "shell.execute_reply": "2022-04-06T08:12:19.867633Z"
                 }
             },
             "outputs": [],
             "source": [
-                "print(ds100.calibration_single_ended.__doc__)"
+                "filepathlist = sorted(glob.glob(os.path.join(filepath, \"*.ddf\")))\n",
+                "filenamelist = [os.path.basename(path) for path in filepathlist]\n",
+                "\n",
+                "for fn in filenamelist:\n",
+                "    print(fn)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We will simply load in the sensornet files. As the sensornet files are of low spatial and temporal resolution, reading the data lazily into dask is not supported."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:37.725778Z",
-                    "iopub.status.busy": "2022-04-06T08:09:37.725580Z",
-                    "iopub.status.idle": "2022-04-06T08:09:37.767953Z",
-                    "shell.execute_reply": "2022-04-06T08:09:37.767360Z"
+                    "iopub.execute_input": "2022-04-06T08:12:19.871525Z",
+                    "iopub.status.busy": "2022-04-06T08:12:19.871278Z",
+                    "iopub.status.idle": "2022-04-06T08:12:20.102791Z",
+                    "shell.execute_reply": "2022-04-06T08:12:20.102077Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds100.calibration_single_ended(method='ols')"
+                "ds = read_sensornet_files(directory=filepath)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Lets compare our calibrated values with the device calibration"
+                "The object tries to gather as much metadata from the measurement files as possible (temporal and spatial coordinates, filenames, temperature probes measurements). All other configuration settings are loaded from the first files and stored as attributes of the `DataStore`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:37.772158Z",
-                    "iopub.status.busy": "2022-04-06T08:09:37.771685Z",
-                    "iopub.status.idle": "2022-04-06T08:09:38.073557Z",
-                    "shell.execute_reply": "2022-04-06T08:09:38.073028Z"
+                    "iopub.execute_input": "2022-04-06T08:12:20.105803Z",
+                    "iopub.status.busy": "2022-04-06T08:12:20.105530Z",
+                    "iopub.status.idle": "2022-04-06T08:12:20.121624Z",
+                    "shell.execute_reply": "2022-04-06T08:12:20.120865Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds1 = ds100.isel(time=0)  # take only the first timestep\n",
+                "print(ds)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "\n",
                 "\n",
-                "ds1.tmpf.plot(linewidth=1, figsize=(12, 8), label='User calibrated')  # plot the temperature calibrated by us\n",
-                "ds1.tmp.plot(linewidth=1, label='Device calibrated')  # plot the temperature calibrated by the device\n",
-                "plt.title('Temperature at the first time step')\n",
-                "plt.legend();"
+                "Double ended sensornet files are also supported. Note the REV-ST and REV-AST data variables."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "execution": {
+                    "iopub.execute_input": "2022-04-06T08:12:20.124573Z",
+                    "iopub.status.busy": "2022-04-06T08:12:20.124284Z",
+                    "iopub.status.idle": "2022-04-06T08:12:20.285504Z",
+                    "shell.execute_reply": "2022-04-06T08:12:20.284773Z"
+                }
+            },
             "outputs": [],
-            "source": []
+            "source": [
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"sensornet_halo_v1.0\")\n",
+                "ds = read_sensornet_files(directory=filepath)\n",
+                "print(ds)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
@@ -151,9 +161,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.11"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/06Calibrate_double_ols.ipynb` & `dtscalibration-2.0.0/docs/notebooks/13Fixed_parameter_calibration.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.944187075260266%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# 13. Fixing calibration parameters\\n'), (1, 'In this "*

 * *            'notebook we will demonstrate how to fix the calibration parameters $\\\\gamma$ and '*

 * *            '$\\\\alpha$. This can be useful in setups where you have insufficient reference '*

 * *            'sections to calibrate these, but you do have information on these parameters from '*

 * *            "previous setups with the same fiber.\\n'), (3, 'We will be using the same dataset as "*

 * *            "notebook  […]*

```diff
@@ -1,195 +1,164 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# 6. Calibration of double ended measurement with OLS"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Use WLS instead. See `examples/notebooks/08Calibrate_double_wls.ipynb`.\n",
+                "# 13. Fixing calibration parameters\n",
+                "In this notebook we will demonstrate how to fix the calibration parameters $\\gamma$ and $\\alpha$. This can be useful in setups where you have insufficient reference sections to calibrate these, but you do have information on these parameters from previous setups with the same fiber.\n",
                 "\n",
-                "A double ended calibration is performed with ordinary least squares. Over all timesteps simultaneous. $\\gamma$ and $\\int_0^l\\alpha$d$x$ remain constant, while $C$ varies over time. The weights are considered equal here and no variance is calculated.\n",
-                "\n",
-                "Before starting the calibration procedure, the forward and the backward channel should be aligned."
+                "We will be using the same dataset as notebook 5. Calibration of single-ended measurement with OLS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:46.793203Z",
-                    "iopub.status.busy": "2022-04-06T08:09:46.792653Z",
-                    "iopub.status.idle": "2022-04-06T08:09:48.805880Z",
-                    "shell.execute_reply": "2022-04-06T08:09:48.805278Z"
+                    "iopub.execute_input": "2022-04-06T08:11:15.471807Z",
+                    "iopub.status.busy": "2022-04-06T08:11:15.470954Z",
+                    "iopub.status.idle": "2022-04-06T08:11:17.137093Z",
+                    "shell.execute_reply": "2022-04-06T08:11:17.136561Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "\n",
                 "from dtscalibration import read_silixa_files\n",
                 "import matplotlib.pyplot as plt\n",
-                "%matplotlib inline"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:48.808712Z",
-                    "iopub.status.busy": "2022-04-06T08:09:48.808445Z",
-                    "iopub.status.idle": "2022-04-06T08:09:49.147190Z",
-                    "shell.execute_reply": "2022-04-06T08:09:49.146093Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
                 "\n",
-                "ds = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')\n",
+                "%matplotlib inline\n",
+                "\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"single_ended\")\n",
+                "\n",
+                "ds = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")\n",
                 "\n",
-                "ds100 = ds.sel(x=slice(0, 100))  # only calibrate parts of the fiber\n",
+                "ds100 = ds.sel(x=slice(-30, 101))  # only calibrate parts of the fiber, in meters\n",
                 "sections = {\n",
-                "    'probe1Temperature': [slice(7.5, 17.), slice(70., 80.)],  # cold bath\n",
-                "    'probe2Temperature': [slice(24., 34.), slice(85., 95.)],  # warm bath\n",
-                "    }"
+                "    \"probe1Temperature\": [\n",
+                "        slice(20, 25.5)\n",
+                "    ],  # we only use the warm bath in this notebook\n",
+                "}\n",
+                "ds100.sections = sections"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:49.150289Z",
-                    "iopub.status.busy": "2022-04-06T08:09:49.150011Z",
-                    "iopub.status.idle": "2022-04-06T08:09:49.155322Z",
-                    "shell.execute_reply": "2022-04-06T08:09:49.154228Z"
-                }
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "print(ds100.calibration_double_ended.__doc__)"
+                "From the previous calibration we know that the $\\gamma$ parameter value was 481.9 and the $\\alpha$ value was -2.014e-05.\n",
+                "We define these, along with their variance. In this case we do not know what the variance was, as we ran an OLS calibration, so we will set the variance to 0.\n",
+                "\n",
+                "It is important to note that when setting parameters, the covariances between the parameters are not taken into account in the uncertainty."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:49.159254Z",
-                    "iopub.status.busy": "2022-04-06T08:09:49.158748Z",
-                    "iopub.status.idle": "2022-04-06T08:09:49.325305Z",
-                    "shell.execute_reply": "2022-04-06T08:09:49.324611Z"
+                    "iopub.execute_input": "2022-04-06T08:11:17.162098Z",
+                    "iopub.status.busy": "2022-04-06T08:11:17.161917Z",
+                    "iopub.status.idle": "2022-04-06T08:11:17.193198Z",
+                    "shell.execute_reply": "2022-04-06T08:11:17.192690Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds100.calibration_double_ended(sections=sections,\n",
-                "                               method='ols')"
+                "fix_gamma = (481.9, 0)  # (gamma value, gamma variance)\n",
+                "fix_dalpha = (-2.014e-5, 0)  # (alpha value, alpha variance)\n",
+                "\n",
+                "st_var, resid = ds100.variance_stokes_constant(st_label=\"st\")\n",
+                "ast_var, _ = ds100.variance_stokes_constant(st_label=\"ast\")\n",
+                "ds100.calibration_single_ended(\n",
+                "    st_var=st_var, ast_var=ast_var, fix_gamma=fix_gamma, fix_dalpha=fix_dalpha\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "After calibration, two data variables are added to the `DataStore` object:\n",
-                "- `tmpf`, temperature calculated along the forward direction\n",
-                "- `tmpb`, temperature calculated along the backward direction\n",
-                "\n",
-                "A better estimate, with a lower expected variance, of the temperature along the fiber is the average of the two. We cannot weigh on more than the other, as we do not have more information about the weighing."
+                "Let's see if fixing the parameters worked:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:49.328702Z",
-                    "iopub.status.busy": "2022-04-06T08:09:49.328431Z",
-                    "iopub.status.idle": "2022-04-06T08:09:49.658369Z",
-                    "shell.execute_reply": "2022-04-06T08:09:49.657823Z"
+                    "iopub.execute_input": "2022-04-06T08:11:17.195822Z",
+                    "iopub.status.busy": "2022-04-06T08:11:17.195484Z",
+                    "iopub.status.idle": "2022-04-06T08:11:17.199167Z",
+                    "shell.execute_reply": "2022-04-06T08:11:17.198526Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds1 = ds100.isel(time=0)  # take only the first timestep\n",
-                "\n",
-                "ds1.tmpf.plot(linewidth=1, label='User cali. Forward', figsize=(12, 8))  # plot the temperature calibrated by us\n",
-                "ds1.tmpb.plot(linewidth=1, label='User cali. Backward')  # plot the temperature calibrated by us\n",
-                "ds1.tmp.plot(linewidth=1, label='Device calibrated')  # plot the temperature calibrated by the device\n",
-                "plt.legend();"
+                "print(\"gamma used in calibration:\", ds100.gamma.values)\n",
+                "print(\"dalpha used in calibration:\", ds100.dalpha.values)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Lets compare our calibrated values with the device calibration. Lets average the temperature of the forward channel and the backward channel first."
+                "Let's plot the calibrated temperature. You'll see that this gives the same result as in notebook 05."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:09:49.661194Z",
-                    "iopub.status.busy": "2022-04-06T08:09:49.661029Z",
-                    "iopub.status.idle": "2022-04-06T08:09:49.883632Z",
-                    "shell.execute_reply": "2022-04-06T08:09:49.882492Z"
+                    "iopub.execute_input": "2022-04-06T08:11:17.201528Z",
+                    "iopub.status.busy": "2022-04-06T08:11:17.201340Z",
+                    "iopub.status.idle": "2022-04-06T08:11:17.411075Z",
+                    "shell.execute_reply": "2022-04-06T08:11:17.410449Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds1['TMPAVG'] = (ds1.tmpf + ds1.tmpb) / 2\n",
-                "ds1_diff = ds1.tmp - ds1.TMPAVG\n",
+                "ds1 = ds100.isel(time=0)  # take only the first timestep\n",
                 "\n",
-                "ds1_diff.plot(figsize=(12, 8));"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The device calibration sections and calibration sections defined by us differ. The device only allows for 2 sections, one per thermometer. And most likely the $\\gamma$ is fixed in the device calibration."
+                "ds1.tmpf.plot(\n",
+                "    linewidth=1, figsize=(12, 8), label=\"User calibrated\"\n",
+                ")  # plot the temperature calibrated by us\n",
+                "ds1.tmp.plot(\n",
+                "    linewidth=1, label=\"Device calibrated\"\n",
+                ")  # plot the temperature calibrated by the device\n",
+                "plt.title(\"Temperature at the first time step\")\n",
+                "plt.legend();"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.11"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/07Calibrate_single_wls.ipynb` & `dtscalibration-2.0.0/docs/notebooks/07Calibrate_single_ended.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9551331991129786%*

 * *Differences: {"'cells'": "{0: {'source': ['# 7. Calibration of single-ended measurement']}, 1: {'source': "*

 * *            "{insert: [(0, 'A single-ended DTS measurement setup is a setup where the measurements "*

 * *            'are taken from one ending of the fiber, e.g., only one ending is connected to the DTS '*

 * *            'device. Opposed to double-ended setups, where measurements are taken from both '*

 * *            'endings of the fiber, the calibration of single-ended setups require the additional '*

 * *            'assumptio […]*

```diff
@@ -1,28 +1,32 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# 7. Calibration of single ended measurement with WLS and confidence intervals"
+                "# 7. Calibration of single-ended measurement"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A single-ended calibration is performed where the unknown parameters are estimated using fiber sections that have a reference temperature. The parameters are estimated with a weighted least squares optimization using Stokes and anti-Stokes measurements from all timesteps. Thus Stokes and anti-Stokes measurements with a large signal to noise ratio contribute more towards estimating the optimal parameter set. But an estimate of the noise variance is required.\n",
+                "A single-ended DTS measurement setup is a setup where the measurements are taken from one ending of the fiber, e.g., only one ending is connected to the DTS device. Opposed to double-ended setups, where measurements are taken from both endings of the fiber, the calibration of single-ended setups require the additional assumption that the losses (differential attenuation) is constant along the fiber. E.g., a sharp bend result additional losses and causes a false jump in the temperature. The estimation of the measurement uncertainty also assumes constant losses.\n",
                 "\n",
-                "Single-ended calibration requires a few steps. Please have a look at [1] for more information:\n",
+                "A single-ended calibration is performed where the unknown parameters are estimated using fiber sections that have a reference temperature. The parameters are estimated with a weighted least squares optimization using Stokes and anti-Stokes measurements from all timesteps. Thus Stokes and anti-Stokes measurements with a large signal to noise ratio contribute more towards estimating the optimal parameter set, but an estimate of the noise variance is required.\n",
+                "\n",
+                "Single-ended calibration requires a few steps:\n",
                 "1. Read the raw data files loaded from your DTS machine\n",
                 "2. Define the reference sections: fiber sections that have a known temperature.\n",
                 "3. Estimate the variance of the noise in the Stokes and anti-Stokes measurements\n",
                 "4. Perform the parameter search and compute the temperature along the entire fiber.\n",
-                "5. Compute the confidence intervals for the temperature\n",
+                "5. Plot the temperature and uncertainty of the estimated temperature\n",
+                "\n",
+                "Please have a look at [1] for more information.\n",
                 "\n",
                 "[1]: des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation of Temperature and Associated Uncertainty from Fiber-Optic Raman-Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235. https://doi.org/10.3390/s20082235"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -33,75 +37,77 @@
                     "iopub.status.idle": "2022-04-06T08:10:00.524659Z",
                     "shell.execute_reply": "2022-04-06T08:10:00.524090Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
-                "import warnings\n",
-                "\n",
-                "warnings.simplefilter('ignore')  # Hide warnings to avoid clutter in the notebook\n",
-                "\n",
                 "\n",
                 "from dtscalibration import read_silixa_files\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "%matplotlib inline"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Read the raw data files loaded from your DTS machine\n",
+                "Use `read_silixa_files` for reading files from a Silixa device. The following functions are available for reading files from other devices: `read_sensortran_files`, `read_apsensing_files`, and `read_sensornet_files`. See Notebook 1.\n",
+                "\n",
+                "Calibration is performed on sections that have a known"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
                     "iopub.execute_input": "2022-04-06T08:10:00.527515Z",
                     "iopub.status.busy": "2022-04-06T08:10:00.526942Z",
                     "iopub.status.idle": "2022-04-06T08:10:00.730573Z",
                     "shell.execute_reply": "2022-04-06T08:10:00.729897Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'single_ended')\n",
-                "ds = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')\n",
-                "\n",
-                "ds = ds.sel(x=slice(-30, 101))  # only calibrate parts of the fiber\n",
-                "sections = {\n",
-                "            'probe1Temperature':    [slice(20, 25.5)],  # warm bath\n",
-                "            'probe2Temperature':    [slice(5.5, 15.5)],  # cold bath\n",
-                "#             'referenceTemperature': [slice(-24., -4)]  # The internal coil is not so uniform\n",
-                "            }\n",
-                "ds.sections = sections"
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"single_ended\")\n",
+                "ds = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Define the reference fiber sections that have a known temperature\n",
+                "As explained in Notebook 3. DTS devices come with temperature probes to measure the temperature of the water baths. These measurements are stored in the data that was loaded in the previous step and are loaded automatically. In the case you would like to use an external temperature sensor, have a look at notebook `09Import_timeseries` to append those measurements to the `ds` before continuing with the calibration. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:00.754830Z",
-                    "iopub.status.busy": "2022-04-06T08:10:00.754655Z",
-                    "iopub.status.idle": "2022-04-06T08:10:00.758286Z",
-                    "shell.execute_reply": "2022-04-06T08:10:00.757744Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "print(ds.calibration_single_ended.__doc__)"
+                "ds = ds.sel(x=slice(-30, 101))  # dismiss parts of the fiber that are not interesting\n",
+                "ds.sections = {\n",
+                "    \"probe1Temperature\": [slice(20, 25.5)],  # warm bath\n",
+                "    \"probe2Temperature\": [slice(5.5, 15.5)],  # cold bath\n",
+                "}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First calculate the variance in the measured Stokes and anti-Stokes signals, in the forward and backward direction.\n",
+                "# Estimate the variance of the noise in the Stokes and anti-Stokes measurements\n",
+                "First calculate the variance of the noise in the measured Stokes and anti-Stokes signals. See Notebook 4 for more information.\n",
                 "\n",
-                "The Stokes and anti-Stokes signals should follow a smooth decaying exponential. This function fits a decaying exponential to each reference section for each time step. The variance of the residuals between the measured Stokes and anti-Stokes signals and the fitted signals is used as an estimate of the variance in measured signals."
+                "The Stokes and anti-Stokes signals should follow a smooth decaying exponential. This function fits a decaying exponential to each reference section for each time step. The variance of the residuals between the measured Stokes and anti-Stokes signals and the fitted signals is used as an estimate of the variance in measured signals. This algorithm assumes that the temperature is the same for the entire section but may vary over time and differ per section."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -109,153 +115,85 @@
                     "iopub.status.busy": "2022-04-06T08:10:00.760354Z",
                     "iopub.status.idle": "2022-04-06T08:10:00.914629Z",
                     "shell.execute_reply": "2022-04-06T08:10:00.914071Z"
                 }
             },
             "outputs": [],
             "source": [
-                "st_var, resid = ds.variance_stokes_constant(st_label='st')\n",
-                "ast_var, _ = ds.variance_stokes_constant(st_label='ast')"
+                "st_var, resid = ds.variance_stokes_constant(st_label=\"st\")\n",
+                "ast_var, _ = ds.variance_stokes_constant(st_label=\"ast\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Similar to the ols procedure, we make a single function call to calibrate the temperature. If the method is `wls` and confidence intervals are passed to `conf_ints`, confidence intervals calculated. As weigths are correctly passed to the least squares procedure, the covariance matrix can be used. This matrix holds the covariances between all the parameters. A large parameter set is generated from this matrix, assuming the parameter space is normally distributed with their mean at the best estimate of the least squares procedure.\n",
-                "\n",
-                "The large parameter set is used to calculate a large set of temperatures. By using `percentiles` or `quantile` the 95% confidence interval of the calibrated temperature between 2.5% and 97.5% are calculated.\n",
-                "\n",
-                "The confidence intervals differ per time step. If you would like to calculate confidence intervals of temporal averages or of averages of fiber sections see notebook 16."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:00.916985Z",
-                    "iopub.status.busy": "2022-04-06T08:10:00.916764Z",
-                    "iopub.status.idle": "2022-04-06T08:10:00.967445Z",
-                    "shell.execute_reply": "2022-04-06T08:10:00.966707Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "ds.calibration_single_ended(sections=sections,\n",
-                "                            st_var=st_var,\n",
-                "                            ast_var=ast_var,\n",
-                "                            method='wls')"
+                "The following plot can be used to check if there are no spatial or temporal correlated residuals. If you see horizontal or vertical lines that means that you overestimate the st_var. Common reasons are that the temperature of that section is not uniform, e.g. that the reference sections were defined falsely or that the temperature of the water baths were not uniform."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:00.969870Z",
-                    "iopub.status.busy": "2022-04-06T08:10:00.969667Z",
-                    "iopub.status.idle": "2022-04-06T08:10:01.062010Z",
-                    "shell.execute_reply": "2022-04-06T08:10:01.061477Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "ds.conf_int_single_ended(\n",
-                "    st_var=st_var,\n",
-                "    ast_var=ast_var,\n",
-                "    conf_ints=[2.5, 97.5],\n",
-                "    mc_sample_size=500)"
+                "resid.plot(figsize=(12, 4));"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Lets compare our calibrated values with the device calibration"
+                "# Perform calibration and compute the temperature\n",
+                "We calibrate the measurements and their uncertainty with a single method call. The temperature is stored by default as the `ds.tmpf` dataarray and the variance of its approximation as `ds.tmpf_var`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:01.064432Z",
-                    "iopub.status.busy": "2022-04-06T08:10:01.064239Z",
-                    "iopub.status.idle": "2022-04-06T08:10:01.452267Z",
-                    "shell.execute_reply": "2022-04-06T08:10:01.451782Z"
+                    "iopub.execute_input": "2022-04-06T08:10:00.916985Z",
+                    "iopub.status.busy": "2022-04-06T08:10:00.916764Z",
+                    "iopub.status.idle": "2022-04-06T08:10:00.967445Z",
+                    "shell.execute_reply": "2022-04-06T08:10:00.966707Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds1 = ds.isel(time=0)  # take only the first timestep\n",
-                "ds1.tmpf.plot(linewidth=0.8, figsize=(12, 8), label='User calibrated')  # plot the temperature calibrated by us\n",
-                "ds1.tmp.plot(linewidth=0.8, label='Device calibrated')  # plot the temperature calibrated by the device\n",
-                "ds1.tmpf_mc.plot(linewidth=0.8, hue='CI', label='CI device')\n",
-                "plt.title('Temperature at the first time step')\n",
-                "plt.legend();"
+                "ds.calibration_single_ended(st_var=st_var, ast_var=ast_var)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:01.454642Z",
-                    "iopub.status.busy": "2022-04-06T08:10:01.454452Z",
-                    "iopub.status.idle": "2022-04-06T08:10:01.785627Z",
-                    "shell.execute_reply": "2022-04-06T08:10:01.785039Z"
-                }
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "ds.tmpf_mc_var.plot(figsize=(12, 8));"
+                "# Plot the temperature and uncertainty of the estimated temperature\n",
+                "First, the temperature for the entire fiber is plotted. Second, the temperature and its standard error are plotted for the first timestep."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:01.787752Z",
-                    "iopub.status.busy": "2022-04-06T08:10:01.787560Z",
-                    "iopub.status.idle": "2022-04-06T08:10:02.358032Z",
-                    "shell.execute_reply": "2022-04-06T08:10:02.357460Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "ds1.tmpf_mc.sel(CI=2.5).plot(label = '2.5% CI', figsize=(12, 8))\n",
-                "ds1.tmpf_mc.sel(CI=97.5).plot(label = '97.5% CI')\n",
-                "ds1.tmpf.plot(label='User calibrated')\n",
-                "plt.title('User calibrated temperature with 95% confidence interval')\n",
-                "plt.legend();"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "We can tell from the graph above that the 95% confidence interval widens furtherdown the cable. Lets have a look at the calculated variance along the cable for a single timestep. According to the device manufacturer this should be around 0.0059 degC."
+                "ds.tmpf.plot(figsize=(12, 4));"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:02.360492Z",
-                    "iopub.status.busy": "2022-04-06T08:10:02.360281Z",
-                    "iopub.status.idle": "2022-04-06T08:10:02.665410Z",
-                    "shell.execute_reply": "2022-04-06T08:10:02.664935Z"
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "ds1.tmpf_mc_var.plot(figsize=(12, 8));"
+                "ds1 = ds.isel(time=0)\n",
+                "ds1.tmpf.plot(figsize=(12, 4))\n",
+                "(ds1.tmpf_var**0.5).plot(figsize=(12, 4))\n",
+                "plt.ylabel(\"$\\sigma$ ($^\\circ$C)\");"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The variance of the temperature measurement appears to be larger than what the manufacturer reports. This is already the case for the internal cable; it is not caused by a dirty connector/bad splice on our side. Maybe the length of the calibration section was not sufficient.\n",
@@ -284,31 +222,38 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Clearly there was a bad splice at 30 m that resulted in the sharp increase of measurement uncertainty for the cable section after the bad splice."
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Note that the uncertainty of the temperature strongly varies along the fiber. Dive deeper in the uncertainty of the temperature estimate in another notebook"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.11"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/08Calibrate_double_wls.ipynb` & `dtscalibration-2.0.0/docs/notebooks/14Lossy_splices.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8264811985400221%*

 * *Differences: {"'cells'": "{0: {'source': ['# 14. Calibration over (lossy) splices and connectors']}, 1: "*

 * *            '{\'source\': {insert: [(0, \'## Background\\n\'), (1, "While it is best practice to '*

 * *            "not have connectors or splices within a DTS calibration, sometimes it can't be "*

 * *            'avoided. For example, in a borehole the fibers in a duplex cable are often connected '*

 * *            'with either a splice or a loopback connector. \\n"), (3, \'Splices and connectors '*

 * *            'will cause a ste […]*

```diff
@@ -1,257 +1,223 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# 8. Calibration of double ended measurement with WLS and confidence intervals"
+                "# 14. Calibration over (lossy) splices and connectors"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A double-ended calibration is performed where the unknown parameters are estimated using fiber sections that have a reference temperature. The parameters are estimated with a weighted least squares optimization using Stokes and anti-Stokes measurements from all timesteps. Thus Stokes and anti-Stokes measurements with a large signal to noise ratio contribute more towards estimating the optimal parameter set. But an estimate of the noise variance is required.\n",
+                "## Background\n",
+                "While it is best practice to not have connectors or splices within a DTS calibration, sometimes it can't be avoided. For example, in a borehole the fibers in a duplex cable are often connected with either a splice or a loopback connector. \n",
                 "\n",
-                "Double-ended calibration requires a few steps. Please have a look at [1] for more information:\n",
-                "1. Read the raw data files loaded from your DTS machine\n",
-                "2. Define the reference sections: fiber sections that have a known temperature.\n",
-                "3. Estimate the variance of the noise in the Stokes and anti-Stokes measurements\n",
-                "4. Perform the parameter search and compute the temperature along the entire fiber.\n",
-                "5. Compute the confidence intervals for the temperature\n",
+                "Splices and connectors will cause a step loss in the signal strength, and with varying strain and temperature, this step loss will vary. In double ended setups this step loss can even be asymmetrical for the forward and backward measurements. All these effects have to be taken into account in the calibration.\n",
                 "\n",
-                "[1]: des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation of Temperature and Associated Uncertainty from Fiber-Optic Raman-Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235. https://doi.org/10.3390/s20082235"
+                "To calibrate over these splices/connectors, locations with 'transient attenuation' can be defined along the length of the fiber. Adding these does mean that more information is needed to perform the calibration, such as extra reference sections or matching sections of fiber. Matching sections will be explained in notebook 15.\n",
+                "\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Demonstration\n",
+                "To demonstrate the effect of a lossy splice, we'll load the same dataset that was used in previous notebooks, and modify the data to simulate a lossy splice."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:13.277128Z",
-                    "iopub.status.busy": "2022-04-06T08:10:13.276102Z",
-                    "iopub.status.idle": "2022-04-06T08:10:14.748590Z",
-                    "shell.execute_reply": "2022-04-06T08:10:14.748034Z"
+                    "iopub.execute_input": "2022-04-06T08:11:25.641322Z",
+                    "iopub.status.busy": "2022-04-06T08:11:25.640590Z",
+                    "iopub.status.idle": "2022-04-06T08:11:27.122032Z",
+                    "shell.execute_reply": "2022-04-06T08:11:27.121371Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
-                "import warnings\n",
-                "\n",
-                "warnings.simplefilter('ignore')  # Hide warnings to avoid clutter in the notebook\n",
-                "\n",
                 "\n",
                 "from dtscalibration import read_silixa_files\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:14.751185Z",
-                    "iopub.status.busy": "2022-04-06T08:10:14.750883Z",
-                    "iopub.status.idle": "2022-04-06T08:10:15.050453Z",
-                    "shell.execute_reply": "2022-04-06T08:10:15.049751Z"
+                    "iopub.execute_input": "2022-04-06T08:11:27.124582Z",
+                    "iopub.status.busy": "2022-04-06T08:11:27.124371Z",
+                    "iopub.status.idle": "2022-04-06T08:11:27.423254Z",
+                    "shell.execute_reply": "2022-04-06T08:11:27.422619Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
+                "\n",
+                "ds_ = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")\n",
+                "\n",
+                "ds = ds_.sel(x=slice(0, 110))  # only calibrate parts of the fiber\n",
                 "\n",
-                "ds_ = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')\n",
                 "\n",
-                "ds = ds_.sel(x=slice(0, 100))  # only calibrate parts of the fiber\n",
                 "sections = {\n",
-                "    'probe1Temperature': [slice(7.5, 17.), slice(70., 80.)],  # cold bath\n",
-                "    'probe2Temperature': [slice(24., 34.), slice(85., 95.)],  # warm bath\n",
-                "    }\n",
+                "    \"probe1Temperature\": [slice(7.5, 17.0), slice(70.0, 80.0)],  # cold bath\n",
+                "    \"probe2Temperature\": [slice(24.0, 34.0), slice(85.0, 95.0)],  # warm bath\n",
+                "}\n",
                 "ds.sections = sections"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First calculate the variance in the measured Stokes and anti-Stokes signals, in the forward and backward direction.\n",
+                "To simulate the lossy splice, we introduce a step loss in the signal strength at x = 50 m. For the forward channel, this means all data beyond 50 meters is reduced with a 'random' factor. For the backward channel, this means all data up to 50 meters is reduced with a 'random' factor.\n",
                 "\n",
-                "The Stokes and anti-Stokes signals should follow a smooth decaying exponential. This function fits a decaying exponential to each reference section for each time step. The variance of the residuals between the measured Stokes and anti-Stokes signals and the fitted signals is used as an estimate of the variance in measured signals."
+                "In the plots of the Stokes and anti-Stokes signal the big step loss is clearly visible."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:15.053145Z",
-                    "iopub.status.busy": "2022-04-06T08:10:15.052975Z",
-                    "iopub.status.idle": "2022-04-06T08:10:15.811537Z",
-                    "shell.execute_reply": "2022-04-06T08:10:15.810996Z"
+                    "iopub.execute_input": "2022-04-06T08:11:27.425744Z",
+                    "iopub.status.busy": "2022-04-06T08:11:27.425525Z",
+                    "iopub.status.idle": "2022-04-06T08:11:27.446200Z",
+                    "shell.execute_reply": "2022-04-06T08:11:27.444863Z"
                 }
             },
             "outputs": [],
             "source": [
-                "st_var, resid = ds.variance_stokes_constant(st_label='st')\n",
-                "ast_var, _ = ds.variance_stokes_constant(st_label='ast')\n",
-                "rst_var, _ = ds.variance_stokes_constant(st_label='rst')\n",
-                "rast_var, _ = ds.variance_stokes_constant(st_label='rast')"
+                "ds[\"st\"] = ds.st.where(ds.x < 50, ds.st * 0.8)\n",
+                "ds[\"ast\"] = ds.ast.where(ds.x < 50, ds.ast * 0.82)\n",
+                "\n",
+                "ds[\"rst\"] = ds.rst.where(ds.x > 50, ds.rst * 0.85)\n",
+                "ds[\"rast\"] = ds.rast.where(ds.x > 50, ds.rast * 0.81)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:15.813904Z",
-                    "iopub.status.busy": "2022-04-06T08:10:15.813688Z",
-                    "iopub.status.idle": "2022-04-06T08:10:16.081331Z",
-                    "shell.execute_reply": "2022-04-06T08:10:16.080696Z"
+                    "iopub.execute_input": "2022-04-06T08:11:27.451194Z",
+                    "iopub.status.busy": "2022-04-06T08:11:27.450909Z",
+                    "iopub.status.idle": "2022-04-06T08:11:27.730773Z",
+                    "shell.execute_reply": "2022-04-06T08:11:27.730254Z"
                 }
             },
             "outputs": [],
             "source": [
-                "resid.plot(figsize=(12, 8));"
+                "ds.isel(time=0).st.plot(label=\"st\")\n",
+                "ds.isel(time=0).ast.plot(label=\"ast\")\n",
+                "ds.isel(time=0).rst.plot(label=\"rst\")\n",
+                "ds.isel(time=0).rast.plot(label=\"rast\")\n",
+                "plt.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We calibrate the measurement with a single method call. The labels refer to the keys in the DataStore object containing the Stokes, anti-Stokes, reverse Stokes and reverse anti-Stokes. The variance in those measurements were calculated in the previous step. We use a sparse solver because it saves us memory."
+                "We will first run a calibration without adding the transient attenuation location. A big jump in the calibrated temperature is visible at x = 50, and all temperatures before the jump are too low, and the temperatures after the jump are too high."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:16.083711Z",
-                    "iopub.status.busy": "2022-04-06T08:10:16.083510Z",
-                    "iopub.status.idle": "2022-04-06T08:10:16.591924Z",
-                    "shell.execute_reply": "2022-04-06T08:10:16.591485Z"
+                    "iopub.execute_input": "2022-04-06T08:11:27.733065Z",
+                    "iopub.status.busy": "2022-04-06T08:11:27.732874Z",
+                    "iopub.status.idle": "2022-04-06T08:11:29.152616Z",
+                    "shell.execute_reply": "2022-04-06T08:11:29.152100Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds.calibration_double_ended(\n",
+                "ds_a = ds.copy(deep=True)\n",
+                "\n",
+                "st_var, resid = ds_a.variance_stokes(st_label=\"st\")\n",
+                "ast_var, _ = ds_a.variance_stokes(st_label=\"ast\")\n",
+                "rst_var, _ = ds_a.variance_stokes(st_label=\"rst\")\n",
+                "rast_var, _ = ds_a.variance_stokes(st_label=\"rast\")\n",
+                "\n",
+                "ds_a.calibration_double_ended(\n",
                 "    st_var=st_var,\n",
                 "    ast_var=ast_var,\n",
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
-                "    store_tmpw='tmpw',\n",
-                "    method='wls',\n",
-                "    solver='sparse')"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:16.594307Z",
-                    "iopub.status.busy": "2022-04-06T08:10:16.594086Z",
-                    "iopub.status.idle": "2022-04-06T08:10:16.849150Z",
-                    "shell.execute_reply": "2022-04-06T08:10:16.848523Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "ds.tmpw.plot()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Confidence intervals"
+                "    store_tmpw=\"tmpw\",\n",
+                "    method=\"wls\",\n",
+                "    solver=\"sparse\",\n",
+                ")\n",
+                "\n",
+                "ds_a.isel(time=0).tmpw.plot(label=\"calibrated\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "With another method call we estimate the confidence intervals. If the method is `wls` and confidence intervals are passed to `conf_ints`, confidence intervals calculated. As weigths are correctly passed to the least squares procedure, the covariance matrix can be used as an estimator for the uncertainty in the parameters. This matrix holds the covariances between all the parameters. A large parameter set is generated from this matrix as part of the Monte Carlo routine, assuming the parameter space is normally distributed with their mean at the best estimate of the least squares procedure.\n",
-                "\n",
-                "The large parameter set is used to calculate a large set of temperatures. By using `percentiles` or `quantile` the 95% confidence interval of the calibrated temperature between 2.5% and 97.5% are calculated.\n",
+                "Now we run a calibration, adding the keyword argument '**trans_att**', and provide a list of floats containing the locations of the splices. In this case we only add a single one at x = 50 m. After running the calibration you will see that by adding the transient attenuation location the calibration returns the correct temperature, without the big jump.\n",
                 "\n",
-                "The confidence intervals differ per time step. If you would like to calculate confidence intervals temporal averages or averages of fiber sections see notebook 16."
+                "*In single-ended calibration the keyword is called '**trans_att**'.*"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:16.851418Z",
-                    "iopub.status.busy": "2022-04-06T08:10:16.851224Z",
-                    "iopub.status.idle": "2022-04-06T08:10:17.113065Z",
-                    "shell.execute_reply": "2022-04-06T08:10:17.112475Z"
+                    "iopub.execute_input": "2022-04-06T08:11:29.154854Z",
+                    "iopub.status.busy": "2022-04-06T08:11:29.154652Z",
+                    "iopub.status.idle": "2022-04-06T08:11:30.631923Z",
+                    "shell.execute_reply": "2022-04-06T08:11:30.631414Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds.conf_int_double_ended(\n",
+                "st_var, resid = ds.variance_stokes(st_label=\"st\")\n",
+                "ast_var, _ = ds.variance_stokes(st_label=\"ast\")\n",
+                "rst_var, _ = ds.variance_stokes(st_label=\"rst\")\n",
+                "rast_var, _ = ds.variance_stokes(st_label=\"rast\")\n",
+                "\n",
+                "ds.calibration_double_ended(\n",
                 "    st_var=st_var,\n",
                 "    ast_var=ast_var,\n",
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
-                "    conf_ints=[2.5, 50., 97.5],\n",
-                "    mc_sample_size=500)  # <- choose a much larger sample size)"
+                "    trans_att=[50.0],\n",
+                "    store_tmpw=\"tmpw\",\n",
+                "    method=\"wls\",\n",
+                "    solver=\"sparse\",\n",
+                ")\n",
+                "\n",
+                "ds_a.isel(time=0).tmpw.plot(label=\"no trans. att.\")\n",
+                "ds.isel(time=0).tmpw.plot(label=\"with trans. att.\")\n",
+                "plt.legend()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:17.115378Z",
-                    "iopub.status.busy": "2022-04-06T08:10:17.115193Z",
-                    "iopub.status.idle": "2022-04-06T08:10:18.229389Z",
-                    "shell.execute_reply": "2022-04-06T08:10:18.228867Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "ds1 = ds.isel(time=-1)  # take only the first timestep\n",
-                "ds1.tmpw.plot(linewidth=0.7, figsize=(12, 8))\n",
-                "ds1.tmpw_mc.isel(CI=0).plot(linewidth=0.7, label='CI: 2.5%')\n",
-                "ds1.tmpw_mc.isel(CI=2).plot(linewidth=0.7, label='CI: 97.5%')\n",
-                "plt.legend();"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "metadata": {},
-            "source": [
-                "The DataArrays `tmpf_mc` and `tmpb_mc` and the dimension `CI` are added. `MC` stands for monte carlo and the `CI` dimension holds the confidence interval 'coordinates'."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:10:18.231907Z",
-                    "iopub.status.busy": "2022-04-06T08:10:18.231718Z",
-                    "iopub.status.idle": "2022-04-06T08:10:19.045574Z",
-                    "shell.execute_reply": "2022-04-06T08:10:19.045043Z"
-                }
-            },
             "outputs": [],
-            "source": [
-                "(ds1.tmpw_mc_var**0.5).plot(figsize=(12, 4));\n",
-                "plt.ylabel('$\\sigma$ ($^\\circ$C)');"
-            ]
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
@@ -266,9 +232,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.11"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/09Import_timeseries.ipynb` & `dtscalibration-2.0.0/docs/notebooks/09Import_timeseries.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9884970238095238%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(0, 'filepath = os.path.join(\\n'), (1, '    "*

 * *            '"..",\\n\'), (2, \'    "..",\\n\'), (3, \'    "tests",\\n\'), (4, \'    '*

 * *            '"data",\\n\'), (5, \'    "external_temperature_timeseries",\\n\'), (6, \'    '*

 * *            '"Loodswaternet2018-03-28 02h.csv",\\n\'), (7, \')\\n\'), (10, \'print(filepath, '*

 * *            '"\\\\n")\\n\'), (11, \'with open(filepath, "r") as f:\\n\'), (13, \'print(" '*

 * *            '".join(head))\')], delete: [8, 6, 5, 2, 1, 0]}},  […]*

```diff
@@ -52,23 +52,28 @@
                     "iopub.status.busy": "2022-04-06T08:10:32.901062Z",
                     "iopub.status.idle": "2022-04-06T08:10:32.905451Z",
                     "shell.execute_reply": "2022-04-06T08:10:32.904987Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', \n",
-                "                        'external_temperature_timeseries', \n",
-                "                        'Loodswaternet2018-03-28 02h.csv')\n",
+                "filepath = os.path.join(\n",
+                "    \"..\",\n",
+                "    \"..\",\n",
+                "    \"tests\",\n",
+                "    \"data\",\n",
+                "    \"external_temperature_timeseries\",\n",
+                "    \"Loodswaternet2018-03-28 02h.csv\",\n",
+                ")\n",
                 "\n",
                 "# Bonus:\n",
-                "print(filepath, '\\n')\n",
-                "with open(filepath, 'r') as f:\n",
+                "print(filepath, \"\\n\")\n",
+                "with open(filepath, \"r\") as f:\n",
                 "    head = [next(f) for _ in range(5)]\n",
-                "print(' '.join(head))"
+                "print(\" \".join(head))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -76,17 +81,18 @@
                     "iopub.status.busy": "2022-04-06T08:10:32.927992Z",
                     "iopub.status.idle": "2022-04-06T08:10:33.076019Z",
                     "shell.execute_reply": "2022-04-06T08:10:33.075543Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ts = pd.read_csv(filepath, sep=',', index_col=0, parse_dates=True, \n",
-                "                 squeeze=True, engine='python')  # the latter 2 kwargs are to ensure a pd.Series is returned\n",
-                "ts = ts.tz_localize('Europe/Amsterdam')  # set the timezone"
+                "ts = pd.read_csv(\n",
+                "    filepath, sep=\",\", index_col=0, parse_dates=True, squeeze=True, engine=\"python\"\n",
+                ")  # the latter 2 kwargs are to ensure a pd.Series is returned\n",
+                "ts = ts.tz_localize(\"Europe/Amsterdam\")  # set the timezone"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -117,18 +123,16 @@
                     "iopub.status.busy": "2022-04-06T08:10:33.090642Z",
                     "iopub.status.idle": "2022-04-06T08:10:33.301302Z",
                     "shell.execute_reply": "2022-04-06T08:10:33.300636Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath_ds = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
-                "ds = read_silixa_files(directory=filepath_ds,\n",
-                "                       timezone_netcdf='UTC',\n",
-                "                       file_ext='*.xml')"
+                "filepath_ds = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
+                "ds = read_silixa_files(directory=filepath_ds, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 2: Add the temperature measurements of the external probe to the DataStore.\n",
@@ -145,15 +149,15 @@
                     "iopub.status.busy": "2022-04-06T08:10:33.303562Z",
                     "iopub.status.idle": "2022-04-06T08:10:33.308068Z",
                     "shell.execute_reply": "2022-04-06T08:10:33.307543Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds.coords['time_external'] = ts.index.values"
+                "ds.coords[\"time_external\"] = ts.index.values"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Second we add the measured values"
@@ -168,15 +172,15 @@
                     "iopub.status.busy": "2022-04-06T08:10:33.310255Z",
                     "iopub.status.idle": "2022-04-06T08:10:33.315622Z",
                     "shell.execute_reply": "2022-04-06T08:10:33.315088Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds['external_probe'] = (('time_external',), ts)"
+                "ds[\"external_probe\"] = ((\"time_external\",), ts)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 3: Align the time of the external measurements to the Stokes measurement times\n",
@@ -192,15 +196,15 @@
                     "iopub.status.busy": "2022-04-06T08:10:33.317912Z",
                     "iopub.status.idle": "2022-04-06T08:10:33.328112Z",
                     "shell.execute_reply": "2022-04-06T08:10:33.327546Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds['external_probe_dts'] = ds['external_probe'].interp(time_external=ds.time)"
+                "ds[\"external_probe_dts\"] = ds[\"external_probe\"].interp(time_external=ds.time)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -229,27 +233,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.11"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/10Align_double_ended_measurements.ipynb` & `dtscalibration-2.0.0/docs/notebooks/10Align_double_ended_measurements.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959804084804085%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'from dtscalibration.datastore_utils import (\\n'), (3, "*

 * *            "'    suggest_cable_shift_double_ended,\\n'), (4, '    shift_double_ended,\\n'), (5, "*

 * *            "')\\n'), (8, '\\n')], delete: [2]}}, 3: {'source': "*

 * *            "['?suggest_cable_shift_double_ended']}, 4: {'source': {insert: [(0, 'filepath = "*

 * *            'os.path.join("..", "..", "tests", "data", "double_ended2")\\n\'), (3, \'    '*

 * *            'directory=filepath, timezone_netcdf="UTC", file_ […]*

```diff
@@ -29,17 +29,21 @@
                     "shell.execute_reply": "2022-04-06T08:10:42.969681Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "from dtscalibration import read_silixa_files\n",
-                "from dtscalibration.datastore_utils import suggest_cable_shift_double_ended, shift_double_ended\n",
+                "from dtscalibration.datastore_utils import (\n",
+                "    suggest_cable_shift_double_ended,\n",
+                "    shift_double_ended,\n",
+                ")\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -48,15 +52,15 @@
                     "iopub.status.busy": "2022-04-06T08:10:42.972519Z",
                     "iopub.status.idle": "2022-04-06T08:10:43.009664Z",
                     "shell.execute_reply": "2022-04-06T08:10:43.009175Z"
                 }
             },
             "outputs": [],
             "source": [
-                "suggest_cable_shift_double_ended?"
+                "?suggest_cable_shift_double_ended"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -64,20 +68,19 @@
                     "iopub.status.busy": "2022-04-06T08:10:43.011645Z",
                     "iopub.status.idle": "2022-04-06T08:10:43.349302Z",
                     "shell.execute_reply": "2022-04-06T08:10:43.348715Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
                 "\n",
                 "ds_aligned = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')  # this one is already correctly aligned"
+                "    directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\"\n",
+                ")  # this one is already correctly aligned"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Because our loaded files were already nicely aligned, we are purposely offsetting the forward and backward channel by 3 `spacial indices'."
@@ -116,18 +119,16 @@
                     "iopub.status.idle": "2022-04-06T08:10:43.946995Z",
                     "shell.execute_reply": "2022-04-06T08:10:43.946514Z"
                 }
             },
             "outputs": [],
             "source": [
                 "suggested_shift = suggest_cable_shift_double_ended(\n",
-                "    ds_notaligned, \n",
-                "    np.arange(-5, 5), \n",
-                "    plot_result=True, \n",
-                "    figsize=(12,8))"
+                "    ds_notaligned, np.arange(-5, 5), plot_result=True, figsize=(12, 8)\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The two approaches suggest a shift of -3 and -4. It is up to the user which suggestion to follow. Usually the two suggested shift are close"
@@ -158,15 +159,15 @@
                     "iopub.status.busy": "2022-04-06T08:10:43.961520Z",
                     "iopub.status.idle": "2022-04-06T08:10:43.967547Z",
                     "shell.execute_reply": "2022-04-06T08:10:43.967128Z"
                 }
             },
             "outputs": [],
             "source": [
-                "print(ds_aligned.x, 3*'\\n', ds_restored.x)"
+                "print(ds_aligned.x, 3 * \"\\n\", ds_restored.x)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note that our fiber has become shorter by 2*3 spatial indices"
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/11Merge_single_measurements_into_double.ipynb` & `dtscalibration-2.0.0/docs/notebooks/11Merge_single_measurements_into_double.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788799395049395%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'from dtscalibration.datastore_utils import (\\n'), (3, "*

 * *            "'    suggest_cable_shift_double_ended,\\n'), (4, '    shift_double_ended,\\n'), (5, "*

 * *            "'    merge_double_ended,\\n'), (6, ')\\n'), (9, '\\n')], delete: [2]}}, 4: {'source': "*

 * *            '{insert: [(0, \'filepath_ch1 = os.path.join(\\n\'), (1, \'    "..", "..", "tests", '*

 * *            '"data", "double_single_ended", "channel_1"\\n\'), (2, \')\\n\'), (3, \'filepath_ch2 = '*

 * *            ' […]*

```diff
@@ -25,17 +25,22 @@
                     "shell.execute_reply": "2022-04-06T08:10:54.162117Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "from dtscalibration import read_silixa_files\n",
-                "from dtscalibration.datastore_utils import suggest_cable_shift_double_ended, shift_double_ended, merge_double_ended\n",
+                "from dtscalibration.datastore_utils import (\n",
+                "    suggest_cable_shift_double_ended,\n",
+                "    shift_double_ended,\n",
+                "    merge_double_ended,\n",
+                ")\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -51,26 +56,28 @@
                     "iopub.status.busy": "2022-04-06T08:10:54.165182Z",
                     "iopub.status.idle": "2022-04-06T08:10:55.230962Z",
                     "shell.execute_reply": "2022-04-06T08:10:55.230377Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath_ch1 = os.path.join('..', '..', 'tests', 'data', 'double_single_ended', 'channel_1')\n",
-                "filepath_ch2 = os.path.join('..', '..', 'tests', 'data', 'double_single_ended', 'channel_2')\n",
+                "filepath_ch1 = os.path.join(\n",
+                "    \"..\", \"..\", \"tests\", \"data\", \"double_single_ended\", \"channel_1\"\n",
+                ")\n",
+                "filepath_ch2 = os.path.join(\n",
+                "    \"..\", \"..\", \"tests\", \"data\", \"double_single_ended\", \"channel_2\"\n",
+                ")\n",
                 "\n",
                 "ds_ch1 = read_silixa_files(\n",
-                "    directory=filepath_ch1,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')\n",
+                "    directory=filepath_ch1, timezone_netcdf=\"UTC\", file_ext=\"*.xml\"\n",
+                ")\n",
                 "\n",
                 "ds_ch2 = read_silixa_files(\n",
-                "    directory=filepath_ch2,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')"
+                "    directory=filepath_ch2, timezone_netcdf=\"UTC\", file_ext=\"*.xml\"\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "When plotting the data the two datasets already look quite similar as it is a duplex measurement."
@@ -85,16 +92,16 @@
                     "iopub.status.busy": "2022-04-06T08:10:55.233341Z",
                     "iopub.status.idle": "2022-04-06T08:10:55.444418Z",
                     "shell.execute_reply": "2022-04-06T08:10:55.443824Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds_ch1.isel(time=0).st.plot(label='ST ch1', lw=2)\n",
-                "ds_ch2.isel(time=0).st.plot(label='ST ch2')\n",
+                "ds_ch1.isel(time=0).st.plot(label=\"ST ch1\", lw=2)\n",
+                "ds_ch2.isel(time=0).st.plot(label=\"ST ch2\")\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -114,27 +121,26 @@
                     "shell.execute_reply": "2022-04-06T08:10:55.470990Z"
                 }
             },
             "outputs": [],
             "source": [
                 "cable_length = 2017.7\n",
                 "\n",
-                "ds = merge_double_ended(ds_fw = ds_ch1,\n",
-                "                        ds_bw = ds_ch2,\n",
-                "                        cable_length = cable_length,\n",
-                "                        plot_result = False)\n",
+                "ds = merge_double_ended(\n",
+                "    ds_fw=ds_ch1, ds_bw=ds_ch2, cable_length=cable_length, plot_result=False\n",
+                ")\n",
                 "\n",
                 "print((ds.isel(time=0).st - ds.isel(time=0).rst).sum().values)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To perfectly align the two measurements we can use the alignment utility. Before we do so, we select only the data of the phyisical cable and 10 meters of the internal reference coil.\n",
+                "To perfectly align the two measurements we can use the alignment utility. See the `align double-ended measurements Example notebook`. Before we do so, we select only the data of the phyisical cable and 10 meters of the internal reference coil.\n",
                 "\n",
                 "It turns out we were off by 3 datapoints, so let's shift it by that."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -147,43 +153,51 @@
                 },
                 "scrolled": true
             },
             "outputs": [],
             "source": [
                 "ds = ds.sel(x=slice(-10, cable_length + 10))\n",
                 "\n",
-                "shift1, shift2 = suggest_cable_shift_double_ended(ds.isel(time=[0,-1]).compute(),\n",
-                "                                                  np.arange(-10, 10, 1, dtype=int))\n",
+                "shift1, shift2 = suggest_cable_shift_double_ended(\n",
+                "    ds.isel(time=[0, -1]).compute(), np.arange(-10, 10, 1, dtype=int)\n",
+                ")\n",
                 "\n",
                 "ds = shift_double_ended(ds, shift1)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we can calibrate the data double ended as usual."
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.11"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/12Datastore_from_numpy_arrays.ipynb` & `dtscalibration-2.0.0/docs/notebooks/12Datastore_from_numpy_arrays.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731194366635543%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(0, \'filepath = os.path.join("..", "..", "tests", "data", '*

 * *            '"single_ended")\\n\'), (2, \'ds_silixa = read_silixa_files(directory=filepath, '*

 * *            'silent=True)\')], delete: [3, 2, 0]}}, 7: {\'source\': {insert: [(1, \'ds["x"] = '*

 * *            '("x", x)\\n\'), (2, \'ds["time"] = ("time", time)\\n\'), (3, \'ds["st"] = (["x", '*

 * *            '"time"], ST)\\n\'), (4, \'ds["ast"] = (["x", "time"], AST)\')], delete: [4, 3, 2, '*

 * *            '1]}}, 10: {\'so […]*

```diff
@@ -55,18 +55,17 @@
                     "iopub.status.busy": "2022-04-06T08:11:07.172928Z",
                     "iopub.status.idle": "2022-04-06T08:11:07.369257Z",
                     "shell.execute_reply": "2022-04-06T08:11:07.368742Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'single_ended')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"single_ended\")\n",
                 "\n",
-                "ds_silixa = read_silixa_files(directory=filepath,\n",
-                "                              silent=True)"
+                "ds_silixa = read_silixa_files(directory=filepath, silent=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We will get all the numpy arrays from this `DataStore` to create a new one from 'scratch'.\n",
@@ -110,18 +109,18 @@
                     "iopub.status.idle": "2022-04-06T08:11:07.407067Z",
                     "shell.execute_reply": "2022-04-06T08:11:07.406546Z"
                 }
             },
             "outputs": [],
             "source": [
                 "ds = xr.Dataset()\n",
-                "ds['x'] = ('x', x)\n",
-                "ds['time'] = ('time', time)\n",
-                "ds['st'] = (['x', 'time'], ST)\n",
-                "ds['ast'] = (['x', 'time'], AST)"
+                "ds[\"x\"] = (\"x\", x)\n",
+                "ds[\"time\"] = (\"time\", time)\n",
+                "ds[\"st\"] = ([\"x\", \"time\"], ST)\n",
+                "ds[\"ast\"] = ([\"x\", \"time\"], AST)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -161,19 +160,20 @@
                     "iopub.status.busy": "2022-04-06T08:11:07.419639Z",
                     "iopub.status.idle": "2022-04-06T08:11:07.427490Z",
                     "shell.execute_reply": "2022-04-06T08:11:07.426850Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds['acquisitiontimeFW'] = ds_silixa['acquisitiontimeFW'].values\n",
-                "ds['temp1'] = ds_silixa['probe1Temperature']\n",
-                "ds['temp2'] = ds_silixa['probe2Temperature']\n",
+                "ds[\"acquisitiontimeFW\"] = ds_silixa[\"acquisitiontimeFW\"].values\n",
+                "ds[\"userAcquisitionTimeFW\"] = ds_silixa[\"acquisitiontimeFW\"].values\n",
+                "ds[\"temp1\"] = ds_silixa[\"probe1Temperature\"]\n",
+                "ds[\"temp2\"] = ds_silixa[\"probe2Temperature\"]\n",
                 "\n",
-                "ds.attrs['isDoubleEnded'] = '0'"
+                "ds.attrs[\"isDoubleEnded\"] = \"0\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we can calibrate the data as usual (ordinary least squares in this example)."
@@ -190,40 +190,58 @@
                     "shell.execute_reply": "2022-04-06T08:11:07.508335Z"
                 }
             },
             "outputs": [],
             "source": [
                 "ds = ds.sel(x=slice(-30, 101))\n",
                 "sections = {\n",
-                "            'temp1':    [slice(20, 25.5)],  # warm bath\n",
-                "            'temp2':    [slice(5.5, 15.5)],  # cold bath\n",
-                "            }\n",
+                "    \"temp1\": [slice(20, 25.5)],  # warm bath\n",
+                "    \"temp2\": [slice(5.5, 15.5)],  # cold bath\n",
+                "}\n",
                 "ds.sections = sections\n",
                 "\n",
-                "ds.calibration_single_ended(method='ols')\n",
+                "st_var, resid = ds.variance_stokes_constant(st_label=\"st\")\n",
+                "ast_var, _ = ds.variance_stokes_constant(st_label=\"ast\")\n",
+                "ds.calibration_single_ended(st_var=st_var, ast_var=ast_var)\n",
                 "\n",
-                "ds.isel(time=0).tmpf.plot()"
+                "ds.isel(time=0).tmpf.plot();"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ds"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.11"
+            "version": "3.10.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/14Lossy_splices.ipynb` & `dtscalibration-2.0.0/docs/notebooks/15Matching_sections.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.977610261889108%*

 * *Differences: {"'cells'": "{0: {'source': ['# 15. Calibration using matching sections']}, 1: {'source': {insert: "*

 * *            "[(0, 'In notebook 14 we showed how you can take splices or connectors within your "*

 * *            'calibration into account. To then calibrate the cable we used reference sections on '*

 * *            'both sides of the splice. If these are not available, or in other cases where you '*

 * *            'have a lack of reference sections, matching sections can be used to improve the '*

 * *            "calibratio […]*

```diff
@@ -1,214 +1,199 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# 14. Calibration over (lossy) splices and connectors"
+                "# 15. Calibration using matching sections"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Background\n",
-                "While it is best practice to not have connectors or splices within a DTS calibration, sometimes it can't be avoided. For example, in a borehole the fibers in a duplex cable are often connected with either a splice or a loopback connector. \n",
+                "In notebook 14 we showed how you can take splices or connectors within your calibration into account. To then calibrate the cable we used reference sections on both sides of the splice. If these are not available, or in other cases where you have a lack of reference sections, matching sections can be used to improve the calibration.\n",
                 "\n",
-                "Splices and connectors will cause a step loss in the signal strength, and with varying strain and temperature, this step loss will vary. In double ended setups this step loss can even be asymmetrical for the forward and backward measurements. All these effects have to be taken into account in the calibration.\n",
-                "\n",
-                "To calibrate over these splices/connectors, locations with 'transient attenuation' can be defined along the length of the fiber. Adding these does mean that more information is needed to perform the calibration, such as extra reference sections or matching sections of fiber. Matching sections will be explained in notebook 15.\n",
-                "\n"
+                "For matching sections you need two sections of fiber than you know will be the exact same temperature. This can be, for example, in duplex cables or twisted pairs of cable."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Demonstration\n",
-                "To demonstrate the effect of a lossy splice, we'll load the same dataset that was used in previous notebooks, and modify the data to simulate a lossy splice."
+                "To demonstrate matching sections, we'll load the same dataset that was used in previous notebooks, and modify the data to simulate a lossy splice, just as in notebook 14."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:11:25.641322Z",
-                    "iopub.status.busy": "2022-04-06T08:11:25.640590Z",
-                    "iopub.status.idle": "2022-04-06T08:11:27.122032Z",
-                    "shell.execute_reply": "2022-04-06T08:11:27.121371Z"
+                    "iopub.execute_input": "2022-04-06T08:11:42.175912Z",
+                    "iopub.status.busy": "2022-04-06T08:11:42.175058Z",
+                    "iopub.status.idle": "2022-04-06T08:11:43.633971Z",
+                    "shell.execute_reply": "2022-04-06T08:11:43.633285Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "\n",
                 "from dtscalibration import read_silixa_files\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:11:27.124582Z",
-                    "iopub.status.busy": "2022-04-06T08:11:27.124371Z",
-                    "iopub.status.idle": "2022-04-06T08:11:27.423254Z",
-                    "shell.execute_reply": "2022-04-06T08:11:27.422619Z"
+                    "iopub.execute_input": "2022-04-06T08:11:43.636636Z",
+                    "iopub.status.busy": "2022-04-06T08:11:43.636444Z",
+                    "iopub.status.idle": "2022-04-06T08:11:43.916858Z",
+                    "shell.execute_reply": "2022-04-06T08:11:43.916339Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
                 "\n",
-                "ds_ = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')\n",
+                "ds_ = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")\n",
                 "\n",
                 "ds = ds_.sel(x=slice(0, 110))  # only calibrate parts of the fiber\n",
                 "\n",
                 "\n",
                 "sections = {\n",
-                "    'probe1Temperature': [slice(7.5, 17.), slice(70., 80.)],  # cold bath\n",
-                "    'probe2Temperature': [slice(24., 34.), slice(85., 95.)],  # warm bath\n",
-                "    }\n",
+                "    \"probe1Temperature\": [slice(7.5, 17.0)],  # cold bath\n",
+                "    \"probe2Temperature\": [slice(24.0, 34.0)],  # warm bath\n",
+                "}\n",
                 "ds.sections = sections"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To simulate the lossy splice, we introduce a step loss in the signal strength at x = 50 m. For the forward channel, this means all data beyond 50 meters is reduced with a 'random' factor. For the backward channel, this means all data up to 50 meters is reduced with a 'random' factor.\n",
-                "\n",
-                "In the plots of the Stokes and anti-Stokes signal the big step loss is clearly visible."
+                "Again, we introduce a step loss in the signal strength at x = 50 m. For the forward channel, this means all data beyond 50 meters is reduced with a 'random' factor. For the backward channel, this means all data up to 50 meters is reduced with a 'random' factor."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:11:27.425744Z",
-                    "iopub.status.busy": "2022-04-06T08:11:27.425525Z",
-                    "iopub.status.idle": "2022-04-06T08:11:27.446200Z",
-                    "shell.execute_reply": "2022-04-06T08:11:27.444863Z"
+                    "iopub.execute_input": "2022-04-06T08:11:43.919445Z",
+                    "iopub.status.busy": "2022-04-06T08:11:43.919271Z",
+                    "iopub.status.idle": "2022-04-06T08:11:43.940161Z",
+                    "shell.execute_reply": "2022-04-06T08:11:43.939718Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds['st'] = ds.st.where(ds.x < 50, ds.st*.8)\n",
-                "ds['ast'] = ds.ast.where(ds.x < 50, ds.ast*.82)\n",
+                "ds[\"st\"] = ds.st.where(ds.x < 50, ds.st * 0.8)\n",
+                "ds[\"ast\"] = ds.ast.where(ds.x < 50, ds.ast * 0.82)\n",
                 "\n",
-                "ds['rst'] = ds.rst.where(ds.x > 50, ds.rst*.85)\n",
-                "ds['rast'] = ds.rast.where(ds.x > 50, ds.rast*.81)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "execution": {
-                    "iopub.execute_input": "2022-04-06T08:11:27.451194Z",
-                    "iopub.status.busy": "2022-04-06T08:11:27.450909Z",
-                    "iopub.status.idle": "2022-04-06T08:11:27.730773Z",
-                    "shell.execute_reply": "2022-04-06T08:11:27.730254Z"
-                }
-            },
-            "outputs": [],
-            "source": [
-                "ds.isel(time=0).st.plot(label='st')\n",
-                "ds.isel(time=0).ast.plot(label='ast')\n",
-                "ds.isel(time=0).rst.plot(label='rst')\n",
-                "ds.isel(time=0).rast.plot(label='rast')\n",
-                "plt.legend()"
+                "ds[\"rst\"] = ds.rst.where(ds.x > 50, ds.rst * 0.85)\n",
+                "ds[\"rast\"] = ds.rast.where(ds.x > 50, ds.rast * 0.81)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We will first run a calibration without adding the transient attenuation location. A big jump in the calibrated temperature is visible at x = 50, and all temperatures before the jump are too low, and the temperatures after the jump are too high."
+                "We will first run a calibration without adding the transient attenuation location or matching sections. A big jump in the calibrated temperature is visible at x = 50. \n",
+                "\n",
+                "As all calibration sections are before 50 meters, the first 50 m will be calibrated correctly."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:11:27.733065Z",
-                    "iopub.status.busy": "2022-04-06T08:11:27.732874Z",
-                    "iopub.status.idle": "2022-04-06T08:11:29.152616Z",
-                    "shell.execute_reply": "2022-04-06T08:11:29.152100Z"
+                    "iopub.execute_input": "2022-04-06T08:11:43.942589Z",
+                    "iopub.status.busy": "2022-04-06T08:11:43.942387Z",
+                    "iopub.status.idle": "2022-04-06T08:11:44.853767Z",
+                    "shell.execute_reply": "2022-04-06T08:11:44.853280Z"
                 }
             },
             "outputs": [],
             "source": [
                 "ds_a = ds.copy(deep=True)\n",
                 "\n",
-                "st_var, resid = ds_a.variance_stokes(st_label='st')\n",
-                "ast_var, _ = ds_a.variance_stokes(st_label='ast')\n",
-                "rst_var, _ = ds_a.variance_stokes(st_label='rst')\n",
-                "rast_var, _ = ds_a.variance_stokes(st_label='rast')\n",
+                "st_var, resid = ds_a.variance_stokes(st_label=\"st\")\n",
+                "ast_var, _ = ds_a.variance_stokes(st_label=\"ast\")\n",
+                "rst_var, _ = ds_a.variance_stokes(st_label=\"rst\")\n",
+                "rast_var, _ = ds_a.variance_stokes(st_label=\"rast\")\n",
                 "\n",
                 "ds_a.calibration_double_ended(\n",
                 "    st_var=st_var,\n",
                 "    ast_var=ast_var,\n",
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
-                "    store_tmpw='tmpw',\n",
-                "    method='wls',\n",
-                "    solver='sparse')\n",
+                "    store_tmpw=\"tmpw\",\n",
+                "    method=\"wls\",\n",
+                "    solver=\"sparse\",\n",
+                ")\n",
                 "\n",
-                "ds_a.isel(time=0).tmpw.plot(label='calibrated')"
+                "ds_a.isel(time=0).tmpw.plot(label=\"calibrated\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now we run a calibration, adding the keyword argument '**trans_att**', and provide a list of floats containing the locations of the splices. In this case we only add a single one at x = 50 m. After running the calibration you will see that by adding the transient attenuation location the calibration returns the correct temperature, without the big jump.\n",
+                "Now we run a calibration, adding the keyword argument '**trans_att**', and provide a list of floats containing the locations of the splices. In this case we only add a single one at x = 50 m.\n",
+                "\n",
+                "We will also define the matching sections of cable. The matching sections have to be provided as a list of tuples. A tuple per matching section. Each tuple has three items, the first two items are the slices of the sections that are matching. The third item is a bool and is True if the two sections have a reverse direction (as in the \"J-configuration\").\n",
+                "\n",
+                "In this example we match the two cold baths to each other.\n",
+                "\n",
+                "After running the calibration you will see that by adding the transient attenuation and matching sections the calibration returns the correct temperature, without the big jump.\n",
                 "\n",
                 "*In single-ended calibration the keyword is called '**trans_att**'.*"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2022-04-06T08:11:29.154854Z",
-                    "iopub.status.busy": "2022-04-06T08:11:29.154652Z",
-                    "iopub.status.idle": "2022-04-06T08:11:30.631923Z",
-                    "shell.execute_reply": "2022-04-06T08:11:30.631414Z"
+                    "iopub.execute_input": "2022-04-06T08:11:44.856090Z",
+                    "iopub.status.busy": "2022-04-06T08:11:44.855889Z",
+                    "iopub.status.idle": "2022-04-06T08:11:46.067901Z",
+                    "shell.execute_reply": "2022-04-06T08:11:46.067290Z"
                 }
             },
             "outputs": [],
             "source": [
-                "st_var, resid = ds.variance_stokes(st_label='st')\n",
-                "ast_var, _ = ds.variance_stokes(st_label='ast')\n",
-                "rst_var, _ = ds.variance_stokes(st_label='rst')\n",
-                "rast_var, _ = ds.variance_stokes(st_label='rast')\n",
+                "matching_sections = [(slice(7.5, 17.6), slice(69, 79.1), False)]\n",
+                "\n",
+                "st_var, resid = ds.variance_stokes(st_label=\"st\")\n",
+                "ast_var, _ = ds.variance_stokes(st_label=\"ast\")\n",
+                "rst_var, _ = ds.variance_stokes(st_label=\"rst\")\n",
+                "rast_var, _ = ds.variance_stokes(st_label=\"rast\")\n",
                 "\n",
                 "ds.calibration_double_ended(\n",
                 "    st_var=st_var,\n",
                 "    ast_var=ast_var,\n",
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
-                "    trans_att=[50.],\n",
-                "    store_tmpw='tmpw',\n",
-                "    method='wls',\n",
-                "    solver='sparse')\n",
+                "    trans_att=[50.0],\n",
+                "    matching_sections=matching_sections,\n",
+                "    store_tmpw=\"tmpw\",\n",
+                "    method=\"wls\",\n",
+                "    solver=\"sparse\",\n",
+                ")\n",
                 "\n",
-                "ds_a.isel(time=0).tmpw.plot(label='no trans. att.')\n",
-                "ds.isel(time=0).tmpw.plot(label='with trans. att.')\n",
+                "ds_a.isel(time=0).tmpw.plot(label=\"normal calibration\")\n",
+                "ds.isel(time=0).tmpw.plot(label=\"matching sections\")\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/16Averaging_temperatures.ipynb` & `dtscalibration-2.0.0/docs/notebooks/16Averaging_temperatures.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976107804232804%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, '\\n')]}}, 4: {'source': {insert: [(0, 'filepath = "*

 * *            'os.path.join("..", "..", "tests", "data", "double_ended2")\\n\'), (2, \'ds_ = '*

 * *            'read_silixa_files(directory=filepath, timezone_netcdf="UTC", file_ext="*.xml")\\n\'), '*

 * *            '(6, \'    "probe1Temperature": [slice(7.5, 17.0), slice(70.0, 80.0)],  # cold '*

 * *            'bath\\n\'), (7, \'    "probe2Temperature": [slice(24.0, 34.0), slice(85.0, 95.0)],  # '*

 * *            "warm bath\\n'),  […]*

```diff
@@ -34,14 +34,15 @@
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "\n",
                 "from dtscalibration import read_silixa_files\n",
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -50,26 +51,23 @@
                     "iopub.status.busy": "2022-04-06T08:11:57.558858Z",
                     "iopub.status.idle": "2022-04-06T08:11:57.856068Z",
                     "shell.execute_reply": "2022-04-06T08:11:57.855409Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'double_ended2')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"double_ended2\")\n",
                 "\n",
-                "ds_ = read_silixa_files(\n",
-                "    directory=filepath,\n",
-                "    timezone_netcdf='UTC',\n",
-                "    file_ext='*.xml')\n",
+                "ds_ = read_silixa_files(directory=filepath, timezone_netcdf=\"UTC\", file_ext=\"*.xml\")\n",
                 "\n",
                 "ds = ds_.sel(x=slice(0, 100))  # only calibrate parts of the fiber\n",
                 "sections = {\n",
-                "    'probe1Temperature': [slice(7.5, 17.), slice(70., 80.)],  # cold bath\n",
-                "    'probe2Temperature': [slice(24., 34.), slice(85., 95.)],  # warm bath\n",
-                "    }\n",
+                "    \"probe1Temperature\": [slice(7.5, 17.0), slice(70.0, 80.0)],  # cold bath\n",
+                "    \"probe2Temperature\": [slice(24.0, 34.0), slice(85.0, 95.0)],  # warm bath\n",
+                "}\n",
                 "ds.sections = sections"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -78,18 +76,18 @@
                     "iopub.status.busy": "2022-04-06T08:11:57.858350Z",
                     "iopub.status.idle": "2022-04-06T08:11:58.597727Z",
                     "shell.execute_reply": "2022-04-06T08:11:58.597067Z"
                 }
             },
             "outputs": [],
             "source": [
-                "st_var, resid = ds.variance_stokes(st_label='st')\n",
-                "ast_var, _ = ds.variance_stokes(st_label='ast')\n",
-                "rst_var, _ = ds.variance_stokes(st_label='rst')\n",
-                "rast_var, _ = ds.variance_stokes(st_label='rast')"
+                "st_var, resid = ds.variance_stokes(st_label=\"st\")\n",
+                "ast_var, _ = ds.variance_stokes(st_label=\"ast\")\n",
+                "rst_var, _ = ds.variance_stokes(st_label=\"rst\")\n",
+                "rast_var, _ = ds.variance_stokes(st_label=\"rast\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -102,17 +100,18 @@
             "outputs": [],
             "source": [
                 "ds.calibration_double_ended(\n",
                 "    st_var=st_var,\n",
                 "    ast_var=ast_var,\n",
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
-                "    store_tmpw='tmpw',\n",
-                "    method='wls',\n",
-                "    solver='sparse')"
+                "    store_tmpw=\"tmpw\",\n",
+                "    method=\"wls\",\n",
+                "    solver=\"sparse\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Confidence intervals of averages\n",
@@ -188,16 +187,17 @@
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
                 "    conf_ints=[2.5, 97.5],\n",
                 "    mc_sample_size=500,  # <- choose a much larger sample size\n",
                 "    ci_avg_time_flag1=True,\n",
                 "    ci_avg_time_flag2=False,\n",
                 "    ci_avg_time_isel=[0, 1, 2, 3, 4, 5],\n",
-                "    ci_avg_time_sel=None)\n",
-                "ds.tmpw_mc_avg1.plot(hue='CI', linewidth=0.8);"
+                "    ci_avg_time_sel=None,\n",
+                ")\n",
+                "ds.tmpw_mc_avg1.plot(hue=\"CI\", linewidth=0.8);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 2. Averaging over time while assuming the temperature remains constant over time but varies along the fiber"
@@ -247,16 +247,17 @@
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
                 "    conf_ints=[2.5, 97.5],\n",
                 "    mc_sample_size=500,  # <- choose a much larger sample size\n",
                 "    ci_avg_time_flag1=False,\n",
                 "    ci_avg_time_flag2=True,\n",
                 "    ci_avg_time_isel=[0, 1, 2, 3, 4, 5],\n",
-                "    ci_avg_time_sel=None)\n",
-                "ds.tmpw_mc_avg2.plot(hue='CI', linewidth=0.8);"
+                "    ci_avg_time_sel=None,\n",
+                ")\n",
+                "ds.tmpw_mc_avg2.plot(hue=\"CI\", linewidth=0.8);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 3. Averaging along the fiber while the temperature varies along the cable and over time"
@@ -305,17 +306,18 @@
                 "    ast_var=ast_var,\n",
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
                 "    conf_ints=[2.5, 97.5],\n",
                 "    mc_sample_size=500,  # <- choose a much larger sample size\n",
                 "    ci_avg_x_flag1=True,\n",
                 "    ci_avg_x_flag2=False,\n",
-                "    ci_avg_x_sel=slice(7.5, 17.),\n",
-                "    ci_avg_x_isel=None)\n",
-                "ds.tmpw_mc_avgx1.plot(hue='CI', linewidth=0.8);"
+                "    ci_avg_x_sel=slice(7.5, 17.0),\n",
+                "    ci_avg_x_isel=None,\n",
+                ")\n",
+                "ds.tmpw_mc_avgx1.plot(hue=\"CI\", linewidth=0.8);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### 4. Averaging along the fiber while assuming the temperature is same along the fiber but varies over time"
@@ -364,17 +366,18 @@
                 "    ast_var=ast_var,\n",
                 "    rst_var=rst_var,\n",
                 "    rast_var=rast_var,\n",
                 "    conf_ints=[2.5, 97.5],\n",
                 "    mc_sample_size=500,  # <- choose a much larger sample size\n",
                 "    ci_avg_x_flag1=False,\n",
                 "    ci_avg_x_flag2=True,\n",
-                "    ci_avg_x_sel=slice(7.5, 17.),\n",
-                "    ci_avg_x_isel=None)\n",
-                "ds.tmpw_mc_avgx2.plot(hue='CI', linewidth=0.8);"
+                "    ci_avg_x_sel=slice(7.5, 17.0),\n",
+                "    ci_avg_x_isel=None,\n",
+                ")\n",
+                "ds.tmpw_mc_avgx2.plot(hue=\"CI\", linewidth=0.8);"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/A3Load_ap_sensing_files.ipynb` & `dtscalibration-2.0.0/docs/notebooks/A3Load_ap_sensing_files.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986111111111111%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(0, \'filepath = os.path.join("..", "..", "tests", "data", '*

 * *            '"ap_sensing")\\n\')], delete: [0]}}, 4: {\'source\': {insert: [(0, \'filepathlist = '*

 * *            'sorted(glob.glob(os.path.join(filepath, "*.xml")))\\n\')], delete: [0]}}}'}*

```diff
@@ -43,15 +43,15 @@
                     "iopub.status.busy": "2022-04-06T08:12:31.219507Z",
                     "iopub.status.idle": "2022-04-06T08:12:31.225338Z",
                     "shell.execute_reply": "2022-04-06T08:12:31.224123Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'ap_sensing')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"ap_sensing\")\n",
                 "print(filepath)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -60,15 +60,15 @@
                     "iopub.status.busy": "2022-04-06T08:12:31.254433Z",
                     "iopub.status.idle": "2022-04-06T08:12:31.259760Z",
                     "shell.execute_reply": "2022-04-06T08:12:31.258995Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepathlist = sorted(glob.glob(os.path.join(filepath, '*.xml')))\n",
+                "filepathlist = sorted(glob.glob(os.path.join(filepath, \"*.xml\")))\n",
                 "filenamelist = [os.path.basename(path) for path in filepathlist]\n",
                 "\n",
                 "for fn in filenamelist:\n",
                 "    print(fn)"
             ]
         },
         {
```

### Comparing `dtscalibration-1.2.0/docs/notebooks/A4Load_sensortran_files.ipynb` & `dtscalibration-2.0.0/docs/notebooks/A4Load_sensortran_files.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969350961538461%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, '\\n'), (6, '\\n')], delete: [5]}}, 3: {'source': "*

 * *            '{insert: [(0, \'filepath = os.path.join("..", "..", "tests", "data", '*

 * *            '"sensortran_binary")\\n\')], delete: [0]}}, 4: {\'source\': {insert: [(0, '*

 * *            '\'filepathlist = sorted(glob.glob(os.path.join(filepath, "*.dat")))\\n\')], delete: '*

 * *            '[0]}}, 11: {\'source\': {insert: [(3, \'ds0.st.plot(label="Stokes signal")\\n\'), (4, '*

 * *            '\'plt.axhline(ds0.st_zero.values […]*

```diff
@@ -22,16 +22,17 @@
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import glob\n",
                 "import matplotlib.pyplot as plt\n",
                 "from pandas.plotting import register_matplotlib_converters\n",
+                "\n",
                 "register_matplotlib_converters()\n",
-                "    \n",
+                "\n",
                 "from dtscalibration import read_sensortran_files"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -47,15 +48,15 @@
                     "iopub.status.busy": "2022-04-06T08:12:42.792258Z",
                     "iopub.status.idle": "2022-04-06T08:12:42.796234Z",
                     "shell.execute_reply": "2022-04-06T08:12:42.795702Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepath = os.path.join('..', '..', 'tests', 'data', 'sensortran_binary')\n",
+                "filepath = os.path.join(\"..\", \"..\", \"tests\", \"data\", \"sensortran_binary\")\n",
                 "print(filepath)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -64,15 +65,15 @@
                     "iopub.status.busy": "2022-04-06T08:12:42.823092Z",
                     "iopub.status.idle": "2022-04-06T08:12:42.827800Z",
                     "shell.execute_reply": "2022-04-06T08:12:42.827277Z"
                 }
             },
             "outputs": [],
             "source": [
-                "filepathlist = sorted(glob.glob(os.path.join(filepath, '*.dat')))\n",
+                "filepathlist = sorted(glob.glob(os.path.join(filepath, \"*.dat\")))\n",
                 "filenamelist = [os.path.basename(path) for path in filepathlist]\n",
                 "\n",
                 "for fn in filenamelist:\n",
                 "    print(fn)"
             ]
         },
         {
@@ -158,19 +159,19 @@
                 }
             },
             "outputs": [],
             "source": [
                 "ds0 = ds.isel(time=0)\n",
                 "\n",
                 "plt.figure()\n",
-                "ds0.st.plot(label='Stokes signal')\n",
-                "plt.axhline(ds0.st_zero.values, c='r', label=\"'zero' measurement\")\n",
+                "ds0.st.plot(label=\"Stokes signal\")\n",
+                "plt.axhline(ds0.st_zero.values, c=\"r\", label=\"'zero' measurement\")\n",
                 "plt.legend()\n",
-                "plt.title('')\n",
-                "plt.axhline(c='k')"
+                "plt.title(\"\")\n",
+                "plt.axhline(c=\"k\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "After a correction and rescaling (for human readability) the data will look more like other manufacturer's devices"
@@ -185,16 +186,16 @@
                     "iopub.status.busy": "2022-04-06T08:12:43.132864Z",
                     "iopub.status.idle": "2022-04-06T08:12:43.149273Z",
                     "shell.execute_reply": "2022-04-06T08:12:43.148278Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds['st'] = (ds.st - ds.st_zero)/1e4\n",
-                "ds['ast'] = (ds.ast - ds.ast_zero)/1e4"
+                "ds[\"st\"] = (ds.st - ds.st_zero) / 1e4\n",
+                "ds[\"ast\"] = (ds.ast - ds.ast_zero) / 1e4"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "execution": {
@@ -202,21 +203,21 @@
                     "iopub.status.busy": "2022-04-06T08:12:43.153959Z",
                     "iopub.status.idle": "2022-04-06T08:12:43.197810Z",
                     "shell.execute_reply": "2022-04-06T08:12:43.196411Z"
                 }
             },
             "outputs": [],
             "source": [
-                "ds.isel(time=0).st.plot(label='Stokes intensity')\n",
-                "ds.isel(time=0).ast.plot(label='anti-Stokes intensity')\n",
+                "ds.isel(time=0).st.plot(label=\"Stokes intensity\")\n",
+                "ds.isel(time=0).ast.plot(label=\"anti-Stokes intensity\")\n",
                 "plt.legend()\n",
-                "plt.axhline(c='k', lw=1)\n",
-                "plt.xlabel('')\n",
-                "plt.title('')\n",
-                "plt.ylim([-50,500])"
+                "plt.axhline(c=\"k\", lw=1)\n",
+                "plt.xlabel(\"\")\n",
+                "plt.title(\"\")\n",
+                "plt.ylim([-50, 500])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `dtscalibration-1.2.0/examples/Added uncertainty from fixing parameters.pdf` & `dtscalibration-2.0.0/examples/Added uncertainty from fixing parameters.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/examples/temperature_variance_from_stokes.pdf` & `dtscalibration-2.0.0/examples/temperature_variance_from_stokes.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/examples/conference presentations/EGU2019_poster_dtscalibration.pdf` & `dtscalibration-2.0.0/examples/conference presentations/EGU2019_poster_dtscalibration.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf` & `dtscalibration-2.0.0/examples/conference presentations/EGU2020_presentation_dtscalibration_pyfocs.pdf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/src/dtscalibration/__init__.py` & `dtscalibration-2.0.0/src/dtscalibration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .datastore_utils import suggest_cable_shift_double_ended
 from .plot import plot_accuracy
 from .plot import plot_location_residuals_double_ended
 from .plot import plot_residuals_reference_sections
 from .plot import plot_residuals_reference_sections_single
 from .plot import plot_sigma_report
 
-__version__ = '1.2.0'
+__version__ = '2.0.0'
 __all__ = [
     "DataStore", "open_datastore", "open_mf_datastore", "read_apsensing_files",
     "read_sensornet_files", "read_sensortran_files", "read_silixa_files",
     'check_dims', 'check_timestep_allclose', 'get_netcdf_encoding',
     'merge_double_ended', 'shift_double_ended',
     'suggest_cable_shift_double_ended', 'plot_accuracy',
     'plot_location_residuals_double_ended',
```

### Comparing `dtscalibration-1.2.0/src/dtscalibration/calibrate_utils.py` & `dtscalibration-2.0.0/src/dtscalibration/calibrate_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # coding=utf-8
 import numpy as np
 import scipy.sparse as sp
 import statsmodels.api as sm
+import xarray as xr
 from scipy.sparse import linalg as ln
 
 
-def parse_st_var(ds, st_var, st_label='st', ix_sel=None):
+def parse_st_var(ds, st_var, st_label='st'):
     """
-    Utility function to check the st_var input, and to return in the correct
+    Utility function to check the st_var input and to return in DataArray
     format.
 
     Parameters
     ----------
     ds : DataStore
     st_var : float, callable, array-like
         If `float` the variance of the noise from the Stokes detector is
@@ -20,48 +21,30 @@
         a function of the intensity, as defined in the callable function.
         Or when the variance is a function of the intensity (Poisson
         distributed) define a DataArray of the shape shape as ds.st, where the
         variance can be a function of time and/or x.
     st_label : string
         Name of the (reverse) stokes/anti-stokes data variable which is being
         parsed.
-    ix_sel : None, array-like
-        Index mapping along the x-dimension to apply to st_var. Definition
-        required when st_var is array-like
 
     Returns
     -------
     Parsed st_var
     """
     if callable(st_var):
-        st_var_sec = st_var(ds[st_label].isel(x=ix_sel)).values
-
-    elif np.size(st_var) > 1:
-        if ix_sel is None:
-            raise ValueError(
-                '`ix_sel` kwarg not defined while `st_var` is array-like')
-
-        for a, b in zip(st_var.shape[::-1], ds[st_label].shape[::-1]):
-            if a == 1 or b == 1 or a == b:
-                pass
-            else:
-                raise ValueError(
-                    st_label + '_var is not broadcastable to ds.' + st_label)
-
-        if len(st_var.shape) > 1:
-            st_var_sec = np.asarray(st_var, dtype=float)[ix_sel]
-        else:
-            st_var_sec = np.asarray(st_var, dtype=float)
-
+        st_var_sec = st_var(ds[st_label])
     else:
-        st_var_sec = np.asarray(st_var, dtype=float)
+        st_var_sec = xr.ones_like(ds[st_label]) * st_var
 
     assert np.all(np.isfinite(st_var_sec)), \
         'NaN/inf values detected in ' + st_label + '_var. Please check input.'
 
+    assert np.all(st_var_sec > 0.), \
+        'Negative values detected in ' + st_label + '_var. Please check input.'
+
     return st_var_sec
 
 
 # pylint: disable=too-many-arguments,too-many-locals
 def calibration_single_ended_solver(  # noqa: MC0001
         ds,
         st_var=None,
@@ -74,21 +57,21 @@
     The solver for single-ended setups. Assumes `ds` is pre-configured with
     `sections` and `trans_att`.
 
     Parameters
     ----------
     ds : DataStore
     st_var : float, array-like, optional
-        If `None` use ols calibration. If `float` the variance of the noise
+        If `float` the variance of the noise
         from the Stokes detector is described with a single value. Or when the
         variance is a function of the intensity (Poisson distributed) define an
         array with shape (nx, nt), where nx are the number of calibration
         locations.
     ast_var : float, array-like, optional
-        If `None` use ols calibration. If `float` the variance of the noise
+        If `float` the variance of the noise
         from the Stokes detector is described with a single value. Or when the
         variance is a function of the intensity (Poisson distributed) define an
         array with shape (nx, nt), where nx are the number of calibration
         locations.
     calc_cov : bool
         whether to calculate the covariance matrix. Required for calculation
         of confidence boundaries. But uses a lot of memory.
@@ -252,29 +235,29 @@
             np.log(ds_ms0.st.values / ds_ms0.ast.values)
             - np.log(ds_ms1.st.values / ds_ms1.ast.values)).T.ravel()
 
         y = np.hstack((y, y_m))
 
     # w
     if st_var is not None:
-        st_var_sec = parse_st_var(ds, st_var, st_label='st', ix_sel=ix_sec)
-        ast_var_sec = parse_st_var(ds, ast_var, st_label='ast', ix_sel=ix_sec)
+        st_var_sec = parse_st_var(ds, st_var, st_label='st').isel(x=ix_sec).values
+        ast_var_sec = parse_st_var(ds, ast_var, st_label='ast').isel(x=ix_sec).values
 
         w = 1 / (ds_sec.st**-2 * st_var_sec
                  + ds_sec.ast**-2 * ast_var_sec).values.ravel()
 
         if np.any(matching_indices):
             st_var_ms0 = parse_st_var(
-                ds, st_var, st_label='st', ix_sel=matching_indices[:, 0])
+                ds, st_var, st_label='st').isel(x=matching_indices[:, 0]).values
             st_var_ms1 = parse_st_var(
-                ds, st_var, st_label='st', ix_sel=matching_indices[:, 1])
+                ds, st_var, st_label='st').isel(x=matching_indices[:, 1]).values
             ast_var_ms0 = parse_st_var(
-                ds, ast_var, st_label='ast', ix_sel=matching_indices[:, 0])
+                ds, ast_var, st_label='ast').isel(x=matching_indices[:, 0]).values
             ast_var_ms1 = parse_st_var(
-                ds, ast_var, st_label='ast', ix_sel=matching_indices[:, 1])
+                ds, ast_var, st_label='ast').isel(x=matching_indices[:, 1]).values
 
             w_ms = 1 / (
                 (ds_ms0.st.values**-2 * st_var_ms0) +
                 (ds_ms0.ast.values**-2 * ast_var_ms0) +
                 (ds_ms1.st.values**-2 * st_var_ms1) +
                 (ds_ms1.ast.values**-2 * ast_var_ms1)).ravel()
 
@@ -350,33 +333,33 @@
     y = [F, B, (B-F)/2], F=[F_0, F_1, .., F_M], B=[B_0, B_1, .., B_M],
     where F_m and B_m contain the coefficients for all times.
 
     Parameters
     ----------
     ds : DataStore
     st_var : float, array-like, optional
-        If `None` use ols calibration. If `float` the variance of the noise
+        If `float` the variance of the noise
         from the Stokes detector is described with a single value. Or when the
         variance is a function of the intensity (Poisson distributed) define an
         array with shape (nx, nt), where nx are the number of calibration
         locations.
     ast_var : float, array-like, optional
-        If `None` use ols calibration. If `float` the variance of the noise
+        If `float` the variance of the noise
         from the Stokes detector is described with a single value. Or when the
         variance is a function of the intensity (Poisson distributed) define an
         array with shape (nx, nt), where nx are the number of calibration
         locations.
     rst_var : float, array-like, optional
-        If `None` use ols calibration. If `float` the variance of the noise
+        If `float` the variance of the noise
         from the Stokes detector is described with a single value. Or when the
         variance is a function of the intensity (Poisson distributed) define an
         array with shape (nx, nt), where nx are the number of calibration
         locations.
     rast_var : float, array-like, optional
-        If `None` use ols calibration. If `float` the variance of the noise
+        If `float` the variance of the noise
         from the Stokes detector is described with a single value. Or when the
         variance is a function of the intensity (Poisson distributed) define an
         array with shape (nx, nt), where nx are the number of calibration
         locations.
     calc_cov : bool
         whether to calculate the covariance matrix. Required for calculation
         of confidence boundaries. But uses a lot of memory.
@@ -420,30 +403,25 @@
         construct_submatrices(nt, nx_sec, ds, ds.trans_att.values, x_sec)
 
     # y  # Eq.41--45
     y_F = np.log(ds_sec.st / ds_sec.ast).values.ravel()
     y_B = np.log(ds_sec.rst / ds_sec.rast).values.ravel()
 
     # w
-    if st_var is not None:  # WLS
-        st_var_sec = parse_st_var(ds, st_var, st_label='st', ix_sel=ix_sec)
-        ast_var_sec = parse_st_var(ds, ast_var, st_label='ast', ix_sel=ix_sec)
-        rst_var_sec = parse_st_var(ds, rst_var, st_label='rst', ix_sel=ix_sec)
-        rast_var_sec = parse_st_var(
-            ds, rast_var, st_label='rast', ix_sel=ix_sec)
-
-        w_F = 1 / (ds_sec.st**-2 * st_var_sec
-                   + ds_sec.ast**-2 * ast_var_sec).values.ravel()
-        w_B = 1 / (
-            ds_sec.rst**-2 * rst_var_sec
-            + ds_sec.rast**-2 * rast_var_sec).values.ravel()
-
-    else:  # OLS
-        w_F = np.ones(nt * nx_sec)
-        w_B = np.ones(nt * nx_sec)
+    st_var_sec = parse_st_var(ds, st_var, st_label='st').isel(x=ix_sec).values
+    ast_var_sec = parse_st_var(ds, ast_var, st_label='ast').isel(x=ix_sec).values
+    rst_var_sec = parse_st_var(ds, rst_var, st_label='rst').isel(x=ix_sec).values
+    rast_var_sec = parse_st_var(
+        ds, rast_var, st_label='rast').isel(x=ix_sec).values
+
+    w_F = 1 / (ds_sec.st**-2 * st_var_sec
+               + ds_sec.ast**-2 * ast_var_sec).values.ravel()
+    w_B = 1 / (
+        ds_sec.rst**-2 * rst_var_sec
+        + ds_sec.rast**-2 * rast_var_sec).values.ravel()
 
     if not np.any(matching_indices):
         p0_est = np.concatenate(
             (
                 [485.], df_est, db_est, E_all_guess[ix_sec[1:]],
                 nta * nt * 2 * [0.]))
 
@@ -517,32 +495,32 @@
         y_eq3 = (
             (
                 np.log(ds_mnc.rst / ds_mnc.rast)
                 - np.log(ds_mnc.st / ds_mnc.ast)) / 2).values.ravel()
 
         y = np.concatenate((y_F, y_B, y_eq1, y_eq2, y_eq3))
 
-        st_var_hix = parse_st_var(ds, st_var, st_label='st', ix_sel=hix)
-        ast_var_hix = parse_st_var(ds, ast_var, st_label='ast', ix_sel=hix)
-        rst_var_hix = parse_st_var(ds, rst_var, st_label='rst', ix_sel=hix)
-        rast_var_hix = parse_st_var(ds, rast_var, st_label='rast', ix_sel=hix)
-
-        st_var_tix = parse_st_var(ds, st_var, st_label='st', ix_sel=tix)
-        ast_var_tix = parse_st_var(ds, ast_var, st_label='ast', ix_sel=tix)
-        rst_var_tix = parse_st_var(ds, rst_var, st_label='rst', ix_sel=tix)
-        rast_var_tix = parse_st_var(ds, rast_var, st_label='rast', ix_sel=tix)
+        st_var_hix = parse_st_var(ds, st_var, st_label='st').isel(x=hix).values
+        ast_var_hix = parse_st_var(ds, ast_var, st_label='ast').isel(x=hix).values
+        rst_var_hix = parse_st_var(ds, rst_var, st_label='rst').isel(x=hix).values
+        rast_var_hix = parse_st_var(ds, rast_var, st_label='rast').isel(x=hix).values
+
+        st_var_tix = parse_st_var(ds, st_var, st_label='st').isel(x=tix).values
+        ast_var_tix = parse_st_var(ds, ast_var, st_label='ast').isel(x=tix).values
+        rst_var_tix = parse_st_var(ds, rst_var, st_label='rst').isel(x=tix).values
+        rast_var_tix = parse_st_var(ds, rast_var, st_label='rast').isel(x=tix).values
 
         st_var_mnc = parse_st_var(
-            ds, st_var, st_label='st', ix_sel=ix_match_not_cal)
+            ds, st_var, st_label='st').isel(x=ix_match_not_cal).values
         ast_var_mnc = parse_st_var(
-            ds, ast_var, st_label='ast', ix_sel=ix_match_not_cal)
+            ds, ast_var, st_label='ast').isel(x=ix_match_not_cal).values
         rst_var_mnc = parse_st_var(
-            ds, rst_var, st_label='rst', ix_sel=ix_match_not_cal)
+            ds, rst_var, st_label='rst').isel(x=ix_match_not_cal).values
         rast_var_mnc = parse_st_var(
-            ds, rast_var, st_label='rast', ix_sel=ix_match_not_cal)
+            ds, rast_var, st_label='rast').isel(x=ix_match_not_cal).values
 
         w_eq1 = 1 / (
             (ds_hix.st**-2 * st_var_hix
              + ds_hix.ast**-2 * ast_var_hix).values.ravel() +
             (ds_tix.st**-2 * st_var_tix
              + ds_tix.ast**-2 * ast_var_tix).values.ravel())
         w_eq2 = 1 / (
```

### Comparing `dtscalibration-1.2.0/src/dtscalibration/datastore.py` & `dtscalibration-2.0.0/src/dtscalibration/datastore.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from scipy.optimize import minimize
 from scipy.sparse import linalg as ln
 
 from .calibrate_utils import calc_alpha_double
 from .calibrate_utils import calibration_double_ended_solver
 from .calibrate_utils import calibration_single_ended_solver
 from .calibrate_utils import match_sections
+from .calibrate_utils import parse_st_var
 from .calibrate_utils import wls_sparse
 from .calibrate_utils import wls_stats
 from .datastore_utils import check_timestep_allclose
 from .io import _dim_attrs
 from .io import apsensing_xml_version_check
 from .io import read_apsensing_files_routine
 from .io import read_sensornet_files_routine_v3
@@ -45,54 +46,54 @@
 # pylint: disable=W605
 class DataStore(xr.Dataset):
     """The data class that stores the measurements, contains calibration
     methods to relate Stokes and anti-Stokes to temperature. The user should
     never initiate this class directly, but use read_xml_dir or open_datastore
     functions instead.
 
-        Parameters
-        ----------
-        data_vars : dict-like, optional
-            A mapping from variable names to :py:class:`~xarray.DataArray`
-            objects, :py:class:`~xarray.Variable` objects or tuples of the
-            form ``(dims, data[, attrs])`` which can be used as arguments to
-            create a new ``Variable``. Each dimension must have the same length
-            in all variables in which it appears.
-        coords : dict-like, optional
-            Another mapping in the same form as the `variables` argument,
-            except the each item is saved on the datastore as a "coordinate".
-            These variables have an associated meaning: they describe
-            constant/fixed/independent quantities, unlike the
-            varying/measured/dependent quantities that belong in `variables`.
-            Coordinates values may be given by 1-dimensional arrays or scalars,
-            in which case `dims` do not need to be supplied: 1D arrays will be
-            assumed to give index values along the dimension with the same
-            name.
-        attrs : dict-like, optional
-            Global attributes to save on this datastore.
-        sections : Dict[str, List[slice]], optional
-            Sections for calibration. The dictionary should contain key-var
-            couples in which the key is the name of the calibration temp time
-            series. And the var is a list of slice objects as 'slice(start,
-            stop)'; start and stop in meter (float).
-        compat : {'broadcast_equals', 'equals', 'identical'}, optional
-            String indicating how to compare variables of the same name for
-            potential conflicts when initializing this datastore:
-            - 'broadcast_equals': all values must be equal when variables are
-              broadcast against each other to ensure common dimensions.
-            - 'equals': all values and dimensions must be the same.
-            - 'identical': all values, dimensions and attributes must be the
-              same.
-
-        See Also
-        --------
-        dtscalibration.read_xml_dir : Load measurements stored in XML-files
-        dtscalibration.open_datastore : Load (calibrated) measurements from
-        netCDF-like file
-        """
+    Parameters
+    ----------
+    data_vars : dict-like, optional
+        A mapping from variable names to :py:class:`~xarray.DataArray`
+        objects, :py:class:`~xarray.Variable` objects or tuples of the
+        form ``(dims, data[, attrs])`` which can be used as arguments to
+        create a new ``Variable``. Each dimension must have the same length
+        in all variables in which it appears.
+    coords : dict-like, optional
+        Another mapping in the same form as the `variables` argument,
+        except the each item is saved on the datastore as a "coordinate".
+        These variables have an associated meaning: they describe
+        constant/fixed/independent quantities, unlike the
+        varying/measured/dependent quantities that belong in `variables`.
+        Coordinates values may be given by 1-dimensional arrays or scalars,
+        in which case `dims` do not need to be supplied: 1D arrays will be
+        assumed to give index values along the dimension with the same
+        name.
+    attrs : dict-like, optional
+        Global attributes to save on this datastore.
+    sections : Dict[str, List[slice]], optional
+        Sections for calibration. The dictionary should contain key-var
+        couples in which the key is the name of the calibration temp time
+        series. And the var is a list of slice objects as 'slice(start,
+        stop)'; start and stop in meter (float).
+    compat : {'broadcast_equals', 'equals', 'identical'}, optional
+        String indicating how to compare variables of the same name for
+        potential conflicts when initializing this datastore:
+         - 'broadcast_equals': all values must be equal when variables are
+           broadcast against each other to ensure common dimensions.
+         - 'equals': all values and dimensions must be the same.
+         - 'identical': all values, dimensions and attributes must be the
+           same.
+
+    See Also
+    --------
+    dtscalibration.read_xml_dir : Load measurements stored in XML-files
+    dtscalibration.open_datastore : Load (calibrated) measurements from
+    netCDF-like file
+    """
     def __init__(self, *args, autofill_dim_attrs=True, **kwargs):
         super().__init__(*args, **kwargs)
 
         # check order of the dimensions of the data_vars
         # first 'x' (if in initiated DataStore), then 'time', then the rest
         ideal_dim = []  # perfect order dims
         all_dim = list(self.dims)
@@ -1829,38 +1830,39 @@
                 raise ValueError(
                     'Time dimension of the reference temperature timeseries '
                     + key + 'is not the same as the time dimension'
                     + ' of the Stokes measurement. See examples/notebooks/09'
                     + 'Import_timeseries.ipynb for more info')
 
     def calibration_single_ended(
-            self,
-            sections=None,
-            st_var=None,
-            ast_var=None,
-            store_c='c',
-            store_gamma='gamma',
-            store_dalpha='dalpha',
-            store_alpha='alpha',
-            store_ta='talpha',
-            store_tmpf='tmpf',
-            store_p_cov='p_cov',
-            store_p_val='p_val',
-            variance_suffix='_var',
-            method='wls',
-            solver='sparse',
-            p_val=None,
-            p_var=None,
-            p_cov=None,
-            matching_sections=None,
-            trans_att=None,
-            fix_gamma=None,
-            fix_dalpha=None,
-            fix_alpha=None,
-            **kwargs):
+        self,
+        sections=None,
+        st_var=None,
+        ast_var=None,
+        store_c="c",
+        store_gamma="gamma",
+        store_dalpha="dalpha",
+        store_alpha="alpha",
+        store_ta="talpha",
+        store_tmpf="tmpf",
+        store_p_cov="p_cov",
+        store_p_val="p_val",
+        variance_suffix="_var",
+        method="wls",
+        solver="sparse",
+        p_val=None,
+        p_var=None,
+        p_cov=None,
+        matching_sections=None,
+        trans_att=None,
+        fix_gamma=None,
+        fix_dalpha=None,
+        fix_alpha=None,
+        **kwargs
+    ):
         """
         Calibrate the Stokes (`ds.st`) and anti-Stokes (`ds.ast`) data to
         temperature using fiber sections with a known temperature
         (`ds.sections`) for single-ended setups. The calibrated temperature is
         stored under `ds.tmpf` and its variance under `ds.tmpf_var`.
 
         In single-ended setups, Stokes and anti-Stokes intensity is measured
@@ -1954,18 +1956,17 @@
             Label of where to store transient alpha's
         store_tmpf : str
             Label of where to store the calibrated temperature of the forward
             direction
         variance_suffix : str
             String appended for storing the variance. Only used when method
             is wls.
-        method : {'ols', 'wls'}
-            Use `'ols'` for ordinary least squares and `'wls'` for weighted least
-            squares. `'wls'` is the default, and there is currently no reason to
-            use `'ols'`.
+        method : {'wls',}
+            Use `'wls'` for weighted least
+            squares.
         solver : {'sparse', 'stats'}
             Either use the homemade weighted sparse solver or the weighted
             dense matrix solver of statsmodels. The sparse solver uses much less
             memory, is faster, and gives the same result as the statsmodels
             solver. The statsmodels solver is mostly used to check the sparse
             solver. `'stats'` is the default.
         matching_sections : List[Tuple[slice, slice, bool]], optional
@@ -2003,350 +2004,420 @@
             of Temperature and Associated Uncertainty from Fiber-Optic Raman-
             Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235.
             https://doi.org/10.3390/s20082235
 
         Examples
         --------
         - `Example notebook 7: Calibrate single ended <https://github.com/\
-dtscalibration/python-dts-calibration/blob/main/examples/notebooks/\
-07Calibrate_single_wls.ipynb>`_
+    dtscalibration/python-dts-calibration/blob/main/examples/notebooks/\
+    07Calibrate_single_wls.ipynb>`_
 
         """
         self.check_deprecated_kwargs(kwargs)
         self.set_trans_att(trans_att=trans_att, **kwargs)
 
         if sections:
             self.sections = sections
         else:
-            assert self.sections, 'sections are not defined'
+            assert self.sections, "sections are not defined"
 
-        if method == 'wls':
-            assert st_var is not None and ast_var is not None, 'Set `st_var`'
+        if method == "wls":
+            assert st_var is not None and ast_var is not None, "Set `st_var`"
 
         self.check_reference_section_values()
 
         nx = self.x.size
         time_dim = self.get_time_dim()
         nt = self[time_dim].size
         nta = self.trans_att.size
 
-        assert self.st.dims[0] == 'x', 'Stokes are transposed'
-        assert self.ast.dims[0] == 'x', 'Stokes are transposed'
+        assert self.st.dims[0] == "x", "Stokes are transposed"
+        assert self.ast.dims[0] == "x", "Stokes are transposed"
 
         if matching_sections:
             matching_indices = match_sections(self, matching_sections)
         else:
             matching_indices = None
 
-        ix_sec = self.ufunc_per_section(x_indices=True, calc_per='all')
-        assert not np.any(
-            self.st.isel(x=ix_sec) <= 0.), \
-            'There is uncontrolled noise in the ST signal. Are your sections' \
-            'correctly defined?'
-        assert not np.any(
-            self.ast.isel(x=ix_sec) <= 0.), \
-            'There is uncontrolled noise in the AST signal. Are your sections' \
-            'correctly defined?'
-
-        if method == 'ols' or method == 'wls':
-            if method == 'ols':
-                assert st_var is None and ast_var is None, ''
-                st_var = None  # ols
-                ast_var = None  # ols
-                calc_cov = False
-            else:
-                for input_item in [st_var, ast_var]:
-                    assert input_item is not None, 'For wls define all ' \
-                                                   'variances (`st_var`, ' \
-                                                   '`ast_var`) '
+        ix_sec = self.ufunc_per_section(x_indices=True, calc_per="all")
+        assert not np.any(self.st.isel(x=ix_sec) <= 0.0), (
+            "There is uncontrolled noise in the ST signal. Are your sections"
+            "correctly defined?"
+        )
+        assert not np.any(self.ast.isel(x=ix_sec) <= 0.0), (
+            "There is uncontrolled noise in the AST signal. Are your sections"
+            "correctly defined?"
+        )
+
+        if method == "wls":
+            for input_item in [st_var, ast_var]:
+                assert input_item is not None, (
+                    "For wls define all " "variances (`st_var`, " "`ast_var`) "
+                )
 
-                calc_cov = True
+            calc_cov = True
 
             split = calibration_single_ended_solver(
                 self,
                 st_var,
                 ast_var,
                 calc_cov=calc_cov,
-                solver='external_split',
-                matching_indices=matching_indices)
+                solver="external_split",
+                matching_indices=matching_indices,
+            )
 
-            y = split['y']
-            w = split['w']
+            y = split["y"]
+            w = split["w"]
 
             # Stack all X's
             if fix_alpha:
-                assert not fix_dalpha, 'Use either `fix_dalpha` or `fix_alpha`'
-                assert fix_alpha[0].size == self.x.size, 'fix_alpha also needs to be defined outside the reference ' \
-                                                         'sections'
-                assert fix_alpha[1].size == self.x.size, 'fix_alpha also needs to be defined outside the reference ' \
-                                                         'sections'
-                p_val = split['p0_est_alpha'].copy()
+                assert not fix_dalpha, "Use either `fix_dalpha` or `fix_alpha`"
+                assert fix_alpha[0].size == self.x.size, (
+                    "fix_alpha also needs to be defined outside the reference " "sections"
+                )
+                assert fix_alpha[1].size == self.x.size, (
+                    "fix_alpha also needs to be defined outside the reference " "sections"
+                )
+                p_val = split["p0_est_alpha"].copy()
 
                 if np.any(matching_indices):
                     raise NotImplementedError(
                         "Configuring fix_alpha and matching sections requires extra code"
                     )
 
                 X = sp.hstack(
-                    (
-                        split['X_gamma'], split['X_alpha'], split['X_c'],
-                        split['X_TA'])).tocsr()
+                    (split["X_gamma"], split["X_alpha"], split["X_c"], split["X_TA"])
+                ).tocsr()
                 ip_use = list(range(1 + nx + nt + nta * nt))
 
             else:
                 X = sp.vstack(
                     (
                         sp.hstack(
                             (
-                                split['X_gamma'], split['X_dalpha'],
-                                split['X_c'], split['X_TA'])),
-                        split['X_m'])).tocsr()
-                p_val = split['p0_est_dalpha'].copy()
+                                split["X_gamma"],
+                                split["X_dalpha"],
+                                split["X_c"],
+                                split["X_TA"],
+                            )
+                        ),
+                        split["X_m"],
+                    )
+                ).tocsr()
+                p_val = split["p0_est_dalpha"].copy()
                 ip_use = list(range(1 + 1 + nt + nta * nt))
 
             p_var = np.zeros_like(p_val)
             p_cov = np.zeros((p_val.size, p_val.size), dtype=float)
 
             if fix_gamma is not None:
                 ip_remove = [0]
                 ip_use = [i for i in ip_use if i not in ip_remove]
                 p_val[ip_remove] = fix_gamma[0]
                 p_var[ip_remove] = fix_gamma[1]
 
-                X_gamma = sp.vstack(
-                    (split['X_gamma'],
-                     split['X_m'].tocsr()[:, 0].tocoo())).toarray().flatten()
+                X_gamma = (
+                    sp.vstack((split["X_gamma"], split["X_m"].tocsr()[:, 0].tocoo()))
+                    .toarray()
+                    .flatten()
+                )
 
                 y -= fix_gamma[0] * X_gamma
                 w = 1 / (1 / w + fix_gamma[1] * X_gamma)
 
             if fix_alpha is not None:
                 ip_remove = list(range(1, nx + 1))
                 ip_use = [i for i in ip_use if i not in ip_remove]
                 p_val[ip_remove] = fix_alpha[0]
                 p_var[ip_remove] = fix_alpha[1]
 
                 # X_alpha needs to be vertically extended to support matching sections
-                y -= split['X_alpha'].dot(fix_alpha[0])
-                w = 1 / (1 / w + split['X_alpha'].dot(fix_alpha[1]))
+                y -= split["X_alpha"].dot(fix_alpha[0])
+                w = 1 / (1 / w + split["X_alpha"].dot(fix_alpha[1]))
 
             if fix_dalpha is not None:
                 ip_remove = [1]
                 ip_use = [i for i in ip_use if i not in ip_remove]
                 p_val[ip_remove] = fix_dalpha[0]
                 p_var[ip_remove] = fix_dalpha[1]
 
                 y -= np.hstack(
                     (
-                        fix_dalpha[0] * split['X_dalpha'].toarray().flatten(),
+                        fix_dalpha[0] * split["X_dalpha"].toarray().flatten(),
                         (
-                            fix_dalpha[0] * split['X_m'].tocsr()
-                            [:, 1].tocoo().toarray().flatten())))
+                            fix_dalpha[0]
+                            * split["X_m"].tocsr()[:, 1].tocoo().toarray().flatten()
+                        ),
+                    )
+                )
                 w = 1 / (
-                    1 / w + np.hstack(
+                    1 / w
+                    + np.hstack(
                         (
-                            fix_dalpha[1]
-                            * split['X_dalpha'].toarray().flatten(), (
-                                fix_dalpha[1] * split['X_m'].tocsr()
-                                [:, 1].tocoo().toarray().flatten()))))
+                            fix_dalpha[1] * split["X_dalpha"].toarray().flatten(),
+                            (
+                                fix_dalpha[1]
+                                * split["X_m"].tocsr()[:, 1].tocoo().toarray().flatten()
+                            ),
+                        )
+                    )
+                )
 
-            if solver == 'sparse':
+            if solver == "sparse":
                 out = wls_sparse(
-                    X[:, ip_use],
-                    y,
-                    w=w,
-                    x0=p_val[ip_use],
-                    calc_cov=calc_cov,
-                    verbose=False)
-
-            elif solver == 'stats':
-                out = wls_stats(
-                    X[:, ip_use], y, w=w, calc_cov=calc_cov, verbose=False)
+                    X[:, ip_use], y, w=w, x0=p_val[ip_use], calc_cov=calc_cov, verbose=False
+                )
+
+            elif solver == "stats":
+                out = wls_stats(X[:, ip_use], y, w=w, calc_cov=calc_cov, verbose=False)
+
+            else:
+                assert 0, 'Unknown solver'
 
             p_val[ip_use] = out[0]
             p_var[ip_use] = out[1]
+            np.fill_diagonal(p_cov, p_var)  # set variance of all fixed params
+            p_cov[np.ix_(ip_use, ip_use)] = out[2]
 
-            if calc_cov:
-                np.fill_diagonal(
-                    p_cov, p_var)  # set variance of all fixed params
-                p_cov[np.ix_(ip_use, ip_use)] = out[2]
-
-        elif method == 'external':
+        elif method == "external":
             for input_item in [p_val, p_var, p_cov]:
-                assert input_item is not None, \
-                    'Define p_val, p_var, p_cov when using an external solver'
+                assert (
+                    input_item is not None
+                ), "Define p_val, p_var, p_cov when using an external solver"
 
-        elif method == 'external_split':
-            raise ValueError('Not implemented yet')
+        elif method == "external_split":
+            raise ValueError("Not implemented yet")
 
         else:
-            raise ValueError('Choose a valid method')
+            raise ValueError("Choose a valid method")
 
-        # store calibration parameters in DataStore
-        self[store_gamma] = (tuple(), p_val[0])
+        # all below require the following solution sizes
+        ip = ParameterIndexSingleEnded(nt, nx, nta, fix_alpha=fix_alpha)
+
+        # npar = 1 + 1 + nt + nta * nt
+        assert p_val.size == ip.npar
+        assert p_var.size == ip.npar
+        assert p_cov.shape == (ip.npar, ip.npar)
 
-        if method == 'wls' or method == 'external':
-            self[store_gamma + variance_suffix] = (tuple(), p_var[0])
+        # store calibration parameters in DataStore
+        self[store_gamma] = (tuple(), p_val[ip.gamma].item())
+        self[store_gamma + variance_suffix] = (tuple(), p_var[ip.gamma].item())
 
         if nta > 0:
-            ta = p_val[-nt * nta:].reshape((nt, nta), order='F')
-            self[store_ta] = ((time_dim, 'trans_att'), ta[:, :])
+            self[store_ta + "_fw"] = (
+                ("trans_att", time_dim),
+                ip.get_taf_pars(p_val),
+            )
+            self[store_ta + "_fw" + variance_suffix] = (
+                ("trans_att", time_dim),
+                ip.get_taf_pars(p_var),
+            )
+        else:
+            self[store_ta + "_fw"] = (("trans_att", time_dim), np.zeros((0, nt)))
+            self[store_ta + "_fw" + variance_suffix] = (("trans_att", time_dim), np.zeros((0, nt)))
 
-            if method == 'wls' or method == 'external':
-                tavar = p_var[-nt * nta:].reshape((nt, nta), order='F')
-                self[store_ta + variance_suffix] = (
-                    (time_dim, 'trans_att'), tavar[:, :])
+        self[store_c] = ((time_dim,), p_val[ip.c])
+        self[store_c + variance_suffix] = ((time_dim,), p_var[ip.c])
+
+        self[store_dalpha] = (tuple(), p_val[ip.dalpha].item())
+        self[store_dalpha + variance_suffix] = (tuple(), p_var[ip.dalpha].item())
 
         if fix_alpha:
-            ic_start = 1 + nx
-            self[store_c] = ((time_dim,), p_val[ic_start:nt + ic_start])
-            self[store_alpha] = (('x',), fix_alpha[0])
-
-            if method == 'wls' or method == 'external':
-                self[store_c + variance_suffix] = (
-                    (time_dim,), p_var[ic_start:nt + ic_start])
-                self[store_alpha + variance_suffix] = (('x',), fix_alpha[1])
-        else:
-            self[store_c] = ((time_dim,), p_val[2:nt + 2])
-            dalpha = p_val[1]
-            self[store_dalpha] = (tuple(), dalpha)
-            self[store_alpha] = (('x',), dalpha * self.x.data)
-
-            if method == 'wls' or method == 'external':
-                self[store_c
-                     + variance_suffix] = ((time_dim,), p_var[2:nt + 2])
-                dalpha_var = p_var[1]
-                self[store_dalpha + variance_suffix] = (tuple(), dalpha_var)
-                self[store_alpha
-                     + variance_suffix] = (('x',), dalpha_var * self.x.data)
-
-        # deal with FW
-        if store_tmpf:
-            ta_arr = np.zeros((nx, nt))
-            if nta > 0:
-                for tai, taxi in zip(self[store_ta].values.T,
-                                     self.trans_att.values):
-                    ta_arr[self.x.values >= taxi] = \
-                        ta_arr[self.x.values >= taxi] + tai
+            self[store_alpha] = fix_alpha[0]
+            self[store_alpha + variance_suffix] = fix_alpha[1]
+        else:
+            self[store_alpha] = self[store_dalpha] * self.x
+            self[store_alpha + variance_suffix] = (
+                self[store_dalpha + variance_suffix] * self.x ** 2
+            )
+
+        self[store_ta + "_fw_full"] = (
+            ("x", time_dim),
+            ip.get_taf_values(
+                pval=p_val, x=self.x.values, trans_att=self.trans_att.values, axis=""
+            ),
+        )
+        self[store_ta + "_fw_full" + variance_suffix] = (
+            ("x", time_dim),
+            ip.get_taf_values(
+                pval=p_var, x=self.x.values, trans_att=self.trans_att.values, axis=""
+            ),
+        )
+
+        tmpf = self.gamma / (
+            (np.log(self.st / self.ast) + (self[store_c] + self[store_ta + "_fw_full"]))
+            + self[store_alpha]
+        )
+        self[store_tmpf] = tmpf - 273.15
+
+        # tmpf_var
+        deriv_dict = dict(
+            T_gamma_fw=tmpf / self[store_gamma],
+            T_st_fw=-(tmpf ** 2) / (self[store_gamma] * self.st),
+            T_ast_fw=tmpf ** 2 / (self[store_gamma] * self.ast),
+            T_c_fw=-(tmpf ** 2) / self[store_gamma],
+            T_dalpha_fw=-self.x * (tmpf ** 2) / self[store_gamma],
+            T_alpha_fw=-(tmpf ** 2) / self[store_gamma],
+            T_ta_fw=-(tmpf ** 2) / self[store_gamma],
+        )
+        deriv_ds = xr.Dataset(deriv_dict)
+        # self["deriv"] = deriv_ds.to_array(dim="com2")
+
+        sigma2_gamma_c = p_cov[np.ix_(ip.gamma, ip.c)]
+        sigma2_tafw_gamma = ip.get_taf_values(
+            pval=p_cov[ip.gamma],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="",
+        )
+        sigma2_tafw_c = ip.get_taf_values(
+            pval=p_cov[ip.c],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="time",
+        )
+        var_fw_dict = dict(
+            dT_dst=deriv_ds.T_st_fw ** 2 * parse_st_var(self, st_var, st_label="st"),
+            dT_dast=deriv_ds.T_ast_fw ** 2 * parse_st_var(self, ast_var, st_label="ast"),
+            dT_gamma=deriv_ds.T_gamma_fw ** 2 * self[store_gamma + variance_suffix],
+            dT_dc=deriv_ds.T_c_fw ** 2 * self[store_c + variance_suffix],
+            dT_ddalpha=deriv_ds.T_alpha_fw ** 2 * self[store_alpha + variance_suffix],  # same as dT_dalpha
+            dT_dta=deriv_ds.T_ta_fw ** 2 * self[store_ta + "_fw_full" + variance_suffix],
+            dgamma_dc=(2 * deriv_ds.T_gamma_fw * deriv_ds.T_c_fw * sigma2_gamma_c),
+            dta_dgamma=(2 * deriv_ds.T_ta_fw * deriv_ds.T_gamma_fw * sigma2_tafw_gamma),
+            dta_dc=(2 * deriv_ds.T_ta_fw * deriv_ds.T_c_fw * sigma2_tafw_c),
+        )
+
+        if not fix_alpha:
+            # These correlations don't exist in case of fix_alpha. Including them reduces tmpf_var.
+            sigma2_gamma_dalpha = p_cov[np.ix_(ip.dalpha, ip.gamma)]
+            sigma2_dalpha_c = p_cov[np.ix_(ip.dalpha, ip.c)]
+            sigma2_tafw_dalpha = ip.get_taf_values(
+                pval=p_cov[ip.dalpha],
+                x=self.x.values,
+                trans_att=self.trans_att.values,
+                axis="",
+            )
+            var_fw_dict.update(
+                dict(
+                    dgamma_ddalpha=(
+                        2 * deriv_ds.T_gamma_fw * deriv_ds.T_dalpha_fw * sigma2_gamma_dalpha
+                    ),
+                    ddalpha_dc=(
+                        2 * deriv_ds.T_dalpha_fw * deriv_ds.T_c_fw * sigma2_dalpha_c
+                    ),
+                    dta_ddalpha=(
+                        2 * deriv_ds.T_ta_fw * deriv_ds.T_dalpha_fw * sigma2_tafw_dalpha
+                    ),
+                )
+            )
+
+        self["var_fw_da"] = xr.Dataset(var_fw_dict).to_array(dim="comp_fw")
+        self[store_tmpf + variance_suffix] = self["var_fw_da"].sum(dim="comp_fw")
+
+        self[store_tmpf].attrs.update(_dim_attrs[("tmpf",)])
+        self[store_tmpf + variance_suffix].attrs.update(_dim_attrs[("tmpf_var",)])
+
+        drop_vars = [
+            k for k, v in self.items() if {"params1", "params2"}.intersection(v.dims)
+        ]
 
-            tempF_data = self.gamma.data / (
-                (
-                    np.log(self.st.data) - np.log(self.ast.data) +
-                    (self.c.data[None, :] + ta_arr)) +
-                (self.alpha.data[:, None])) - 273.15
-            self[store_tmpf] = (('x', time_dim), tempF_data)
-
-        if store_p_val:
-            drop_vars = [
-                k for k, v in self.items()
-                if {'params1', 'params2'}.intersection(v.dims)]
-
-            for k in drop_vars:
-                del self[k]
-
-            self[store_p_val] = (('params1',), p_val)
-
-            if method == 'wls' or method == 'external':
-                assert store_p_cov, 'Might as well store the covariance matrix. Already computed.'
-                self[store_p_cov] = (('params1', 'params2'), p_cov)
+        for k in drop_vars:
+            del self[k]
+
+        self[store_p_val] = (("params1",), p_val)
+        self[store_p_cov] = (("params1", "params2"), p_cov)
 
         pass
 
     def calibration_double_ended(
-            self,
-            sections=None,
-            st_var=None,
-            ast_var=None,
-            rst_var=None,
-            rast_var=None,
-            store_df='df',
-            store_db='db',
-            store_gamma='gamma',
-            store_alpha='alpha',
-            store_ta='talpha',
-            store_tmpf='tmpf',
-            store_tmpb='tmpb',
-            store_tmpw='tmpw',
-            tmpw_mc_size=50,
-            store_p_cov='p_cov',
-            store_p_val='p_val',
-            variance_suffix='_var',
-            method='wls',
-            solver='sparse',
-            p_val=None,
-            p_var=None,
-            p_cov=None,
-            remove_mc_set_flag=True,
-            reduce_memory_usage=False,
-            trans_att=None,
-            fix_gamma=None,
-            fix_alpha=None,
-            matching_sections=None,
-            matching_indices=None,
-            verbose=False,
-            **kwargs):
+        self,
+        sections=None,
+        st_var=None,
+        ast_var=None,
+        rst_var=None,
+        rast_var=None,
+        store_df="df",
+        store_db="db",
+        store_gamma="gamma",
+        store_alpha="alpha",
+        store_ta="talpha",
+        store_tmpf="tmpf",
+        store_tmpb="tmpb",
+        store_tmpw="tmpw",
+        mc_sample_size=None,
+        mc_conf_ints=None,
+        mc_da_random_state=None,
+        mc_remove_set_flag=True,
+        mc_reduce_memory_usage=False,
+        store_p_cov="p_cov",
+        store_p_val="p_val",
+        variance_suffix="_var",
+        method="wls",
+        solver="sparse",
+        p_val=None,
+        p_var=None,
+        p_cov=None,
+        trans_att=None,
+        fix_gamma=None,
+        fix_alpha=None,
+        matching_sections=None,
+        matching_indices=None,
+        verbose=False,
+        **kwargs,
+    ):
         """
+        See example notebook 8 for an explanation on how to use this function.
         Calibrate the Stokes (`ds.st`) and anti-Stokes (`ds.ast`) of the forward
         channel and from the backward channel (`ds.rst`, `ds.rast`) data to
         temperature using fiber sections with a known temperature
         (`ds.sections`) for double-ended setups. The calibrated temperature of
         the forward channel is stored under `ds.tmpf` and its variance under
-        `ds.tmpf_var`, and that of the the backward channel under `ds.tmpb` and
+        `ds.tmpf_var`, and that of the backward channel under `ds.tmpb` and
         `ds.tmpb_var`. The inverse-variance weighted average of the forward and
         backward channel is stored under `ds.tmpw` and `ds.tmpw_var`.
-
         In double-ended setups, Stokes and anti-Stokes intensity is measured in
         two directions from both ends of the fiber. The forward-channel
         measurements are denoted with subscript F, and the backward-channel
         measurements are denoted with subscript B. Both measurement channels
         start at a different end of the fiber and have opposite directions, and
-        therefore have different spatial coordinates. The first processing step
+        therefore have different spatial coordinates.
+        The first processing step
         with double-ended measurements is to align the measurements of the two
         measurement channels so that they have the same spatial coordinates. The
         spatial coordinate :math:`x` (m) is defined here positive in the forward
         direction, starting at 0 where the fiber is connected to the forward
         channel of the DTS system; the length of the fiber is :math:`L`.
         Consequently, the backward-channel measurements are flipped and shifted
         to align with the forward-channel measurements. Alignment of the
         measurements of the two channels is prone to error because it requires
         the exact fiber length (McDaniel et al., 2018). Depending on the DTS system
         used, the forward channel and backward channel are measured one after
         another by making use of an optical switch, so that only a single
-        detector is needed. However, it is assumed in this paper that the
+        detector is needed. However, it is assumed in this package that the
         forward channel and backward channel are measured simultaneously, so
         that the temperature of both measurements is the same. This assumption
-        holds better for short acquisition times with respect to the time scale
+        holds better for short acquisition times with respect to the timescale
         of the temperature variation, and when there is no systematic difference
         in temperature between the two channels. The temperature may be computed
         from the forward-channel measurements (Equation 10 [1]_) with:
-
         .. math::
-
             T_\mathrm{F} (x,t)  = \\frac{\gamma}{I_\mathrm{F}(x,t) + \
-C_\mathrm{F}(t) + \int_0^x{\Delta\\alpha(x')\,\mathrm{d}x'}}
-
+    C_\mathrm{F}(t) + \int_0^x{\Delta\\alpha(x')\,\mathrm{d}x'}}
         and from the backward-channel measurements with:
-
         .. math::
             T_\mathrm{B} (x,t)  = \\frac{\gamma}{I_\mathrm{B}(x,t) + \
-C_\mathrm{B}(t) + \int_x^L{\Delta\\alpha(x')\,\mathrm{d}x'}}
-
+    C_\mathrm{B}(t) + \int_x^L{\Delta\\alpha(x')\,\mathrm{d}x'}}
         with
-
         .. math::
-
             I(x,t) = \ln{\left(\\frac{P_+(x,t)}{P_-(x,t)}\\right)}
-
-
         .. math::
-
             C(t) = \ln{\left(\\frac{\eta_-(t)K_-/\lambda_-^4}{\eta_+(t)K_+/\lambda_+^4}\\right)}
-
-
         where :math:`C` is the lumped effect of the difference in gain at
+        :param mc_conf_ints:
         :math:`x=0` between Stokes and anti-Stokes intensity measurements and
         the dependence of the scattering intensity on the wavelength. The
         parameters :math:`P_+` and :math:`P_-` are the Stokes and anti-Stokes
         intensity measurements, respectively.
         :math:`C_\mathrm{F}(t)` and :math:`C_\mathrm{B}(t)` are the
         parameter :math:`C(t)` for the forward-channel and backward-channel
         measurements, respectively. :math:`C_\mathrm{B}(t)` may be different
@@ -2355,50 +2426,42 @@
         connected to the DTS system (:math:`\eta_+` and :math:`\eta_-` in
         Equation~\\ref{eqn:c}). :math:`T` in the listed
         equations is in Kelvin, but is converted to Celsius after calibration.
         The calibration procedure presented in van de
         Giesen et al. 2012 approximates :math:`C(t)` to be
         the same for the forward and backward-channel measurements, but this
         approximation is not made here.
-
         Parameter :math:`A(x)` (`ds.alpha`) is introduced to simplify the notation of the
         double-ended calibration procedure and represents the integrated
         differential attenuation between locations :math:`x_1` and :math:`x`
         along the fiber. Location :math:`x_1` is the first reference section
         location (the smallest x-value of all used reference sections).
-
         .. math::
-            A(x) = \\int_{x_1}^x{\\Delta\\alpha(x')\\,\\mathrm{d}x'}
-
+            A(x) = \int_{x_1}^x{\Delta\\alpha(x')\,\mathrm{d}x'}
         so that the expressions for temperature may be written as:
-
         .. math::
             T_\mathrm{F} (x,t) = \\frac{\gamma}{I_\mathrm{F}(x,t) + D_\mathrm{F}(t) + A(x)},
             T_\mathrm{B} (x,t) = \\frac{\gamma}{I_\mathrm{B}(x,t) + D_\mathrm{B}(t) - A(x)}
-
         where
-
         .. math::
             D_{\mathrm{F}}(t) = C_{\mathrm{F}}(t) + \int_0^{x_1}{\Delta\\alpha(x')\,\mathrm{d}x'},
             D_{\mathrm{B}}(t) = C_{\mathrm{B}}(t) + \int_{x_1}^L{\Delta\\alpha(x')\,\mathrm{d}x'}
-
         Parameters :math:`D_\mathrm{F}` (`ds.df`) and :math:`D_\mathrm{B}`
         (`ds.db`) must be estimated for each time and are constant along the fiber, and parameter
         :math:`A` must be estimated for each location and is constant over time.
         The calibration procedure is discussed in Section 6.
         :math:`T_\mathrm{F}` (`ds.tmpf`) and :math:`T_\mathrm{B}` (`ds.tmpb`)
         are separate
         approximations of the same temperature at the same time. The estimated
         :math:`T_\mathrm{F}` is more accurate near :math:`x=0` because that is
         where the signal is strongest. Similarly, the estimated
         :math:`T_\mathrm{B}` is more accurate near :math:`x=L`. A single best
         estimate of the temperature is obtained from the weighted average of
         :math:`T_\mathrm{F}` and :math:`T_\mathrm{B}` as discussed in
         Section 7.2 [1]_ .
-
         Parameters
         ----------
         store_p_cov : str
             Key to store the covariance matrix of the calibrated parameters
         store_p_val : str
             Key to store the values of the calibrated parameters
         p_val : array-like, optional
@@ -2451,25 +2514,34 @@
             direction
         store_tmpb : str
             Label of where to store the calibrated temperature of the
             backward direction
         store_tmpw : str
             Label of where to store the inverse-variance weighted average
             temperature of the forward and backward channel measurements.
-        tmpw_mc_size : int
+        mc_sample_size : int, optional
+            If set, the variance is also computed using Monte Carlo sampling.
             The number of Monte Carlo samples drawn used to estimate the
             variance of the forward and backward channel temperature estimates
             and estimate the inverse-variance weighted average temperature.
+        conf_ints : iterable object of float
+            A list with the confidence boundaries that are calculated. Valid
+            values are between [0, 1].
+        mc_da_random_state
+            For testing purposes. Similar to random seed. The seed for dask.
+            Makes random not so random. To produce reproducable results for
+            testing environments.
+        mc_remove_set_flag : bool
+            Remove the monte carlo data set, from which the CI and the
+            variance are calculated.
         variance_suffix : str, optional
             String appended for storing the variance. Only used when method
             is wls.
-        method : {'ols', 'wls', 'external'}
-            Use `'ols'` for ordinary least squares and `'wls'` for weighted least
-            squares. `'wls'` is the default, and there is currently no reason to
-            use `'ols'`.
+        method : {'wls', 'external'}
+            Use `'wls'` for weighted least squares.
         solver : {'sparse', 'stats'}
             Either use the homemade weighted sparse solver or the weighted
             dense matrix solver of statsmodels. The sparse solver uses much less
             memory, is faster, and gives the same result as the statsmodels
             solver. The statsmodels solver is mostly used to check the sparse
             solver. `'stats'` is the default.
         transient_att_x, transient_asym_att_x : iterable, optional
@@ -2499,758 +2571,1021 @@
             sections have a reverse direction ("J-configuration").
         matching_indices : array
             Provide an array of x-indices of size (npair, 2), where each pair
             has the same temperature. Used to improve the estimate of the
             integrated differential attenuation.
         verbose : bool
             Show additional calibration information
-
-
         Returns
         -------
-
         References
         ----------
         .. [1] des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation
             of Temperature and Associated Uncertainty from Fiber-Optic Raman-
             Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235.
             https://doi.org/10.3390/s20082235
-
         Examples
         --------
         - `Example notebook 8: Calibrate double ended <https://github.com/\
-dtscalibration/python-dts-calibration/blob/main/examples/notebooks/\
-08Calibrate_double_wls.ipynb>`_
-
+    dtscalibration/python-dts-calibration/blob/master/examples/notebooks/\
+    08Calibrate_double_wls.ipynb>`_
         """
+        # TODO: confidence intervals using the variance approximated by linear error propagation
         self.check_deprecated_kwargs(kwargs)
 
         self.set_trans_att(trans_att=trans_att, **kwargs)
 
         if sections:
             self.sections = sections
         else:
-            assert self.sections, 'sections are not defined'
-
-        if method == 'wls':
-            assert st_var is not None and ast_var is not None and rst_var is not None and rast_var is not None, 'Configure `st_var`'
+            assert self.sections, "sections are not defined"
 
         self.check_reference_section_values()
 
         nx = self.x.size
         time_dim = self.get_time_dim()
         nt = self[time_dim].size
         nta = self.trans_att.size
-        ix_sec = self.ufunc_per_section(x_indices=True, calc_per='all')
+        ix_sec = self.ufunc_per_section(x_indices=True, calc_per="all")
         nx_sec = ix_sec.size
 
-        assert self.st.dims[0] == 'x', 'Stokes are transposed'
-        assert self.ast.dims[0] == 'x', 'Stokes are transposed'
-        assert self.rst.dims[0] == 'x', 'Stokes are transposed'
-        assert self.rast.dims[0] == 'x', 'Stokes are transposed'
-
-        assert not np.any(
-            self.st.isel(x=ix_sec) <= 0.), \
-            'There is uncontrolled noise in the ST signal. Are your sections' \
-            'correctly defined?'
-        assert not np.any(
-            self.ast.isel(x=ix_sec) <= 0.), \
-            'There is uncontrolled noise in the AST signal. Are your sections' \
-            'correctly defined?'
-        assert not np.any(
-            self.rst.isel(x=ix_sec) <= 0.), \
-            'There is uncontrolled noise in the REV-ST signal. Are your ' \
-            'sections correctly defined?'
-        assert not np.any(
-            self.rast.isel(x=ix_sec) <= 0.), \
-            'There is uncontrolled noise in the REV-AST signal. Are your ' \
-            'sections correctly defined?'
+        assert self.st.dims[0] == "x", "Stokes are transposed"
+        assert self.ast.dims[0] == "x", "Stokes are transposed"
+        assert self.rst.dims[0] == "x", "Stokes are transposed"
+        assert self.rast.dims[0] == "x", "Stokes are transposed"
+
+        assert not np.any(self.st.isel(x=ix_sec) <= 0.0), (
+            "There is uncontrolled noise in the ST signal. Are your sections"
+            "correctly defined?"
+        )
+        assert not np.any(self.ast.isel(x=ix_sec) <= 0.0), (
+            "There is uncontrolled noise in the AST signal. Are your sections"
+            "correctly defined?"
+        )
+        assert not np.any(self.rst.isel(x=ix_sec) <= 0.0), (
+            "There is uncontrolled noise in the REV-ST signal. Are your "
+            "sections correctly defined?"
+        )
+        assert not np.any(self.rast.isel(x=ix_sec) <= 0.0), (
+            "There is uncontrolled noise in the REV-AST signal. Are your "
+            "sections correctly defined?"
+        )
 
-        if method == 'wls':
+        if method == "wls":
             for input_item in [st_var, ast_var, rst_var, rast_var]:
-                assert input_item is not None, \
-                    'For wls define all variances (`st_var`, `ast_var`,' +\
-                    ' `rst_var`, `rast_var`)'
+                assert input_item is not None, (
+                    "For wls define all variances (`st_var`, `ast_var`,"
+                    + " `rst_var`, `rast_var`)"
+                )
 
         if np.any(matching_indices):
-            assert not matching_sections, \
-                'Either define `matching_sections` or `matching_indices`'
+            assert (
+                not matching_sections
+            ), "Either define `matching_sections` or `matching_indices`"
 
         if matching_sections:
-            assert not matching_indices, \
-                'Either define `matching_sections` or `matching_indices'
+            assert (
+                not matching_indices
+            ), "Either define `matching_sections` or `matching_indices"
             matching_indices = match_sections(self, matching_sections)
 
-        if method == 'ols' or method == 'wls':
-            if method == 'ols':
-                calc_cov = False
-            else:
-                calc_cov = True
-
+        if method == "wls":
             if fix_alpha or fix_gamma:
                 split = calibration_double_ended_solver(
                     self,
                     st_var,
                     ast_var,
                     rst_var,
                     rast_var,
-                    calc_cov=calc_cov,
-                    solver='external_split',
+                    calc_cov=True,
+                    solver="external_split",
                     matching_indices=matching_indices,
-                    verbose=verbose)
+                    verbose=verbose,
+                )
             else:
                 out = calibration_double_ended_solver(
                     self,
                     st_var,
                     ast_var,
                     rst_var,
                     rast_var,
-                    calc_cov=calc_cov,
+                    calc_cov=True,
                     solver=solver,
                     matching_indices=matching_indices,
-                    verbose=verbose)
+                    verbose=verbose,
+                )
 
-                if calc_cov:
-                    p_val, p_var, p_cov = out
-                else:
-                    p_val, p_var = out
+                p_val, p_var, p_cov = out
 
             # adjust split to fix parameters
             """Wrapped in a function to reduce memory usage.
             Constructing:
             Z_gamma (nt * nx, 1). Data: positive 1/temp
             Z_D (nt * nx, nt). Data: ones
             E (nt * nx, nx). Data: ones
             Zero_gamma (nt * nx, 1)
             zero_d (nt * nx, nt)
             Z_TA_fw (nt * nx, nta * 2 * nt) minus ones
             Z_TA_bw (nt * nx, nta * 2 * nt) minus ones
             Z_TA_E (nt * nx, nta * 2 * nt)
-
             I_fw = 1/Tref*gamma - D_fw - E - TA_fw
             I_bw = 1/Tref*gamma - D_bw + E - TA_bw
             (I_bw - I_fw) / 2 = D_fw/2 - D_bw/2 + E + TA_fw/2 - TA_bw/2 Eq42
             """
             if fix_alpha and fix_gamma:
-                assert np.size(fix_alpha[0]) == self.x.size, \
-                    'define alpha for each location'
-                assert np.size(fix_alpha[1]) == self.x.size, \
-                    'define var alpha for each location'
-                m = 'The integrated differential attenuation is zero at the ' \
-                    'first index of the reference sections.'
+                assert (
+                    np.size(fix_alpha[0]) == self.x.size
+                ), "define alpha for each location"
+                assert (
+                    np.size(fix_alpha[1]) == self.x.size
+                ), "define var alpha for each location"
+                m = (
+                    "The integrated differential attenuation is zero at the "
+                    "first index of the reference sections."
+                )
                 assert np.abs(fix_alpha[0][ix_sec[0]]) < 1e-8, m
                 # The array with the integrated differential att is termed E
 
                 if np.any(matching_indices):
-                    n_E_in_cal = split['ix_from_cal_match_to_glob'].size
+                    n_E_in_cal = split["ix_from_cal_match_to_glob"].size
                     p0_est = np.concatenate(
                         (
-                            split['p0_est'][1:1 + 2 * nt],
-                            split['p0_est'][1 + 2 * nt + n_E_in_cal:]))
-                    X_E1 = sp.csr_matrix(
-                        ([], ([], [])), shape=(nt * nx_sec, self.x.size))
-                    X_E1[:, ix_sec[1:]] = split['E']
-                    X_E2 = X_E1[:, split['ix_from_cal_match_to_glob']]
+                            split["p0_est"][1: 1 + 2 * nt],
+                            split["p0_est"][1 + 2 * nt + n_E_in_cal:],
+                        )
+                    )
+                    X_E1 = sp.csr_matrix(([], ([], [])), shape=(nt * nx_sec, self.x.size))
+                    X_E1[:, ix_sec[1:]] = split["E"]
+                    X_E2 = X_E1[:, split["ix_from_cal_match_to_glob"]]
                     X_E = sp.vstack(
                         (
-                            -X_E2, X_E2, split['E_match_F'],
-                            split['E_match_B'], split['E_match_no_cal']))
+                            -X_E2,
+                            X_E2,
+                            split["E_match_F"],
+                            split["E_match_B"],
+                            split["E_match_no_cal"],
+                        )
+                    )
 
-                    X_gamma = sp.vstack(
-                        (
-                            split['Z_gamma'], split['Z_gamma'],
-                            split['Zero_eq12_gamma'], split['Zero_eq12_gamma'],
-                            split['Zero_eq3_gamma'])).toarray().flatten()
+                    X_gamma = (
+                        sp.vstack(
+                            (
+                                split["Z_gamma"],
+                                split["Z_gamma"],
+                                split["Zero_eq12_gamma"],
+                                split["Zero_eq12_gamma"],
+                                split["Zero_eq3_gamma"],
+                            )
+                        )
+                        .toarray()
+                        .flatten()
+                    )
 
                     X = sp.vstack(
                         (
-                            sp.hstack(
-                                (
-                                    -split['Z_D'], split['Zero_d'],
-                                    split['Z_TA_fw'])),
-                            sp.hstack(
-                                (
-                                    split['Zero_d'], -split['Z_D'],
-                                    split['Z_TA_bw'])),
-                            sp.hstack(
-                                (split['Zero_d_eq12'], split['Z_TA_eq1'])),
-                            sp.hstack(
-                                (split['Zero_d_eq12'], split['Z_TA_eq2'])),
-                            sp.hstack((split['d_no_cal'], split['Z_TA_eq3']))))
+                            sp.hstack((-split["Z_D"], split["Zero_d"], split["Z_TA_fw"])),
+                            sp.hstack((split["Zero_d"], -split["Z_D"], split["Z_TA_bw"])),
+                            sp.hstack((split["Zero_d_eq12"], split["Z_TA_eq1"])),
+                            sp.hstack((split["Zero_d_eq12"], split["Z_TA_eq2"])),
+                            sp.hstack((split["d_no_cal"], split["Z_TA_eq3"])),
+                        )
+                    )
 
                     y = np.concatenate(
                         (
-                            split['y_F'], split['y_B'], split['y_eq1'],
-                            split['y_eq2'], split['y_eq3']))
-                    y -= X_E.dot(
-                        fix_alpha[0][split['ix_from_cal_match_to_glob']])
+                            split["y_F"],
+                            split["y_B"],
+                            split["y_eq1"],
+                            split["y_eq2"],
+                            split["y_eq3"],
+                        )
+                    )
+                    y -= X_E.dot(fix_alpha[0][split["ix_from_cal_match_to_glob"]])
                     y -= fix_gamma[0] * X_gamma
 
                     # variances are added. weight is the inverse of the variance
                     # of the observations
-                    if method == 'wls':
-                        w_ = np.concatenate(
-                            (
-                                split['w_F'], split['w_B'], split['w_eq1'],
-                                split['w_eq2'], split['w_eq3']))
-                        w = 1 / (
-                            1 / w_ + X_E.dot(
-                                fix_alpha[1][split['ix_from_cal_match_to_glob']])
-                            + fix_gamma[1] * X_gamma)
-
-                    else:
-                        w = 1.
+                    w_ = np.concatenate(
+                        (
+                            split["w_F"],
+                            split["w_B"],
+                            split["w_eq1"],
+                            split["w_eq2"],
+                            split["w_eq3"],
+                        )
+                    )
+                    w = 1 / (
+                        1 / w_
+                        + X_E.dot(fix_alpha[1][split["ix_from_cal_match_to_glob"]])
+                        + fix_gamma[1] * X_gamma
+                    )
 
                 else:
                     # X_gamma
-                    X_E = sp.vstack((-split['E'], split['E']))
-                    X_gamma = sp.vstack(
-                        (split['Z_gamma'],
-                         split['Z_gamma'])).toarray().flatten()
+                    X_E = sp.vstack((-split["E"], split["E"]))
+                    X_gamma = (
+                        sp.vstack((split["Z_gamma"], split["Z_gamma"])).toarray().flatten()
+                    )
                     # Use only the remaining coefficients
                     # Stack all X's
                     X = sp.vstack(
                         (
-                            sp.hstack(
-                                (
-                                    -split['Z_D'], split['Zero_d'],
-                                    split['Z_TA_fw'])),
-                            sp.hstack(
-                                (
-                                    split['Zero_d'], -split['Z_D'],
-                                    split['Z_TA_bw']))))
+                            sp.hstack((-split["Z_D"], split["Zero_d"], split["Z_TA_fw"])),
+                            sp.hstack((split["Zero_d"], -split["Z_D"], split["Z_TA_bw"])),
+                        )
+                    )
 
                     # Move the coefficients times the fixed gamma to the
                     # observations
-                    y = np.concatenate((split['y_F'], split['y_B']))
+                    y = np.concatenate((split["y_F"], split["y_B"]))
                     y -= X_E.dot(fix_alpha[0][ix_sec[1:]])
                     y -= fix_gamma[0] * X_gamma
                     # variances are added. weight is the inverse of the variance
                     # of the observations
-                    if method == 'wls':
-                        w_ = np.concatenate((split['w_F'], split['w_B']))
-                        w = 1 / (
-                            1 / w_ + X_E.dot(fix_alpha[1][ix_sec[1:]])
-                            + fix_gamma[1] * X_gamma)
-
-                    else:
-                        w = 1.
+                    w_ = np.concatenate((split["w_F"], split["w_B"]))
+                    w = 1 / (
+                        1 / w_ + X_E.dot(fix_alpha[1][ix_sec[1:]]) + fix_gamma[1] * X_gamma
+                    )
 
                     # [C_1, C_2, .., C_nt, TA_fw_a_1, TA_fw_a_2, TA_fw_a_nt,
                     # TA_bw_a_1, TA_bw_a_2, TA_bw_a_nt] Then continues with
                     # TA for connector b.
                     p0_est = np.concatenate(
                         (
-                            split['p0_est'][1:1 + 2 * nt],
-                            split['p0_est'][1 + 2 * nt + nx_sec - 1:]))
+                            split["p0_est"][1: 1 + 2 * nt],
+                            split["p0_est"][1 + 2 * nt + nx_sec - 1:],
+                        )
+                    )
+
+                if solver == "sparse":
+                    out = wls_sparse(X, y, w=w, x0=p0_est, calc_cov=True, verbose=False)
 
-                if solver == 'sparse':
-                    out = wls_sparse(
-                        X, y, w=w, x0=p0_est, calc_cov=calc_cov, verbose=False)
-
-                elif solver == 'stats':
-                    out = wls_stats(
-                        X, y, w=w, calc_cov=calc_cov, verbose=False)
+                elif solver == "stats":
+                    out = wls_stats(X, y, w=w, calc_cov=True, verbose=False)
 
                 # Added fixed gamma and its variance to the solution
                 p_val = np.concatenate(
-                    (
-                        [fix_gamma[0]], out[0][:2 * nt], fix_alpha[0],
-                        out[0][2 * nt:]))
+                    ([fix_gamma[0]], out[0][: 2 * nt], fix_alpha[0], out[0][2 * nt:])
+                )
                 p_var = np.concatenate(
-                    (
-                        [fix_gamma[1]], out[1][:2 * nt], fix_alpha[1],
-                        out[1][2 * nt:]))
+                    ([fix_gamma[1]], out[1][: 2 * nt], fix_alpha[1], out[1][2 * nt:])
+                )
 
-                if calc_cov:
-                    # whether it returns a copy or a view depends on what
-                    # version of numpy you are using
-                    p_cov = np.diag(p_var).copy()
-                    from_i = np.concatenate(
-                        (
-                            np.arange(1, 2 * nt + 1),
-                            np.arange(
-                                1 + 2 * nt + nx,
-                                1 + 2 * nt + nx + nta * nt * 2)))
-                    iox_sec1, iox_sec2 = np.meshgrid(
-                        from_i, from_i, indexing='ij')
-                    p_cov[iox_sec1, iox_sec2] = out[2]
+                # whether it returns a copy or a view depends on what
+                # version of numpy you are using
+                p_cov = np.diag(p_var).copy()
+                from_i = np.concatenate(
+                    (
+                        np.arange(1, 2 * nt + 1),
+                        np.arange(1 + 2 * nt + nx, 1 + 2 * nt + nx + nta * nt * 2),
+                    )
+                )
+                iox_sec1, iox_sec2 = np.meshgrid(from_i, from_i, indexing="ij")
+                p_cov[iox_sec1, iox_sec2] = out[2]
 
             elif fix_gamma:
                 if np.any(matching_indices):
                     # n_E_in_cal = split['ix_from_cal_match_to_glob'].size
-                    p0_est = split['p0_est'][1:]
-                    X_E1 = sp.csr_matrix(
-                        ([], ([], [])), shape=(nt * nx_sec, self.x.size))
+                    p0_est = split["p0_est"][1:]
+                    X_E1 = sp.csr_matrix(([], ([], [])), shape=(nt * nx_sec, self.x.size))
                     from_i = ix_sec[1:]
-                    X_E1[:, from_i] = split['E']
-                    X_E2 = X_E1[:, split['ix_from_cal_match_to_glob']]
+                    X_E1[:, from_i] = split["E"]
+                    X_E2 = X_E1[:, split["ix_from_cal_match_to_glob"]]
                     X = sp.vstack(
                         (
                             sp.hstack(
                                 (
-                                    -split['Z_D'], split['Zero_d'], -X_E2,
-                                    split['Z_TA_fw'])),
+                                    -split["Z_D"],
+                                    split["Zero_d"],
+                                    -X_E2,
+                                    split["Z_TA_fw"],
+                                )
+                            ),
                             sp.hstack(
-                                (
-                                    split['Zero_d'], -split['Z_D'], X_E2,
-                                    split['Z_TA_bw'])),
+                                (split["Zero_d"], -split["Z_D"], X_E2, split["Z_TA_bw"])
+                            ),
                             sp.hstack(
                                 (
-                                    split['Zero_d_eq12'], split['E_match_F'],
-                                    split['Z_TA_eq1'])),
+                                    split["Zero_d_eq12"],
+                                    split["E_match_F"],
+                                    split["Z_TA_eq1"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['Zero_d_eq12'], split['E_match_B'],
-                                    split['Z_TA_eq2'])),
+                                    split["Zero_d_eq12"],
+                                    split["E_match_B"],
+                                    split["Z_TA_eq2"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['d_no_cal'], split['E_match_no_cal'],
-                                    split['Z_TA_eq3']))))
-                    X_gamma = sp.vstack(
-                        (
-                            split['Z_gamma'], split['Z_gamma'],
-                            split['Zero_eq12_gamma'], split['Zero_eq12_gamma'],
-                            split['Zero_eq3_gamma'])).toarray().flatten()
+                                    split["d_no_cal"],
+                                    split["E_match_no_cal"],
+                                    split["Z_TA_eq3"],
+                                )
+                            ),
+                        )
+                    )
+                    X_gamma = (
+                        sp.vstack(
+                            (
+                                split["Z_gamma"],
+                                split["Z_gamma"],
+                                split["Zero_eq12_gamma"],
+                                split["Zero_eq12_gamma"],
+                                split["Zero_eq3_gamma"],
+                            )
+                        )
+                        .toarray()
+                        .flatten()
+                    )
 
                     y = np.concatenate(
                         (
-                            split['y_F'], split['y_B'], split['y_eq1'],
-                            split['y_eq2'], split['y_eq3']))
+                            split["y_F"],
+                            split["y_B"],
+                            split["y_eq1"],
+                            split["y_eq2"],
+                            split["y_eq3"],
+                        )
+                    )
                     y -= fix_gamma[0] * X_gamma
 
                     # variances are added. weight is the inverse of the variance
                     # of the observations
-                    if method == 'wls':
-                        w_ = np.concatenate(
-                            (
-                                split['w_F'], split['w_B'], split['w_eq1'],
-                                split['w_eq2'], split['w_eq3']))
-                        w = 1 / (1 / w_ + fix_gamma[1] * X_gamma)
-
-                    else:
-                        w = 1.
+                    w_ = np.concatenate(
+                        (
+                            split["w_F"],
+                            split["w_B"],
+                            split["w_eq1"],
+                            split["w_eq2"],
+                            split["w_eq3"],
+                        )
+                    )
+                    w = 1 / (1 / w_ + fix_gamma[1] * X_gamma)
 
                 else:
-                    X_gamma = sp.vstack(
-                        (split['Z_gamma'],
-                         split['Z_gamma'])).toarray().flatten()
+                    X_gamma = (
+                        sp.vstack((split["Z_gamma"], split["Z_gamma"])).toarray().flatten()
+                    )
                     # Use only the remaining coefficients
                     X = sp.vstack(
                         (
                             sp.hstack(
                                 (
-                                    -split['Z_D'], split['Zero_d'],
-                                    -split['E'], split['Z_TA_fw'])),
+                                    -split["Z_D"],
+                                    split["Zero_d"],
+                                    -split["E"],
+                                    split["Z_TA_fw"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['Zero_d'], -split['Z_D'], split['E'],
-                                    split['Z_TA_bw']))))
+                                    split["Zero_d"],
+                                    -split["Z_D"],
+                                    split["E"],
+                                    split["Z_TA_bw"],
+                                )
+                            ),
+                        )
+                    )
                     # Move the coefficients times the fixed gamma to the
                     # observations
-                    y = np.concatenate((split['y_F'], split['y_B']))
+                    y = np.concatenate((split["y_F"], split["y_B"]))
                     y -= fix_gamma[0] * X_gamma
                     # variances are added. weight is the inverse of the variance
                     # of the observations
-                    if method == 'wls':
-                        w_ = np.concatenate((split['w_F'], split['w_B']))
-                        w = 1 / (1 / w_ + fix_gamma[1] * X_gamma)
+                    w_ = np.concatenate((split["w_F"], split["w_B"]))
+                    w = 1 / (1 / w_ + fix_gamma[1] * X_gamma)
 
-                    else:
-                        w = 1.
-                    p0_est = split['p0_est'][1:]
+                    p0_est = split["p0_est"][1:]
 
-                if solver == 'sparse':
-                    out = wls_sparse(
-                        X, y, w=w, x0=p0_est, calc_cov=calc_cov, verbose=False)
-
-                elif solver == 'stats':
-                    out = wls_stats(
-                        X, y, w=w, calc_cov=calc_cov, verbose=False)
+                if solver == "sparse":
+                    out = wls_sparse(X, y, w=w, x0=p0_est, calc_cov=True, verbose=False)
+
+                elif solver == "stats":
+                    out = wls_stats(X, y, w=w, calc_cov=True, verbose=False)
 
                 # put E outside of reference section in solution
                 # concatenating makes a copy of the data instead of using a
                 # pointer
-                ds_sub = self[['st', 'ast', 'rst', 'rast', 'trans_att']]
-                ds_sub['df'] = (('time',), out[0][:nt])
-                ds_sub['df_var'] = (('time',), out[1][:nt])
-                ds_sub['db'] = (('time',), out[0][nt:2 * nt])
-                ds_sub['db_var'] = (('time',), out[1][nt:2 * nt])
+                ds_sub = self[["st", "ast", "rst", "rast", "trans_att"]]
+                ds_sub["df"] = (("time",), out[0][:nt])
+                ds_sub["df_var"] = (("time",), out[1][:nt])
+                ds_sub["db"] = (("time",), out[0][nt: 2 * nt])
+                ds_sub["db_var"] = (("time",), out[1][nt: 2 * nt])
 
                 if nta > 0:
                     if np.any(matching_indices):
-                        n_E_in_cal = split['ix_from_cal_match_to_glob'].size
-                        ta = out[0][2 * nt + n_E_in_cal:].reshape(
-                            (nt, 2, nta), order='F')
+                        n_E_in_cal = split["ix_from_cal_match_to_glob"].size
+                        ta = out[0][2 * nt + n_E_in_cal:].reshape((nt, 2, nta), order="F")
                         ta_var = out[1][2 * nt + n_E_in_cal:].reshape(
-                            (nt, 2, nta), order='F')
+                            (nt, 2, nta), order="F"
+                        )
 
                     else:
-                        ta = out[0][2 * nt + nx_sec - 1:].reshape(
-                            (nt, 2, nta), order='F')
+                        ta = out[0][2 * nt + nx_sec - 1:].reshape((nt, 2, nta), order="F")
                         ta_var = out[1][2 * nt + nx_sec - 1:].reshape(
-                            (nt, 2, nta), order='F')
+                            (nt, 2, nta), order="F"
+                        )
 
                     talpha_fw = ta[:, 0, :]
                     talpha_bw = ta[:, 1, :]
                     talpha_fw_var = ta_var[:, 0, :]
                     talpha_bw_var = ta_var[:, 1, :]
                 else:
                     talpha_fw = None
                     talpha_bw = None
                     talpha_fw_var = None
                     talpha_bw_var = None
 
                 E_all_exact, E_all_var_exact = calc_alpha_double(
-                    'exact',
+                    "exact",
                     ds_sub,
                     st_var,
                     ast_var,
                     rst_var,
                     rast_var,
-                    'df',
-                    'db',
-                    'df_var',
-                    'db_var',
+                    "df",
+                    "db",
+                    "df_var",
+                    "db_var",
                     ix_alpha_is_zero=ix_sec[0],
                     talpha_fw=talpha_fw,
                     talpha_bw=talpha_bw,
                     talpha_fw_var=talpha_fw_var,
-                    talpha_bw_var=talpha_bw_var)
+                    talpha_bw_var=talpha_bw_var,
+                )
 
                 if not np.any(matching_indices):
                     # Added fixed gamma and its variance to the solution. And
                     # expand to include locations outside reference sections.
                     p_val = np.concatenate(
                         (
-                            [fix_gamma[0]], out[0][:2 * nt], E_all_exact,
-                            out[0][2 * nt + nx_sec - 1:]))
-                    p_val[1 + 2 * nt + ix_sec[1:]] = out[0][2 * nt:2 * nt
-                                                            + nx_sec - 1]
-                    p_val[1 + 2 * nt + ix_sec[0]] = 0.
+                            [fix_gamma[0]],
+                            out[0][: 2 * nt],
+                            E_all_exact,
+                            out[0][2 * nt + nx_sec - 1:],
+                        )
+                    )
+                    p_val[1 + 2 * nt + ix_sec[1:]] = out[0][2 * nt: 2 * nt + nx_sec - 1]
+                    p_val[1 + 2 * nt + ix_sec[0]] = 0.0
                     p_var = np.concatenate(
                         (
-                            [fix_gamma[1]], out[1][:2 * nt], E_all_var_exact,
-                            out[1][2 * nt + nx_sec - 1:]))
-                    p_var[1 + 2 * nt + ix_sec[1:]] = out[1][2 * nt:2 * nt
-                                                            + nx_sec - 1]
+                            [fix_gamma[1]],
+                            out[1][: 2 * nt],
+                            E_all_var_exact,
+                            out[1][2 * nt + nx_sec - 1:],
+                        )
+                    )
+                    p_var[1 + 2 * nt + ix_sec[1:]] = out[1][2 * nt: 2 * nt + nx_sec - 1]
                 else:
-                    n_E_in_cal = split['ix_from_cal_match_to_glob'].size
+                    n_E_in_cal = split["ix_from_cal_match_to_glob"].size
 
                     # Added fixed gamma and its variance to the solution. And
                     # expand to include locations outside reference sections.
                     p_val = np.concatenate(
                         (
-                            [fix_gamma[0]], out[0][:2 * nt], E_all_exact,
-                            out[0][2 * nt + n_E_in_cal:]))
-                    p_val[1 + 2 * nt + split['ix_from_cal_match_to_glob']] = \
-                        out[0][2 * nt:2 * nt + n_E_in_cal]
-                    p_val[1 + 2 * nt + ix_sec[0]] = 0.
+                            [fix_gamma[0]],
+                            out[0][: 2 * nt],
+                            E_all_exact,
+                            out[0][2 * nt + n_E_in_cal:],
+                        )
+                    )
+                    p_val[1 + 2 * nt + split["ix_from_cal_match_to_glob"]] = \
+                        out[0][2 * nt: 2 * nt + n_E_in_cal]
+                    p_val[1 + 2 * nt + ix_sec[0]] = 0.0
                     p_var = np.concatenate(
                         (
-                            [fix_gamma[1]], out[1][:2 * nt], E_all_var_exact,
-                            out[1][2 * nt + n_E_in_cal:]))
-                    p_var[1 + 2 * nt + split['ix_from_cal_match_to_glob']] = \
-                        out[1][2 * nt:2 * nt + n_E_in_cal]
+                            [fix_gamma[1]],
+                            out[1][: 2 * nt],
+                            E_all_var_exact,
+                            out[1][2 * nt + n_E_in_cal:],
+                        )
+                    )
+                    p_var[1 + 2 * nt + split["ix_from_cal_match_to_glob"]] = \
+                        out[1][2 * nt: 2 * nt + n_E_in_cal]
 
-                if calc_cov:
-                    p_cov = np.diag(p_var).copy()
+                p_cov = np.diag(p_var).copy()
 
-                    if not np.any(matching_indices):
-                        from_i = np.concatenate(
-                            (
-                                np.arange(1,
-                                          2 * nt + 1), 2 * nt + 1 + ix_sec[1:],
-                                np.arange(
-                                    1 + 2 * nt + nx,
-                                    1 + 2 * nt + nx + nta * nt * 2)))
-                    else:
-                        from_i = np.concatenate(
-                            (
-                                np.arange(1, 2 * nt + 1), 2 * nt + 1
-                                + split['ix_from_cal_match_to_glob'],
-                                np.arange(
-                                    1 + 2 * nt + nx,
-                                    1 + 2 * nt + nx + nta * nt * 2)))
-
-                    iox_sec1, iox_sec2 = np.meshgrid(
-                        from_i, from_i, indexing='ij')
-                    p_cov[iox_sec1, iox_sec2] = out[2]
+                if not np.any(matching_indices):
+                    from_i = np.concatenate(
+                        (
+                            np.arange(1, 2 * nt + 1),
+                            2 * nt + 1 + ix_sec[1:],
+                            np.arange(1 + 2 * nt + nx, 1 + 2 * nt + nx + nta * nt * 2),
+                        )
+                    )
+                else:
+                    from_i = np.concatenate(
+                        (
+                            np.arange(1, 2 * nt + 1),
+                            2 * nt + 1 + split["ix_from_cal_match_to_glob"],
+                            np.arange(1 + 2 * nt + nx, 1 + 2 * nt + nx + nta * nt * 2),
+                        )
+                    )
+
+                iox_sec1, iox_sec2 = np.meshgrid(from_i, from_i, indexing="ij")
+                p_cov[iox_sec1, iox_sec2] = out[2]
 
             elif fix_alpha:
-                assert np.size(fix_alpha[0]) == self.x.size, \
-                    'define alpha for each location'
-                assert np.size(fix_alpha[1]) == self.x.size, \
-                    'define var alpha for each location'
-                m = 'The integrated differential attenuation is zero at the ' \
-                    'first index of the reference sections.'
+                assert (
+                    np.size(fix_alpha[0]) == self.x.size
+                ), "define alpha for each location"
+                assert (
+                    np.size(fix_alpha[1]) == self.x.size
+                ), "define var alpha for each location"
+                m = (
+                    "The integrated differential attenuation is zero at the "
+                    "first index of the reference sections."
+                )
                 assert np.abs(fix_alpha[0][ix_sec[0]]) < 1e-6, m
                 # The array with the integrated differential att is termed E
 
                 if not np.any(matching_indices):
                     # X_gamma
-                    X_E = sp.vstack((-split['E'], split['E']))
+                    X_E = sp.vstack((-split["E"], split["E"]))
                     # Use only the remaining coefficients
                     # Stack all X's
                     X = sp.vstack(
                         (
                             sp.hstack(
                                 (
-                                    split['Z_gamma'], -split['Z_D'],
-                                    split['Zero_d'], split['Z_TA_fw'])),
+                                    split["Z_gamma"],
+                                    -split["Z_D"],
+                                    split["Zero_d"],
+                                    split["Z_TA_fw"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['Z_gamma'], split['Zero_d'],
-                                    -split['Z_D'], split['Z_TA_bw']))))
+                                    split["Z_gamma"],
+                                    split["Zero_d"],
+                                    -split["Z_D"],
+                                    split["Z_TA_bw"],
+                                )
+                            ),
+                        )
+                    )
                     # Move the coefficients times the fixed gamma to the
                     # observations
-                    y = np.concatenate((split['y_F'], split['y_B']))
+                    y = np.concatenate((split["y_F"], split["y_B"]))
                     y -= X_E.dot(fix_alpha[0][ix_sec[1:]])
 
                     # variances are added. weight is the inverse of the variance
                     # of the observations
-                    if method == 'wls':
-                        w_ = np.concatenate((split['w_F'], split['w_B']))
-                        w = 1 / (1 / w_ + X_E.dot(fix_alpha[1][ix_sec[1:]]))
-
-                    else:
-                        w = 1.
+                    w_ = np.concatenate((split["w_F"], split["w_B"]))
+                    w = 1 / (1 / w_ + X_E.dot(fix_alpha[1][ix_sec[1:]]))
 
                     p0_est = np.concatenate(
                         (
-                            split['p0_est'][:1 + 2 * nt],
-                            split['p0_est'][1 + 2 * nt + nx_sec - 1:]))
+                            split["p0_est"][: 1 + 2 * nt],
+                            split["p0_est"][1 + 2 * nt + nx_sec - 1:],
+                        )
+                    )
 
                 else:
-                    n_E_in_cal = split['ix_from_cal_match_to_glob'].size
+                    n_E_in_cal = split["ix_from_cal_match_to_glob"].size
                     p0_est = np.concatenate(
                         (
-                            split['p0_est'][:1 + 2 * nt],
-                            split['p0_est'][1 + 2 * nt + n_E_in_cal:]))
-                    X_E1 = sp.csr_matrix(
-                        ([], ([], [])), shape=(nt * nx_sec, self.x.size))
-                    X_E1[:, ix_sec[1:]] = split['E']
-                    X_E2 = X_E1[:, split['ix_from_cal_match_to_glob']]
+                            split["p0_est"][: 1 + 2 * nt],
+                            split["p0_est"][1 + 2 * nt + n_E_in_cal:],
+                        )
+                    )
+                    X_E1 = sp.csr_matrix(([], ([], [])), shape=(nt * nx_sec, self.x.size))
+                    X_E1[:, ix_sec[1:]] = split["E"]
+                    X_E2 = X_E1[:, split["ix_from_cal_match_to_glob"]]
                     X_E = sp.vstack(
                         (
-                            -X_E2, X_E2, split['E_match_F'],
-                            split['E_match_B'], split['E_match_no_cal']))
+                            -X_E2,
+                            X_E2,
+                            split["E_match_F"],
+                            split["E_match_B"],
+                            split["E_match_no_cal"],
+                        )
+                    )
 
                     X = sp.vstack(
                         (
                             sp.hstack(
                                 (
-                                    split['Z_gamma'], -split['Z_D'],
-                                    split['Zero_d'], split['Z_TA_fw'])),
+                                    split["Z_gamma"],
+                                    -split["Z_D"],
+                                    split["Zero_d"],
+                                    split["Z_TA_fw"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['Z_gamma'], split['Zero_d'],
-                                    -split['Z_D'], split['Z_TA_bw'])),
+                                    split["Z_gamma"],
+                                    split["Zero_d"],
+                                    -split["Z_D"],
+                                    split["Z_TA_bw"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['Zero_eq12_gamma'],
-                                    split['Zero_d_eq12'], split['Z_TA_eq1'])),
+                                    split["Zero_eq12_gamma"],
+                                    split["Zero_d_eq12"],
+                                    split["Z_TA_eq1"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['Zero_eq12_gamma'],
-                                    split['Zero_d_eq12'], split['Z_TA_eq2'])),
+                                    split["Zero_eq12_gamma"],
+                                    split["Zero_d_eq12"],
+                                    split["Z_TA_eq2"],
+                                )
+                            ),
                             sp.hstack(
                                 (
-                                    split['Zero_eq3_gamma'], split['d_no_cal'],
-                                    split['Z_TA_eq3']))))
+                                    split["Zero_eq3_gamma"],
+                                    split["d_no_cal"],
+                                    split["Z_TA_eq3"],
+                                )
+                            ),
+                        )
+                    )
 
                     y = np.concatenate(
                         (
-                            split['y_F'], split['y_B'], split['y_eq1'],
-                            split['y_eq2'], split['y_eq3']))
-                    y -= X_E.dot(
-                        fix_alpha[0][split['ix_from_cal_match_to_glob']])
+                            split["y_F"],
+                            split["y_B"],
+                            split["y_eq1"],
+                            split["y_eq2"],
+                            split["y_eq3"],
+                        )
+                    )
+                    y -= X_E.dot(fix_alpha[0][split["ix_from_cal_match_to_glob"]])
 
                     # variances are added. weight is the inverse of the variance
                     # of the observations
-                    if method == 'wls':
-                        w_ = np.concatenate(
-                            (
-                                split['w_F'], split['w_B'], split['w_eq1'],
-                                split['w_eq2'], split['w_eq3']))
-                        w = 1 / (
-                            1 / w_ + X_E.dot(
-                                fix_alpha[1][
-                                    split['ix_from_cal_match_to_glob']]))
+                    w_ = np.concatenate(
+                        (
+                            split["w_F"],
+                            split["w_B"],
+                            split["w_eq1"],
+                            split["w_eq2"],
+                            split["w_eq3"],
+                        )
+                    )
+                    w = 1 / (
+                        1 / w_ + X_E.dot(fix_alpha[1][split["ix_from_cal_match_to_glob"]])
+                    )
 
-                    else:
-                        w = 1.
+                if solver == "sparse":
+                    out = wls_sparse(X, y, w=w, x0=p0_est, calc_cov=True, verbose=False)
 
-                if solver == 'sparse':
-                    out = wls_sparse(
-                        X, y, w=w, x0=p0_est, calc_cov=calc_cov, verbose=False)
-
-                elif solver == 'stats':
-                    out = wls_stats(
-                        X, y, w=w, calc_cov=calc_cov, verbose=False)
+                elif solver == "stats":
+                    out = wls_stats(X, y, w=w, calc_cov=True, verbose=False)
 
                 # Added fixed gamma and its variance to the solution
                 p_val = np.concatenate(
-                    (out[0][:1 + 2 * nt], fix_alpha[0], out[0][1 + 2 * nt:]))
+                    (out[0][: 1 + 2 * nt], fix_alpha[0], out[0][1 + 2 * nt:])
+                )
                 p_var = np.concatenate(
-                    (out[1][:1 + 2 * nt], fix_alpha[1], out[1][1 + 2 * nt:]))
+                    (out[1][: 1 + 2 * nt], fix_alpha[1], out[1][1 + 2 * nt:])
+                )
 
-                if calc_cov:
-                    p_cov = np.diag(p_var).copy()
+                p_cov = np.diag(p_var).copy()
 
-                    from_i = np.concatenate(
-                        (
-                            np.arange(1 + 2 * nt),
-                            np.arange(
-                                1 + 2 * nt + nx,
-                                1 + 2 * nt + nx + nta * nt * 2)))
-
-                    iox_sec1, iox_sec2 = np.meshgrid(
-                        from_i, from_i, indexing='ij')
-                    p_cov[iox_sec1, iox_sec2] = out[2]
+                from_i = np.concatenate(
+                    (
+                        np.arange(1 + 2 * nt),
+                        np.arange(1 + 2 * nt + nx, 1 + 2 * nt + nx + nta * nt * 2),
+                    )
+                )
+
+                iox_sec1, iox_sec2 = np.meshgrid(from_i, from_i, indexing="ij")
+                p_cov[iox_sec1, iox_sec2] = out[2]
 
             else:
                 pass
 
-        elif method == 'external':
+        elif method == "external":
             for input_item in [p_val, p_var, p_cov]:
                 assert input_item is not None
 
-            calc_cov = True
-
-        elif method == 'external_split':
-            raise ValueError('Not implemented yet')
+        elif method == "external_split":
+            raise ValueError("Not implemented yet")
 
         else:
-            raise ValueError('Choose a valid method')
+            raise ValueError("Choose a valid method")
 
         # all below require the following solution sizes
-        npar = 1 + 2 * nt + nx + 2 * nt * nta
-        assert p_val.size == npar
-        assert p_var.size == npar
-        if calc_cov:
-            assert p_cov.shape == (npar, npar)
+        ip = ParameterIndexDoubleEnded(nt, nx, nta)
 
-        gamma = p_val[0]
-        d_fw = p_val[1:nt + 1]
-        d_bw = p_val[1 + nt:1 + 2 * nt]
-        alpha = p_val[1 + 2 * nt:1 + 2 * nt + nx]
-
-        # store calibration parameters in DataStore
-        self[store_gamma] = (tuple(), gamma)
-        self[store_alpha] = (('x',), alpha)
-        self[store_df] = ((time_dim,), d_fw)
-        self[store_db] = ((time_dim,), d_bw)
+        # npar = 1 + 2 * nt + nx + 2 * nt * nta
+        assert p_val.size == ip.npar
+        assert p_var.size == ip.npar
+        assert p_cov.shape == (ip.npar, ip.npar)
+
+        # save estimates and variances to datastore, skip covariances
+        self[store_gamma] = (tuple(), p_val[ip.gamma].item())
+        self[store_alpha] = (("x",), p_val[ip.alpha])
+        self[store_df] = ((time_dim,), p_val[ip.df])
+        self[store_db] = ((time_dim,), p_val[ip.db])
 
-        if nta > 0:
-            ta = p_val[1 + 2 * nt + nx:].reshape((nt, 2, nta), order='F')
-            self[store_ta + '_fw'] = ((time_dim, 'trans_att'), ta[:, 0, :])
-            self[store_ta + '_bw'] = ((time_dim, 'trans_att'), ta[:, 1, :])
-
-        # store variances in DataStore
-        if method == 'wls' or method == 'external':
-            # the variances only have meaning if the observations are weighted
-            gammavar = p_var[0]
-            dfvar = p_var[1:nt + 1]
-            dbvar = p_var[1 + nt:1 + 2 * nt]
-            alphavar = p_var[2 * nt + 1:2 * nt + 1 + nx]
-
-            self[store_gamma + variance_suffix] = (tuple(), gammavar)
-            self[store_alpha + variance_suffix] = (('x',), alphavar)
-            self[store_df + variance_suffix] = ((time_dim,), dfvar)
-            self[store_db + variance_suffix] = ((time_dim,), dbvar)
-
-            if nta > 0:
-                # neglecting the covariances. Better include them
-                tavar = p_var[2 * nt + 1 + nx:].reshape(
-                    (nt, 2, nta), order='F')
-                self[store_ta + '_fw' + variance_suffix] = (
-                    (time_dim, 'trans_att'), tavar[:, 0, :])
-                self[store_ta + '_bw' + variance_suffix] = (
-                    (time_dim, 'trans_att'), tavar[:, 1, :])
-
-        # deal with FW
-        if store_tmpf or (store_tmpw and method == 'ols'):
-            ta_arr = np.zeros((nx, nt))
-            if nta > 0:
-                for tai, taxi in zip(self[store_ta + '_fw'].values.T,
-                                     self.trans_att.values):
-                    ta_arr[self.x.values >= taxi] = \
-                        ta_arr[self.x.values >= taxi] + tai
-
-            tempF_data = gamma / (
-                np.log(self.st.data / self.ast.data) + d_fw + alpha[:, None]
-                + ta_arr) - 273.15
-            self[store_tmpf] = (('x', time_dim), tempF_data)
-
-        # deal with BW
-        if store_tmpb or (store_tmpw and method == 'ols'):
-            ta_arr = np.zeros((nx, nt))
-            if nta > 0:
-                for tai, taxi in zip(self[store_ta + '_bw'].values.T,
-                                     self.trans_att.values):
-                    ta_arr[self.x.values < taxi] = \
-                        ta_arr[self.x.values < taxi] + tai
-            tempB_data = gamma / (
-                np.log(self.rst.data / self.rast.data) + d_bw - alpha[:, None]
-                + ta_arr) - 273.15
-            self[store_tmpb] = (('x', time_dim), tempB_data)
-
-        if store_tmpw and (method == 'wls' or method == 'external'):
-            self.conf_int_double_ended(
-                p_val=p_val,
-                p_cov=p_cov,
-                store_ta=store_ta if self.trans_att.size > 0 else None,
-                st_var=st_var,
-                ast_var=ast_var,
-                rst_var=rst_var,
-                rast_var=rast_var,
-                store_tmpf='',
-                store_tmpb='',
-                store_tmpw=store_tmpw,
-                store_tempvar=variance_suffix,
-                conf_ints=[],
-                mc_sample_size=tmpw_mc_size,
-                da_random_state=None,
-                remove_mc_set_flag=remove_mc_set_flag,
-                reduce_memory_usage=reduce_memory_usage)
-
-        elif store_tmpw and method == 'ols':
-            self[store_tmpw] = (self[store_tmpf] + self[store_tmpb]) / 2
+        if nta:
+            self[store_ta + "_fw"] = (
+                (time_dim, "trans_att"),
+                p_val[ip.taf].reshape((nt, nta), order="C"),
+            )
+            self[store_ta + "_bw"] = (
+                (time_dim, "trans_att"),
+                p_val[ip.tab].reshape((nt, nta), order="C"),
+            )
+            self[store_ta + "_fw" + variance_suffix] = (
+                (time_dim, "trans_att"),
+                p_var[ip.taf].reshape((nt, nta), order="C"),
+            )
+            self[store_ta + "_bw" + variance_suffix] = (
+                (time_dim, "trans_att"),
+                p_var[ip.tab].reshape((nt, nta), order="C"),
+            )
         else:
-            pass
+            self[store_ta + "_fw"] = ((time_dim, "trans_att"), np.zeros((nt, 0)))
+            self[store_ta + "_bw"] = ((time_dim, "trans_att"), np.zeros((nt, 0)))
+            self[store_ta + "_fw" + variance_suffix] = ((time_dim, "trans_att"), np.zeros((nt, 0)))
+            self[store_ta + "_bw" + variance_suffix] = ((time_dim, "trans_att"), np.zeros((nt, 0)))
+
+        self[store_ta + "_fw_full"] = (
+            ("x", time_dim),
+            ip.get_taf_values(
+                pval=p_val, x=self.x.values, trans_att=self.trans_att.values, axis=""
+            ),
+        )
+        self[store_ta + "_bw_full"] = (
+            ("x", time_dim),
+            ip.get_tab_values(
+                pval=p_val, x=self.x.values, trans_att=self.trans_att.values, axis=""
+            ),
+        )
+
+        self[store_tmpf] = (
+            self[store_gamma]
+            / (
+                np.log(self.st / self.ast)
+                + self[store_df]
+                + self[store_alpha]
+                + self[store_ta + "_fw_full"]
+            )
+            - 273.15
+        )
+
+        self[store_tmpb] = (
+            self[store_gamma]
+            / (
+                np.log(self.rst / self.rast)
+                + self[store_db]
+                - self[store_alpha]
+                + self[store_ta + "_bw_full"]
+            )
+            - 273.15
+        )
+
+        self[store_gamma + variance_suffix] = (tuple(), p_var[ip.gamma].item())
+        self[store_alpha + variance_suffix] = (("x",), p_var[ip.alpha])
+        self[store_df + variance_suffix] = ((time_dim,), p_var[ip.df])
+        self[store_db + variance_suffix] = ((time_dim,), p_var[ip.db])
+        self[store_ta + "_fw_full" + variance_suffix] = (
+            ("x", time_dim),
+            ip.get_taf_values(
+                pval=p_var, x=self.x.values, trans_att=self.trans_att.values, axis=""
+            ),
+        )
+        self[store_ta + "_bw_full" + variance_suffix] = (
+            ("x", time_dim),
+            ip.get_tab_values(
+                pval=p_var, x=self.x.values, trans_att=self.trans_att.values, axis=""
+            ),
+        )
+
+        # extract covariances and ensure broadcastable to (nx, nt)
+        sigma2_gamma_df = p_cov[np.ix_(ip.gamma, ip.df)]
+        sigma2_gamma_db = p_cov[np.ix_(ip.gamma, ip.db)]
+        sigma2_gamma_alpha = p_cov[np.ix_(ip.alpha, ip.gamma)]
+        sigma2_df_db = p_cov[ip.df, ip.db][None]  # Shape is [0, nt] ?
+        sigma2_alpha_df = p_cov[np.ix_(ip.alpha, ip.df)]
+        sigma2_alpha_db = p_cov[np.ix_(ip.alpha, ip.db)]
+        sigma2_tafw_gamma = ip.get_taf_values(
+            pval=p_cov[ip.gamma],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="",
+        )
+        sigma2_tabw_gamma = ip.get_tab_values(
+            pval=p_cov[ip.gamma],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="",
+        )
+        sigma2_tafw_alpha = ip.get_taf_values(
+            pval=p_cov[ip.alpha],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="x",
+        )
+        sigma2_tabw_alpha = ip.get_tab_values(
+            pval=p_cov[ip.alpha],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="x",
+        )
+        sigma2_tafw_df = ip.get_taf_values(
+            pval=p_cov[ip.df],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="time",
+        )
+        sigma2_tafw_db = ip.get_taf_values(
+            pval=p_cov[ip.db],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="time",
+        )
+        sigma2_tabw_db = ip.get_tab_values(
+            pval=p_cov[ip.db],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="time",
+        )
+        sigma2_tabw_df = ip.get_tab_values(
+            pval=p_cov[ip.df],
+            x=self.x.values,
+            trans_att=self.trans_att.values,
+            axis="time",
+        )
+        # sigma2_tafw_tabw
+
+        tmpf = self[store_tmpf] + 273.15
+        tmpb = self[store_tmpb] + 273.15
+
+        deriv_dict = dict(
+            T_gamma_fw=tmpf / self[store_gamma],
+            T_st_fw=-(tmpf ** 2) / (self[store_gamma] * self.st),
+            T_ast_fw=tmpf ** 2 / (self[store_gamma] * self.ast),
+            T_df_fw=-(tmpf ** 2) / self[store_gamma],
+            T_alpha_fw=-(tmpf ** 2) / self[store_gamma],
+            T_ta_fw=-(tmpf ** 2) / self[store_gamma],
+            T_gamma_bw=tmpb / self[store_gamma],
+            T_rst_bw=-(tmpb ** 2) / (self[store_gamma] * self.rst),
+            T_rast_bw=tmpb ** 2 / (self[store_gamma] * self.rast),
+            T_db_bw=-(tmpb ** 2) / self[store_gamma],
+            T_alpha_bw=tmpb ** 2 / self[store_gamma],
+            T_ta_bw=-(tmpb ** 2) / self[store_gamma],
+        )
+        deriv_ds = xr.Dataset(deriv_dict)
+        self["deriv"] = deriv_ds.to_array(dim="com2")
+
+        var_fw_dict = dict(
+            dT_dst=deriv_ds.T_st_fw ** 2 * parse_st_var(self, st_var, st_label="st"),
+            dT_dast=deriv_ds.T_ast_fw ** 2 * parse_st_var(self, ast_var, st_label="ast"),
+            dT_gamma=deriv_ds.T_gamma_fw ** 2 * self[store_gamma + variance_suffix],
+            dT_ddf=deriv_ds.T_df_fw ** 2 * self[store_df + variance_suffix],
+            dT_dalpha=deriv_ds.T_alpha_fw ** 2 * self[store_alpha + variance_suffix],
+            dT_dta=deriv_ds.T_ta_fw ** 2 * self[store_ta + "_fw_full" + variance_suffix],
+            dgamma_ddf=(2 * deriv_ds.T_gamma_fw * deriv_ds.T_df_fw * sigma2_gamma_df),
+            dgamma_dalpha=(
+                2 * deriv_ds.T_gamma_fw * deriv_ds.T_alpha_fw * sigma2_gamma_alpha
+            ),
+            dalpha_ddf=(
+                2 * deriv_ds.T_alpha_fw * deriv_ds.T_df_fw * sigma2_alpha_df
+            ),
+            dta_dgamma=(2 * deriv_ds.T_ta_fw * deriv_ds.T_gamma_fw * sigma2_tafw_gamma),
+            dta_ddf=(2 * deriv_ds.T_ta_fw * deriv_ds.T_df_fw * sigma2_tafw_df),
+            dta_dalpha=(2 * deriv_ds.T_ta_fw * deriv_ds.T_alpha_fw * sigma2_tafw_alpha),
+        )
+        var_bw_dict = dict(
+            dT_drst=deriv_ds.T_rst_bw ** 2 * parse_st_var(self, rst_var, st_label="rst"),
+            dT_drast=deriv_ds.T_rast_bw ** 2 * parse_st_var(self, rast_var, st_label="rast"),
+            dT_gamma=deriv_ds.T_gamma_bw ** 2 * self[store_gamma + variance_suffix],
+            dT_ddb=deriv_ds.T_db_bw ** 2 * self[store_db + variance_suffix],
+            dT_dalpha=deriv_ds.T_alpha_bw ** 2 * self[store_alpha + variance_suffix],
+            dT_dta=deriv_ds.T_ta_bw ** 2 * self[store_ta + "_bw_full" + variance_suffix],
+            dgamma_ddb=(2 * deriv_ds.T_gamma_bw * deriv_ds.T_db_bw * sigma2_gamma_db),
+            dgamma_dalpha=(
+                2 * deriv_ds.T_gamma_bw * deriv_ds.T_alpha_bw * sigma2_gamma_alpha
+            ),
+            dalpha_ddb=(2 * deriv_ds.T_alpha_bw * deriv_ds.T_db_bw * sigma2_alpha_db),
+            dta_dgamma=(2 * deriv_ds.T_ta_bw * deriv_ds.T_gamma_bw * sigma2_tabw_gamma),
+            dta_ddb=(2 * deriv_ds.T_ta_bw * deriv_ds.T_db_bw * sigma2_tabw_db),
+            dta_dalpha=(2 * deriv_ds.T_ta_bw * deriv_ds.T_alpha_bw * sigma2_tabw_alpha),
+        )
+
+        self["var_fw_da"] = xr.Dataset(var_fw_dict).to_array(dim="comp_fw")
+        self["var_bw_da"] = xr.Dataset(var_bw_dict).to_array(dim="comp_bw")
+
+        self[store_tmpf + variance_suffix] = self["var_fw_da"].sum(dim="comp_fw")
+        self[store_tmpb + variance_suffix] = self["var_bw_da"].sum(dim="comp_bw")
+
+        # First estimate of tmpw_var
+        self[store_tmpw + variance_suffix + "_approx"] = 1 / (
+            1 / self[store_tmpf + variance_suffix] + 1 / self[store_tmpb + variance_suffix]
+        )
+        self[store_tmpw] = ((tmpf / self[store_tmpf + variance_suffix] +
+                             tmpb / self[store_tmpb + variance_suffix]
+                             ) * self[store_tmpw + variance_suffix + "_approx"]) - 273.15
+
+        weightsf = self[store_tmpw + variance_suffix + "_approx"] / self[store_tmpf + variance_suffix]
+        weightsb = self[store_tmpw + variance_suffix + "_approx"] / self[store_tmpb + variance_suffix]
+
+        deriv_dict2 = dict(
+            T_gamma_w=weightsf * deriv_dict['T_gamma_fw'] + weightsb * deriv_dict['T_gamma_bw'],
+            T_st_w=weightsf * deriv_dict['T_st_fw'],
+            T_ast_w=weightsf * deriv_dict['T_ast_fw'],
+            T_rst_w=weightsb * deriv_dict['T_rst_bw'],
+            T_rast_w=weightsb * deriv_dict['T_rast_bw'],
+            T_df_w=weightsf * deriv_dict['T_df_fw'],
+            T_db_w=weightsb * deriv_dict['T_db_bw'],
+            T_alpha_w=weightsf * deriv_dict['T_alpha_fw'] + weightsb * deriv_dict['T_alpha_bw'],
+            T_taf_w=weightsf * deriv_dict['T_ta_fw'],
+            T_tab_w=weightsb * deriv_dict['T_ta_bw'],
+        )
+        deriv_ds2 = xr.Dataset(deriv_dict2)
+
+        # TODO: sigma2_tafw_tabw
+        var_w_dict = dict(
+            dT_dst=deriv_ds2.T_st_w ** 2 * parse_st_var(self, st_var, st_label="st"),
+            dT_dast=deriv_ds2.T_ast_w ** 2 * parse_st_var(self, ast_var, st_label="ast"),
+            dT_drst=deriv_ds2.T_rst_w ** 2 * parse_st_var(self, rst_var, st_label="rst"),
+            dT_drast=deriv_ds2.T_rast_w ** 2 * parse_st_var(self, rast_var, st_label="rast"),
+            dT_gamma=deriv_ds2.T_gamma_w ** 2 * self[store_gamma + variance_suffix],
+            dT_ddf=deriv_ds2.T_df_w ** 2 * self[store_df + variance_suffix],
+            dT_ddb=deriv_ds2.T_db_w ** 2 * self[store_db + variance_suffix],
+            dT_dalpha=deriv_ds2.T_alpha_w ** 2 * self[store_alpha + variance_suffix],
+            dT_dtaf=deriv_ds2.T_taf_w ** 2 * self[store_ta + "_fw_full" + variance_suffix],
+            dT_dtab=deriv_ds2.T_tab_w ** 2 * self[store_ta + "_bw_full" + variance_suffix],
+            dgamma_ddf=2 * deriv_ds2.T_gamma_w * deriv_ds2.T_df_w * sigma2_gamma_df,
+            dgamma_ddb=2 * deriv_ds2.T_gamma_w * deriv_ds2.T_db_w * sigma2_gamma_db,
+            dgamma_dalpha=2 * deriv_ds2.T_gamma_w * deriv_ds2.T_alpha_w * sigma2_gamma_alpha,
+            dgamma_dtaf=2 * deriv_ds2.T_gamma_w * deriv_ds2.T_taf_w * sigma2_tafw_gamma,
+            dgamma_dtab=2 * deriv_ds2.T_gamma_w * deriv_ds2.T_tab_w * sigma2_tabw_gamma,
+            ddf_ddb=2 * deriv_ds2.T_df_w * deriv_ds2.T_db_w * sigma2_df_db,
+            ddf_dalpha=2 * deriv_ds2.T_df_w * deriv_ds2.T_alpha_w * sigma2_alpha_df,
+            ddf_dtaf=2 * deriv_ds2.T_df_w * deriv_ds2.T_taf_w * sigma2_tafw_df,
+            ddf_dtab=2 * deriv_ds2.T_df_w * deriv_ds2.T_tab_w * sigma2_tabw_df,
+            ddb_dalpha=2 * deriv_ds2.T_db_w * deriv_ds2.T_alpha_w * sigma2_alpha_db,
+            ddb_dtaf=2 * deriv_ds2.T_db_w * deriv_ds2.T_taf_w * sigma2_tafw_db,
+            ddb_dtab=2 * deriv_ds2.T_db_w * deriv_ds2.T_tab_w * sigma2_tabw_db,
+            # dtaf_dtab=2 * deriv_ds2.T_tab_w * deriv_ds2.T_tab_w * sigma2_tafw_tabw,
+        )
+        self["var_w_da"] = xr.Dataset(var_w_dict).to_array(dim="comp_w")
+        self[store_tmpw + variance_suffix] = self["var_w_da"].sum(dim="comp_w")
+
+        tmpf_var_excl_par = (
+            self["var_fw_da"].sel(comp_fw=["dT_dst", "dT_dast"]).sum(dim="comp_fw")
+        )
+        tmpb_var_excl_par = (
+            self["var_bw_da"].sel(comp_bw=["dT_drst", "dT_drast"]).sum(dim="comp_bw")
+        )
+        self[store_tmpw + variance_suffix + "_lower"] = 1 / (
+            1 / tmpf_var_excl_par + 1 / tmpb_var_excl_par
+        )
+
+        self[store_tmpf].attrs.update(_dim_attrs[("tmpf",)])
+        self[store_tmpb].attrs.update(_dim_attrs[("tmpb",)])
+        self[store_tmpw].attrs.update(_dim_attrs[("tmpw",)])
+        self[store_tmpf + variance_suffix].attrs.update(_dim_attrs[("tmpf_var",)])
+        self[store_tmpb + variance_suffix].attrs.update(_dim_attrs[("tmpb_var",)])
+        self[store_tmpw + variance_suffix].attrs.update(
+            _dim_attrs[("tmpw_var",)]
+        )
+        self[store_tmpw + variance_suffix + "_approx"].attrs.update(
+            _dim_attrs[("tmpw_var_approx",)]
+        )
+        self[store_tmpw + variance_suffix + "_lower"].attrs.update(
+            _dim_attrs[("tmpw_var_lower",)]
+        )
+
+        drop_vars = [
+            k for k, v in self.items() if {"params1", "params2"}.intersection(v.dims)
+        ]
 
-        if store_p_val:
-            drop_vars = [
-                k for k, v in self.items()
-                if {'params1', 'params2'}.intersection(v.dims)]
-
-            for k in drop_vars:
-                del self[k]
-
-            self[store_p_val] = (('params1',), p_val)
-
-            if method == 'wls' or method == 'external':
-                assert store_p_cov, 'Might as well store the covariance matrix. Already computed.'
-                self[store_p_cov] = (('params1', 'params2'), p_cov)
+        for k in drop_vars:
+            del self[k]
+
+        self[store_p_val] = (("params1",), p_val)
+        self[store_p_cov] = (("params1", "params2"), p_cov)
 
         pass
 
     def conf_int_single_ended(
             self,
             p_val='p_val',
             p_cov='p_cov',
             st_var=None,
             ast_var=None,
             store_tmpf='tmpf',
             store_tempvar='_var',
             conf_ints=None,
             mc_sample_size=100,
             da_random_state=None,
-            remove_mc_set_flag=True,
+            mc_remove_set_flag=True,
             reduce_memory_usage=False,
             **kwargs):
         """
         Estimation of the confidence intervals for the temperatures measured
         with a single-ended setup. It consists of five steps. First, the variances
         of the Stokes and anti-Stokes intensity measurements are estimated
         following the steps in Section 4 [1]_. A Normal
@@ -3305,15 +3640,15 @@
         mc_sample_size : int
             Size of the monte carlo parameter set used to calculate the
             confidence interval
         da_random_state
             For testing purposes. Similar to random seed. The seed for dask.
             Makes random not so random. To produce reproducable results for
             testing environments.
-        remove_mc_set_flag : bool
+        mc_remove_set_flag : bool
             Remove the monte carlo data set, from which the CI and the
             variance are calculated.
         reduce_memory_usage : bool
             Use less memory but at the expense of longer computation time
 
 
         References
@@ -3477,15 +3812,15 @@
                 lambda x: np.percentile(x, q=conf_ints, axis=avg_axis),
                 chunks=new_chunks,  #
                 drop_axis=avg_axis,  # avg dimesnions are dropped from input arr
                 new_axis=0)  # The new CI dimension is added as first axis
 
             self[store_tmpf + '_mc'] = (('CI', 'x', time_dim), q)
 
-        if remove_mc_set_flag:
+        if mc_remove_set_flag:
             drop_var = [
                 'gamma_mc', 'dalpha_mc', 'alpha_mc', 'c_mc', 'mc', 'r_st',
                 'r_ast', store_tmpf + '_mc_set', 'ta_mc_arr']
             for k in drop_var:
                 if k in self:
                     del self[k]
 
@@ -3507,15 +3842,15 @@
             ci_avg_time_isel=None,
             ci_avg_x_flag1=False,
             ci_avg_x_flag2=False,
             ci_avg_x_sel=None,
             ci_avg_x_isel=None,
             var_only_sections=None,
             da_random_state=None,
-            remove_mc_set_flag=True,
+            mc_remove_set_flag=True,
             reduce_memory_usage=False,
             **kwargs):
         """
         Average temperatures from single-ended setups.
 
         Four types of averaging are implemented. Please see Example Notebook 16.
 
@@ -3636,15 +3971,15 @@
             reference sections. Where the accuracy is the variance of the
             residuals between the estimated temperature and temperature of the
             water baths.
         da_random_state
             For testing purposes. Similar to random seed. The seed for dask.
             Makes random not so random. To produce reproducable results for
             testing environments.
-        remove_mc_set_flag : bool
+        mc_remove_set_flag : bool
             Remove the monte carlo data set, from which the CI and the
             variance are calculated.
         reduce_memory_usage : bool
             Use less memory but at the expense of longer computation time
 
         Returns
         -------
@@ -3661,15 +3996,15 @@
             st_var=st_var,
             ast_var=ast_var,
             store_tmpf=store_tmpf,
             store_tempvar=store_tempvar,
             conf_ints=None,
             mc_sample_size=mc_sample_size,
             da_random_state=da_random_state,
-            remove_mc_set_flag=False,
+            mc_remove_set_flag=False,
             reduce_memory_usage=reduce_memory_usage,
             **kwargs)
 
         time_dim = self.get_time_dim(data_var_key='st')
 
         if ci_avg_time_sel is not None:
             time_dim2 = time_dim + '_avg'
@@ -3843,15 +4178,15 @@
                     drop_axis=avg_axis_avg2,
                     # avg dimensions are dropped from input arr
                     new_axis=0,
                     dtype=float)  # The new CI dimension is added as
                 # firsaxis
                 self[store_tmpf + '_mc_avg2'] = (('CI', x_dim2), qq)
         # Clean up the garbage. All arrays with a Monte Carlo dimension.
-        if remove_mc_set_flag:
+        if mc_remove_set_flag:
             remove_mc_set = [
                 'r_st', 'r_ast', 'gamma_mc', 'dalpha_mc', 'c_mc', 'x_avg',
                 'time_avg', 'mc', 'ta_mc_arr']
             remove_mc_set.append(store_tmpf + '_avgsec')
             remove_mc_set.append(store_tmpf + '_mc_set')
             remove_mc_set.append(store_tmpf + '_mc_avg2_set')
             remove_mc_set.append(store_tmpf + '_mc_avgx2_set')
@@ -3875,15 +4210,15 @@
             store_tmpb='tmpb',
             store_tmpw='tmpw',
             store_tempvar='_var',
             conf_ints=None,
             mc_sample_size=100,
             var_only_sections=False,
             da_random_state=None,
-            remove_mc_set_flag=True,
+            mc_remove_set_flag=True,
             reduce_memory_usage=False,
             **kwargs):
         """
         Estimation of the confidence intervals for the temperatures measured
         with a double-ended setup.
         Double-ended setups require four additional steps to estimate the
         confidence intervals for the temperature. First, the variances of the
@@ -4006,15 +4341,15 @@
             reference sections. Where the accuracy is the variance of the
             residuals between the estimated temperature and temperature of the
             water baths.
         da_random_state
             For testing purposes. Similar to random seed. The seed for dask.
             Makes random not so random. To produce reproducable results for
             testing environments.
-        remove_mc_set_flag : bool
+        mc_remove_set_flag : bool
             Remove the monte carlo data set, from which the CI and the
             variance are calculated.
         reduce_memory_usage : bool
             Use less memory but at the expense of longer computation time
 
         Returns
         -------
@@ -4088,14 +4423,15 @@
 
         if store_ta:
             ta_dim = [
                 i for i in self[store_ta + '_fw'].dims if i != time_dim][0]
             tax = self[ta_dim].values
             nta = tax.size
             npar += nt * 2 * nta
+
         else:
             nta = 0
 
         rsize = (mc_sample_size, no, nt)
 
         if reduce_memory_usage:
             memchunk = da.ones(
@@ -4363,15 +4699,15 @@
                 chunks=new_chunks_weighted,  # Explicitly define output chunks
                 drop_axis=avg_axis,  # avg dimensions are dropped
                 new_axis=0,
                 dtype=float)  # The new CI dimension is added as first axis
             self[store_tmpw + '_mc'] = (('CI', 'x', time_dim), q2)
 
         # Clean up the garbage. All arrays with a Monte Carlo dimension.
-        if remove_mc_set_flag:
+        if mc_remove_set_flag:
             remove_mc_set = [
                 'r_st', 'r_ast', 'r_rst', 'r_rast', 'gamma_mc', 'alpha_mc',
                 'df_mc', 'db_mc']
 
             for i in [store_tmpf, store_tmpb, store_tmpw]:
                 remove_mc_set.append(i + '_mc_set')
 
@@ -4409,15 +4745,15 @@
             ci_avg_time_sel=None,
             ci_avg_time_isel=None,
             ci_avg_x_flag1=False,
             ci_avg_x_flag2=False,
             ci_avg_x_sel=None,
             ci_avg_x_isel=None,
             da_random_state=None,
-            remove_mc_set_flag=True,
+            mc_remove_set_flag=True,
             reduce_memory_usage=False,
             **kwargs):
         """
         Average temperatures from double-ended setups.
 
         Four types of averaging are implemented. Please see Example Notebook 16.
 
@@ -4543,15 +4879,15 @@
         ci_avg_x_isel : iterable of int
             Compute ci_avg_time_flag1 and ci_avg_time_flag2 using only a
             selection of the data
         da_random_state
             For testing purposes. Similar to random seed. The seed for dask.
             Makes random not so random. To produce reproducable results for
             testing environments.
-        remove_mc_set_flag : bool
+        mc_remove_set_flag : bool
             Remove the monte carlo data set, from which the CI and the
             variance are calculated.
         reduce_memory_usage : bool
             Use less memory but at the expense of longer computation time
 
         Returns
         -------
@@ -4612,15 +4948,15 @@
             store_tmpf=store_tmpf,
             store_tmpb=store_tmpb,
             store_tmpw=store_tmpw,
             store_tempvar=store_tempvar,
             conf_ints=None,
             mc_sample_size=mc_sample_size,
             da_random_state=da_random_state,
-            remove_mc_set_flag=False,
+            mc_remove_set_flag=False,
             reduce_memory_usage=reduce_memory_usage,
             **kwargs)
 
         time_dim = self.get_time_dim(data_var_key='st')
 
         for label in [store_tmpf, store_tmpb]:
             if ci_avg_time_sel is not None:
@@ -4940,15 +5276,15 @@
                     # Explicitly define output chunks
                     drop_axis=avg_axis_avgx2,  # avg dimensions are dropped
                     new_axis=0,
                     dtype=float)  # The new CI dimension is added as firstax
                 self[store_tmpw + '_mc_avgx2'] = (('CI', time_dim2), q2)
 
         # Clean up the garbage. All arrays with a Monte Carlo dimension.
-        if remove_mc_set_flag:
+        if mc_remove_set_flag:
             remove_mc_set = [
                 'r_st', 'r_ast', 'r_rst', 'r_rast', 'gamma_mc', 'alpha_mc',
                 'df_mc', 'db_mc', 'x_avg', 'time_avg', 'mc']
 
             for i in [store_tmpf, store_tmpb, store_tmpw]:
                 remove_mc_set.append(i + '_avgsec')
                 remove_mc_set.append(i + '_mc_set')
@@ -5253,14 +5589,342 @@
                 c_new = list(c_old)
                 c_new[ixdim] = sum(c_old[ixdim])
                 out = out.rechunk(c_new)
 
         return out
 
 
+class ParameterIndexDoubleEnded:
+    """
+    npar = 1 + 2 * nt + nx + 2 * nt * nta
+    assert pval.size == npar
+    assert p_var.size == npar
+    if calc_cov:
+        assert p_cov.shape == (npar, npar)
+    gamma = pval[0]
+    d_fw = pval[1:nt + 1]
+    d_bw = pval[1 + nt:1 + 2 * nt]
+    alpha = pval[1 + 2 * nt:1 + 2 * nt + nx]
+    # store calibration parameters in DataStore
+    self[store_gamma] = (tuple(), gamma)
+    self[store_alpha] = (('x',), alpha)
+    self[store_df] = ((time_dim,), d_fw)
+    self[store_db] = ((time_dim,), d_bw)
+    if nta > 0:
+        ta = pval[1 + 2 * nt + nx:].reshape((nt, 2, nta), order='F')
+        self[store_ta + '_fw'] = ((time_dim, 'trans_att'), ta[:, 0, :])
+        self[store_ta + '_bw'] = ((time_dim, 'trans_att'), ta[:, 1, :])
+    """
+
+    def __init__(self, nt, nx, nta, fix_gamma=False, fix_alpha=False):
+        self.nt = nt
+        self.nx = nx
+        self.nta = nta
+        self.fix_gamma = fix_gamma
+        self.fix_alpha = fix_alpha
+
+    @property
+    def all(self):
+        return np.concatenate((
+            self.gamma,
+            self.df,
+            self.db,
+            self.alpha,
+            self.ta.flatten(order='F')
+        ))
+
+    @property
+    def npar(self):
+        if not self.fix_gamma and not self.fix_alpha:
+            return 1 + 2 * self.nt + self.nx + 2 * self.nt * self.nta
+        elif self.fix_gamma and not self.fix_alpha:
+            return 2 * self.nt + self.nx + 2 * self.nt * self.nta
+        elif not self.fix_gamma and self.fix_alpha:
+            return 1 + 2 * self.nt + 2 * self.nt * self.nta
+        elif self.fix_gamma and self.fix_alpha:
+            return 2 * self.nt + 2 * self.nt * self.nta
+
+    @property
+    def gamma(self):
+        if self.fix_gamma:
+            return []
+        else:
+            return [0]
+
+    @property
+    def df(self):
+        if self.fix_gamma:
+            return list(range(self.nt))
+        else:
+            return list(range(1, self.nt + 1))
+
+    @property
+    def db(self):
+        if self.fix_gamma:
+            return list(range(self.nt, 2 * self.nt))
+        else:
+            return list(range(1 + self.nt, 1 + 2 * self.nt))
+
+    @property
+    def alpha(self):
+        if self.fix_alpha:
+            return []
+        elif self.fix_gamma:
+            return list(range(2 * self.nt, 1 + 2 * self.nt + self.nx))
+        elif not self.fix_gamma:
+            return list(range(1 + 2 * self.nt, 1 + 2 * self.nt + self.nx))
+
+    @property
+    def ta(self):
+        if self.nta == 0:
+            return np.zeros((self.nt, 2, 0))
+        elif not self.fix_gamma and not self.fix_alpha:
+            arr = np.arange(1 + 2 * self.nt + self.nx, self.npar)
+        elif self.fix_gamma and not self.fix_alpha:
+            arr = np.arange(2 * self.nt + self.nx, self.npar)
+        elif not self.fix_gamma and self.fix_alpha:
+            arr = np.arange(1 + 2 * self.nt, self.npar)
+        elif self.fix_gamma and self.fix_alpha:
+            arr = np.arange(2 * self.nt, self.npar)
+
+        return arr.reshape((self.nt, 2, self.nta), order="F")
+
+    @property
+    def taf(self):
+        """
+        Use `.reshape((nt, nta))` to convert array to (time-dim and transatt-dim). Order is the default C order.
+        ta = pval[1 + 2 * nt + nx:].reshape((nt, 2, nta), order='F')
+        self[store_ta + '_fw'] = ((time_dim, 'trans_att'), ta[:, 0, :])
+        """
+        return self.ta[:, 0, :].flatten(order="C")
+
+    @property
+    def tab(self):
+        """
+        Use `.reshape((nt, nta))` to convert array to (time-dim and transatt-dim). Order is the default C order.
+        ta = pval[1 + 2 * nt + nx:].reshape((nt, 2, nta), order='F')
+        self[store_ta + '_bw'] = ((time_dim, 'trans_att'), ta[:, 1, :])
+        """
+        return self.ta[:, 1, :].flatten(order="C")
+
+    def get_ta_pars(self, pval):
+        if self.nta > 0:
+            if pval.ndim == 1:
+                return np.take_along_axis(pval[None, None], self.ta, axis=-1)
+
+            else:
+                # assume shape is (a, npar) and returns shape (nt, 2, nta, a)
+                assert pval.shape[1] == self.npar and pval.ndim == 2
+                return np.stack([self.get_ta_pars(v) for v in pval], axis=-1)
+
+        else:
+            return np.zeros(shape=(self.nt, 2, 0))
+
+    def get_taf_pars(self, pval):
+        """returns taf parameters of shape (nt, nta) or (nt, nta, a)"""
+        return self.get_ta_pars(pval=pval)[:, 0, :]
+
+    def get_tab_pars(self, pval):
+        """returns taf parameters of shape (nt, nta) or (nt, nta, a)"""
+        return self.get_ta_pars(pval=pval)[:, 1, :]
+
+    def get_taf_values(self, pval, x, trans_att, axis=""):
+        """returns taf parameters of shape (nx, nt)"""
+        pval = np.atleast_2d(pval)
+
+        assert pval.ndim == 2 and pval.shape[1] == self.npar
+
+        arr_out = np.zeros((self.nx, self.nt))
+
+        if self.nta == 0:
+            pass
+
+        elif axis == "":
+            assert pval.shape[0] == 1
+
+            arr = np.transpose(self.get_taf_pars(pval), axes=(1, 2, 0))  # (nta, 1, nt)
+
+            for tai, taxi in zip(arr, trans_att):
+                arr_out[x >= taxi] += tai
+
+        elif axis == "x":
+            assert pval.shape[0] == self.nx
+
+            arr = np.transpose(self.get_taf_pars(pval), axes=(1, 2, 0))  # (nta, nx, nt)
+
+            for tai, taxi in zip(arr, trans_att):
+                # loop over nta, tai has shape (x, t)
+                arr_out[x >= taxi] += tai[x >= taxi]
+
+        elif axis == "time":
+            assert pval.shape[0] == self.nt
+
+            # arr (nt, nta, nt) to have shape (nta, nt, nt)
+            arr = np.transpose(self.get_taf_pars(pval), axes=(1, 2, 0))
+
+            for tai, taxi in zip(arr, trans_att):
+                # loop over nta, tai has shape (t, t)
+                arr_out[x >= taxi] += np.diag(tai)[None]
+
+        return arr_out
+
+    def get_tab_values(self, pval, x, trans_att, axis=""):
+        """returns tab parameters of shape (nx, nt)"""
+        assert pval.shape[-1] == self.npar
+
+        arr_out = np.zeros((self.nx, self.nt))
+
+        if self.nta == 0:
+            pass
+
+        elif axis == "":
+            pval = np.squeeze(pval)
+            assert pval.ndim == 1
+            arr = np.transpose(self.get_tab_pars(pval), axes=(1, 0))
+
+            for tai, taxi in zip(arr, trans_att):
+                arr_out[x < taxi] += tai
+
+        elif axis == "x":
+            assert pval.ndim == 2 and pval.shape[0] == self.nx
+
+            arr = np.transpose(self.get_tab_pars(pval), axes=(1, 2, 0))
+
+            for tai, taxi in zip(arr, trans_att):
+                # loop over nta, tai has shape (x, t)
+                arr_out[x < taxi] += tai[x < taxi]
+
+        elif axis == "time":
+            assert pval.ndim == 2 and pval.shape[0] == self.nt
+
+            # arr (nt, nta, nt) to have shape (nta, nt, nt)
+            arr = np.transpose(self.get_tab_pars(pval), axes=(1, 2, 0))
+
+            for tai, taxi in zip(arr, trans_att):
+                # loop over nta, tai has shape (t, t)
+                arr_out[x < taxi] += np.diag(tai)
+
+        return arr_out
+
+
+class ParameterIndexSingleEnded:
+    """
+    npar = 1 + 1 + nt + nta * nt
+    """
+
+    def __init__(self, nt, nx, nta, fix_alpha=False):
+        self.nt = nt
+        self.nx = nx
+        self.nta = nta
+        self.fix_alpha = fix_alpha
+
+    @property
+    def all(self):
+        return np.concatenate((
+            self.gamma,
+            self.dalpha,
+            self.alpha,
+            self.c,
+            self.ta.flatten(order='F')
+        ))
+
+    @property
+    def npar(self):
+        if not self.fix_alpha:
+            return 1 + 1 + self.nt + self.nta * self.nt
+        else:
+            return 1 + self.nt + self.nta * self.nt
+
+    @property
+    def gamma(self):
+        return [0]
+
+    @property
+    def dalpha(self):
+        if not self.fix_alpha:
+            return [1]
+        else:
+            return []
+
+    @property
+    def alpha(self):
+        if not self.fix_alpha:
+            return []
+        else:
+            return list(range(1, 1 + self.nx))
+
+    @property
+    def c(self):
+        if self.fix_alpha:
+            return list(range(1 + self.nx, 1 + self.nx + self.nt))
+        else:
+            return list(range(1 + 1, 1 + 1 + self.nt))
+
+    @property
+    def taf(self):
+        """returns taf parameters of shape (nt, nta) or (nt, nta, a)"""
+        # ta = p_val[-nt * nta:].reshape((nt, nta), order='F')
+        # self[store_ta] = ((time_dim, 'trans_att'), ta[:, :])
+
+        return np.arange(1 + 1 + self.nt, 1 + 1 + self.nt + self.nt * self.nta).reshape((self.nt, self.nta), order='F')
+
+    def get_taf_pars(self, pval):
+        if self.nta > 0:
+            if pval.ndim == 1:
+                # returns shape (nta, nt)
+                assert len(pval) == self.npar, "Length of pval is incorrect"
+                return np.stack([pval[tafi] for tafi in self.taf.T])
+
+            else:
+                # assume shape is (a, npar) and returns shape (nta, nt, a)
+                assert pval.shape[1] == self.npar and pval.ndim == 2
+                return np.stack([self.get_taf_pars(v) for v in pval], axis=-1)
+
+        else:
+            return np.zeros(shape=(self.nt, 0))
+
+    def get_taf_values(self, pval, x, trans_att, axis=""):
+        """returns taf parameters of shape (nx, nt)"""
+        # assert pval.ndim == 2 and pval.shape[1] == self.npar
+
+        arr_out = np.zeros((self.nx, self.nt))
+
+        if self.nta == 0:
+            pass
+
+        elif axis == "":
+            pval = pval.flatten()
+            assert pval.shape == (self.npar,)
+            arr = self.get_taf_pars(pval)
+            assert arr.shape == (self.nta, self.nt, )
+
+            for tai, taxi in zip(arr, trans_att):
+                arr_out[x >= taxi] += tai
+
+        elif axis == "x":
+            assert pval.shape == (self.nx, self.npar)
+            arr = self.get_taf_pars(pval)
+            assert arr.shape == (self.nta, self.nx, self.nt)
+
+            for tai, taxi in zip(arr, trans_att):
+                # loop over nta, tai has shape (x, t)
+                arr_out[x >= taxi] += tai[x >= taxi]
+
+        elif axis == "time":
+            assert pval.shape == (self.nt, self.npar)
+            arr = self.get_taf_pars(pval)
+            assert arr.shape == (self.nta, self.nt, self.nt)
+
+            for tai, taxi in zip(arr, trans_att):
+                # loop over nta, tai has shape (t, t)
+                arr_out[x >= taxi] += np.diag(tai)[None]
+
+        return arr_out
+
+
 def open_datastore(
         filename_or_obj,
         group=None,
         decode_cf=True,
         mask_and_scale=None,
         decode_times=True,
         concat_characters=True,
```

### Comparing `dtscalibration-1.2.0/src/dtscalibration/datastore_utils.py` & `dtscalibration-2.0.0/src/dtscalibration/datastore_utils.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/src/dtscalibration/io.py` & `dtscalibration-2.0.0/src/dtscalibration/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,35 +7,93 @@
 import dask
 import dask.array as da
 import numpy as np
 import pandas as pd
 
 # Returns a dictionary with the attributes to the dimensions.
 #  The keys refer to the naming used in the raw files.
+# TODO: attrs for st_var and use it in parse_st_var function
 _dim_attrs = {
     ('x', 'distance'):
         dict(
             name='distance',
             description='Length along fiber',
             long_description='Starting at connector of forward channel',
             units='m'),
     ('tmp', 'temperature'):
         dict(
             name='tmp',
             description='Temperature calibrated by device',
-            units='degC'),
+            units=r'$^\circ$C'),
     ('st',): dict(name='st', description='Stokes intensity', units='-'),
     ('ast',): dict(name='ast', description='anti-Stokes intensity', units='-'),
     ('rst',):
         dict(name='rst', description='reverse Stokes intensity', units='-'),
     ('rast',):
         dict(
             name='rast',
             description='reverse anti-Stokes intensity',
             units='-'),
+    ('tmpf',):
+        dict(
+            name='tmpf',
+            description='Temperature estimated using the Stokes and anti-Stokes from the Forward channel',
+            units=r'$^\circ$C'),
+    ('tmpb',):
+        dict(
+            name='tmpb',
+            description='Temperature estimated using the Stokes and anti-Stokes from the Backward channel',
+            units=r'$^\circ$C'),
+    ('tmpw',):
+        dict(
+            name='tmpw',
+            description='Temperature estimated using the Stokes and anti-Stokes from both the Forward and Backward channel.',
+            units=r'$^\circ$C'),
+    ('tmpf_var',):
+        dict(
+            name='tmpf_var',
+            description='Uncertainty variance in tmpf estimated with linear-error propagation',
+            units=r'$^\circ$C$^2$'),
+    ('tmpb_var',):
+        dict(
+            name='tmpb_var',
+            description='Uncertainty variance in tmpb estimated with linear-error propagation',
+            units=r'$^\circ$C$^2$'),
+    ('tmpw_var',):
+        dict(
+            name='tmpw_var',
+            description='Uncertainty variance in tmpw estimated with linear-error propagation',
+            units=r'$^\circ$C$^2$'),
+    ('tmpw_var_lower',):
+        dict(
+            name='tmpw_var_lower',
+            description='Lower bound of uncertainty variance in tmpw estimated with linear-error propagation. '
+                        'Excludes the parameter uncertainties.',
+            units=r'$^\circ$C$^2$'),
+    ('tmpw_var_approx',):
+        dict(
+            name='tmpw_var_upper',
+            description='Upper bound of uncertainty variance in tmpw estimated with linear-error propagation. '
+                        'Excludes the correlation between tmpf and tmpb caused by alpha.',
+            units=r'$^\circ$C$^2$'),
+    ('tmpf_mc_var',):
+        dict(
+            name='tmpf_mc_var',
+            description='Uncertainty variance in tmpf estimated with Monte Carlo',
+            units=r'$^\circ$C$^2$'),
+    ('tmpb_mc_var',):
+        dict(
+            name='tmpb_mc_var',
+            description='Uncertainty variance in tmpb estimated with Monte Carlo',
+            units=r'$^\circ$C$^2$'),
+    ('tmpw_mc_var',):
+        dict(
+            name='tmpw_mc_var',
+            description='Uncertainty variance in tmpw estimated with Monte Carlo',
+            units=r'$^\circ$C$^2$'),
     ('acquisitionTime',):
         dict(
             name='acquisitionTime',
             description='Measurement duration of forward channel',
             long_description='Actual measurement duration of forward '
             'channel',
             units='seconds'),
@@ -959,29 +1017,29 @@
         'tmp': (['x', 'time'], TMP, dim_attrs['tmp']),
         'probe1Temperature':
             (
                 'time', probe1temperature, {
                     'name': 'Probe 1 temperature',
                     'description': 'reference probe 1 '
                                    'temperature',
-                    'units': 'degC'}),
+                    'units': r'$^\circ$C'}),
         'probe2Temperature':
             (
                 'time', probe2temperature, {
                     'name': 'Probe 2 temperature',
                     'description': 'reference probe 2 '
                                    'temperature',
-                    'units': 'degC'}),
+                    'units': r'$^\circ$C'}),
         'referenceTemperature':
             (
                 'time', referenceTemperature, {
                     'name': 'reference temperature',
                     'description': 'Internal reference '
                                    'temperature',
-                    'units': 'degC'}),
+                    'units': r'$^\circ$C'}),
         'gamma_ddf':
             (
                 'time', gamma_ddf, {
                     'name': 'gamma ddf',
                     'description': 'machine '
                                    'calibrated gamma',
                     'units': '-'}),
@@ -1203,15 +1261,15 @@
                     'units': meta_temp['y_units']}),
         'referenceTemperature':
             (
                 'time', referenceTemperature, {
                     'name': 'reference temperature',
                     'description': 'Internal reference '
                                    'temperature',
-                    'units': 'degC'}),
+                    'units': r'$^\circ$C'}),
         'st_zero':
             (
                 ['time'], ST_zero, {
                     'name': 'ST_zero',
                     'description': 'Stokes zero count',
                     'units': meta_dts['y_units']}),
         'ast_zero':
@@ -1819,21 +1877,21 @@
             ('time', index_time_FWend)]
 
     if timezone_input_files is not None:
         coords = {
             k: (
                 'time', pd.DatetimeIndex(v).tz_localize(
                     tz=timezone_input_files).tz_convert(
-                        timezone_netcdf).astype('datetime64[ns]'),
+                        timezone_netcdf).tz_localize(None).astype('datetime64[ns]'),
                 time_attrs[k])
             for k, v in coords_zip}
     else:
         coords = {
             k: (
-                'time', pd.DatetimeIndex(v).tz_convert(timezone_netcdf).astype(
+                'time', pd.DatetimeIndex(v).tz_convert(timezone_netcdf).tz_localize(None).astype(
                     'datetime64[ns]'), time_attrs[k])
             for k, v in coords_zip}
 
     # The units are already stored in the dtype
     coords['acquisitiontimeFW'] = (
         'time', dt1, {
             'description': 'Acquisition time of the forward measurement'})
```

### Comparing `dtscalibration-1.2.0/src/dtscalibration/plot.py` & `dtscalibration-2.0.0/src/dtscalibration/plot.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/test_datastore.py` & `dtscalibration-2.0.0/tests/test_datastore.py`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/test_dtscalibration.py` & `dtscalibration-2.0.0/tests/test_dtscalibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -844,15 +844,15 @@
     test_st_var, _ = ds.variance_stokes_exponential(
         st_label='st', sections=sections)
 
     assert_almost_equal_verbose(test_st_var, yvar, decimal=1)
     pass
 
 
-def test_double_ended_ols_wls_estimate_synthetic():
+def test_double_ended_wls_estimate_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
     from dtscalibration import DataStore
 
@@ -902,44 +902,33 @@
             'time': time},
         attrs={'isDoubleEnded': '1'})
 
     sections = {
         'cold': [slice(0., 0.4 * cable_len)],
         'warm': [slice(0.65 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_double_ended(
-        sections=sections, method='ols', solver='sparse')
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=11)
-    assert_almost_equal_verbose(
-        ds.alpha.values, alpha, decimal=12)  # 13 in 64-bit
-    assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=10)
-    assert_almost_equal_verbose(ds.tmpb.values, temp_real - 273.15, decimal=10)
-    assert_almost_equal_verbose(ds.tmpw.values, temp_real - 273.15, decimal=11)
-
     # WLS
     ds.calibration_double_ended(
         sections=sections,
         st_var=1e-7,
         ast_var=1e-7,
         rst_var=1e-7,
         rast_var=1e-7,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=5)
+        mc_sample_size=5)
 
     assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=10)
     assert_almost_equal_verbose(ds.alpha.values, alpha, decimal=8)
     assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=6)
     assert_almost_equal_verbose(ds.tmpb.values, temp_real - 273.15, decimal=6)
     assert_almost_equal_verbose(ds.tmpw.values, temp_real - 273.15, decimal=6)
 
 
-def test_double_ended_ols_wls_estimate_synthetic_df_and_db_are_different():
+def test_double_ended_wls_estimate_synthetic_df_and_db_are_different():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set. This one has a different D for the forward channel than
     for the backward channel."""
     from dtscalibration import DataStore
@@ -1018,17 +1007,17 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=1000,
+        mc_sample_size=1000,
         fix_gamma=(gamma, 0.),
-        remove_mc_set_flag=True)
+        mc_remove_set_flag=True)
 
     assert_almost_equal_verbose(df, ds.df.values, decimal=14)
     assert_almost_equal_verbose(db, ds.db.values, decimal=13)
     assert_almost_equal_verbose(
         x * (dalpha_p - dalpha_m),
         ds.alpha.values - ds.alpha.values[0],
         decimal=13)
@@ -1037,15 +1026,15 @@
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpb.values, decimal=10)
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpw.values, decimal=10)
     pass
 
 
 def test_reneaming_old_default_labels_to_new_fixed_labels():
     """Same as
-    `test_double_ended_ols_wls_estimate_synthetic_df_and_db_are_different`
+    `test_double_ended_wls_estimate_synthetic_df_and_db_are_different`
     Which runs fast, but using the renaming function."""
     from dtscalibration import DataStore
 
     cable_len = 100.
     nt = 3
     time = np.arange(nt)
     x = np.linspace(0., cable_len, 8)
@@ -1120,17 +1109,17 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=1000,
+        mc_sample_size=1000,
         fix_gamma=(gamma, 0.),
-        remove_mc_set_flag=True)
+        mc_remove_set_flag=True)
 
     assert_almost_equal_verbose(df, ds.df.values, decimal=14)
     assert_almost_equal_verbose(db, ds.db.values, decimal=13)
     assert_almost_equal_verbose(
         x * (dalpha_p - dalpha_m),
         ds.alpha.values - ds.alpha.values[0],
         decimal=13)
@@ -1140,15 +1129,15 @@
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpw.values, decimal=10)
     pass
 
 
 @pytest.mark.xfail
 def test_fail_if_st_labels_are_passed_to_calibration_function():
     """Same as
-    `test_double_ended_ols_wls_estimate_synthetic_df_and_db_are_different`
+    `test_double_ended_wls_estimate_synthetic_df_and_db_are_different`
     Which runs fast."""
     from dtscalibration import DataStore
 
     cable_len = 100.
     nt = 3
     time = np.arange(nt)
     x = np.linspace(0., cable_len, 8)
@@ -1211,17 +1200,17 @@
         rast_label='REV-AST',
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=1000,
+        mc_sample_size=1000,
         fix_gamma=(gamma, 0.),
-        remove_mc_set_flag=True)
+        mc_remove_set_flag=True)
     pass
 
 
 def test_double_ended_asymmetrical_attenuation():
     from dtscalibration import DataStore
 
     cable_len = 100.
@@ -1299,16 +1288,16 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=1000,
-        remove_mc_set_flag=True,
+        mc_sample_size=1000,
+        mc_remove_set_flag=True,
         trans_att=[50.])
 
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpf.values, decimal=7)
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpb.values, decimal=7)
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpw.values, decimal=7)
 
     # test `trans_att` related functions
@@ -1329,16 +1318,16 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=1000,
-        remove_mc_set_flag=True,
+        mc_sample_size=1000,
+        mc_remove_set_flag=True,
         transient_asym_att_x=[50.])
 
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpf.values, decimal=7)
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpb.values, decimal=7)
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpw.values, decimal=7)
     pass
 
@@ -1417,16 +1406,16 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=3,
-        remove_mc_set_flag=True,
+        mc_sample_size=3,
+        mc_remove_set_flag=True,
         trans_att=[50.],
         matching_sections=[
             (
                 slice(x[3 * nx_per_sec], x[4 * nx_per_sec - 1]),
                 slice(x[4 * nx_per_sec], x[5 * nx_per_sec - 1]), True)])
 
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpf.values, decimal=7)
@@ -1523,26 +1512,26 @@
     ds.calibration_double_ended(
         st_var=.5,
         ast_var=.5,
         rst_var=0.1,
         rast_var=0.1,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=3,
-        remove_mc_set_flag=True,
+        mc_sample_size=3,
+        mc_remove_set_flag=True,
         trans_att=[x[3 * nx_per_sec], x[6 * nx_per_sec]],
         matching_sections=ms)
 
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpf.values, decimal=7)
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpb.values, decimal=7)
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpw.values, decimal=7)
     pass
 
 
-def test_double_ended_ols_wls_fix_gamma_estimate_synthetic():
+def test_double_ended_wls_fix_gamma_estimate_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
     from dtscalibration import DataStore
 
@@ -1597,50 +1586,36 @@
             'time': time},
         attrs={'isDoubleEnded': '1'})
 
     sections = {
         'cold': [slice(0., 0.35 * cable_len)],
         'warm': [slice(0.67 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_double_ended(
-        sections=sections,
-        method='ols',
-        solver='sparse',
-        fix_gamma=(gamma, 0.))
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=18)
-    assert_almost_equal_verbose(
-        ds.alpha.values, alpha, decimal=10)  # 11 in 64-bit
-    assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=8)
-    assert_almost_equal_verbose(ds.tmpb.values, temp_real - 273.15, decimal=8)
-    assert_almost_equal_verbose(ds.tmpw.values, temp_real - 273.15, decimal=8)
-
     # WLS
     ds.calibration_double_ended(
         sections=sections,
         st_var=1e-12,
         ast_var=1e-12,
         rst_var=1e-12,
         rast_var=1e-12,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=5,
+        mc_sample_size=5,
         fix_gamma=(gamma, 0.))
 
     assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=18)
     assert_almost_equal_verbose(ds.alpha.values, alpha, decimal=9)
     assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=6)
     assert_almost_equal_verbose(ds.tmpb.values, temp_real - 273.15, decimal=6)
     assert_almost_equal_verbose(ds.tmpw.values, temp_real - 273.15, decimal=6)
 
     pass
 
 
-def test_double_ended_ols_wls_fix_alpha_estimate_synthetic():
+def test_double_ended_wls_fix_alpha_estimate_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
     from dtscalibration import DataStore
 
@@ -1690,52 +1665,36 @@
             'time': time},
         attrs={'isDoubleEnded': '1'})
 
     sections = {
         'cold': [slice(0., 0.4 * cable_len)],
         'warm': [slice(0.78 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_double_ended(
-        sections=sections,
-        method='ols',
-        solver='sparse',
-        fix_alpha=(alpha, np.zeros_like(alpha)))
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=9)
-    assert_almost_equal_verbose(ds.alpha.values, alpha, decimal=18)
-    assert_almost_equal_verbose(
-        ds.tmpf.values, temp_real - 273.15, decimal=8)  # 9 on 64-bit
-    assert_almost_equal_verbose(
-        ds.tmpb.values, temp_real - 273.15, decimal=8)  # 9 on 64-bit
-    assert_almost_equal_verbose(
-        ds.tmpw.values, temp_real - 273.15, decimal=7)  # 11 on 64-bit
-
     # WLS
     ds.calibration_double_ended(
         sections=sections,
         st_var=1e-7,
         ast_var=1e-7,
         rst_var=1e-7,
         rast_var=1e-7,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=5,
+        mc_sample_size=5,
         fix_alpha=(alpha, np.zeros_like(alpha)))
 
     assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=8)
     assert_almost_equal_verbose(ds.alpha.values, alpha, decimal=18)
     assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=7)
     assert_almost_equal_verbose(ds.tmpb.values, temp_real - 273.15, decimal=7)
     assert_almost_equal_verbose(ds.tmpw.values, temp_real - 273.15, decimal=7)
 
     pass
 
 
-def test_double_ended_ols_wls_fix_alpha_fix_gamma_estimate_synthetic():
+def test_double_ended_wls_fix_alpha_fix_gamma_estimate_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
     from dtscalibration import DataStore
 
@@ -1785,38 +1744,24 @@
             'time': time},
         attrs={'isDoubleEnded': '1'})
 
     sections = {
         'cold': [slice(0., 0.5 * cable_len)],
         'warm': [slice(0.5 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_double_ended(
-        sections=sections,
-        method='ols',
-        solver='sparse',
-        fix_gamma=(gamma, 0.),
-        fix_alpha=(alpha, np.zeros_like(alpha)))
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=18)
-    assert_almost_equal_verbose(ds.alpha.values, alpha, decimal=18)
-    assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=9)
-    assert_almost_equal_verbose(ds.tmpb.values, temp_real - 273.15, decimal=9)
-    assert_almost_equal_verbose(ds.tmpw.values, temp_real - 273.15, decimal=9)
-
     # WLS
     ds.calibration_double_ended(
         sections=sections,
         st_var=1e-7,
         ast_var=1e-7,
         rst_var=1e-7,
         rast_var=1e-7,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=5,
+        mc_sample_size=5,
         fix_gamma=(gamma, 0.),
         fix_alpha=(alpha, np.zeros_like(alpha)))
 
     assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=18)
     assert_almost_equal_verbose(ds.alpha.values, alpha, decimal=18)
     assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=11)
     assert_almost_equal_verbose(ds.tmpb.values, temp_real - 273.15, decimal=11)
@@ -1899,41 +1844,40 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=3,
-        remove_mc_set_flag=True,
+        mc_sample_size=3,
+        mc_remove_set_flag=True,
         trans_att=[50.],
         matching_sections=[
             (
                 slice(x[3 * nx_per_sec], x[4 * nx_per_sec - 1]),
                 slice(x[4 * nx_per_sec], x[5 * nx_per_sec - 1]), True)])
 
     # remove TA vars
-    k = [
-        'talpha_fw', 'talpha_bw', 'talpha_fw_var', 'talpha_bw_var',
-        'trans_att']
+    k = ['talpha_fw', 'talpha_bw', 'trans_att']
+
     for ki in k:
         del ds[ki]
 
     alpha_adj = ds.alpha.values.copy()
     alpha_var_adj = ds.alpha_var.values.copy()
 
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=3,
-        remove_mc_set_flag=True,
+        mc_sample_size=3,
+        mc_remove_set_flag=True,
         fix_alpha=(alpha_adj, alpha_var_adj),
         trans_att=[50.],
         matching_sections=[
             (
                 slice(x[3 * nx_per_sec], x[4 * nx_per_sec - 1]),
                 slice(x[4 * nx_per_sec], x[5 * nx_per_sec - 1]), True)])
 
@@ -2017,41 +1961,40 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=3,
-        remove_mc_set_flag=True,
+        mc_sample_size=3,
+        mc_remove_set_flag=True,
         trans_att=[50.],
         matching_sections=[
             (
                 slice(x[3 * nx_per_sec], x[4 * nx_per_sec - 1]),
                 slice(x[4 * nx_per_sec], x[5 * nx_per_sec - 1]), True)])
 
     # remove TA vars
-    k = [
-        'talpha_fw', 'talpha_bw', 'talpha_fw_var', 'talpha_bw_var',
-        'trans_att']
+    k = ['talpha_fw', 'talpha_bw', 'trans_att']
+
     for ki in k:
         del ds[ki]
 
     alpha_adj = ds.alpha.values.copy()
     alpha_var_adj = ds.alpha_var.values.copy()
 
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=3,
-        remove_mc_set_flag=True,
+        mc_sample_size=3,
+        mc_remove_set_flag=True,
         fix_alpha=(alpha_adj, alpha_var_adj),
         fix_gamma=(gamma, 0.),
         trans_att=[50.],
         matching_sections=[
             (
                 slice(x[3 * nx_per_sec], x[4 * nx_per_sec - 1]),
                 slice(x[4 * nx_per_sec], x[5 * nx_per_sec - 1]), True)])
@@ -2136,17 +2079,17 @@
     ds.calibration_double_ended(
         st_var=1.5,
         ast_var=1.5,
         rst_var=1.,
         rast_var=1.,
         method='wls',
         solver='sparse',
-        tmpw_mc_size=3,
+        mc_sample_size=3,
         fix_gamma=(gamma, 0.),
-        remove_mc_set_flag=True,
+        mc_remove_set_flag=True,
         trans_att=[50.],
         matching_sections=[
             (
                 slice(x[3 * nx_per_sec], x[4 * nx_per_sec - 1]),
                 slice(x[4 * nx_per_sec], x[5 * nx_per_sec - 1]), True)])
 
     assert_almost_equal_verbose(temp_real_celsius, ds.tmpf.values, decimal=7)
@@ -2303,17 +2246,17 @@
 
     from dtscalibration import DataStore
 
     state = da.random.RandomState(0)
 
     stokes_m_var = 0.1
     cable_len = 10.
-    nt = 150
+    nt = 1002
     time = np.arange(nt)
-    nmc = 201
+    nmc = 501
     x = np.linspace(0., cable_len, 64)
     ts_cold = np.ones(nt) * 4.
     ts_warm = np.ones(nt) * 20.
 
     C_p = 1524.
     C_m = 2400.
     dalpha_r = 0.0005284
@@ -2350,18 +2293,14 @@
     print('alphaint', cable_len * (dalpha_p - dalpha_m))
     print('alpha', dalpha_p - dalpha_m)
     print('C', np.log(C_p / C_m))
     print('x0', x.max())
 
     ds = DataStore(
         {
-            # 'st':                    (['x', 'time'], st),
-            # 'ast':                   (['x', 'time'], ast),
-            # 'rst':                   (['x', 'time'], rst),
-            # 'rast':                  (['x', 'time'], rast),
             'st': (['x', 'time'], st_m),
             'ast': (['x', 'time'], ast_m),
             'rst': (['x', 'time'], rst_m),
             'rast': (['x', 'time'], rast_m),
             'userAcquisitionTimeFW': (['time'], np.ones(nt)),
             'userAcquisitionTimeBW': (['time'], np.ones(nt)),
             'cold': (['time'], ts_cold),
@@ -2370,92 +2309,85 @@
             'x': x,
             'time': time},
         attrs={'isDoubleEnded': '1'})
 
     sections = {
         'cold': [slice(0., 0.25 * cable_len)],
         'warm': [slice(0.5 * cable_len, 0.75 * cable_len)]}
-
-    # st_label = 'mst'
-    # ast_label = 'mast'
-    # rst_label = 'mrst'
-    # rast_label = 'mrast'
-
     # MC variance
     ds.calibration_double_ended(
         sections=sections,
         st_var=mst_var,
         ast_var=mast_var,
         rst_var=mrst_var,
         rast_var=mrast_var,
         # fix_gamma=(gamma, 0.),
         # fix_alpha=(alpha, 0. * alpha),
         method='wls',
         solver='stats',
-        tmpw_mc_size=nmc)
+        mc_sample_size=nmc)
 
     ds.conf_int_double_ended(
         p_val='p_val',
         p_cov='p_cov',
         st_var=mst_var,
         ast_var=mast_var,
         rst_var=mrst_var,
         rast_var=mrast_var,
         store_tmpf='tmpf',
         store_tmpb='tmpb',
         store_tmpw='tmpw',
         store_tempvar='_var',
-        conf_ints=[20., 80.],
+        # conf_ints=[20., 80.],
         mc_sample_size=nmc,
         da_random_state=state,
-        remove_mc_set_flag=False,
+        mc_remove_set_flag=False,
         reduce_memory_usage=1)
 
     assert_almost_equal_verbose(
         (ds.r_st - ds.st).var(dim=['mc', 'time']), mst_var, decimal=2)
     assert_almost_equal_verbose(
         (ds.r_ast - ds.ast).var(dim=['mc', 'time']), mast_var, decimal=2)
     assert_almost_equal_verbose(
         (ds.r_rst - ds.rst).var(dim=['mc', 'time']), mrst_var, decimal=2)
     assert_almost_equal_verbose(
         (ds.r_rast - ds.rast).var(dim=['mc', 'time']), mrast_var, decimal=3)
 
     assert_almost_equal_verbose(ds.gamma_mc.var(dim='mc'), 0., decimal=2)
     assert_almost_equal_verbose(ds.alpha_mc.var(dim='mc'), 0., decimal=8)
-    assert_almost_equal_verbose(ds.df_mc.var(dim='mc'), ds.df_var, decimal=7)
+    assert_almost_equal_verbose(ds.df_mc.var(dim='mc'), ds.df_var, decimal=8)
     assert_almost_equal_verbose(ds.db_mc.var(dim='mc'), ds.db_var, decimal=8)
 
     # tmpf
     temp_real2 = temp_real[:, 0] - 273.15
-    actual = (
-        np.square(ds.tmpf - temp_real2[:, None]).sum(dim='time')
-        / ds.time.size)
-    desire = ds.tmpf_mc_var.values
+    actual = (ds.tmpf - temp_real2[:, None]).var(dim='time')
+    desire2 = ds.tmpf_var.mean(dim='time')
 
     # Validate on sections that were not used for calibration.
     assert_almost_equal_verbose(
-        actual[16:32].mean(), desire[16:32].mean(), decimal=3)
-    assert_almost_equal_verbose(
-        actual[48:].mean(), desire[48:].mean(), decimal=3)
+        actual[16:32], desire2[16:32], decimal=2)
 
     # tmpb
-    actual = (
-        np.square(ds.tmpb - temp_real2[:, None]).sum(dim='time')
-        / ds.time.size)
-    desire = ds.tmpb_mc_var.values
+    actual = (ds.tmpb - temp_real2[:, None]).var(dim='time')
+    desire2 = ds.tmpb_var.mean(dim='time')
 
     # Validate on sections that were not used for calibration.
     assert_almost_equal_verbose(
-        actual[16:32].mean(), desire[16:32].mean(), decimal=4)
+        actual[16:32], desire2[16:32], decimal=2)
+
+    # tmpw
+    actual = (ds.tmpw - temp_real2[:, None]).var(dim='time')
+    desire2 = ds.tmpw_var.mean(dim='time')
     assert_almost_equal_verbose(
-        actual[48:].mean(), desire[48:].mean(), decimal=4)
+        actual[16:32], desire2[16:32], decimal=3)
+
     pass
 
 
-def test_single_ended_ols_wls_estimate_synthetic():
+def test_single_ended_wls_estimate_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
 
     from dtscalibration import DataStore
@@ -2502,23 +2434,14 @@
             'time': time},
         attrs={'isDoubleEnded': '0'})
 
     sections = {
         'cold': [slice(0., 0.5 * cable_len)],
         'warm': [slice(0.5 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_single_ended(
-        sections=sections, method='ols', solver='sparse')
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=6)
-    assert_almost_equal_verbose(
-        ds.dalpha.values, dalpha_p - dalpha_m, decimal=8)
-    assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=4)
-
     # WLS
     ds.calibration_single_ended(
         sections=sections,
         st_var=1.,
         ast_var=1.,
         method='wls',
         solver='sparse')
@@ -2527,15 +2450,15 @@
     assert_almost_equal_verbose(
         ds.dalpha.values, dalpha_p - dalpha_m, decimal=8)
     assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=4)
 
     pass
 
 
-def test_single_ended_ols_wls_fix_dalpha_synthetic():
+def test_single_ended_wls_fix_dalpha_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
 
     from dtscalibration import DataStore
@@ -2582,26 +2505,14 @@
             'time': time},
         attrs={'isDoubleEnded': '0'})
 
     sections = {
         'cold': [slice(0., 0.5 * cable_len)],
         'warm': [slice(0.5 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_single_ended(
-        sections=sections,
-        method='ols',
-        solver='sparse',
-        fix_dalpha=(dalpha_p - dalpha_m, 0.))
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=11)
-    assert_almost_equal_verbose(
-        ds.dalpha.values, dalpha_p - dalpha_m, decimal=18)
-    assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=12)
-
     # WLS
     ds.calibration_single_ended(
         sections=sections,
         st_var=1.,
         ast_var=1.,
         method='wls',
         solver='sparse',
@@ -2611,15 +2522,15 @@
     assert_almost_equal_verbose(
         ds.dalpha.values, dalpha_p - dalpha_m, decimal=14)
     assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=10)
 
     pass
 
 
-def test_single_ended_ols_wls_fix_gamma_synthetic():
+def test_single_ended_wls_fix_gamma_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
 
     from dtscalibration import DataStore
@@ -2666,26 +2577,14 @@
             'time': time},
         attrs={'isDoubleEnded': '0'})
 
     sections = {
         'cold': [slice(0., 0.5 * cable_len)],
         'warm': [slice(0.5 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_single_ended(
-        sections=sections,
-        method='ols',
-        solver='sparse',
-        fix_gamma=(gamma, 0.))
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=18)
-    assert_almost_equal_verbose(
-        ds.dalpha.values, dalpha_p - dalpha_m, decimal=10)
-    assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=8)
-
     # WLS
     ds.calibration_single_ended(
         sections=sections,
         st_var=1.,
         ast_var=1.,
         method='wls',
         solver='sparse',
@@ -2695,15 +2594,15 @@
     assert_almost_equal_verbose(
         ds.dalpha.values, dalpha_p - dalpha_m, decimal=10)
     assert_almost_equal_verbose(ds.tmpf.values, temp_real - 273.15, decimal=8)
 
     pass
 
 
-def test_single_ended_ols_wls_fix_gamma_fix_dalpha_synthetic():
+def test_single_ended_wls_fix_gamma_fix_dalpha_synthetic():
     """Checks whether the coefficients are correctly defined by creating a
     synthetic measurement set, and derive the parameters from this set.
     Without variance.
     They should be the same as the parameters used to create the synthetic
     measurment set"""
 
     from dtscalibration import DataStore
@@ -2750,28 +2649,14 @@
             'time': time},
         attrs={'isDoubleEnded': '0'})
 
     sections = {
         'cold': [slice(0., 0.5 * cable_len)],
         'warm': [slice(0.5 * cable_len, cable_len)]}
 
-    # OLS
-    ds.calibration_single_ended(
-        sections=sections,
-        method='ols',
-        solver='sparse',
-        fix_gamma=(gamma, 0.),
-        fix_dalpha=(dalpha_p - dalpha_m, 0.))
-
-    assert_almost_equal_verbose(ds.gamma.values, gamma, decimal=18)
-    assert_almost_equal_verbose(
-        ds.dalpha.values, dalpha_p - dalpha_m, decimal=18)
-    assert_almost_equal_verbose(
-        ds.tmpf.values, temp_real - 273.15, decimal=8)  # 11 on 64-bit
-
     # WLS
     ds.calibration_single_ended(
         sections=sections,
         st_var=1.,
         ast_var=1.,
         method='wls',
         solver='sparse',
@@ -2848,47 +2733,30 @@
             [
                 slice(0.125 * cable_len, 0.25 * cable_len),
                 slice(0.65 * cable_len, 0.70 * cable_len)],
         'warm': [slice(0.25 * cable_len, 0.375 * cable_len)]}
 
     ds_test = ds.copy(deep=True)
 
-    # OLS
-    ds_test.calibration_single_ended(
-        sections=sections,
-        method='ols',
-        trans_att=[40, 60],
-        solver='sparse')
-
-    assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=8)
-    assert_almost_equal_verbose(
-        ds_test.tmpf.values, temp_real - 273.15, decimal=8)
-    assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
-    assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
-
-    ds_test = ds.copy(deep=True)
-
     # WLS
     ds_test.calibration_single_ended(
         sections=sections,
         st_var=1.0,
         ast_var=1.0,
         method='wls',
         trans_att=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=8)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
     # test `trans_att` related functions
     # Clear out old results
     ds_test.set_trans_att([])
 
     assert ds_test.trans_att.size == 0, 'clear out trans_att config'
 
@@ -2907,17 +2775,17 @@
         transient_att_x=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=8)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
     ds_test = ds.copy(deep=True)
 
     # Test fixing gamma + transient att.
     ds_test.calibration_single_ended(
         sections=sections,
         st_var=1.0,
@@ -2927,17 +2795,17 @@
         trans_att=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=10)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
     ds_test = ds.copy(deep=True)
 
     # Test fixing alpha + transient att.
     ds_test.calibration_single_ended(
         sections=sections,
         st_var=1.0,
@@ -2947,17 +2815,17 @@
         trans_att=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=8)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
 
 def test_single_ended_matching_sections_synthetic():
     """Checks whether the matching sections routines perform as intended,
     and calibrate to the correct temperature"""
     from dtscalibration import DataStore
 
@@ -3024,49 +2892,31 @@
         (
             slice(.01 * cable_len,
                   .09 * cable_len), slice(.91 * cable_len,
                                           .99 * cable_len), True)]
 
     ds_test = ds.copy(deep=True)
 
-    # OLS
-    ds_test.calibration_single_ended(
-        sections=sections,
-        method='ols',
-        matching_sections=matching_sections,
-        trans_att=[40, 60],
-        solver='sparse')
-
-    assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=8)
-    assert_almost_equal_verbose(
-        ds_test.tmpf.values, temp_real - 273.15, decimal=8)
-    assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
-    assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
-
-    ds_test = ds.copy(deep=True)
-
     # WLS
     ds_test.calibration_single_ended(
         sections=sections,
         st_var=1.0,
         ast_var=1.0,
         method='wls',
         matching_sections=matching_sections,
         trans_att=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=8)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
     ds_test = ds.copy(deep=True)
 
     # Test fixing gamma + transient att.
     ds_test.calibration_single_ended(
         sections=sections,
         st_var=1.0,
@@ -3077,17 +2927,17 @@
         trans_att=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=10)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
     ds_test = ds.copy(deep=True)
 
     # Test fixing dalpha + transient att.
     ds_test.calibration_single_ended(
         sections=sections,
         st_var=1.0,
@@ -3098,17 +2948,17 @@
         trans_att=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=10)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
     ds_test = ds.copy(deep=True)
 
     # Test fixing gamma & dalpha + transient att.
     ds_test.calibration_single_ended(
         sections=sections,
         st_var=1.0,
@@ -3120,33 +2970,33 @@
         trans_att=[40, 60],
         solver='sparse')
 
     assert_almost_equal_verbose(ds_test.gamma.values, gamma, decimal=10)
     assert_almost_equal_verbose(
         ds_test.tmpf.values, temp_real - 273.15, decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=0).talpha, -np.log(tr_att), decimal=8)
+        ds_test.isel(trans_att=0).talpha_fw, -np.log(tr_att), decimal=8)
     assert_almost_equal_verbose(
-        ds_test.isel(trans_att=1).talpha, -np.log(tr_att2), decimal=8)
+        ds_test.isel(trans_att=1).talpha_fw, -np.log(tr_att2), decimal=8)
 
     # Test conf. ints. for the combination of everything
     ds_test.conf_int_single_ended(
         p_val='p_val',
         p_cov='p_cov',
         st_var=1.0,
         ast_var=1.0,
         store_tmpf='tmpf',
         store_tempvar='_var',
         conf_ints=[2.5, 50., 97.5],
         mc_sample_size=50)
 
     ds_test_1 = ds_test.isel(time=-1)
-    ds_test_1.tmpf
-    ds_test_1.tmpf_mc.isel(CI=0).values
-    ds_test_1.tmpf_mc.isel(CI=2).values
+    # ds_test_1.tmpf
+    # ds_test_1.tmpf_mc.isel(CI=0).values
+    # ds_test_1.tmpf_mc.isel(CI=2).values
 
     assert np.all(
         np.less(ds_test_1.tmpf_mc.isel(CI=0).values, ds_test_1.tmpf)
     ), 'Single-ended, trans. att.; 2.5% confidence interval is incorrect'
 
     assert np.all(
         np.greater(ds_test_1.tmpf_mc.isel(CI=2).values, ds_test_1.tmpf)
@@ -3261,40 +3111,14 @@
             print('Real VAR: ', v1i, 'Estimated VAR: ', v2i_c)
             assert_almost_equal_verbose(v1i, v2i_c, decimal=1)
 
     pass
     print('hoi')
 
 
-def test_calibration_ols():
-    """Testing ordinary least squares procedure. And compare with device calibrated temperature.
-    The measurements were calibrated by the device using only section 8--17.m. Those temperatures
-    are compared up to 2 decimals. Silixa only uses a single calibration constant (I think they
-    fix gamma), or a different formulation, see Shell primer.
-    """
-    filepath = data_dir_double_ended2
-    ds = read_silixa_files(
-        directory=filepath, timezone_netcdf='UTC', file_ext='*.xml')
-    ds100 = ds.sel(x=slice(0, 100))
-    sections_ultima = {
-        'probe1Temperature': [slice(8., 17.)],  # cold bath
-    }
-
-    ds100.calibration_double_ended(
-        sections=sections_ultima, store_tmpw='tmpw', method='ols')
-
-    np.testing.assert_array_almost_equal(
-        ds100['tmpw'].data, ds100.tmp.data, decimal=1)
-
-    ds009 = ds100.sel(x=sections_ultima['probe1Temperature'][0])
-    np.testing.assert_array_almost_equal(
-        ds009['tmpw'].data, ds009.tmp.data, decimal=2)
-    pass
-
-
 def test_calibrate_wls_procedures():
     x = np.linspace(0, 10, 25 * 4)
     np.random.shuffle(x)
 
     X = x.reshape((25, 4))
     beta = np.array([1, 0.1, 10, 5])
     beta_w = np.concatenate((np.ones(10), np.ones(15) * 1.0))
```

### Comparing `dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml` & `dtscalibration-2.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118201727.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml` & `dtscalibration-2.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118202957.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml` & `dtscalibration-2.0.0/tests/data/ap_sensing/_AP Sensing_N4386B_3_20180118205357.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112245510.xml` & `dtscalibration-2.0.0/tests/data/double_ended/channel 1_20170921112245510.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921112746818.xml` & `dtscalibration-2.0.0/tests/data/double_ended/channel 1_20170921112746818.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended/channel 1_20170921113248085.xml` & `dtscalibration-2.0.0/tests/data/double_ended/channel 1_20170921113248085.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014052498.xml` & `dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014052498.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014057119.xml` & `dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014057119.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014101652.xml` & `dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014101652.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014106243.xml` & `dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014106243.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014110917.xml` & `dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014110917.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_ended2/channel 1_20180328014115480.xml` & `dtscalibration-2.0.0/tests/data/double_ended2/channel 1_20180328014115480.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052744117.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052816397.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052848681.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052921002.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028052953332.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_1/channel 1_20181028053025647.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052805425.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052837699.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052910030.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028052942339.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053014664.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml` & `dtscalibration-2.0.0/tests/data/double_single_ended/channel_2/channel 2_20181028053046978.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv` & `dtscalibration-2.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 00h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv` & `dtscalibration-2.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 01h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv` & `dtscalibration-2.0.0/tests/data/external_temperature_timeseries/Loodswaternet2018-03-28 02h.csv`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00003.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00004.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_halo_v1.0/channel 1 20030111 002 00005.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202119 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202149 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202219 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202249 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202319 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202349 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7/channel 1 20180107 202418 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 183346 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 184846 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 190347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 191847 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_oryx_v3.7_double/channel 1 20200306 193347 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00001.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf` & `dtscalibration-2.0.0/tests/data/sensornet_sentinel_v5.1_double/channel 7 20180101 001 00002.ddf`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat` & `dtscalibration-2.0.0/tests/data/sensortran_binary/15_56_47_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat` & `dtscalibration-2.0.0/tests/data/sensortran_binary/15_56_47_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat` & `dtscalibration-2.0.0/tests/data/sensortran_binary/16_11_31_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat` & `dtscalibration-2.0.0/tests/data/sensortran_binary/16_11_31_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat` & `dtscalibration-2.0.0/tests/data/sensortran_binary/16_29_23_BinaryRawDTS.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat` & `dtscalibration-2.0.0/tests/data/sensortran_binary/16_29_23_BinaryTemp.dat`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml` & `dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060301031.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml` & `dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060342281.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml` & `dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060423515.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml` & `dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060504750.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml` & `dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060545968.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml` & `dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060627218.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml` & `dtscalibration-2.0.0/tests/data/silixa_v4.5/channel 3_20151002060708453.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml` & `dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145850.340.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml` & `dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145852.599.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml` & `dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145854.889.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml` & `dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145857.188.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml` & `dtscalibration-2.0.0/tests/data/silixa_v7.0/channel 2_UTC_20191010_145859.477.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml` & `dtscalibration-2.0.0/tests/data/silixa_v8.1/channel.1_UTC_20220824_125501.866.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132202074.xml` & `dtscalibration-2.0.0/tests/data/single_ended/channel 2_20180504132202074.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132232903.xml` & `dtscalibration-2.0.0/tests/data/single_ended/channel 2_20180504132232903.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/single_ended/channel 2_20180504132303723.xml` & `dtscalibration-2.0.0/tests/data/single_ended/channel 2_20180504132303723.xml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/zipped data/double_ended.zip` & `dtscalibration-2.0.0/tests/data/zipped data/double_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/zipped data/double_ended2.zip` & `dtscalibration-2.0.0/tests/data/zipped data/double_ended2.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/zipped data/double_single_ended.zip` & `dtscalibration-2.0.0/tests/data/zipped data/double_single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/zipped data/silixa_v4.5.zip` & `dtscalibration-2.0.0/tests/data/zipped data/silixa_v4.5.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/tests/data/zipped data/single_ended.zip` & `dtscalibration-2.0.0/tests/data/zipped data/single_ended.zip`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/.gitignore` & `dtscalibration-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/LICENSE` & `dtscalibration-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/README.rst` & `dtscalibration-2.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,30 @@
       - |docs|
     * - Tests
       - |tests|
     * - Package
       - | |version| |supported-versions| |commits-since|
     * - Citable
       - |zenodo|
+    * - Example notebooks
+      - |example-notebooks|
 
 .. |docs| image:: https://readthedocs.org/projects/python-dts-calibration/badge/?style=flat
     :target: https://python-dts-calibration.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 .. |tests| image:: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml/badge.svg
     :target: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml
     :alt: Test Status
 
 .. |version| image:: https://img.shields.io/pypi/v/dtscalibration.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/dtscalibration
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v1.2.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v2.0.0.svg
     :alt: Commits since latest release
     :target: https://github.com/dtscalibration/python-dts-calibration/compare/v1.1.1...main
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/dtscalibration.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/dtscalibration
 
@@ -39,14 +41,18 @@
     :alt: Supported versions
     :target: https://pypi.python.org/pypi/dtscalibration
 
 .. |zenodo| image:: https://zenodo.org/badge/143077491.svg
    :alt: It would be greatly appreciated if you could cite this package in eg articles presentations
    :target: https://zenodo.org/badge/latestdoi/143077491
 
+.. |example-notebooks| image:: https://mybinder.org/badge.svg
+   :alt: Interactively run the example notebooks online
+   :target: https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?labpath=docs%2Fnotebooks
+
 .. end-badges
 
 A Python package to load Distributed Temperature Sensing files, perform a calibration, and plot the result. A detailed description of the calibration procedure can be found at https://doi.org/10.3390/s20082235 .
 
 * Free software: BSD 3-Clause License
 
 
@@ -83,17 +89,16 @@
 * Sensornet Ltd.: **Oryx**, **Halo** & **Sentinel** .ddf files
 * AP Sensing: **CP320** .xml files *(single ended only)*
 * SensorTran: **SensorTran 5100** .dat binary files *(single ended only)*
 
 Documentation
 =============
 
-https://python-dts-calibration.readthedocs.io/
-Example notebooks can be viewed [here](https://python-dts-calibration.readthedocs.io/en/latest/learn_by_examples.html).
-
+* Documentation at https://python-dts-calibration.readthedocs.io/ .
+* Example notebooks that work within the browser can be viewed `here <https://python-dts-calibration.readthedocs.io/en/latest/learn_by_examples.html>`_.
 
 How to cite
 ===========
 The following article explains and discusses the calibration procedure:
 
     des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation of Temperature and Associated Uncertainty from Fiber-Optic Raman-Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235. https://doi.org/10.3390/s20082235
```

### Comparing `dtscalibration-1.2.0/pyproject.toml` & `dtscalibration-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dtscalibration-1.2.0/PKG-INFO` & `dtscalibration-2.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtscalibration
-Version: 1.2.0
+Version: 2.0.0
 Summary: A Python package to load raw DTS files, perform a calibration, and plot the result.
 Author: Bas des Tombe, Bart Schilperoort
 Author-email: bdestombe@gmail.com
 Maintainer-email: Bas des Tombe <bdestombe@gmail.com>, Bart Schilperoort <b.schilperoort@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: AUTHORS.rst
 License-File: LICENSE
@@ -69,28 +69,30 @@
       - |docs|
     * - Tests
       - |tests|
     * - Package
       - | |version| |supported-versions| |commits-since|
     * - Citable
       - |zenodo|
+    * - Example notebooks
+      - |example-notebooks|
 
 .. |docs| image:: https://readthedocs.org/projects/python-dts-calibration/badge/?style=flat
     :target: https://python-dts-calibration.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 .. |tests| image:: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml/badge.svg
     :target: https://github.com/dtscalibration/python-dts-calibration/actions/workflows/build.yml
     :alt: Test Status
 
 .. |version| image:: https://img.shields.io/pypi/v/dtscalibration.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/dtscalibration
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v1.2.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/dtscalibration/python-dts-calibration/v2.0.0.svg
     :alt: Commits since latest release
     :target: https://github.com/dtscalibration/python-dts-calibration/compare/v1.1.1...main
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/dtscalibration.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/dtscalibration
 
@@ -98,14 +100,18 @@
     :alt: Supported versions
     :target: https://pypi.python.org/pypi/dtscalibration
 
 .. |zenodo| image:: https://zenodo.org/badge/143077491.svg
    :alt: It would be greatly appreciated if you could cite this package in eg articles presentations
    :target: https://zenodo.org/badge/latestdoi/143077491
 
+.. |example-notebooks| image:: https://mybinder.org/badge.svg
+   :alt: Interactively run the example notebooks online
+   :target: https://mybinder.org/v2/gh/dtscalibration/python-dts-calibration/main?labpath=docs%2Fnotebooks
+
 .. end-badges
 
 A Python package to load Distributed Temperature Sensing files, perform a calibration, and plot the result. A detailed description of the calibration procedure can be found at https://doi.org/10.3390/s20082235 .
 
 * Free software: BSD 3-Clause License
 
 
@@ -142,17 +148,16 @@
 * Sensornet Ltd.: **Oryx**, **Halo** & **Sentinel** .ddf files
 * AP Sensing: **CP320** .xml files *(single ended only)*
 * SensorTran: **SensorTran 5100** .dat binary files *(single ended only)*
 
 Documentation
 =============
 
-https://python-dts-calibration.readthedocs.io/
-Example notebooks can be viewed [here](https://python-dts-calibration.readthedocs.io/en/latest/learn_by_examples.html).
-
+* Documentation at https://python-dts-calibration.readthedocs.io/ .
+* Example notebooks that work within the browser can be viewed `here <https://python-dts-calibration.readthedocs.io/en/latest/learn_by_examples.html>`_.
 
 How to cite
 ===========
 The following article explains and discusses the calibration procedure:
 
     des Tombe, B., Schilperoort, B., & Bakker, M. (2020). Estimation of Temperature and Associated Uncertainty from Fiber-Optic Raman-Spectrum Distributed Temperature Sensing. Sensors, 20(8), 2235. https://doi.org/10.3390/s20082235
```

