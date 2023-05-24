# Comparing `tmp/obsinfo-0.111.1.post5.tar.gz` & `tmp/obsinfo-0.111b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsinfo-0.111.1.post5.tar", last modified: Thu Apr 27 08:51:46 2023, max compression
+gzip compressed data, was "obsinfo-0.111b1.tar", last modified: Wed Apr 12 06:31:11 2023, max compression
```

## Comparing `obsinfo-0.111.1.post5.tar` & `obsinfo-0.111b1.tar`

### file list

```diff
@@ -1,312 +1,301 @@
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.943015 obsinfo-0.111.1.post5/
--rw-r--r--   0 crawford   (501) admin       (80)    35148 2021-10-18 08:41:35.000000 obsinfo-0.111.1.post5/LICENSE.txt
--rw-r--r--   0 crawford   (501) admin       (80)       96 2023-04-27 08:49:46.000000 obsinfo-0.111.1.post5/MANIFEST.in
--rw-r--r--   0 crawford   (501) admin       (80)     1925 2023-04-27 08:51:46.943189 obsinfo-0.111.1.post5/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)     1032 2021-10-18 08:41:35.000000 obsinfo-0.111.1.post5/README.rst
--rw-r--r--   0 crawford   (501) admin       (80)       85 2023-04-27 08:19:27.000000 obsinfo-0.111.1.post5/pyproject.toml
--rw-r--r--   0 crawford   (501) admin       (80)       63 2023-04-27 08:51:46.943775 obsinfo-0.111.1.post5/setup.cfg
--rw-r--r--   0 crawford   (501) admin       (80)     2224 2023-04-27 08:49:51.000000 obsinfo-0.111.1.post5/setup.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.825720 obsinfo-0.111.1.post5/src/
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.836312 obsinfo-0.111.1.post5/src/obsinfo/
--rw-r--r--   0 crawford   (501) admin       (80)       17 2023-04-26 18:08:49.000000 obsinfo-0.111.1.post5/src/obsinfo/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.838835 obsinfo-0.111.1.post5/src/obsinfo/_examples/
--rw-r--r--   0 crawford   (501) admin       (80)    10244 2023-02-06 14:21:22.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/.DS_Store
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.839932 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/
--rw-r--r--   0 crawford   (501) admin       (80)    12292 2023-04-14 15:43:34.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      831 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/README.rst
--rw-r--r--   0 crawford   (501) admin       (80)       90 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/README.txt
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.840299 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/datacites/
--rw-r--r--   0 crawford   (501) admin       (80)     1731 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.841066 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/
--rw-r--r--   0 crawford   (501) admin       (80)     1763 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     5880 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.845591 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 18:40:52.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      618 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      605 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      556 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      592 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      596 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      436 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR1.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      435 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR2.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      443 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR3_LINEAR.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      443 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR4_LINEAR.stage_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.848054 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/
--rw-r--r--   0 crawford   (501) admin       (80)      480 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR2.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2412 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      283 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR1.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      268 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR2.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      578 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1118 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.848869 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/experiments/
--rw-r--r--   0 crawford   (501) admin       (80)    16208 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml
--rw-r--r--   0 crawford   (501) admin       (80)    19366 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.850502 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation/
--rw-r--r--   0 crawford   (501) admin       (80)     1882 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation/GURALP_CP.instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1882 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation/GURALP_CP.instrumentation.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)     1095 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation/HYDROCT1.instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1095 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation/HYDROCT1.instrumentation.yaml.orig
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.854947 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:33:43.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)     3519 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/BBOBS1_2012+.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2191 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/BBOBS1_pre2012.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     4527 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/GURALP_CP.instrumentation_base.yaml_error
--rw-r--r--   0 crawford   (501) admin       (80)     1084 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/HYDROCT1.instrumentation_base.yaml_error
--rw-r--r--   0 crawford   (501) admin       (80)     1186 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS1.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1454 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS2.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1734 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1556 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/WBOBS1.instrumentation_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1885 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/empty.instrumentation_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.855814 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/location_bases/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/location_bases/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)     1357 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.856709 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/networks/
--rw-r--r--   0 crawford   (501) admin       (80)      329 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/networks/EMSO-AZORES.network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      413 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/networks/RHUM-RUM.network.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.857548 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/operators/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-11-30 17:19:05.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/operators/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      345 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/operators/INSU-IPGP.operator.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.859254 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/persons/
--rw-r--r--   0 crawford   (501) admin       (80)      159 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/persons/Kevin_Canjamale.person.yaml
--rw-r--r--   0 crawford   (501) admin       (80)       98 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/persons/Romuald_Daniel.person.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      100 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/persons/Simon_Besancon.person.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      166 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/persons/Wayne_Crawford.person.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.861992 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/
--rw-r--r--   0 crawford   (501) admin       (80)      707 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      448 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      939 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      869 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1740 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1740 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      869 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.866255 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/
--rw-r--r--   0 crawford   (501) admin       (80)      451 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      392 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x16_theoretical.stage.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      392 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x16_theoretical.stage.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      392 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x32_theoretical.stage.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      392 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x32_theoretical.stage.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      392 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x64_theoretical.stage.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      392 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x64_theoretical.stage.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      663 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      698 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      821 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.871578 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/
--rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      710 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/BUBBLEPHONE_HTI90U.sensor.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      556 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/GURALP_CMG3T_ESPC.sensor.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      661 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      752 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      826 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI96-MIN.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2517 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1425 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      869 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      652 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      698 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2009 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.877645 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/
--rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      381 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/BUBBLEPHONE_HTI90U_SIO-preamp_theoretical.stage.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      381 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/BUBBLEPHONE_HTI90U_SIO-preamp_theoretical.stage.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      353 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Guralp_CMG3T_ESPC_theoretical.stage.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      353 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Guralp_CMG3T_ESPC_theoretical.stage.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      430 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1341 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      387 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-96-Min_voltage-mode_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      539 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      530 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      382 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_generic_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      485 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L22D_LCHEAPO_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      537 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1233 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      586 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.883516 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-04-21 07:40:46.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      342 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Guralp_CMG3T_ESPC_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      329 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Guralp_CMG3T_ESPC_generic.filter.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      280 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      236 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-96-Min_voltage-mode_theoretical.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      230 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-96-Min_voltage-mode_theoretical.filter.yaml.orig
--rw-r--r--   0 crawford   (501) admin       (80)      310 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5004_2007.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      306 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5017_2007.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      364 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      383 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L22D_C510-S2000_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      236 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L28LB-obs_C395-S2490_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      728 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      873 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      547 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.888350 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-04-11 10:41:26.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)        5 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/.obsinfo
--rw-r--r--   0 crawford   (501) admin       (80)     3521 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3372 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2808 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2769 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2173 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1857 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3131 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3102 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2709 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2027 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.889114 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/timing_bases/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/timing_bases/.DS_Store
--rw-r--r--   0 crawford   (501) admin       (80)      252 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/timing_bases/Seascan_GNSS.timing_base.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.829006 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.891765 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/
--rw-r--r--   0 crawford   (501) admin       (80)     1308 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3185 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1501 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1625 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      573 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/CS5322.stage.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1047 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/T240.stage.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.893437 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/
--rw-r--r--   0 crawford   (501) admin       (80)     3049 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     3053 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      907 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/preamplifier.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/sensor.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.896895 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/
--rw-r--r--   0 crawford   (501) admin       (80)      263 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/AD_Conversion.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      673 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      607 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      409 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/HiTechPZ.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      416 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/HiTech_PolesZeros.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      191 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/analog.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      390 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/coefficients.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      310 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/digital.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      379 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/response_list.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2175 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/network.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.898717 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/
--rw-r--r--   0 crawford   (501) admin       (80)      292 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/README.rst
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.899527 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/add_ons/
--rw-r--r--   0 crawford   (501) admin       (80)      331 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/add_ons/README.rst
--rw-r--r--   0 crawford   (501) admin       (80)      952 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)      376 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/make_stationXML.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)      420 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/print_info_files.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)     1646 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/validate_all.sh
--rwxr-xr-x   0 crawford   (501) admin       (80)      315 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/validate_files.sh
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.901776 obsinfo-0.111.1.post5/src/obsinfo/addons/
--rw-r--r--   0 crawford   (501) admin       (80)    11113 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/addons/LC2SDS.py
--rw-r--r--   0 crawford   (501) admin       (80)    10887 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/addons/LCHEAPO.py
--rw-r--r--   0 crawford   (501) admin       (80)     9134 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/addons/OCA.py
--rw-r--r--   0 crawford   (501) admin       (80)    15899 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/addons/SDPCHAIN.py
--rw-r--r--   0 crawford   (501) admin       (80)       64 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/addons/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     2481 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/addons/infodump.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.905019 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/
--rw-r--r--   0 crawford   (501) admin       (80)      104 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/__init__.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    62825 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/_test.py
--rw-r--r--   0 crawford   (501) admin       (80)     7112 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/makeStationXML.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     7821 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/print.py
--rw-r--r--   0 crawford   (501) admin       (80)      289 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/print_version.py
--rw-r--r--   0 crawford   (501) admin       (80)     8214 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/setup.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    13974 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/console_scripts/validate.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.829954 obsinfo-0.111.1.post5/src/obsinfo/data/
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.911677 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/
--rw-r--r--   0 crawford   (501) admin       (80)     8861 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/datacite.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     5514 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/datalogger_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)    10023 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/definitions.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/experiment.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)    13582 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/filter.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     8689 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/instrumentation_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1378 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/iris_units.json
--rw-r--r--   0 crawford   (501) admin       (80)     6575 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/location_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1922 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/network.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1407 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/operator.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     1735 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/person.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     4650 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/preamplifier_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     6472 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/sensor_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     8257 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/stage_base.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     2051 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/stages.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     7216 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/subnetwork.schema.json
--rw-r--r--   0 crawford   (501) admin       (80)     3997 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/data/schemas/timing_base.schema.json
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.912074 obsinfo-0.111.1.post5/src/obsinfo/datacite/
--rw-r--r--   0 crawford   (501) admin       (80)        0 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/datacite/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.916863 obsinfo-0.111.1.post5/src/obsinfo/helpers/
--rw-r--r--   0 crawford   (501) admin       (80)      871 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     3091 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/comments.py
--rw-r--r--   0 crawford   (501) admin       (80)     1552 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/external_references.py
--rw-r--r--   0 crawford   (501) admin       (80)     3089 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/float_with_uncert.py
--rw-r--r--   0 crawford   (501) admin       (80)     1690 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/functions.py
--rw-r--r--   0 crawford   (501) admin       (80)     1493 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/identifiers.py
--rw-r--r--   0 crawford   (501) admin       (80)     6455 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/location.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     3336 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/logger.py
--rw-r--r--   0 crawford   (501) admin       (80)     2675 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/obsinfo_class_list.py
--rw-r--r--   0 crawford   (501) admin       (80)     3169 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/oi_date.py
--rw-r--r--   0 crawford   (501) admin       (80)     2621 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/person.py
--rw-r--r--   0 crawford   (501) admin       (80)     7685 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/helpers/phone.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.920436 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/
--rw-r--r--   0 crawford   (501) admin       (80)      830 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    11540 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/channel.py
--rw-r--r--   0 crawford   (501) admin       (80)     4950 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/equipment.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.924845 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/
--rw-r--r--   0 crawford   (501) admin       (80)     1806 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/AD_conversion.py
--rw-r--r--   0 crawford   (501) admin       (80)     2843 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/FIR.py
--rw-r--r--   0 crawford   (501) admin       (80)      506 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     1511 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/analog.py
--rw-r--r--   0 crawford   (501) admin       (80)     2309 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/coefficients.py
--rw-r--r--   0 crawford   (501) admin       (80)     1212 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/digital.py
--rw-r--r--   0 crawford   (501) admin       (80)     3202 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/filter.py
--rw-r--r--   0 crawford   (501) admin       (80)     1612 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/filter_template.py
--rw-r--r--   0 crawford   (501) admin       (80)     4963 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/poles_zeros.py
--rw-r--r--   0 crawford   (501) admin       (80)     2398 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/polynomial.py
--rw-r--r--   0 crawford   (501) admin       (80)     1588 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/response_list.py
--rw-r--r--   0 crawford   (501) admin       (80)    12127 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/instrument.py
--rw-r--r--   0 crawford   (501) admin       (80)    10005 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/instrument_component.py
--rw-r--r--   0 crawford   (501) admin       (80)    10115 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/instrumentation.py
--rw-r--r--   0 crawford   (501) admin       (80)     5482 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/orientation.py
--rw-r--r--   0 crawford   (501) admin       (80)    17385 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/stage.py
--rw-r--r--   0 crawford   (501) admin       (80)     2959 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/instrumentation/stages.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.928039 obsinfo-0.111.1.post5/src/obsinfo/misc/
--rw-r--r--   0 crawford   (501) admin       (80)        0 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/misc/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     2497 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/misc/configuration.py
--rw-r--r--   0 crawford   (501) admin       (80)      866 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/misc/const.py
--rw-r--r--   0 crawford   (501) admin       (80)     4660 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/misc/discoveryfiles.py
--rw-r--r--   0 crawford   (501) admin       (80)     3062 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/misc/printobs.py
--rw-r--r--   0 crawford   (501) admin       (80)     4026 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/misc/remoteGitLab.py
--rw-r--r--   0 crawford   (501) admin       (80)    28035 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/misc/yamlref.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.928875 obsinfo-0.111.1.post5/src/obsinfo/obsmetadata/
--rw-r--r--   0 crawford   (501) admin       (80)       36 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/obsmetadata/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)    25468 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/obsmetadata/obsmetadata.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.931582 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/
--rw-r--r--   0 crawford   (501) admin       (80)      438 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/__init__.py
--rw-r--r--   0 crawford   (501) admin       (80)     3090 2023-04-26 21:31:44.000000 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/network.py
--rw-r--r--   0 crawford   (501) admin       (80)     2147 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/operator.py
--rw-r--r--   0 crawford   (501) admin       (80)     2094 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/processing.py
--rw-r--r--   0 crawford   (501) admin       (80)      654 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/site.py
--rw-r--r--   0 crawford   (501) admin       (80)    10459 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/station.py
--rw-r--r--   0 crawford   (501) admin       (80)     4727 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/subnetwork/subnetwork.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.933483 obsinfo-0.111.1.post5/src/obsinfo/templates/
--rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/.DS_Store
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.934669 obsinfo-0.111.1.post5/src/obsinfo/templates/components/
--rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/components/datalogger.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      907 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/components/preamplifier.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/components/sensor.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.938028 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/
--rw-r--r--   0 crawford   (501) admin       (80)      263 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/AD_Conversion.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      435 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/FIR.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      561 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/PolesZeros.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      191 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/analog.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      390 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/coefficients.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      310 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/digital.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)      379 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/filters/response_list.filter.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1327 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/instrumentation.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     2176 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/network.yaml
--rw-r--r--   0 crawford   (501) admin       (80)     1055 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/templates/stage.yaml
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.941782 obsinfo-0.111.1.post5/src/obsinfo/tests/
--rw-r--r--   0 crawford   (501) admin       (80)     2880 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/CompareXMLTree.py
--rw-r--r--   0 crawford   (501) admin       (80)       17 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/__init__.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.942661 obsinfo-0.111.1.post5/src/obsinfo/tests/_old/
--rw-r--r--   0 crawford   (501) admin       (80)     5743 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/_old/testlog.py
--rw-r--r--   0 crawford   (501) admin       (80)     4295 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/_old/testmain.py
--rw-r--r--   0 crawford   (501) admin       (80)     1159 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/remoteGithub.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    73575 2023-04-26 20:47:39.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/run_test_script.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    35088 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/test_datapath.py
--rwxr-xr-x   0 crawford   (501) admin       (80)    53975 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/test_infofile.py
--rwxr-xr-x   0 crawford   (501) admin       (80)     2148 2023-04-26 20:38:49.000000 obsinfo-0.111.1.post5/src/obsinfo/tests/test_main.py
--rw-r--r--   0 crawford   (501) admin       (80)       30 2023-04-27 08:43:48.000000 obsinfo-0.111.1.post5/src/obsinfo/version.py
-drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-27 08:51:46.838441 obsinfo-0.111.1.post5/src/obsinfo.egg-info/
--rw-r--r--   0 crawford   (501) admin       (80)     1925 2023-04-27 08:51:46.000000 obsinfo-0.111.1.post5/src/obsinfo.egg-info/PKG-INFO
--rw-r--r--   0 crawford   (501) admin       (80)    17328 2023-04-27 08:51:46.000000 obsinfo-0.111.1.post5/src/obsinfo.egg-info/SOURCES.txt
--rw-r--r--   0 crawford   (501) admin       (80)        1 2023-04-27 08:51:46.000000 obsinfo-0.111.1.post5/src/obsinfo.egg-info/dependency_links.txt
--rw-r--r--   0 crawford   (501) admin       (80)      586 2023-04-27 08:51:46.000000 obsinfo-0.111.1.post5/src/obsinfo.egg-info/entry_points.txt
--rw-r--r--   0 crawford   (501) admin       (80)       85 2023-04-27 08:51:46.000000 obsinfo-0.111.1.post5/src/obsinfo.egg-info/requires.txt
--rw-r--r--   0 crawford   (501) admin       (80)        8 2023-04-27 08:51:46.000000 obsinfo-0.111.1.post5/src/obsinfo.egg-info/top_level.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.575257 obsinfo-0.111b1/
+-rw-r--r--   0 crawford   (501) admin       (80)    35148 2021-10-18 08:41:35.000000 obsinfo-0.111b1/LICENSE.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      140 2021-10-18 08:41:35.000000 obsinfo-0.111b1/MANIFEST.in
+-rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:31:11.575447 obsinfo-0.111b1/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)     1032 2021-10-18 08:41:35.000000 obsinfo-0.111b1/README.rst
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.481113 obsinfo-0.111b1/obsinfo/
+-rw-r--r--   0 crawford   (501) admin       (80)       17 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.483686 obsinfo-0.111b1/obsinfo/_examples/
+-rw-r--r--   0 crawford   (501) admin       (80)    10244 2023-02-06 14:21:22.000000 obsinfo-0.111b1/obsinfo/_examples/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.484720 obsinfo-0.111b1/obsinfo/_examples/Information_Files/
+-rw-r--r--   0 crawford   (501) admin       (80)    12292 2023-04-10 11:11:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      828 2023-02-06 14:15:15.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.rst
+-rw-r--r--   0 crawford   (501) admin       (80)       90 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.txt
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.485116 obsinfo-0.111b1/obsinfo/_examples/Information_Files/campaigns/
+-rw-r--r--   0 crawford   (501) admin       (80)     2053 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/campaigns/SPOBS.campaign.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.485576 obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/
+-rw-r--r--   0 crawford   (501) admin       (80)     1731 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.486341 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/
+-rw-r--r--   0 crawford   (501) admin       (80)     1763 2023-03-22 08:38:06.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     5880 2023-03-22 08:38:32.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.490625 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 18:40:52.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 18:33:44.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      618 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      605 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      556 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      592 2023-02-28 16:43:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      596 2023-02-28 16:43:14.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      436 2023-02-28 16:43:36.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR1.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      435 2023-02-28 16:43:35.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR2.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:29.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR3_LINEAR.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      443 2023-02-28 16:43:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR4_LINEAR.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.492895 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      480 2023-02-28 16:44:38.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR2.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2412 2023-02-28 16:44:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      283 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR1.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      268 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR2.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      578 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1118 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.493597 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/
+-rw-r--r--   0 crawford   (501) admin       (80)    16208 2023-03-01 16:50:51.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)    19366 2023-04-10 16:23:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.497398 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:33:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)     3594 2023-04-12 06:20:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2189 2023-04-11 21:33:49.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     4527 2023-03-22 08:38:31.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1084 2023-03-07 15:14:40.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-07 15:14:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS1.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1451 2023-03-07 15:15:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1732 2023-03-07 15:20:23.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1554 2023-03-07 15:20:21.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1885 2023-03-07 15:14:30.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.498130 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)     1356 2023-02-27 22:12:01.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.499002 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/
+-rw-r--r--   0 crawford   (501) admin       (80)      329 2023-04-11 08:09:43.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/EMSO-AZORES.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      413 2023-04-11 08:09:59.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/networks/RHUM-RUM.network.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.499765 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-11-30 17:19:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      345 2023-02-28 16:41:26.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/INSU-IPGP.operator.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.501222 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/
+-rw-r--r--   0 crawford   (501) admin       (80)      159 2023-02-28 16:46:55.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Kevin_Canjamale.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)       98 2023-02-28 16:47:13.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Romuald_Daniel.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      100 2023-02-28 16:47:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Simon_Besancon.person.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      166 2023-02-28 16:46:47.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/persons/Wayne_Crawford.person.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.503298 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/
+-rw-r--r--   0 crawford   (501) admin       (80)      643 2023-02-27 22:11:57.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      448 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      811 2023-02-27 22:11:40.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:34.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      797 2023-02-27 22:11:25.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.504754 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)      451 2023-02-27 22:11:22.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      662 2023-02-27 22:11:20.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      821 2023-02-27 22:11:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.508004 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      661 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      752 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2341 2023-04-11 21:38:03.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1425 2023-02-27 22:11:14.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      835 2023-04-11 14:10:42.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      652 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      698 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2009 2023-02-27 22:11:07.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.512065 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-02-06 14:13:53.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      430 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1341 2023-01-09 11:31:34.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      536 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      527 2023-04-11 13:55:08.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      382 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_generic_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      485 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L22D_LCHEAPO_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      537 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1233 2023-02-27 22:11:02.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      586 2023-02-27 22:11:00.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.516249 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-01-09 11:32:20.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      280 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5004_2007.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      306 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5017_2007.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      364 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      383 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L22D_C510-S2000_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      236 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L28LB-obs_C395-S2490_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      728 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      873 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      547 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      854 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/test---attributes-poleszeros.filter.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.521703 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2023-04-11 10:41:26.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)        5 2022-12-19 08:46:18.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.obsinfo
+-rw-r--r--   0 crawford   (501) admin       (80)     3690 2023-04-11 08:10:25.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3429 2023-04-11 21:13:12.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2798 2023-04-11 10:40:05.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2835 2023-04-12 06:00:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2211 2023-04-11 08:10:30.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1890 2023-04-11 21:46:11.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3197 2023-04-11 18:07:50.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3092 2023-04-11 18:07:24.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2699 2023-04-11 18:07:16.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2017 2023-04-11 18:44:22.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.522621 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-15 16:53:33.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/.DS_Store
+-rw-r--r--   0 crawford   (501) admin       (80)      252 2023-01-17 15:49:59.000000 obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/Seascan_GNSS.timing_base.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.473509 obsinfo-0.111b1/obsinfo/_examples/Training/
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.525281 obsinfo-0.111b1/obsinfo/_examples/Training/templates/
+-rw-r--r--   0 crawford   (501) admin       (80)     1308 2023-04-11 08:12:26.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3185 2023-04-11 08:12:46.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1501 2023-01-17 18:01:07.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1625 2023-01-17 18:00:12.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      573 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/CS5322.stage.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1047 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/T240.stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.526768 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     3049 2023-03-22 08:38:30.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     3053 2023-03-22 08:38:26.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:43:56.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:44:03.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.530043 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      673 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      607 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      409 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/HiTechPZ.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      416 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/HiTech_PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2175 2023-04-11 08:12:58.000000 obsinfo-0.111b1/obsinfo/_examples/Training/templates/network.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.531754 obsinfo-0.111b1/obsinfo/_examples/scripts/
+-rw-r--r--   0 crawford   (501) admin       (80)      292 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/README.rst
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.532400 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/
+-rw-r--r--   0 crawford   (501) admin       (80)      331 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/README.rst
+-rw-r--r--   0 crawford   (501) admin       (80)      952 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      376 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/make_stationXML.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      420 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/print_info_files.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)     1646 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/validate_all.sh
+-rwxr-xr-x   0 crawford   (501) admin       (80)      315 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/_examples/scripts/validate_files.sh
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.534403 obsinfo-0.111b1/obsinfo/addons/
+-rw-r--r--   0 crawford   (501) admin       (80)     9904 2023-01-05 14:22:59.000000 obsinfo-0.111b1/obsinfo/addons/LC2SDS.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10899 2023-01-05 14:26:17.000000 obsinfo-0.111b1/obsinfo/addons/LCHEAPO.py
+-rw-r--r--   0 crawford   (501) admin       (80)     9134 2023-04-11 08:13:40.000000 obsinfo-0.111b1/obsinfo/addons/OCA.py
+-rw-r--r--   0 crawford   (501) admin       (80)    15899 2023-04-11 08:13:46.000000 obsinfo-0.111b1/obsinfo/addons/SDPCHAIN.py
+-rw-r--r--   0 crawford   (501) admin       (80)       64 2021-09-09 21:44:08.000000 obsinfo-0.111b1/obsinfo/addons/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2481 2023-01-05 14:20:29.000000 obsinfo-0.111b1/obsinfo/addons/infodump.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.537195 obsinfo-0.111b1/obsinfo/console_scripts/
+-rw-r--r--   0 crawford   (501) admin       (80)      104 2023-04-11 12:05:29.000000 obsinfo-0.111b1/obsinfo/console_scripts/__init__.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    63491 2023-03-22 08:38:16.000000 obsinfo-0.111b1/obsinfo/console_scripts/_test.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7941 2023-04-12 05:49:55.000000 obsinfo-0.111b1/obsinfo/console_scripts/makeStationXML.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     8399 2023-04-12 05:27:13.000000 obsinfo-0.111b1/obsinfo/console_scripts/print.py
+-rw-r--r--   0 crawford   (501) admin       (80)      289 2022-06-20 07:21:38.000000 obsinfo-0.111b1/obsinfo/console_scripts/print_version.py
+-rw-r--r--   0 crawford   (501) admin       (80)     8160 2023-04-12 05:54:26.000000 obsinfo-0.111b1/obsinfo/console_scripts/setup.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    17057 2023-04-12 05:58:43.000000 obsinfo-0.111b1/obsinfo/console_scripts/validate.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.475272 obsinfo-0.111b1/obsinfo/data/
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.544142 obsinfo-0.111b1/obsinfo/data/schemas/
+-rw-r--r--   0 crawford   (501) admin       (80)     8861 2023-03-03 09:25:57.000000 obsinfo-0.111b1/obsinfo/data/schemas/datacite.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     5514 2023-03-25 15:00:10.000000 obsinfo-0.111b1/obsinfo/data/schemas/datalogger_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)    10023 2023-04-11 15:24:46.000000 obsinfo-0.111b1/obsinfo/data/schemas/definitions.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8196 2023-04-11 08:14:23.000000 obsinfo-0.111b1/obsinfo/data/schemas/experiment.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)    13582 2023-04-06 17:48:52.000000 obsinfo-0.111b1/obsinfo/data/schemas/filter.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8241 2023-04-11 10:28:57.000000 obsinfo-0.111b1/obsinfo/data/schemas/instrumentation_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1378 2022-11-30 17:16:16.000000 obsinfo-0.111b1/obsinfo/data/schemas/iris_units.json
+-rw-r--r--   0 crawford   (501) admin       (80)     6575 2023-04-11 15:31:38.000000 obsinfo-0.111b1/obsinfo/data/schemas/location_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1922 2023-04-11 08:14:35.000000 obsinfo-0.111b1/obsinfo/data/schemas/network.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1407 2023-04-06 14:54:32.000000 obsinfo-0.111b1/obsinfo/data/schemas/operator.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     1735 2023-02-28 08:30:05.000000 obsinfo-0.111b1/obsinfo/data/schemas/person.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     4650 2023-03-25 15:00:19.000000 obsinfo-0.111b1/obsinfo/data/schemas/preamplifier_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     6472 2023-03-25 15:00:00.000000 obsinfo-0.111b1/obsinfo/data/schemas/sensor_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     8193 2023-04-06 17:50:39.000000 obsinfo-0.111b1/obsinfo/data/schemas/stage_base.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     2051 2023-03-21 13:52:11.000000 obsinfo-0.111b1/obsinfo/data/schemas/stages.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     7216 2023-04-11 10:58:00.000000 obsinfo-0.111b1/obsinfo/data/schemas/subnetwork.schema.json
+-rw-r--r--   0 crawford   (501) admin       (80)     3997 2023-02-28 16:48:56.000000 obsinfo-0.111b1/obsinfo/data/schemas/timing_base.schema.json
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.544468 obsinfo-0.111b1/obsinfo/datacite/
+-rw-r--r--   0 crawford   (501) admin       (80)        0 2023-01-19 09:54:12.000000 obsinfo-0.111b1/obsinfo/datacite/__init__.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.548405 obsinfo-0.111b1/obsinfo/helpers/
+-rw-r--r--   0 crawford   (501) admin       (80)      729 2023-04-11 09:20:15.000000 obsinfo-0.111b1/obsinfo/helpers/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3091 2023-04-06 13:54:33.000000 obsinfo-0.111b1/obsinfo/helpers/comments.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1565 2023-04-06 13:06:26.000000 obsinfo-0.111b1/obsinfo/helpers/external_references.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3089 2023-04-12 05:45:13.000000 obsinfo-0.111b1/obsinfo/helpers/float_with_uncert.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1518 2023-04-11 16:29:35.000000 obsinfo-0.111b1/obsinfo/helpers/functions.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1506 2023-04-11 09:14:43.000000 obsinfo-0.111b1/obsinfo/helpers/identifiers.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6469 2023-04-05 13:41:46.000000 obsinfo-0.111b1/obsinfo/helpers/location.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3401 2023-04-11 14:33:07.000000 obsinfo-0.111b1/obsinfo/helpers/obsinfo_class_list.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3622 2023-04-02 23:37:37.000000 obsinfo-0.111b1/obsinfo/helpers/oi_date.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2621 2023-04-11 14:26:19.000000 obsinfo-0.111b1/obsinfo/helpers/person.py
+-rw-r--r--   0 crawford   (501) admin       (80)     7685 2023-04-06 07:43:07.000000 obsinfo-0.111b1/obsinfo/helpers/phone.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.551585 obsinfo-0.111b1/obsinfo/instrumentation/
+-rw-r--r--   0 crawford   (501) admin       (80)      830 2023-04-11 10:13:55.000000 obsinfo-0.111b1/obsinfo/instrumentation/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    11457 2023-04-12 05:43:58.000000 obsinfo-0.111b1/obsinfo/instrumentation/channel.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4969 2023-04-11 15:24:42.000000 obsinfo-0.111b1/obsinfo/instrumentation/equipment.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.555415 obsinfo-0.111b1/obsinfo/instrumentation/filter/
+-rw-r--r--   0 crawford   (501) admin       (80)     1850 2023-04-03 16:39:05.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/AD_conversion.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2814 2023-04-12 06:16:41.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/FIR.py
+-rw-r--r--   0 crawford   (501) admin       (80)      506 2023-01-30 15:51:03.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1555 2023-04-11 16:22:34.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/analog.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2353 2023-04-03 16:39:20.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/coefficients.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1256 2023-04-03 16:40:13.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/digital.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3106 2023-03-10 16:10:10.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/filter.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1656 2023-04-06 17:54:00.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/filter_template.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5290 2023-04-11 16:27:01.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/poles_zeros.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2442 2023-04-03 16:39:41.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/polynomial.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1854 2023-04-03 16:39:53.000000 obsinfo-0.111b1/obsinfo/instrumentation/filter/response_list.py
+-rw-r--r--   0 crawford   (501) admin       (80)    12143 2023-04-11 22:07:58.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrument.py
+-rw-r--r--   0 crawford   (501) admin       (80)     9710 2023-04-11 18:45:31.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrument_component.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10284 2023-04-11 18:01:13.000000 obsinfo-0.111b1/obsinfo/instrumentation/instrumentation.py
+-rw-r--r--   0 crawford   (501) admin       (80)     5442 2023-03-27 23:26:01.000000 obsinfo-0.111b1/obsinfo/instrumentation/orientation.py
+-rw-r--r--   0 crawford   (501) admin       (80)    17057 2023-04-06 17:59:14.000000 obsinfo-0.111b1/obsinfo/instrumentation/stage.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2771 2023-04-03 14:12:36.000000 obsinfo-0.111b1/obsinfo/instrumentation/stages.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.557913 obsinfo-0.111b1/obsinfo/misc/
+-rw-r--r--   0 crawford   (501) admin       (80)        0 2022-06-24 14:31:17.000000 obsinfo-0.111b1/obsinfo/misc/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2497 2022-06-24 14:30:50.000000 obsinfo-0.111b1/obsinfo/misc/configuration.py
+-rw-r--r--   0 crawford   (501) admin       (80)      866 2022-06-24 14:29:23.000000 obsinfo-0.111b1/obsinfo/misc/const.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4660 2022-06-24 14:27:52.000000 obsinfo-0.111b1/obsinfo/misc/discoveryfiles.py
+-rw-r--r--   0 crawford   (501) admin       (80)     3062 2023-03-21 09:50:57.000000 obsinfo-0.111b1/obsinfo/misc/printobs.py
+-rw-r--r--   0 crawford   (501) admin       (80)     4026 2022-06-24 14:17:30.000000 obsinfo-0.111b1/obsinfo/misc/remoteGitLab.py
+-rw-r--r--   0 crawford   (501) admin       (80)    28034 2023-04-06 17:16:02.000000 obsinfo-0.111b1/obsinfo/misc/yamlref.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.558622 obsinfo-0.111b1/obsinfo/obsMetadata/
+-rw-r--r--   0 crawford   (501) admin       (80)       37 2023-02-15 09:27:51.000000 obsinfo-0.111b1/obsinfo/obsMetadata/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)    25122 2023-04-11 21:42:28.000000 obsinfo-0.111b1/obsinfo/obsMetadata/obsmetadata.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.560673 obsinfo-0.111b1/obsinfo/subnetwork/
+-rw-r--r--   0 crawford   (501) admin       (80)      376 2023-04-06 14:04:52.000000 obsinfo-0.111b1/obsinfo/subnetwork/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2138 2023-04-11 10:19:15.000000 obsinfo-0.111b1/obsinfo/subnetwork/operator.py
+-rw-r--r--   0 crawford   (501) admin       (80)     2094 2023-04-11 18:04:18.000000 obsinfo-0.111b1/obsinfo/subnetwork/processing.py
+-rw-r--r--   0 crawford   (501) admin       (80)      654 2023-04-06 13:55:11.000000 obsinfo-0.111b1/obsinfo/subnetwork/site.py
+-rw-r--r--   0 crawford   (501) admin       (80)    10316 2023-04-11 18:15:51.000000 obsinfo-0.111b1/obsinfo/subnetwork/station.py
+-rw-r--r--   0 crawford   (501) admin       (80)     6326 2023-04-11 10:58:08.000000 obsinfo-0.111b1/obsinfo/subnetwork/subnetwork.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.562051 obsinfo-0.111b1/obsinfo/template_specifications/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111b1/obsinfo/template_specifications/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.563040 obsinfo-0.111b1/obsinfo/template_specifications/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     1439 2023-03-22 08:38:14.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1076 2023-03-21 09:51:15.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1438 2023-03-21 09:51:26.000000 obsinfo-0.111b1/obsinfo/template_specifications/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.565577 obsinfo-0.111b1/obsinfo/template_specifications/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      276 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      449 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      603 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      194 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      410 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      320 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      401 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1419 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2483 2023-04-11 08:15:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1113 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/template_specifications/stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.567437 obsinfo-0.111b1/obsinfo/templates/
+-rw-r--r--   0 crawford   (501) admin       (80)     6148 2022-12-12 12:14:05.000000 obsinfo-0.111b1/obsinfo/templates/.DS_Store
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.568612 obsinfo-0.111b1/obsinfo/templates/components/
+-rw-r--r--   0 crawford   (501) admin       (80)     1265 2023-03-22 08:38:17.000000 obsinfo-0.111b1/obsinfo/templates/components/datalogger.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      907 2023-03-21 09:51:36.000000 obsinfo-0.111b1/obsinfo/templates/components/preamplifier.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1257 2023-03-21 09:51:42.000000 obsinfo-0.111b1/obsinfo/templates/components/sensor.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.571652 obsinfo-0.111b1/obsinfo/templates/filters/
+-rw-r--r--   0 crawford   (501) admin       (80)      263 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/AD_Conversion.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      435 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/FIR.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      561 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/PolesZeros.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      191 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/analog.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      390 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/coefficients.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      310 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/digital.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)      379 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/filters/response_list.filter.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1327 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/instrumentation.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     2176 2023-04-11 08:15:41.000000 obsinfo-0.111b1/obsinfo/templates/network.yaml
+-rw-r--r--   0 crawford   (501) admin       (80)     1055 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/templates/stage.yaml
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.574845 obsinfo-0.111b1/obsinfo/tests/
+-rw-r--r--   0 crawford   (501) admin       (80)     2880 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/CompareXMLTree.py
+-rw-r--r--   0 crawford   (501) admin       (80)       17 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/__init__.py
+-rw-r--r--   0 crawford   (501) admin       (80)     1159 2021-10-18 08:41:35.000000 obsinfo-0.111b1/obsinfo/tests/remoteGithub.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    74280 2023-03-25 15:32:18.000000 obsinfo-0.111b1/obsinfo/tests/run_test_script.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    35142 2023-03-25 15:32:14.000000 obsinfo-0.111b1/obsinfo/tests/test_datapath.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)    54029 2023-03-25 15:30:33.000000 obsinfo-0.111b1/obsinfo/tests/test_infofile.py
+-rwxr-xr-x   0 crawford   (501) admin       (80)     2148 2023-02-15 16:43:20.000000 obsinfo-0.111b1/obsinfo/tests/test_main.py
+-rw-r--r--   0 crawford   (501) admin       (80)       24 2023-04-12 06:30:25.000000 obsinfo-0.111b1/obsinfo/version.py
+drwxr-xr-x   0 crawford   (501) admin       (80)        0 2023-04-12 06:31:11.483199 obsinfo-0.111b1/obsinfo.egg-info/
+-rw-r--r--   0 crawford   (501) admin       (80)     1919 2023-04-12 06:31:10.000000 obsinfo-0.111b1/obsinfo.egg-info/PKG-INFO
+-rw-r--r--   0 crawford   (501) admin       (80)    14855 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        1 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      586 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/entry_points.txt
+-rw-r--r--   0 crawford   (501) admin       (80)       85 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/requires.txt
+-rw-r--r--   0 crawford   (501) admin       (80)        8 2023-04-12 06:31:11.000000 obsinfo-0.111b1/obsinfo.egg-info/top_level.txt
+-rw-r--r--   0 crawford   (501) admin       (80)      104 2021-10-18 08:41:35.000000 obsinfo-0.111b1/pyproject.toml
+-rw-r--r--   0 crawford   (501) admin       (80)       63 2023-04-12 06:31:11.576223 obsinfo-0.111b1/setup.cfg
+-rw-r--r--   0 crawford   (501) admin       (80)     2261 2023-04-12 05:54:29.000000 obsinfo-0.111b1/setup.py
```

### Comparing `obsinfo-0.111.1.post5/LICENSE.txt` & `obsinfo-0.111b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/PKG-INFO` & `obsinfo-0.111b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinfo
-Version: 0.111.1.post5
+Version: 0.111b1
 Summary: Tools for documenting ocean bottom seismometer experiments and creating metadata
 Home-page: https://gitlab.com/resif/obsinfo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: seismology OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `obsinfo-0.111.1.post5/README.rst` & `obsinfo-0.111b1/README.rst`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/setup.py` & `obsinfo-0.111b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
     print(long_description)
     
 version={}
-with open("src/obsinfo/version.py") as fp:
+with open("obsinfo/version.py") as fp:
     exec(fp.read(),version)
 
 setuptools.setup(
     name="obsinfo",
     version=version['__version__'],
     author="Wayne Crawford",
     author_email="crawford@ipgp.fr",
     description="Tools for documenting ocean bottom seismometer experiments and creating metadata",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://gitlab.com/resif/obsinfo",
+    packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
           'numpy>=1',
           'obspy>=1.1',
           'pyyaml>=3.0',
           'jsonschema>=3.2,<4',
           'python-gitlab>=2.9.0',
@@ -38,22 +39,22 @@
             'obsinfo-makescripts_LCHEAPO=obsinfo.addons.LCHEAPO:_console_script',
             'obsinfo-makescripts_LC2SDS=obsinfo.addons.LC2SDS:_console_script'
         ]
     },
     python_requires='>=3.9',
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
-    classifiers=[
+    classifiers=(
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics"
-    ],
+    ),
     keywords='seismology OBS'
 )
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 2800 0000 0800  ....Bud1..(.....
 00000010: 0000 2800 0000 100c 0000 040a 0000 200b  ..(........... .
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0003 0000 0001 0000 0032  ...............2
+00000040: 0000 0000 0000 0003 0000 0001 0000 0036  ...............6
 00000050: 0000 0003 0000 1000 0063 0061 0074 0069  .........c.a.t.i
 00000060: 006f 006e 0000 0000 0000 0000 0000 0000  .o.n............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -103,34 +103,34 @@
 00000660: 5901 5b01 5c01 5d01 6601 6801 6a01 6b01  Y.[.\.].f.h.j.k.
 00000670: 6c01 7501 7701 7901 7a01 7b01 8401 8601  l.u.w.y.z.{.....
 00000680: 8801 8901 8a01 9301 9501 9601 9701 a001  ................
 00000690: a201 a401 a501 a601 af01 b101 b401 b501  ................
 000006a0: b601 bf01 c101 c301 c401 c501 ce01 d701  ................
 000006b0: dc00 0000 0000 0002 0100 0000 0000 0000  ................
 000006c0: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
-000006d0: dd61 0074 0069 006f 006e 005f 0062 0061  .a.t.i.o.n._.b.a
-000006e0: 0073 0065 0073 6277 7370 626c 6f62 0000  .s.e.sbwspblob..
-000006f0: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00000700: 0607 0809 0809 080d 085d 5368 6f77 5374  .........]ShowSt
-00000710: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00000720: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00000730: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00000740: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00000750: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00000760: 5368 6f77 5369 6465 6261 7209 0809 0809  ShowSidebar.....
-00000770: 5f10 187b 7b37 302c 2034 3130 7d2c 207b  _..{{70, 410}, {
-00000780: 3131 3835 2c20 3436 357d 7d09 0817 2531  1185, 465}}...%1
-00000790: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
-000007a0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
-000007b0: 0000 0000 0000 0000 0000 9a00 0000 0e00  ................
-000007c0: 6c00 6f00 6300 6100 7400 6900 6f00 6e00  l.o.c.a.t.i.o.n.
-000007d0: 5f00 6200 6100 7300 6500 736c 6731 5363  _.b.a.s.e.slg1Sc
-000007e0: 6f6d 7000 0000 0000 001d 5b00 0000 0e00  omp.......[.....
-000007f0: 6c00 6f00 6300 6100 7400 6900 6f00 6e00  l.o.c.a.t.i.o.n.
-00000800: 5f00 6200 0000 0001 0000 0000 0000 080b  _.b.............
+000006d0: dd73 0074 0072 0075 006d 0065 006e 0074  .s.t.r.u.m.e.n.t
+000006e0: 0061 0074 0069 006f 006e 0073 6d6f 6444  .a.t.i.o.n.smodD
+000006f0: 626c 6f62 0000 0008 7996 722d 2ea8 c441  blob....y.r-...A
+00000700: 0000 0010 0069 006e 0073 0074 0072 0075  .....i.n.s.t.r.u
+00000710: 006d 0065 006e 0074 0061 0074 0069 006f  .m.e.n.t.a.t.i.o
+00000720: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
+00000730: 0000 c000 0000 000e 006c 006f 0063 0061  .........l.o.c.a
+00000740: 0074 0069 006f 006e 005f 0062 0061 0073  .t.i.o.n._.b.a.s
+00000750: 0065 0073 6277 7370 626c 6f62 0000 00c9  .e.sbwspblob....
+00000760: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00000770: 0809 0809 080d 085d 5368 6f77 5374 6174  .......]ShowStat
+00000780: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+00000790: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+000007a0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+000007b0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+000007c0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+000007d0: 6f77 5369 6465 6261 7209 0809 0809 5f10  owSidebar....._.
+000007e0: 187b 7b37 302c 2034 3130 7d2c 207b 3131  .{{70, 410}, {11
+000007f0: 3835 2c20 3436 357d 7d09 0817 2531 3d49  85, 465}}...%1=I
+00000800: 606d 797a 0000 0001 0000 0000 0000 080b  `myz............
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -506,139 +506,139 @@
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000 0000 0000 0000 0011 0000 000b  ................
-00002010: 0064 0061 0074 0061 006c 006f 0067 0067  .d.a.t.a.l.o.g.g
-00002020: 0065 0072 0073 6473 636c 626f 6f6c 0000  .e.r.sdsclbool..
-00002030: 0000 0b00 6400 6100 7400 6100 6c00 6f00  ....d.a.t.a.l.o.
-00002040: 6700 6700 6500 7200 736c 6731 5363 6f6d  g.g.e.r.slg1Scom
-00002050: 7000 0000 0000 005f 4e00 0000 0b00 6400  p......_N.....d.
-00002060: 6100 7400 6100 6c00 6f00 6700 6700 6500  a.t.a.l.o.g.g.e.
-00002070: 7200 736d 6f44 4462 6c6f 6200 0000 08d1  r.smoDDblob.....
-00002080: b270 2d2e a8c4 4100 0000 0b00 6400 6100  .p-...A.....d.a.
-00002090: 7400 6100 6c00 6f00 6700 6700 6500 7200  t.a.l.o.g.g.e.r.
-000020a0: 736d 6f64 4462 6c6f 6200 0000 08d1 b270  smodDblob......p
-000020b0: 2d2e a8c4 4100 0000 0b00 6400 6100 7400  -...A.....d.a.t.
-000020c0: 6100 6c00 6f00 6700 6700 6500 7200 7370  a.l.o.g.g.e.r.sp
-000020d0: 6831 5363 6f6d 7000 0000 0000 0150 0000  h1Scomp......P..
-000020e0: 0000 0b00 6500 7800 7000 6500 7200 6900  ....e.x.p.e.r.i.
-000020f0: 6d00 6500 6e00 7400 736c 6731 5363 6f6d  m.e.n.t.slg1Scom
-00002100: 7000 0000 0000 0000 0000 0000 0b00 6500  p.............e.
-00002110: 7800 7000 6500 7200 6900 6d00 6500 6e00  x.p.e.r.i.m.e.n.
-00002120: 7400 736d 6f44 4462 6c6f 6200 0000 08a5  t.smoDDblob.....
-00002130: c771 a1ae d7c4 4100 0000 0b00 6500 7800  .q....A.....e.x.
-00002140: 7000 6500 7200 6900 6d00 6500 6e00 7400  p.e.r.i.m.e.n.t.
-00002150: 736d 6f64 4462 6c6f 6200 0000 08a5 c771  smodDblob......q
-00002160: a1ae d7c4 4100 0000 0b00 6500 7800 7000  ....A.....e.x.p.
-00002170: 6500 7200 6900 6d00 6500 6e00 7400 7370  e.r.i.m.e.n.t.sp
-00002180: 6831 5363 6f6d 7000 0000 0000 0000 0000  h1Scomp.........
-00002190: 0000 1500 6900 6e00 7300 7400 7200 7500  ....i.n.s.t.r.u.
-000021a0: 6d00 6500 6e00 7400 6100 7400 6900 6f00  m.e.n.t.a.t.i.o.
-000021b0: 6e00 5f00 6200 6100 7300 6500 7364 7363  n._.b.a.s.e.sdsc
-000021c0: 6c62 6f6f 6c00 0000 0015 0069 006e 0073  lbool......i.n.s
-000021d0: 0074 0072 0075 006d 0065 006e 0074 0061  .t.r.u.m.e.n.t.a
-000021e0: 0074 0069 006f 006e 005f 0062 0061 0073  .t.i.o.n._.b.a.s
-000021f0: 0065 0073 6c67 3153 636f 6d70 0000 0000  .e.slg1Scomp....
-00002200: 0000 643c 0000 0015 0069 006e 0073 0074  ..d<.....i.n.s.t
-00002210: 0072 0075 006d 0065 006e 0074 0061 0074  .r.u.m.e.n.t.a.t
-00002220: 0069 006f 006e 005f 0062 0061 0073 0065  .i.o.n._.b.a.s.e
-00002230: 0073 6d6f 4444 626c 6f62 0000 0008 7996  .smoDDblob....y.
-00002240: 722d 2ea8 c441 0000 0015 0069 006e 0073  r-...A.....i.n.s
-00002250: 0074 0072 0075 006d 0065 006e 0074 0061  .t.r.u.m.e.n.t.a
-00002260: 0074 0069 006f 006e 005f 0062 0061 0073  .t.i.o.n._.b.a.s
-00002270: 0065 0073 6d6f 6444 626c 6f62 0000 0008  .e.smodDblob....
-00002280: 7996 722d 2ea8 c441 0000 0015 0069 006e  y.r-...A.....i.n
-00002290: 0073 0074 0072 0075 006d 0065 006e 0074  .s.t.r.u.m.e.n.t
-000022a0: 0061 0074 0069 006f 006e 005f 0062 0061  .a.t.i.o.n._.b.a
-000022b0: 0073 0065 0073 7068 3153 636f 6d70 0000  .s.e.sph1Scomp..
-000022c0: 0000 0000 c000 0000 000e 006c 006f 0063  ...........l.o.c
-000022d0: 0061 0074 0069 006f 006e 005f 0062 0061  .a.t.i.o.n._.b.a
-000022e0: 0073 0065 0073 6277 7370 626c 6f62 0000  .s.e.sbwspblob..
-000022f0: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00002300: 0607 0809 0809 080d 085d 5368 6f77 5374  .........]ShowSt
-00002310: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00002320: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00002330: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00002340: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00002350: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00002360: 5368 6f77 5369 6465 6261 7209 0809 0809  ShowSidebar.....
-00002370: 5f10 187b 7b37 302c 2034 3130 7d2c 207b  _..{{70, 410}, {
-00002380: 3131 3835 2c20 3436 357d 7d09 0817 2531  1185, 465}}...%1
-00002390: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
-000023a0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
-000023b0: 0000 0000 0000 0000 0000 9a00 0000 0e00  ................
-000023c0: 6c00 6f00 6300 6100 7400 6900 6f00 6e00  l.o.c.a.t.i.o.n.
-000023d0: 5f00 6200 6100 7300 6500 736c 6731 5363  _.b.a.s.e.slg1Sc
-000023e0: 6f6d 7000 0000 0000 001d 5b00 0000 0e00  omp.......[.....
-000023f0: 6c00 6f00 6300 6100 7400 6900 6f00 6e00  l.o.c.a.t.i.o.n.
-00002400: 5f00 6200 6100 7300 6500 736c 7376 4362  _.b.a.s.e.slsvCb
-00002410: 6c6f 6200 0003 3e62 706c 6973 7430 30da  lob...>bplist00.
-00002420: 0102 0304 0506 0708 090a 0b0c 0c0e 5859  ..............XY
-00002430: 585a 0c5c 5869 636f 6e53 697a 655f 100f  XZ.\XiconSize_..
-00002440: 7368 6f77 4963 6f6e 5072 6576 6965 775f  showIconPreview_
-00002450: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-00002460: 7a65 7357 636f 6c75 6d6e 735f 100f 7363  zesWcolumns_..sc
-00002470: 726f 6c6c 506f 7369 7469 6f6e 5958 7465  rollPositionYXte
-00002480: 7874 5369 7a65 5f10 0f73 6372 6f6c 6c50  xtSize_..scrollP
-00002490: 6f73 6974 696f 6e58 5a73 6f72 7443 6f6c  ositionXZsortCol
-000024a0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
-000024b0: 6544 6174 6573 5f10 1276 6965 774f 7074  eDates_..viewOpt
-000024c0: 696f 6e73 5665 7273 696f 6e23 4030 0000  ionsVersion#@0..
-000024d0: 0000 0000 0909 ae0f 1820 2529 2e33 383d  ......... %).38=
-000024e0: 4247 4b50 54d4 1011 1213 0c15 0c17 5776  BGKPT.........Wv
-000024f0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00002500: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-00002510: 7209 1101 1809 546e 616d 65d4 1319 1a1b  r.....Tname.....
-00002520: 1c1d 1e1e 5577 6964 7468 5961 7363 656e  ....UwidthYascen
-00002530: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
-00002540: 7175 6974 7910 2308 08d4 1011 1213 0c22  quity.#........"
-00002550: 1e24 0910 b508 5c64 6174 654d 6f64 6966  .$....\dateModif
-00002560: 6965 64d4 1011 1213 1e22 1e28 0808 5b64  ied......".(..[d
-00002570: 6174 6543 7265 6174 6564 d410 1112 130c  ateCreated......
-00002580: 2b1e 2d09 1050 0854 7369 7a65 d410 1112  +.-..P.Tsize....
-00002590: 130c 300c 3209 1073 0954 6b69 6e64 d410  ..0.2..s.Tkind..
-000025a0: 1112 130c 350c 3709 1064 0955 6c61 6265  ....5.7..d.Ulabe
-000025b0: 6cd4 1011 1213 1e3a 0c3c 0810 4b09 5776  l......:.<..K.Wv
-000025c0: 6572 7369 6f6e d410 1112 131e 3f0c 4108  ersion......?.A.
-000025d0: 1101 2c09 5863 6f6d 6d65 6e74 73d4 1011  ..,.Xcomments...
-000025e0: 1213 1e44 1e46 0810 c808 5e64 6174 654c  ...D.F....^dateL
-000025f0: 6173 744f 7065 6e65 64d4 1312 1110 481e  astOpened.....H.
-00002600: 221e 5964 6174 6541 6464 6564 0808 d41b  ".YdateAdded....
-00002610: 191a 131e 4d1e 4f08 10d2 085a 7368 6172  ....M.O....Zshar
-00002620: 654f 776e 6572 d41b 191a 131e 4d1e 5308  eOwner......M.S.
-00002630: 085f 100f 7368 6172 654c 6173 7445 6469  ._..shareLastEdi
-00002640: 746f 72d4 1b19 1a13 1e4d 1e57 0808 5f10  tor......M.W.._.
-00002650: 1069 6e76 6974 6174 696f 6e53 7461 7475  .invitationStatu
-00002660: 7323 0000 0000 0000 0000 2340 2400 0000  s#........#@$...
-00002670: 0000 0054 6e61 6d65 0910 0000 0800 1d00  ...Tname........
-00002680: 2600 3800 4c00 5400 6600 6f00 8100 8c00  &.8.L.T.f.o.....
-00002690: 9f00 b400 bd00 be00 bf00 ce00 d700 df00  ................
-000026a0: e500 ef00 fa00 fb00 fe00 ff01 0401 0d01  ................
-000026b0: 1301 1d01 2501 2e01 3001 3101 3201 3b01  ....%...0.1.2.;.
-000026c0: 3c01 3e01 3f01 4c01 5501 5601 5701 6301  <.>.?.L.U.V.W.c.
-000026d0: 6c01 6d01 6f01 7001 7501 7e01 7f01 8101  l.m.o.p.u.~.....
-000026e0: 8201 8701 9001 9101 9301 9401 9a01 a301  ................
-000026f0: a401 a601 a701 af01 b801 b901 bc01 bd01  ................
-00002700: c601 cf01 d001 d201 d301 e201 eb01 f501  ................
-00002710: f601 f702 0002 0102 0302 0402 0f02 1802  ................
-00002720: 1902 1a02 2c02 3502 3602 3702 4a02 5302  ....,.5.6.7.J.S.
-00002730: 5c02 6102 6200 0000 0000 0002 0100 0000  \.a.b...........
-00002740: 0000 0000 5d00 0000 0000 0000 0000 0000  ....]...........
-00002750: 0000 0002 6400 005a 0000 0000 0000 0000  ....d..Z........
-00002760: 0000 0000 0000 024c 0000 0007 0073 0065  .......L.....s.e
-00002770: 006e 0073 006f 0072 0073 6c73 7670 626c  .n.s.o.r.slsvpbl
-00002780: 6f62 0000 0295 6270 6c69 7374 3030 da01  ob....bplist00..
-00002790: 0203 0405 0607 0809 0a0b 0b0b 0e48 4948  .............HIH
-000027a0: 4a4b 425f 1010 7573 6552 656c 6174 6976  JKB_..useRelativ
-000027b0: 6544 6174 6573 5f10 0f73 686f 7749 636f  eDates_..showIco
-000027c0: 6e50 7265 7669 6577 5f10 1163 616c 6375  nPreview_..calcu
+00002000: 0000 0000 0000 0000 0000 0015 0000 0009  ................
+00002010: 0063 0061 006d 0070 0061 0069 0067 006e  .c.a.m.p.a.i.g.n
+00002020: 0073 6c67 3153 636f 6d70 0000 0000 0000  .slg1Scomp......
+00002030: 0804 0000 0009 0063 0061 006d 0070 0061  .......c.a.m.p.a
+00002040: 0069 0067 006e 0073 6d6f 4444 626c 6f62  .i.g.n.smoDDblob
+00002050: 0000 0008 905f 702d 2ea8 c441 0000 0009  ....._p-...A....
+00002060: 0063 0061 006d 0070 0061 0069 0067 006e  .c.a.m.p.a.i.g.n
+00002070: 0073 6d6f 6444 626c 6f62 0000 0008 905f  .smodDblob....._
+00002080: 702d 2ea8 c441 0000 0009 0063 0061 006d  p-...A.....c.a.m
+00002090: 0070 0061 0069 0067 006e 0073 7068 3153  .p.a.i.g.n.sph1S
+000020a0: 636f 6d70 0000 0000 0000 1000 0000 000b  comp............
+000020b0: 0064 0061 0074 0061 006c 006f 0067 0067  .d.a.t.a.l.o.g.g
+000020c0: 0065 0072 0073 6473 636c 626f 6f6c 0000  .e.r.sdsclbool..
+000020d0: 0000 0b00 6400 6100 7400 6100 6c00 6f00  ....d.a.t.a.l.o.
+000020e0: 6700 6700 6500 7200 736c 6731 5363 6f6d  g.g.e.r.slg1Scom
+000020f0: 7000 0000 0000 005f 4e00 0000 0b00 6400  p......_N.....d.
+00002100: 6100 7400 6100 6c00 6f00 6700 6700 6500  a.t.a.l.o.g.g.e.
+00002110: 7200 736d 6f44 4462 6c6f 6200 0000 08d1  r.smoDDblob.....
+00002120: b270 2d2e a8c4 4100 0000 0b00 6400 6100  .p-...A.....d.a.
+00002130: 7400 6100 6c00 6f00 6700 6700 6500 7200  t.a.l.o.g.g.e.r.
+00002140: 736d 6f64 4462 6c6f 6200 0000 08d1 b270  smodDblob......p
+00002150: 2d2e a8c4 4100 0000 0b00 6400 6100 7400  -...A.....d.a.t.
+00002160: 6100 6c00 6f00 6700 6700 6500 7200 7370  a.l.o.g.g.e.r.sp
+00002170: 6831 5363 6f6d 7000 0000 0000 0150 0000  h1Scomp......P..
+00002180: 0000 0b00 6500 7800 7000 6500 7200 6900  ....e.x.p.e.r.i.
+00002190: 6d00 6500 6e00 7400 736c 6731 5363 6f6d  m.e.n.t.slg1Scom
+000021a0: 7000 0000 0000 0000 0000 0000 0b00 6500  p.............e.
+000021b0: 7800 7000 6500 7200 6900 6d00 6500 6e00  x.p.e.r.i.m.e.n.
+000021c0: 7400 736d 6f44 4462 6c6f 6200 0000 08a5  t.smoDDblob.....
+000021d0: c771 a1ae d7c4 4100 0000 0b00 6500 7800  .q....A.....e.x.
+000021e0: 7000 6500 7200 6900 6d00 6500 6e00 7400  p.e.r.i.m.e.n.t.
+000021f0: 736d 6f64 4462 6c6f 6200 0000 08a5 c771  smodDblob......q
+00002200: a1ae d7c4 4100 0000 0b00 6500 7800 7000  ....A.....e.x.p.
+00002210: 6500 7200 6900 6d00 6500 6e00 7400 7370  e.r.i.m.e.n.t.sp
+00002220: 6831 5363 6f6d 7000 0000 0000 0000 0000  h1Scomp.........
+00002230: 0000 1000 6900 6e00 7300 7400 7200 7500  ....i.n.s.t.r.u.
+00002240: 6d00 6500 6e00 7400 6100 7400 6900 6f00  m.e.n.t.a.t.i.o.
+00002250: 6e00 7364 7363 6c62 6f6f 6c00 0000 0010  n.sdsclbool.....
+00002260: 0069 006e 0073 0074 0072 0075 006d 0065  .i.n.s.t.r.u.m.e
+00002270: 006e 0074 0061 0074 0069 006f 006e 0073  .n.t.a.t.i.o.n.s
+00002280: 6c67 3153 636f 6d70 0000 0000 0000 643c  lg1Scomp......d<
+00002290: 0000 0010 0069 006e 0073 0074 0072 0075  .....i.n.s.t.r.u
+000022a0: 006d 0065 006e 0074 0061 0074 0069 006f  .m.e.n.t.a.t.i.o
+000022b0: 006e 0073 6d6f 4444 626c 6f62 0000 0008  .n.smoDDblob....
+000022c0: 7996 722d 2ea8 c441 0000 0010 0069 006e  y.r-...A.....i.n
+000022d0: 0073 0074 0072 0075 006d 0065 006e 0074  .s.t.r.u.m.e.n.t
+000022e0: 0061 0074 0069 006f 006e 0073 6d6f 6444  .a.t.i.o.n.smodD
+000022f0: 626c 6f62 0000 0008 7996 722d 2ea8 c441  blob....y.r-...A
+00002300: 0000 0010 0069 006e 0073 0074 0072 0075  .....i.n.s.t.r.u
+00002310: 006d 0065 006e 0074 0061 0074 0069 006f  .m.e.n.t.a.t.i.o
+00002320: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
+00002330: 0000 c000 0000 000e 006c 006f 0063 0061  .........l.o.c.a
+00002340: 0074 0069 006f 006e 005f 0062 0061 0073  .t.i.o.n._.b.a.s
+00002350: 0065 0073 6277 7370 626c 6f62 0000 00c9  .e.sbwspblob....
+00002360: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
+00002370: 0809 0809 080d 085d 5368 6f77 5374 6174  .......]ShowStat
+00002380: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
+00002390: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
+000023a0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
+000023b0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
+000023c0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
+000023d0: 6f77 5369 6465 6261 7209 0809 0809 5f10  owSidebar....._.
+000023e0: 187b 7b37 302c 2034 3130 7d2c 207b 3131  .{{70, 410}, {11
+000023f0: 3835 2c20 3436 357d 7d09 0817 2531 3d49  85, 465}}...%1=I
+00002400: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
+00002410: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
+00002420: 0000 0000 0000 0000 9a00 0000 0e00 6c00  ..............l.
+00002430: 6f00 6300 6100 7400 6900 6f00 6e00 5f00  o.c.a.t.i.o.n._.
+00002440: 6200 6100 7300 6500 736c 6731 5363 6f6d  b.a.s.e.slg1Scom
+00002450: 7000 0000 0000 001d 5b00 0000 0e00 6c00  p.......[.....l.
+00002460: 6f00 6300 6100 7400 6900 6f00 6e00 5f00  o.c.a.t.i.o.n._.
+00002470: 6200 6100 7300 6500 736c 7376 4362 6c6f  b.a.s.e.slsvCblo
+00002480: 6200 0003 3e62 706c 6973 7430 30da 0102  b...>bplist00...
+00002490: 0304 0506 0708 090a 0b0c 0c0e 5859 585a  ............XYXZ
+000024a0: 0c5c 5869 636f 6e53 697a 655f 100f 7368  .\XiconSize_..sh
+000024b0: 6f77 4963 6f6e 5072 6576 6965 775f 1011  owIconPreview_..
+000024c0: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+000024d0: 7357 636f 6c75 6d6e 735f 100f 7363 726f  sWcolumns_..scro
+000024e0: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
+000024f0: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
+00002500: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+00002510: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
+00002520: 6174 6573 5f10 1276 6965 774f 7074 696f  ates_..viewOptio
+00002530: 6e73 5665 7273 696f 6e23 4030 0000 0000  nsVersion#@0....
+00002540: 0000 0909 ae0f 1820 2529 2e33 383d 4247  ....... %).38=BG
+00002550: 4b50 54d4 1011 1213 0c15 0c17 5776 6973  KPT.........Wvis
+00002560: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00002570: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
+00002580: 1101 1809 546e 616d 65d4 1319 1a1b 1c1d  ....Tname.......
+00002590: 1e1e 5577 6964 7468 5961 7363 656e 6469  ..UwidthYascendi
+000025a0: 6e67 5776 6973 6962 6c65 5875 6269 7175  ngWvisibleXubiqu
+000025b0: 6974 7910 2308 08d4 1011 1213 0c22 1e24  ity.#........".$
+000025c0: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+000025d0: 64d4 1011 1213 1e22 1e28 0808 5b64 6174  d......".(..[dat
+000025e0: 6543 7265 6174 6564 d410 1112 130c 2b1e  eCreated......+.
+000025f0: 2d09 1050 0854 7369 7a65 d410 1112 130c  -..P.Tsize......
+00002600: 300c 3209 1073 0954 6b69 6e64 d410 1112  0.2..s.Tkind....
+00002610: 130c 350c 3709 1064 0955 6c61 6265 6cd4  ..5.7..d.Ulabel.
+00002620: 1011 1213 1e3a 0c3c 0810 4b09 5776 6572  .....:.<..K.Wver
+00002630: 7369 6f6e d410 1112 131e 3f0c 4108 1101  sion......?.A...
+00002640: 2c09 5863 6f6d 6d65 6e74 73d4 1011 1213  ,.Xcomments.....
+00002650: 1e44 1e46 0810 c808 5e64 6174 654c 6173  .D.F....^dateLas
+00002660: 744f 7065 6e65 64d4 1312 1110 481e 221e  tOpened.....H.".
+00002670: 5964 6174 6541 6464 6564 0808 d41b 191a  YdateAdded......
+00002680: 131e 4d1e 4f08 10d2 085a 7368 6172 654f  ..M.O....ZshareO
+00002690: 776e 6572 d41b 191a 131e 4d1e 5308 085f  wner......M.S.._
+000026a0: 100f 7368 6172 654c 6173 7445 6469 746f  ..shareLastEdito
+000026b0: 72d4 1b19 1a13 1e4d 1e57 0808 5f10 1069  r......M.W.._..i
+000026c0: 6e76 6974 6174 696f 6e53 7461 7475 7323  nvitationStatus#
+000026d0: 0000 0000 0000 0000 2340 2400 0000 0000  ........#@$.....
+000026e0: 0054 6e61 6d65 0910 0000 0800 1d00 2600  .Tname........&.
+000026f0: 3800 4c00 5400 6600 6f00 8100 8c00 9f00  8.L.T.f.o.......
+00002700: b400 bd00 be00 bf00 ce00 d700 df00 e500  ................
+00002710: ef00 fa00 fb00 fe00 ff01 0401 0d01 1301  ................
+00002720: 1d01 2501 2e01 3001 3101 3201 3b01 3c01  ..%...0.1.2.;.<.
+00002730: 3e01 3f01 4c01 5501 5601 5701 6301 6c01  >.?.L.U.V.W.c.l.
+00002740: 6d01 6f01 7001 7501 7e01 7f01 8101 8201  m.o.p.u.~.......
+00002750: 8701 9001 9101 9301 9401 9a01 a301 a401  ................
+00002760: a601 a701 af01 b801 b901 bc01 bd01 c601  ................
+00002770: cf01 d001 d201 d301 e201 eb01 f501 f601  ................
+00002780: f702 0002 0102 0302 0402 0f02 1802 1902  ................
+00002790: 1a02 2c02 3502 3602 3702 4a02 5302 5c02  ..,.5.6.7.J.S.\.
+000027a0: 6102 6200 0000 0000 0002 0100 0000 0000  a.b.............
+000027b0: 0000 5d00 0000 0000 0000 0000 0000 0000  ..].............
+000027c0: 0002 6465 7669 6577 5f10 1163 616c 6375  ..deview_..calcu
 000027d0: 6c61 7465 416c 6c53 697a 6573 5763 6f6c  lateAllSizesWcol
 000027e0: 756d 6e73 5f10 0f73 6372 6f6c 6c50 6f73  umns_..scrollPos
 000027f0: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
 00002800: 100f 7363 0000 0005 0000 0000 0000 280b  ..sc..........(.
 00002810: 0000 0045 0000 100c 0000 040a 0000 200b  ...E.......... .
 00002820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -713,57 +713,57 @@
 00002c80: 0100 0100 0000 0000 0100 0200 0000 0000  ................
 00002c90: 0100 0400 0000 0000 0100 0800 0000 0000  ................
 00002ca0: 0100 1000 0000 0000 0100 2000 0000 0000  .......... .....
 00002cb0: 0100 4000 0000 0000 0100 8000 0000 0000  ..@.............
 00002cc0: 0101 0000 0000 0000 0102 0000 0000 0000  ................
 00002cd0: 0104 0000 0000 0000 0108 0000 0000 0000  ................
 00002ce0: 0110 0000 0000 0000 0120 0000 0000 0000  ......... ......
-00002cf0: 0140 0000 0000 0000 0064 7468 5961 7363  .@.......dthYasc
-00002d00: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-00002d10: 7209 1101 1809 546e 616d 65d4 1319 1a1b  r.....Tname.....
-00002d20: 1c1d 1e1e 5577 6964 7468 5961 7363 656e  ....UwidthYascen
-00002d30: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
-00002d40: 7175 6974 7910 2308 08d4 1011 1213 0c22  quity.#........"
-00002d50: 1e24 0910 b508 5c64 6174 654d 6f64 6966  .$....\dateModif
-00002d60: 6965 64d4 1011 1213 1e22 1e28 0808 5b64  ied......".(..[d
-00002d70: 6174 6543 7265 6174 6564 d410 1112 130c  ateCreated......
-00002d80: 2b1e 2d09 1050 0854 7369 7a65 d410 1112  +.-..P.Tsize....
-00002d90: 130c 300c 3209 1073 0954 6b69 6e64 d410  ..0.2..s.Tkind..
-00002da0: 1112 130c 350c 3709 1064 0955 6c61 6265  ....5.7..d.Ulabe
-00002db0: 6cd4 1011 1213 1e3a 0c3c 0810 4b09 5776  l......:.<..K.Wv
-00002dc0: 6572 7369 6f6e d410 1112 131e 3f0c 4108  ersion......?.A.
-00002dd0: 1101 2c09 5863 6f6d 6d65 6e74 73d4 1011  ..,.Xcomments...
-00002de0: 1213 1e44 1e46 0810 c808 5e64 6174 654c  ...D.F....^dateL
-00002df0: 6173 744f 7065 6e65 64d4 1312 1110 481e  astOpened.....H.
-00002e00: 221e 5964 6174 6541 6464 6564 0808 d41b  ".YdateAdded....
-00002e10: 191a 131e 4d1e 4f08 10d2 085a 7368 6172  ....M.O....Zshar
-00002e20: 654f 776e 6572 d41b 191a 131e 4d1e 5308  eOwner......M.S.
-00002e30: 085f 100f 7368 6172 654c 6173 7445 6469  ._..shareLastEdi
-00002e40: 746f 72d4 1b19 1a13 1e4d 1e57 0808 5f10  tor......M.W.._.
-00002e50: 1069 6e76 6974 6174 696f 6e53 7461 7475  .invitationStatu
-00002e60: 7323 0000 0000 0000 0000 2340 2400 0000  s#........#@$...
-00002e70: 0000 0054 6e61 6d65 0910 0000 0800 1d00  ...Tname........
-00002e80: 2600 3800 4c00 5400 6600 6f00 8100 8c00  &.8.L.T.f.o.....
-00002e90: 9f00 b400 bd00 be00 bf00 ce00 d700 df00  ................
-00002ea0: e500 ef00 fa00 fb00 fe00 ff01 0401 0d01  ................
-00002eb0: 1301 1d01 2501 2e01 3001 3101 3201 3b01  ....%...0.1.2.;.
-00002ec0: 3c01 3e01 3f01 4c01 5501 5601 5701 6301  <.>.?.L.U.V.W.c.
-00002ed0: 6c01 6d01 6f01 7001 7501 7e01 7f01 8101  l.m.o.p.u.~.....
-00002ee0: 8201 8701 9001 9101 9301 9401 9a01 a301  ................
-00002ef0: a401 a601 a701 af01 b801 b901 bc01 bd01  ................
-00002f00: c601 cf01 d001 d201 d301 e201 eb01 f501  ................
-00002f10: f601 f702 0002 0102 0302 0402 0f02 1802  ................
-00002f20: 1902 1a02 2c02 3502 3602 3702 4a02 5302  ....,.5.6.7.J.S.
-00002f30: 5c02 6102 6200 0000 0000 0002 0100 0000  \.a.b...........
-00002f40: 0000 0000 5d00 0000 0000 0000 0000 0000  ....]...........
-00002f50: 0000 0002 6400 005a 0000 0000 0000 0000  ....d..Z........
-00002f60: 0000 0000 0000 024c 0000 0007 0073 0065  .......L.....s.e
-00002f70: 006e 0073 006f 0072 0073 6c73 7670 626c  .n.s.o.r.slsvpbl
-00002f80: 6f62 0000 0295 6270 6c69 7374 3030 da01  ob....bplist00..
-00002f90: 0203 0405 0607 0809 0a0b 0b0b 0e48 4948  .............HIH
-00002fa0: 4a4b 425f 1010 7573 6552 656c 6174 6976  JKB_..useRelativ
-00002fb0: 6544 6174 6573 5f10 0f73 686f 7749 636f  eDates_..showIco
-00002fc0: 6e50 7265 7669 6577 5f10 1163 616c 6375  nPreview_..calcu
+00002cf0: 0140 0000 0000 0000 0072 6f6c 6c50 6f73  .@.......rollPos
+00002d00: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
+00002d10: 6e5f 1010 7573 6552 656c 6174 6976 6544  n_..useRelativeD
+00002d20: 6174 6573 5f10 1276 6965 774f 7074 696f  ates_..viewOptio
+00002d30: 6e73 5665 7273 696f 6e23 4030 0000 0000  nsVersion#@0....
+00002d40: 0000 0909 ae0f 1820 2529 2e33 383d 4247  ....... %).38=BG
+00002d50: 4b50 54d4 1011 1213 0c15 0c17 5776 6973  KPT.........Wvis
+00002d60: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00002d70: 6469 6e67 5a69 6465 6e74 6966 6965 7209  dingZidentifier.
+00002d80: 1101 1809 546e 616d 65d4 1319 1a1b 1c1d  ....Tname.......
+00002d90: 1e1e 5577 6964 7468 5961 7363 656e 6469  ..UwidthYascendi
+00002da0: 6e67 5776 6973 6962 6c65 5875 6269 7175  ngWvisibleXubiqu
+00002db0: 6974 7910 2308 08d4 1011 1213 0c22 1e24  ity.#........".$
+00002dc0: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00002dd0: 64d4 1011 1213 1e22 1e28 0808 5b64 6174  d......".(..[dat
+00002de0: 6543 7265 6174 6564 d410 1112 130c 2b1e  eCreated......+.
+00002df0: 2d09 1050 0854 7369 7a65 d410 1112 130c  -..P.Tsize......
+00002e00: 300c 3209 1073 0954 6b69 6e64 d410 1112  0.2..s.Tkind....
+00002e10: 130c 350c 3709 1064 0955 6c61 6265 6cd4  ..5.7..d.Ulabel.
+00002e20: 1011 1213 1e3a 0c3c 0810 4b09 5776 6572  .....:.<..K.Wver
+00002e30: 7369 6f6e d410 1112 131e 3f0c 4108 1101  sion......?.A...
+00002e40: 2c09 5863 6f6d 6d65 6e74 73d4 1011 1213  ,.Xcomments.....
+00002e50: 1e44 1e46 0810 c808 5e64 6174 654c 6173  .D.F....^dateLas
+00002e60: 744f 7065 6e65 64d4 1312 1110 481e 221e  tOpened.....H.".
+00002e70: 5964 6174 6541 6464 6564 0808 d41b 191a  YdateAdded......
+00002e80: 131e 4d1e 4f08 10d2 085a 7368 6172 654f  ..M.O....ZshareO
+00002e90: 776e 6572 d41b 191a 131e 4d1e 5308 085f  wner......M.S.._
+00002ea0: 100f 7368 6172 654c 6173 7445 6469 746f  ..shareLastEdito
+00002eb0: 72d4 1b19 1a13 1e4d 1e57 0808 5f10 1069  r......M.W.._..i
+00002ec0: 6e76 6974 6174 696f 6e53 7461 7475 7323  nvitationStatus#
+00002ed0: 0000 0000 0000 0000 2340 2400 0000 0000  ........#@$.....
+00002ee0: 0054 6e61 6d65 0910 0000 0800 1d00 2600  .Tname........&.
+00002ef0: 3800 4c00 5400 6600 6f00 8100 8c00 9f00  8.L.T.f.o.......
+00002f00: b400 bd00 be00 bf00 ce00 d700 df00 e500  ................
+00002f10: ef00 fa00 fb00 fe00 ff01 0401 0d01 1301  ................
+00002f20: 1d01 2501 2e01 3001 3101 3201 3b01 3c01  ..%...0.1.2.;.<.
+00002f30: 3e01 3f01 4c01 5501 5601 5701 6301 6c01  >.?.L.U.V.W.c.l.
+00002f40: 6d01 6f01 7001 7501 7e01 7f01 8101 8201  m.o.p.u.~.......
+00002f50: 8701 9001 9101 9301 9401 9a01 a301 a401  ................
+00002f60: a601 a701 af01 b801 b901 bc01 bd01 c601  ................
+00002f70: cf01 d001 d201 d301 e201 eb01 f501 f601  ................
+00002f80: f702 0002 0102 0302 0402 0f02 1802 1902  ................
+00002f90: 1a02 2c02 3502 3602 3702 4a02 5302 5c02  ..,.5.6.7.J.S.\.
+00002fa0: 6102 6200 0000 0000 0002 0100 0000 0000  a.b.............
+00002fb0: 0000 5d00 0000 0000 0000 0000 0000 0000  ..].............
+00002fc0: 0002 6465 7669 6577 5f10 1163 616c 6375  ..deview_..calcu
 00002fd0: 6c61 7465 416c 6c53 697a 6573 5763 6f6c  lateAllSizesWcol
 00002fe0: 756d 6e73 5f10 0f73 6372 6f6c 6c50 6f73  umns_..scrollPos
 00002ff0: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
 00003000: 100f 7363                                ..sc
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/README.rst` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 This directory contains sample information files in several directories:
 
 * the ``./subnetwork`` directory, which has files for each data collection
   campaign.
   
-* the ``./instrumentation_bases`` directory, which contains files which represent an inventory of park instruments.
+* the ``./instrumentations`` directory, which contains files which represent an inventory of park instruments.
   
 * the ``./sensors`` directory, which contains files which represent sensors.
 
 * the ``./preamplifiers`` directory, which contains files which represent preamplifiers.
 
 * the ``./dataloggers`` directory, which contains files which represent dataloggers
 
 Each one has:
 
   * a ``responses`` subdirectory containing individual sensor, datalogger and filter stages. These in turn have:
-  * a  ``filters`` subdirectory containing filters related to the stages.
+    * a  ``filters`` subdirectory containing filters related to the stages.
 
 The rest are auxiliary directories.
 
 The information files can be in YAML or JSON format.
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/BBOBS1_2012+.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
         "2":
             orientation: {"1": {azimuth.deg: {value: 90, uncertainty: 180}}}
         "3": 
             orientation: {"Z":  {azimuth.deg: {value: 0}, dip.deg: {value: -90}}}
             preamplifier: {configuration: "1x gain"}
         "4":
             orientation : {"H": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
-            ^preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml#preamplifier_base"}}
-            ^sensor: {base: {$ref: "sensors/SIO_DPG.sensor_base.yaml#sensor_base"}}         
+            preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml#preamplifier_base"},
+                           configuration: ~}  # This should not be necessary
+            sensor: {base: {$ref: "sensors/SIO_DPG.sensor_base.yaml#sensor_base"}}         
             extras:
                 DBIRD_response_type : "CALIBRATED"   
     configurations:
         "SN01":
             equipment: {serial_number: '01'}
             channels:
                 default: {sensor: {configuration: "Sphere01"}}
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/BBOBS1_pre2012.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
             sensor: {base: {$ref: "sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml#sensor_base"},
                      configuration: "SN1-399, single-sided"}
         "1": {orientation: {"2": {azimuth.deg: {value: 90, uncertainty: 180}, dip.deg: {value: 0}}}}
         "2": {orientation: {"1": {azimuth.deg: {value: 0, uncertainty: 180},  dip.deg: {value: 0}}}}
         "3": {orientation: {"Z": {azimuth.deg: {value: 0}, dip.deg: {value: -90}}}}
         "4":
             orientation: {"H": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
-            ^preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml#preamplifier_base"},
+            preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml#preamplifier_base"},
                            configuration: ~}
-            ^sensor: {base: {$ref: "sensors/SIO_DPG.sensor_base.yaml#sensor_base"}}
+            sensor: {base: {$ref: "sensors/SIO_DPG.sensor_base.yaml#sensor_base"}}
     configurations:
         "SN01":
             equipment: {serial_number: '01'}
             channels:
                 default: {sensor: {configuration: "Sphere01"}}
                 "4": {sensor: {configuration: "generic"}}
         "SN02":
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/GURALP_CP.instrumentation_base.yaml_error` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/HYDROCT1.instrumentation_base.yaml_error` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS1.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 ---
 format_version: "0.111"
 revision: 
     date: "2018-06-01"
     authors:
         - {$ref: "persons/Wayne_Crawford.person.yaml#person"}
         - {$ref: "persons/Romuald_Daniel.person.yaml#person"}
-        
 instrumentation_base:
     equipment:
         model: "SPOBS1"
         type: "Short Period Ocean Bottom Seismometer"
-        description: "LCHEAPO 2000 SPOBS, 2 channels, L-22 vertical geophone"
+        description: "LCHEAP 2000 SPOBS, 2 channels, L-22 vertical geophone"
         manufacturer: "Scripps Inst. Oceanography"
         vendor: "Scripps Inst. Oceanography"
     channels:
         default:
-            datalogger:
-                base: {$ref: "dataloggers/LC2000.datalogger_base.yaml#datalogger_base"}
-            preamplifier:
-                base: {$ref: "preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml#preamplifier_base"}
-                configuration: "128x gain"
-            sensor:
-                base: {$ref: "sensors/SERCEL_L22.sensor_base.yaml#sensor_base"}
+            datalogger: {base: {$ref: "dataloggers/LC2000.datalogger_base.yaml#datalogger_base"}}
+            # For testing of preamplifier configuration, can switch between these two.
+            # LCHEAPO_HYDRO should give warning of no config found
+            # Note: if a field is repeated in a yaml file is repeated, the last value is taken
+            preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml#preamplifier_base"},
+                           configuration: "128x gain"}
+            sensor: {base: {$ref: "sensors/SERCEL_L22.sensor_base.yaml#sensor_base"}}
         "1":
             orientation: {"3": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
         "2":
             orientation: {"H": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
-            ^sensor: {base: {$ref: "sensors/HITECH_HTI90U.sensor_base.yaml#sensor_base"}}
+            sensor: {base: {$ref: "sensors/HITECH_HTI90U.sensor_base.yaml#sensor_base"}}
+        "3":
+            orientation: {"H": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
+            location_code: "01"
+            sensor: {base: {$ref: "sensors/HITECH_HTI90U.sensor_base.yaml#sensor_base"}}
+        "4":
+            orientation: {"3": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
+            location_code: "02"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS2.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,14 @@
         default:
             datalogger: {base: {$ref: "dataloggers/LC2000.datalogger_base.yaml#datalogger_base"}}
             preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml#preamplifier_base"},
                            configuration: "128x gain"}
             sensor: {base: {$ref: "sensors/SERCEL_L28.sensor_base.yaml#sensor_base"}}
         "1":
             orientation : {"H": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
-            ^preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml#preamplifier_base"},
-                            configuration: "16x gain"}
-            ^sensor: {base: {$ref: "sensors/HITECH_HTI90U.sensor_base.yaml#sensor_base"}}
+            preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml#preamplifier_base"},
+                           configuration: "16x gain"}
+            sensor: {base: {$ref: "sensors/HITECH_HTI90U.sensor_base.yaml#sensor_base"}}
             
         "2": {orientation: {"2": {azimuth.deg: {value: 90, uncertainty: 180}}}}
         "3": {orientation: {"1": {azimuth.deg: {value: 0, uncertainty: 180}}}}
         "4": {orientation: {"3": {dip.deg: {value: 90}}}}
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/WBOBS1.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -23,10 +23,10 @@
         
         "1": {orientation: {"2": {azimuth.deg: {value: 90, uncertainty: 180}, dip.deg: {value: 0}}}}
         "2": {orientation: {"1": {azimuth.deg: {value: 0, uncertainty: 180}, dip.deg: {value: 0}}}}
         "3": {orientation: {"Z": {azimuth.deg: {value: 0},  dip.deg: {value: -90}}}}
            
         "4":
             orientation : {"H": {azimuth.deg: {value: 0}, dip.deg: {value: 90}}}
-            ^preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml#preamplifier_base"},
+            preamplifier: {base: {$ref: "preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml#preamplifier_base"},
                            configuration: "16x gain"}
-            ^sensor: {base: {$ref: "sensors/HITECH_HTI90U.sensor_base.yaml#sensor_base"}}
+            sensor: {base: {$ref: "sensors/HITECH_HTI90U.sensor_base.yaml#sensor_base"}}
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/instrumentation_bases/empty.instrumentation_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/location_bases/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
             measurement_method: "Airgun survey"
             notes: ["Uncertainty will generally be least along-line"]
         "BUC_DIRECT":
             uncertainties.m: {lon: 5, lat: 5, elev: 10}
             measurement_method: "Short baseline transponder, seafloor release"
         "BUC_DROP":
             uncertainties.m: {lon: 20, lat: 20, elev: 20}
-            measurement_method: "Short baseline transponder, near-seafloor release"
+            measurement_method: "Short baseline transponder, near-seafloor release"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/operators/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/operators/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -12,12 +12,10 @@
         manufacturer: "SIO or IPGP"
         vendor: "LCHEAPO"
     stages:
         - {base: {$ref: "preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml#stage_base"}}
     configuration_default: "1x gain"
     configurations:
         "0.225x gain":
-            stage_modifications:
-                '*': {configuration: "0.225x"}
+            stages: [{configuration: "0.225x"}]
         "1x gain":
-            stage_modifications:
-                '*': {configuration: "1.0x"}
+            stages: [{configuration: "1.0x"}]
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     gain:  {value : 128, frequency : 10.}
     filter : {type : "ANALOG"}
     configuration_default: "128x"
     configurations:
         "16x": {gain:  {value : 16, frequency : 10.}}
         "32x": {gain:  {value : 32, frequency : 10.}}
         "64x": {gain:  {value : 64, frequency : 10.}}
-        "128x": {gain:  {value : 128, frequency : 10.}}
+        "128": {gain:  {value : 128, frequency : 10.}}
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         type : "PolesZeros"
         transfer_function_type: "LAPLACE (RADIANS/SECOND)"
         zeros : ['0 + 0j']
         poles : ['-6.667 + 0j']
     delay: 0
     configuration_default: "64x"
     configurations:
-        "16x":
-            gain: {value: 16, frequency: 10}
-        "32x":
-            gain: {value: 32, frequency: 10}
         "64x":
             gain: {value: 64, frequency: 10}
+        "32x":
+            gain: {value: 32, frequency: 10}
+        "16x":
+            gain: {value: 16, frequency: 10}
         "128x":
             gain: {value: 128, frequency: 10}
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 format_version: "0.111"
 stage_base:
     description : "SENSOR - DPG 5004" # optionel
     input_units :  {name: "Pa", description: "PRESSURE"}
     output_units : {name: "V", description: "VOLTS"}
-    calibration_dates: ["2007-01-01"]
+    calibration_date: "2007-01-01"
     gain: {value: 4.25e-4, frequency: 1}
     filter:
         type : "PolesZeros"
         transfer_function_type: "LAPLACE (RADIANS/SECOND)"
         zeros :
             - '0 + 0j'
         poles :
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 format_version: "0.111"
 stage_base:
     description : "SENSOR - DPG 5018" 
     input_units :  {name: "Pa", description: "PRESSURE"}
     output_units : {name: "V", description: "VOLTS"}
-    calibration_dates: ["2007-01-01"]
+    calibration_date: "2007-01-01"
     gain:  {value: 4.38e-4, frequency: 1}
     filter:
         type : "PolesZeros"
         transfer_function_type: "LAPLACE (RADIANS/SECOND)"
         zeros :
             - '0 + 0j'
         poles :
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,22 @@
     stations:
         "BB_1":
             site: "My favorite site"
             start_date: "2011-04-23T10:00:00"
             end_date: "2011-05-28T15:37:00"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/BBOBS1_pre2012.instrumentation_base.yaml#instrumentation_base"}
+                base: {$ref: "instrumentations/BBOBS1_pre2012.instrumentation_base.yaml#instrumentation_base"}
                 serial_number: "07"
-                datalogger_configuration: "62.5sps"
+                modifications:
+                    datalogger:
+                        equipment: {serial_number: "27"}
+                        configuration: "62.5sps"
+                    preamplifier: {equipment: {serial_number: "27"}}
                 channel_modifications:
-                    "*-*": {datalogger: {serial_number: "27"},
-                            preamplifier: {serial_number: "27"}}
                     "1-*": {sensor: {configuration: "Sphere07"}}
                     "2-*": {sensor: {configuration: "Sphere07"}}
                     "Z-*": {sensor: {configuration: "Sphere07"}}
                     "H-*": {sensor: {configuration: "IP007"}}
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
@@ -46,28 +48,31 @@
         "BB_2":
             site: "My other favorite site"
             start_date: "2015-04-23T10:00:00Z"
             end_date: "2016-05-28T15:37:00Z"
             location_code: "00"
             notes: ["example of deploying with a different sphere"]
             instrumentation:
-                base: {$ref: "instrumentation_bases/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"} 
+                base: {$ref: "instrumentations/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"} 
                 serial_number: "06"
-                datalogger_configuration: "62.5sps"
+                modifications:
+                    datalogger: {configuration: "62.5sps", equipment: {serial_number: "26"}}
+                    preamplifier: {equipment: {serial_number: "26"}}
                 channel_modifications:
-                    "*-*": {datalogger: {serial_number: "26"},
-                            preamplifier: {serial_number: "26"}}
                     "1-*": {sensor: {configuration: "Sphere08"}}
                     "2-*": {sensor: {configuration: "Sphere08"}}
                     "Z-*": {sensor: {configuration: "Sphere08"}}
-                    "H-*":  {sensor: {configuration: "5004"}}
+    #                 "H-*": {sensor_: {configuration: "5004"}}
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "BUC_DROP"
                     position: {lon: -32.29756, lat: 37.26049, elev: -1887}
             processing:
                 - clock_correction_linear:
                         base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
                         start_sync_reference: "2015-04-22T12:24:00"
                         end_sync_reference: "2016-05-28T15:35:00.3660"
                         end_sync_instrument: "2016-05-28T15:35:02" 
+notes: 
+    - "In version 0.110, I need to specify the sensor serial numbers"
+    - "BB_2 gives example "
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     stations:
         "BB_1":
             site: "My favorite site"
             start_date: "2015-04-23T10:00:00"
             end_date: "2016-05-28T15:37:00"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"}
-                datalogger_configuration: "62.5sps"
+                base: {$ref: "instrumentations/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"}
                 channel_modifications:
+                    "*-*": {datalogger: {configuration: "62.5sps"}}
                     "2":
                         sensor:
                             stage_modifications:
                                "1": {gain: {value: 753.27}}             
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
@@ -37,26 +37,26 @@
             processing:
                 - clock_correction_linear:
                         base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
                         start_sync_reference: "2015-04-23T11:20:00"
                         end_sync_reference: "2016-05-27T14:00:00.2450"
                         end_sync_instrument: "2016-05-27T14:00:00"
         "BB_2":
-            notes: ["An example of changing the sensor"]
             site: "My other favorite site"
             start_date: "2015-04-23T10:00:00Z"
             end_date: "2016-05-28T15:37:00Z"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"}
-                datalogger_configuration: "62.5sps"
+                base: {$ref: "instrumentations/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"}
+                modifications:
+                    sensor: {equipment: {serial_number: "Sphere06"}}
+                    datalogger: {configuration: "62.5sps"}
                 channel_modifications:
-                    "*":   {sensor: {serial_number: "Sphere06"}}
                     "2":   {sensor: {stage_modifications:{ "1": {gain: {value: 762.16}}}}}
-                    "H-*": {sensor: {serial_number: "IP007"}}
+                    "H-*": {sensor: {equipment: {serial_number: "IP007"}}}
                     "1":   
                         datalogger: 
                             stage_modifications:
                                "1": {gain: {value: 1533742}}
                         sensor:
                             stage_modifications: 
                                "1": {gain: {value: 1247.3}}
@@ -68,8 +68,9 @@
             processing:
                 - clock_correction_linear:
                         base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
                         start_sync_reference: "2015-04-22T12:24:00"
                         end_sync_reference: "2016-05-28T15:35:00.3660"
                         end_sync_instrument: "2016-05-28T15:35:02"
                         
+notes: ["BB_2 is an example of changing the sensor"]
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             location_code: "00"
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "BUC_DROP"
                     position: {lon: -32.5, lat: 37.5, elev: -2000}
             instrumentation:
-                base: {$ref: 'instrumentation_bases/empty.instrumentation_base.yaml#instrumentation_base'}
+                base: {$ref: 'instrumentations/empty.instrumentation_base.yaml#instrumentation_base'}
             processing:
                 - clock_correction_linear:
                         base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
                         start_sync_reference: "2015-04-23T11:20:00"
                         end_sync_reference: "2016-05-27T14:00:00.2450"
                         end_sync_instrument: "2016-05-27T14:00:00"
                         
@@ -52,14 +52,14 @@
             location_code: "00"
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "BUC_DROP"
                     position: {lon: -32.3, lat: 37.3, elev: -1500}
             instrumentation:
-                base: {$ref: 'instrumentation_bases/empty.instrumentation_base.yaml#instrumentation_base'}           
+                base: {$ref: 'instrumentations/empty.instrumentation_base.yaml#instrumentation_base'}           
             processing:
                 - clock_correction_linear:
                         base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
                         start_sync_reference: "2015-04-22T12:24:00"
                         end_sync_reference: "2016-05-28T15:35:00.3660"
                         end_sync_instrument: "2016-05-28T15:35:02"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
             location_code: "00"
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "BUC_DROP"
                     position: {lon: -32.234, lat: 37.2806, elev: -1950}
             instrumentation:
-                base: {$ref: "instrumentation_bases/BBOBS1_pre2012.instrumentation_base.yaml#instrumentation_base"}
+                base: {$ref: "instrumentations/BBOBS1_pre2012.instrumentation_base.yaml#instrumentation_base"}
                 configuration: "SN03"
-                datalogger_configuration: "250sps"
+                modifications:
+                    datalogger: {configuration: "250sps"}
             processing:
                 - clock_correction_linear:
                         base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
                         start_sync_reference: "2015-04-23T11:20:00"
                         end_sync_reference: "2016-05-27T14:00:00.2450"
                         end_sync_instrument: "2016-05-27T14:00:00"       
         "BB_2":
@@ -38,17 +39,18 @@
             location_code: "00"
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "ACOUSTIC_SURVEY"
                     position: {lon: -32.29756, lat: 37.26049, elev: -1887}
             instrumentation:
-                base: {$ref: "instrumentation_bases/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"} 
+                base: {$ref: "instrumentations/BBOBS1_2012+.instrumentation_base.yaml#instrumentation_base"} 
                 configuration: "SN06"
-                datalogger_configuration: "125sps"
+                modifications:
+                    datalogger: {configuration: "125sps"}
                 channel_modifications:
                     "1-*": {sensor: {configuration: "Sphere08"}}
                     "2-*": {sensor: {configuration: "Sphere08"}}
                     "Z-*": {sensor: {configuration: "Sphere08"}}
                     "H-*": {sensor: {configuration: "5004"}}
             processing:
                 - clock_correction_linear:
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,16 @@
                         vault: "Sea floor"
                         uncertainties.m: {lon: 20, lat: 20, elev: 20}
                         measurement_method: "Short baseline transponder, near-seafloor release"
                     position: {lon: -32.234, lat: 37.2806, elev: -1950}
             instrumentation:
                 base: "INSU_BBOBS"
                 configuration: "SN07"
-                datalogger_configuration: "62.5sps"
+                modifications:
+                    datalogger: {configuration: "62.5sps"}
             processing:
                 - clock_correction_linear:
                         base:
                             instrument: "Seascan MCXO, ~1e-8 nominal drift"
                             reference: "GNSS"
                             start_sync_instrument: 0
                         start_sync_reference: "2015-04-23T11:20:00"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     stations:
         "LPSCD":
             site: "Lucky Strike Volcano Center"
             start_date: "2016-07-01T12:00:00"
             end_date: ~
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
-                datalogger_configuration: "250sps"
+                base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+                modifications:
+                    datalogger: {configuration: "250sps"}
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "BUC_DIRECT"
                     position: {lon: -32.280, lat: 37.290, elev: -1760}
             processing:
                 - clock_correction_leapsecond:
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,63 @@
 ---
 format_version: "0.111"
 revision:
     authors:
         - {$ref: "persons/Wayne_Crawford.person.yaml#person"}
     date: "2017-10-04"
 subnetwork:
-    operators:
-        - agency: "INSU-IPGP OBS Park"
-    reference_names:
-        operator: "INSU-IPGP"
-        campaign: "ORIENTED"
     network:
         code: "4G"
-        name: "ORIENTED STATIONS"
+        name: "Short period OBSs"
         start_date: "2007-07-01"
         end_date: "2025-12-31"
-        description: "EMSO-AZORES"
+        description: "Short Period OBS network"
+    operators:
+        - agency: "INSU-IPGP OBS Park"
+    reference_names:
+        operator: "INSU-IPGP"
+        campaign: "SPOBS_noAnchors"  
     stations:
         "LSVW":
-            
             site: "Lucky Strike Volcano West"
             start_date: "2015-04-22T12:00:00Z"
             end_date: "2016-05-28T21:01:00Z"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
-                datalogger_configuration : "125sps"
+                base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
                 channel_modifications:
-                   '1-00': { orientation: {'1': {azimuth.deg: {value: 33, uncertainty: 5, measurement_method: "Ppol"}}}}
-                   '2-00': { orientation: {'2': {azimuth.deg: {value: 23, uncertainty: 5, measurement_method: "Ppol"}}}}
+                   "*-*": {datalogger: {configuration: "125sps"}}
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "SEA_SURFACE"
                     position: {lon: -32.32504, lat: 37.29744, elev: -2030}
             processing:
                 - clock_correction_linear:
-                    base: {$ref: 'timing_bases/Seascan_GNSS.timing_base.yaml#timing_base'}
+                    base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
                     start_sync_reference: "2015-04-21T21:06:00Z"
                     end_sync_reference: "2016-05-28T20:59:00.32Z"
                     end_sync_instrument: "2016-05-28T20:59:03Z"
         "LSVE":
             site: "Lucky Strike Volcano East"
             start_date: "2015-04-22T12:00:00Z"
             end_date: "2016-05-28T21:01:00Z"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
-                datalogger_configuration : "125sps"
+                base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
                 channel_modifications:
-                   '1-00': {orientation: {'1': {azimuth.deg: {value: 154, uncertainty: 7, measurement_method: "Ppol"}}}}
-                   '2-00': {orientation: {'2': {azimuth.deg: {value: 244, uncertainty: 7, measurement_method: "Ppol"}}}}
+                   "*-*": {datalogger: {configuration: "125sps"}}
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
-                    configuration: "SEA_SURFACE"
+                    configuration: "ACOUSTIC_SURVEY"
                     position: {lon: -32.02504, lat: 37.25744, elev: -2130}
             processing:
                 - clock_correction_linear:
-                    base: {$ref: 'timing_bases/Seascan_GNSS.timing_base.yaml#timing_base'}
-                    start_sync_reference: "2015-04-21T21:06:00Z"
-                    end_sync_reference: "2016-05-28T20:59:00.32Z"
-                    end_sync_instrument: "2016-05-28T20:59:01Z"
-
-notes:
-    - "An example with station orientations provided"
-    - "Provide azimuths for channels 1 and 2"
+                        base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
+                        start_sync_reference: "2015-04-21T21:06:00Z"
+                        end_sync_reference: "2016-05-28T20:59:00.32Z"
+                        end_sync_instrument: "2016-05-28T20:59:01Z"
     
+notes: 
+    - "Same as SPOBS, without using YAML anchors"
+    - "Lucky Strike Volcano, North Mid-Atlantic Ridge"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     stations:
         "LSVW":
             site: "Lucky Strike Volcano West"
             start_date: "2015-04-22T12:00:00Z"
             end_date: "2016-05-28T21:01:00Z"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+                base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
                 channel_modifications:
                     "*": {datalogger: {configuration: "125sps"}}
                 serial_number: "20"
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "SEA_SURFACE"
@@ -50,15 +50,15 @@
                     end_sync_instrument: "2016-05-28T20:59:03Z"
         "LSVE":
             site: "Lucky Strike Volcano East"
             start_date: "2015-04-22T12:00:00Z"
             end_date: "2016-05-28T21:01:00Z"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+                base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
                 channel_modifications:
                     "*": {datalogger: {configuration: "125sps"}}
                 serial_number: "12"
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "ACOUSTIC_SURVEY"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 ---
 format_version: "0.111"
 revision:
     authors:
         - {$ref: "persons/Wayne_Crawford.person.yaml#person"}
     date: "2017-10-04"
 subnetwork:
-    network:
-        code: "4G"
-        name: "Short period OBSs"
-        start_date: "2007-07-01"
-        end_date: "2025-12-31"
-        description: "Short Period OBS network"
     operators:
         - agency: "INSU-IPGP OBS Park"
     reference_names:
         operator: "INSU-IPGP"
-        campaign: "SPOBS_noAnchors"  
+        campaign: "ORIENTED"
+    network:
+        code: "4G"
+        name: "ORIENTED STATIONS"
+        start_date: "2007-07-01"
+        end_date: "2025-12-31"
+        description: "EMSO-AZORES"
     stations:
         "LSVW":
+            
             site: "Lucky Strike Volcano West"
             start_date: "2015-04-22T12:00:00Z"
             end_date: "2016-05-28T21:01:00Z"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+                base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+                modifications:
+                    datalogger: {configuration : "125sps"}
                 channel_modifications:
-                   "*-*": {datalogger: {configuration: "125sps"}}
+                   '1-00': { orientation: {'1': {azimuth.deg: {value: 33, uncertainty: 5, measurement_method: "Ppol"}}}}
+                   '2-00': { orientation: {'2': {azimuth.deg: {value: 23, uncertainty: 5, measurement_method: "Ppol"}}}}
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
                     configuration: "SEA_SURFACE"
                     position: {lon: -32.32504, lat: 37.29744, elev: -2030}
             processing:
                 - clock_correction_linear:
-                    base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
+                    base: {$ref: 'timing_bases/Seascan_GNSS.timing_base.yaml#timing_base'}
                     start_sync_reference: "2015-04-21T21:06:00Z"
                     end_sync_reference: "2016-05-28T20:59:00.32Z"
                     end_sync_instrument: "2016-05-28T20:59:03Z"
         "LSVE":
             site: "Lucky Strike Volcano East"
             start_date: "2015-04-22T12:00:00Z"
             end_date: "2016-05-28T21:01:00Z"
             location_code: "00"
             instrumentation:
-                base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+                base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+                modifications:
+                    datalogger: {configuration : "125sps"}
                 channel_modifications:
-                   "*-*": {datalogger: {configuration: "125sps"}}
+                   '1-00': {orientation: {'1': {azimuth.deg: {value: 154, uncertainty: 7, measurement_method: "Ppol"}}}}
+                   '2-00': {orientation: {'2': {azimuth.deg: {value: 244, uncertainty: 7, measurement_method: "Ppol"}}}}
             locations:
                 "00":
                     base: {$ref: 'location_bases/INSU-IPGP.location_base.yaml#location_base'}
-                    configuration: "ACOUSTIC_SURVEY"
+                    configuration: "SEA_SURFACE"
                     position: {lon: -32.02504, lat: 37.25744, elev: -2130}
             processing:
                 - clock_correction_linear:
-                        base: {$ref: "timing_bases/Seascan_GNSS.timing_base.yaml#timing_base"}
-                        start_sync_reference: "2015-04-21T21:06:00Z"
-                        end_sync_reference: "2016-05-28T20:59:00.32Z"
-                        end_sync_instrument: "2016-05-28T20:59:01Z"
+                    base: {$ref: 'timing_bases/Seascan_GNSS.timing_base.yaml#timing_base'}
+                    start_sync_reference: "2015-04-21T21:06:00Z"
+                    end_sync_reference: "2016-05-28T20:59:00.32Z"
+                    end_sync_instrument: "2016-05-28T20:59:01Z"
+
+notes:
+    - "An example with station orientations provided"
+    - "Provide azimuths for channels 1 and 2"
     
-notes: 
-    - "Same as SPOBS, without using YAML anchors"
-    - "Lucky Strike Volcano, North Mid-Atlantic Ridge"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -33,23 +33,23 @@
         campaign: "INSTRUMENTS"
         operator: "INSU-IPGP"
     stations:
         "SP1":
             <<: *STATION_DEFAULTS
             site: "SPOBS1 (2 channels)"
             instrumentation:
-              base: {$ref: "instrumentation_bases/SPOBS1.instrumentation_base.yaml#instrumentation_base"}
+              base: {$ref: "instrumentations/SPOBS1.instrumentation_base.yaml#instrumentation_base"}
               channel_modifications:
                 "H-00": {datalogger: {configuration: "62.5sps"}}
                 "3-00": {datalogger: {configuration: "125sps"}}
         "SP2":
             <<: *STATION_DEFAULTS
             site: "SPOBS2 (4 channels)"
             instrumentation:
-              base: {$ref: "instrumentation_bases/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
+              base: {$ref: "instrumentations/SPOBS2.instrumentation_base.yaml#instrumentation_base"}
               channel_modifications:
                 "H-00": {datalogger: {configuration: "125sps"}}
                 "1-00": {datalogger: {configuration: "250sps"}}
                 "2-00": {datalogger: {configuration: "500sps"}}
                 "3-00": {datalogger: {configuration: "1000sps"}}
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Information_Files/timing_bases/.DS_Store` & `obsinfo-0.111b1/obsinfo/_examples/Information_Files/timing_bases/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/CS5322.stage.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/CS5322.stage.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/T240.stage.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/T240.stage.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/preamplifier.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/preamplifier.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/components/sensor.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/components/sensor.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/Training/templates/network.yaml` & `obsinfo-0.111b1/obsinfo/_examples/Training/templates/network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh` & `obsinfo-0.111b1/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/_examples/scripts/validate_all.sh` & `obsinfo-0.111b1/obsinfo/_examples/scripts/validate_all.sh`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/addons/LC2SDS.py` & `obsinfo-0.111b1/obsinfo/addons/LC2SDS.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 """
 Write a script to convert LCHEAPO data to SDS* using the lcheapo** python package
 
 Includes clock drift and leap-second correction
 Script is a BASH shell script
 *SDS = SeisComp Data Structure
-**THIS PROGRAM DOES NOT CREATE DATA-CENTER QUALITY DATA:
+**THE LCHEAPO PACKAGE DOES NOT CREATE DATA-CENTER QUALITY DATA:
     - drift correction is calculated for each day, not each record
     - does not set drift correction record header flags
     - does not fill in record header time_correction field
 """
 import os.path
 from pathlib import Path
 import warnings
 
 # import obsinfo
 from obsinfo.subnetwork import Subnetwork
 from ..misc.discoveryfiles import (Datapath)
-from ..obsmetadata import (ObsMetadata)
+from ..obsMetadata.obsmetadata import (ObsMetadata)
 from .LCHEAPO import _get_ref_code
 
 SEPARATOR_LINE = "\n# " + 60 * "=" + "\n"
 
 
 def process_script(network_code, stations, station_data_path, input_dir=".",
-                   output_dir="../", include_header=True, no_drift_correct=False):
+                   output_dir="../", include_header=True):
     """
     Writes script to transform raw OBS data to SeisComp Data Structure
 
     Arguments:
         network_code (str): FDSN network_code
         stations (list of :class:`.Station`): the stations to process
         station_data_path (str): the base directory beneath the station data dirs
         input_dir (str): directory beneath station_dir for LCHEAPO data
         output_dir (str): directory beneath station_dir for SDS directory
         include_header (bool): include the header that sets up paths
                                (should be done once)
-        no_drift_correct (bool): Do NOT drift correct
     """
     fixed_dir = "lcheapo_fixed"
     s = _header(station_data_path)
     s += _run_station_function(network_code, fixed_dir, output_dir)
     for station in stations:
         # station_dir = os.path.join(station_data_path, station.label)
-        s += _run_station_call(station, no_drift_correct)
+        s += _run_station_call(station)
     return s
 
 
 def _header(station_data_path):
     s = "#!/bin/bash\n\n"
     s += f'DATA_DIR={station_data_path}\n\n'
     return s
@@ -55,15 +54,15 @@
 def _run_station_function(network_code, fixed_dir='lcheapo_fixed', output_dir="../"):
     s = ('run_station () {\n'
          '    # Run lcfix and lc2SDS_weak for one station\n'
          '    # $1: station name\n'
          '    # $2: obs type\n'
          '    # $3: reference start sync time\n'
          '    # $4: instrument start sync time [if empty, uses $3]\n'
-         '    # $5: reference end sync time [if empty, do not shift times]\n'
+         '    # $5: reference end sync time\n'
          '    # $6: obs clock end sync time\n'
          '    # $7: leap-second times [empty if none]\n'
          '    # $8: leap-second types [empty if none]\n'
          '    echo "Working on station $1"\n'
          '    STATION_DIR=$DATA_DIR/$1\n'
          '    echo "------------------------------------------------------------"\n'
          '    echo "Running LCFIX"\n'
@@ -77,29 +76,23 @@
          '    echo "Running LC2SDS_weak"\n'
          f'    mkdir -p $STATION_DIR/{output_dir}\n'
          f'    command cd $STATION_DIR/{fixed_dir}\n'
          '    lchfiles=$(command ls *.fix.lch)\n'
          '    command cd -\n'
          '    echo "lchfiles:" $lchfiles\n'
          '    if [ -z "$7" ]\n'
-         '    then  # NO LEAP-SECOND INFORMATION\n'
-         '        if [ -z "$5" ]\n'
-         '        then  # NO END SYNC, DO NOT SHIFT TIMES\n'
-         f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\""\n'
-         '        elif [ -z "$4" ]\n'
-         '        then  # NO INSTRUMENT START SYNC, ASSUME SAME AS REFERENCE\n'
+         '    then\n'
+         '        if [ -z "$4" ]\n'
+         '        then\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" --end_times \\"$5\\" \\"$6\\""\n'
-         '        else  # INSTRUMENT START SYNC SUPPLIED\n'
+         '        else\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" \\"$4\\" --end_times \\"$5\\" \\"$6\\""\n'
          '        fi\n'
-         '    else  # THERE IS LEAP-SECOND INFORMATION\n'
-         '        if [ -z "$5" ]\n'
-         '        then\n'
-         f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --leapsecond_times \\"$7\\" --leapsecond_types \\"$8\\""\n'
-         '        elif [ -z "$4" ]\n'
+         '    else\n'
+         '        if [ -z "$4" ]\n'
          '        then\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" --end_times \\"$5\\" \\"$6\\" --leapsecond_times \\"$7\\" --leapsecond_types \\"$8\\""\n'
          '        else\n'
          f'            cmd="lc2SDS_weak $lchfiles -d \\"$STATION_DIR\\" -i \\"{fixed_dir}\\" -o \\"{output_dir}\\" --network \\"{network_code}\\" --station \\"$1\\" --obs_type \\"$2\\" --start_times \\"$3\\" \\"$4\\" --end_times \\"$5\\" \\"$6\\" --leapsecond_times \\"$7\\" --leapsecond_types \\"$8\\""\n'
          '        fi\n'
          '    fi\n'
          '    echo "Running: $cmd"\n'
@@ -107,22 +100,21 @@
          '    echo "------------------------------------------------------------"\n'
          '    echo "Removing intermediate files"\n'
          f'    command rm -r $STATION_DIR/{fixed_dir}\n'
          '}\n\n')
     return s
 
 
-def _run_station_call(station, no_drift_correct):
+def _run_station_call(station):
 
     """
     Write a call to the run_station() function
 
     Args:
         station (:class:`.Station`): station information
-        no_drift_correct (bool): do NOT drift correct
     Returns:
         s (str): single-line call
     """
     station_code = station.label
     obs_type = _get_ref_code(station.instrumentation)
     leaptimes, leaptypes = [], []
     ccld = None
@@ -146,18 +138,15 @@
         end_sync_ref = ccld["end_sync_reference"]
         end_sync_inst = ccld["end_sync_instrument"]
     if leaptimes:
         raise ValueError("the network file provides leapseconds: run_station can't (yet) handle that")
         leaptimes_str = " ".join(leaptimes)
         leaptypes_str = " ".join(leaptypes)
     s = f'run_station "{station_code}" "{obs_type}" '
-    if no_drift_correct is True:
-        s += '"" "" "" "" '
-    else:
-        s += f'"{start_sync_ref}" "{start_sync_inst}" "{end_sync_ref}" "{end_sync_inst}" '
+    s += f'"{start_sync_ref}" "{start_sync_inst}" "{end_sync_ref}" "{end_sync_inst}" '
     s += f'"{leaptimes_str}" "{leaptypes_str}"\n'
 
     return s
 
 
 def _console_script(argv=None):
     """
@@ -184,16 +173,14 @@
                              "(default: %(default)s)")
     # parser.add_argument("--append", action="store_true",
     #                     help="append to existing script file")
     parser.add_argument("-v", "--verbose", action="store_true",
                         help="increase output verbosity")
     parser.add_argument("--no_header", action="store_true",
                         help="do not include a script header")
-    parser.add_argument("--no_drift_correct", action="store_true",
-                        help="do not correct for instrument drift")
     parser.add_argument("-q", "--quiet", action="store_true",
                         help="run silently")
     args = parser.parse_args()
 
     if not args.quiet:
         print("Creating LC2SDS_weak process script, ", end="", flush=True)
 
@@ -217,16 +204,15 @@
 
     # scripts = []
     # first_time = True
     script = process_script(subnetwork.fdsn_code,
                             subnetwork.stations,
                             args.station_data_path,
                             input_dir=args.input_dir,
-                            output_dir=args.output_dir,
-                            no_drift_correct=args.no_drift_correct)
+                            output_dir=args.output_dir)
     if not args.quiet:
         print(', '.join([s.label for s in subnetwork.stations]))
     fname = "process" + args.suffix + ".sh"
     if args.verbose:
         print(f" ... writing file {fname}", flush=True)
     with open(fname, 'w') as f:
         f.write(script)
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/addons/LCHEAPO.py` & `obsinfo-0.111b1/obsinfo/addons/LCHEAPO.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Write extraction script for LCHEAPO instruments (proprietary to miniseed)
 """
 # import obsinfo
 from obsinfo.subnetwork import Subnetwork
 from ..misc.discoveryfiles import (Datapath)
-from ..obsmetadata import (ObsMetadata)
+from ..obsMetadata.obsmetadata import (ObsMetadata)
 from pathlib import Path
 import os.path
 
 SEPARATOR_LINE = "\n# " + 60 * "=" + "\n"
 
 
 def process_script(network_code,
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/addons/OCA.py` & `obsinfo-0.111b1/obsinfo/addons/OCA.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/addons/SDPCHAIN.py` & `obsinfo-0.111b1/obsinfo/addons/SDPCHAIN.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/addons/infodump.py` & `obsinfo-0.111b1/obsinfo/addons/infodump.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/console_scripts/_test.py` & `obsinfo-0.111b1/obsinfo/console_scripts/_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,33 +62,31 @@
 from logging.handlers import RotatingFileHandler
 
 # Third party  imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import Site
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
-                               Stages, Stage, Location)
-from ..network import (Station, Subnetwork)
-from ..instrumentation.filter import (Filter, PolesZeros, FIR,
-                                      Coefficients, ResponseList)
-from ..misc.printobs import PrintObs
-from ..misc.discoveryfiles import Datapath
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
+                                     Stages, Stage, Location)
+from obsinfo.network import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (Filter, PolesZeros, FIR,
+                                            Coefficients, ResponseList)
+from obsinfo.misc.printobs import PrintObs
+from obsinfo.misc.discoveryfiles import Datapath
 # import obsinfo
-from ..misc.const import (EXIT_SUCCESS, EXIT_FAILURE, EXIT_NOINPUT,
-                          EXIT_SOFTWARE, EXIT_DATAERR, EXIT_UNAVAILABLE)
-from ..helpers import init_logging
+from obsinfo.misc.const import (EXIT_SUCCESS, EXIT_FAILURE, EXIT_NOINPUT,
+                                EXIT_SOFTWARE, EXIT_DATAERR, EXIT_UNAVAILABLE)
+# from obsinfo.misc.configuration import Singleton
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = False
 
-logger = init_logging("test")
-
 
 class JsonRefTest(unittest.TestCase):
     """
     Class of test methods for information file format
 
     Attributes:
         testing_path (str): path to datafiles to be tested aside from the examples
@@ -1316,14 +1314,15 @@
 
     """
 
     args = retrieve_arguments()
     tst = TestObsinfo()
     tst.setUp(test=False, print_output=True, level=args.level)
     # dp = Datapath()
+    logger = init_logging()
 
     try:
 
         type = ObsMetadata.get_information_file_type(args.input_filename)
 
         print(f'Printing {type} file: {args.input_filename}')
 
@@ -1339,16 +1338,14 @@
             tst._test_sensor(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "instrumentation":
             tst._test_instrumentation(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "station":
             tst._test_station(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "network":
             tst._test_network(tst.infofiles_path.build_datapath(args.input_filename))
-        else:
-            logger.warning(f'Could not find type of {args.input_filename}')
 
     except TypeError:
         print("Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         logger.error("TypeError: Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         if args.debug:
             raise
         sys.exit(EXIT_DATAERR)
@@ -1424,7 +1421,28 @@
 
     args = parser_args.parse_args()
 
     if not Path(args.input_filename[0]).is_absolute():
         args.input_filename = str(Path(os.getcwd()).joinpath(args.input_filename[0]).resolve())
 
     return args
+
+
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/console_scripts/makeStationXML.py` & `obsinfo-0.111b1/obsinfo/console_scripts/makeStationXML.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,37 @@
 # General library imports
 import sys
 import os
 # import re
 import warnings
 
 from pathlib import Path  # , PurePath
+# from json.decoder import JSONDecodeError
+import logging
+from logging.handlers import RotatingFileHandler
 
 from argparse import ArgumentParser
 
 # Third party imports
 # import obspy
 from obspy.core.inventory import Inventory  # , Station, Channel, Site
 from obspy.core.inventory import Network
 # from obspy.clients.nrl import NRL
 
 # obsinfo imports
 from ..subnetwork import (Subnetwork)
-from ..obsmetadata import (ObsMetadata)
+from ..obsMetadata.obsmetadata import (ObsMetadata)
 from ..misc.discoveryfiles import (Datapath)
 from .print_version import main as print_version
+import obsinfo
 from ..misc.const import EXIT_USAGE, EXIT_SUCCESS
-from ..helpers import init_logging
+# from ..misc.configuration import ObsinfoConfiguration
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
-logger = init_logging("makeStationXML")
 
 
 def main(argv=None, dp=None):
     """
     Entry point for obsinfo-makeStationXML.
 
      1) Setups status variables from command line arguments.
@@ -53,14 +56,15 @@
             If None, will use values specified in .obsinforc
     """
 
     # create list of directories to search for files
     if dp is None:
         dp = Datapath()
     args = retrieve_arguments(argv, dp)
+    logger = init_logging()
 
     if args.verbose:
         print(f'Using OBSINFO_DATAPATH: {dp.datapath_list}')
 
     logger.info(f'Using OBSINFO_DATAPATH: {dp.datapath_list}')
 
     _make_StationXML(logger, args, dp)
@@ -175,24 +179,46 @@
         args = parser_args.parse_args()
 
     if args.version:
         print_version()
         sys.exit(EXIT_SUCCESS)
 
     # schemas must always be installed under obsinfo/data/schemas
-    args.schemapath = Path(__file__).parent.joinpath('data', 'schemas')
+    args.schemapath = Path(obsinfo.__file__).parent.joinpath('data', 'schemas')
 
     if not args.input_filename:
         print("No input filename specified")
         sys.exit(EXIT_USAGE)
 
     input_filename = args.input_filename[0]
 
     args.input_filename = str(datapath.build_datapath(input_filename)
                               if args.remote
                               else Path(os.getcwd()).joinpath(input_filename))
 
     return args
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-makeStationXML')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/console_scripts/print.py` & `obsinfo-0.111b1/obsinfo/console_scripts/print.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 Application to print obsinfo information files.
 """
 import os
 import warnings
 from pathlib import Path
 from argparse import ArgumentParser
 
+import logging
+from logging.handlers import RotatingFileHandler
+
 # obsinfo modules
-from ..obsmetadata import ObsMetadata
-from ..instrumentation import (Instrumentation, Stage, Filter,
+import obsinfo
+from obsinfo.obsMetadata.obsmetadata import ObsMetadata
+from obsinfo.instrumentation import (Instrumentation, Stage, Filter,
                                      Preamplifier, Sensor, Datalogger)
-from ..helpers import Location, Locations, Person, init_logging
-from ..subnetwork import (Subnetwork, Network, Operator)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.helpers import Location, Locations, Person
+from obsinfo.subnetwork import (Subnetwork, Operator)
+from obsinfo.misc.discoveryfiles import Datapath
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = False
 
-logger = init_logging("print", console_level='WARNING')
-
 
 def print_single_file(info_file, n_sublevels=0, configs=False, verbose=True):
     """
     Print a single obsinfo file.
 
     Args:
         info_file (str): info file to validate.
@@ -40,16 +42,14 @@
         print(str(e))
         return False
     if configs is not True:
         print(f'{Path(info_file).name}: ', end='', flush=True)
         no_class_msg = f"Can't print {filetype} files (no associated class)"
         if filetype == 'subnetwork':
             obj = Subnetwork(attributes_dict[filetype])
-        elif filetype == 'network':
-            obj = Network(attributes_dict[filetype])
         elif filetype == 'instrumentation_base':
             location_code='00'
             locations = Locations(
                 [Location({'position': {'lat': 0, 'lon': 0, 'elev': 0},
                            'base': {'uncertainties.m': {'lat': 0, 'lon': 0, 'elev':0},
                                     'depth.m': 0,
                                     'geology': 'seafloor',
@@ -62,33 +62,31 @@
         elif filetype == 'datalogger_base':
             obj = Datalogger({'base': attributes_dict[filetype]})
         elif filetype == 'sensor_base':
             obj = Sensor({'base': attributes_dict[filetype]})
         elif filetype == 'preamplifier_base':
             obj = Preamplifier({'base': attributes_dict[filetype]})
         elif filetype == 'location_base':
-            obj = Location({'base': attributes_dict[filetype],
-                             'position': {'lat': 0, 'lon': 0, 'elev': 0}})
+            obj = Location({'base': attributes_dict[filetype]})
         elif filetype == 'stage_base':
             obj = Stage({'base': attributes_dict[filetype]})
         elif filetype == 'network':
             print(no_class_msg)
             return
         elif filetype == 'operator':
             obj = Operator(attributes_dict[filetype])
         elif filetype == 'filter':
-            obj = Filter.construct(attributes_dict[filetype], 1, 'print')
+            obj = Filter.construct(attributes_dict[filetype])
         elif filetype == 'person':
             obj = Person(attributes_dict[filetype])
         elif filetype == 'timing_base':
             print(no_class_msg)
             return
         else:
             print(f"Unknown information file type: '{filetype}")
-            return
         print("\n    " + obj.__str__(indent=4, n_subclasses=n_sublevels))
     else:
         if filetype in ('instrumentation_base', 'datalogger_base',
                         'sensor_base' 'preamplifier_base',
                         'location_base', 'stage_base', 'timing_base'):
             configs = attributes_dict[filetype].get('configurations', {})
             keys = list(configs.keys())
@@ -98,15 +96,15 @@
         else:
             if verbose:
                 print(f'{Path(info_file).name}: ', end='', flush=True)
                 print(f"file type: '{filetype}' has no configurations")
             return
 
 
-def print_directory(info_dir, n_sublevels=1, configs=False,
+def print_directory(info_dir, n_sublevels=False, configs=False,
                     drilldown=False, verbose=False):
     """
     Validate all information files in a directory.
 
     Args:
         info_dir (:class:`Path`): directory where files reside
         drilldown (bool): drill down through subdirectories
@@ -186,17 +184,40 @@
                              "--n_sublevels=0)")
 
     args = parser.parse_args()
 
     if args.input == 'DATAPATH':
         args.input = Datapath().datapath_list[0]
         args.drilldown = True
+        args.n_levels = 0
         print('Validating first DATAPATH dir')
     args.input = Path(args.input)
     if not args.input.is_absolute():
         args.input = Path(os.getcwd()).joinpath(args.input).resolve()
 
     return args
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s',
+                             datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/console_scripts/setup.py` & `obsinfo-0.111b1/obsinfo/console_scripts/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 # import sys
 import re
 # import site
 import shutil
 import datetime
 import platform
 from pathlib import Path
+# import logging
 import warnings
 
 from argparse import ArgumentParser
 
+import obsinfo
 from ..misc.const import EXIT_IOERR
-from ..version import __version__
-from ..helpers import init_logging
-
-logger = init_logging("setup")
+from obsinfo.version import __version__
 
 
 def main():
     """
     Entry point to configure variables in file .obsinforc
 
     and to copy examples and templates out of the distribution directories
     """
     # initialize variables
     version = platform.python_version()
-    path_to_package = Path(__file__).parent.parent
+    path_to_package = Path(obsinfo.__file__).parent
     examples_dir = path_to_package.joinpath("_examples/Information_Files")
     templates_dir = path_to_package.joinpath("templates")
     home = Path.home()
     configuration_file = home.joinpath('.obsinforc')
 
     args = retrieve_arguments()
 
@@ -54,17 +53,16 @@
                 os.rename(dest, new_dest)
 
             shutil.copytree(examples_dir, dest.joinpath("Information_Files"))
             shutil.copytree(templates_dir, dest.joinpath("templates"))
         except NotADirectoryError:
             print("Directory not found")
             exit(EXIT_IOERR)
-        except OSError as e:
+        except OSError:
             print("Operating system error")
-            print(e)
             exit(EXIT_IOERR)
     # create configuration file
     output = []
 
     output.append("gitlab_repository: " + args.gitlab + "\n")
     output.append("gitlab_project: " + args.project + "\n")
     output.append("gitlab_path: " + args.remote_path + "\n")
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/console_scripts/validate.py` & `obsinfo-0.111b1/obsinfo/console_scripts/validate.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 """
 import os
 from pathlib import Path
 import glob
 import re
 import sys
 from argparse import ArgumentParser
+import logging
+from logging.handlers import RotatingFileHandler
 
-from ..misc.discoveryfiles import Datapath
-from ..obsmetadata import ObsMetadata
-from ..misc.const import EXIT_SUCCESS
-from ..helpers import init_logging
+from obsinfo.misc.discoveryfiles import Datapath
+import obsinfo
+from obsinfo.obsMetadata.obsmetadata import ObsMetadata
+from obsinfo.misc.const import EXIT_SUCCESS
 
-logger = init_logging("validate")
 
 class ValidateObsinfo():
     """
     Methods to validate each level of information files.
 
     Attributes:
         datapath (:class:`/.Datapath`): Store datapath list(s)
@@ -44,15 +45,15 @@
             debug (bool): Print more detailed messages and enable traceback
                 of exceptions
         Returns: self
         """
         dp = Datapath()
         self.datapath = dp
         self.datapath.infofiles_path = dp.datapath_list
-        self.datapath.validate_path = Path(__file__).parent.parent.joinpath('data', 'schemas')
+        self.datapath.validate_path = Path(obsinfo.__file__).parent.joinpath('data', 'schemas')
 
         self.verbose = verbose
         self.remote = remote
         self.debug = debug
 
         return self
 
@@ -67,15 +68,15 @@
             filetype (str): the information file type
             file_format (str): the information file format ('json' or 'yaml')
             check_schema (bool): validate schema file as well
         Returns:
             (bool): True if validated, False if not
         """
         if file_format not in ('json', 'yaml'):
-            logger.error('file_format ("{file_format}") not in ("json", "yaml")')
+            logging.error('file_format ("{file_format}") not in ("json", "yaml")')
             raise ValueError('file_format ("{file_format}") not in ("json", "yaml")')
         try:
             ret = ObsMetadata().validate(info_file,
                                          self.datapath.validate_path,
                                          self.remote,
                                          file_format,
                                          filetype,
@@ -100,15 +101,15 @@
             forced_filetype (str): file type.  If None, determine it.
             drilldown (bool): drill down through directories beneath the specified one
             continue_on_fail (bool): continue testing if a validation fails
             check_schema (bool): check schema on first use
         Returns:
             false if any file failed
         """
-        suffixes = ['.yaml', '.json']
+        suffixes = ['.yaml', '.yml']
         checked_schemas = []
         if not dir.is_dir():
             raise ValueError(f'"{dir}" is not a directory!')
         if drilldown is True:
             print(f'Validating files in and below directory {dir}')
             if forced_filetype is not None:
                 raise ValueError('Cannot specify filetype when drilling down '
@@ -126,16 +127,17 @@
         results = {'passed': 0, 'failed': 0, 'skipped': 0}
         for file in files:
             if file.suffix.lower() not in suffixes:
                 print(f'Skipping {str(file.relative_to(dir))}')
                 results['skipped'] += 1
                 continue
             if forced_filetype==None:
-                filetype = ObsMetadata.get_information_file_type(str(file))
-                if filetype is None:
+                try:
+                    filetype = ObsMetadata.get_information_file_type(str(file))
+                except Exception:
                     print(f"Could not find a schema for {str(file.relative_to(dir))}, skipping...")
                     results['skipped'] += 1
                     continue
             print(f"Validating {str(file.relative_to(dir))} against "
                   f"{filetype}.schema.json ... ", end='', flush=True)
             if check_schema is True:
                 if filetype in checked_schemas: 
@@ -269,14 +271,15 @@
     Entry point for obsinfo-validate.
 
      1) Sets up status variables from command line arguments.
      2) Validates file according to file type contained in name
      3) Manages all uncaught exceptions
     """
     args = retrieve_arguments()
+    # logger = init_logging()
 
     val = ValidateObsinfo()
     val.setUp(verbose=args.verbose, remote=args.remote, debug=args.debug)
 
     filetype = None
     if args.schema:
         if ObsMetadata.is_valid_type(args.schema):
@@ -294,14 +297,72 @@
     elif args.input.is_dir():
         if args.schema and args.drilldown:
             raise ValueError("Cannot specify schema for a drill-down "
                              "directory validation")
         val.validate_directory(args.input, filetype, args.drilldown,
                                args.continue_on_fail, check_schema=args.check_schema)
 
+#     try:
+#         val.validate_single_file(input_filename, filetype)
+#     except TypeError as e:
+#         print("TypeError:" + str(e))
+#         logger.error("TypeError: Illegal format: fields may be missing or "
+#                      "with wrong format in input file, or there is a "
+#                      "programming error")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_DATAERR)
+#     except (KeyError, IndexError) as e:
+#         print("Illegal value in dictionary key or list index:" + str(e))
+#         logger.error("KeyError, IndexError: Illegal value in dictionary key "
+#                      "or list index")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_SOFTWARE)
+#     except ValueError as e:
+#         print("ValueError:" + str(e))
+#         logger.error("ValueError: An illegal value was detected")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_DATAERR)
+#     except FileNotFoundError as e:
+#         if args.debug:
+#             raise
+#         print("File not found:" + str(e))
+#         logger.error(f"FileNotFoundError: {str(e)}")
+#         sys.exit(EXIT_NOINPUT)
+#     except JSONDecodeError as e:
+#         print("JSONDecodeError:" + str(e))
+#         logger.error("JSONDecodeError: File and/or subfiles have an illegal "
+#                      "format. Probably indentation or missing "
+#                      "quotes/parentheses/brackets")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_DATAERR)
+#     except (IOError, OSError, LookupError) as e:
+#         print("File could not be opened or read:" + str(e))
+#         logger.error("IOError, OSError, LookupError: File could not be "
+#                      "opened or read")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_UNAVAILABLE)
+#     except AttributeError as e:
+#         print("Attribute error: " + str(e))
+#         logger.debug("AttributeError: Programming error: an object in code "
+#                      "had a wrong attribute")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_SOFTWARE)
+#     except:
+#         print("General exception")
+#         logger.debug("General exception:")
+#         if args.debug:
+#             raise
+#         sys.exit(EXIT_FAILURE)
+#
     sys.exit(EXIT_SUCCESS)
 
 
 def retrieve_arguments():
     """
     Retrieve command line arguments.
 
@@ -357,9 +418,31 @@
     args.input = Path(args.input)
     if not args.input.is_absolute():
         args.input = Path(os.getcwd()).joinpath(args.input).resolve()
 
     return args
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+
+    :returns: object of Logger class
+    """
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+
+    logger = logging.getLogger("obsinfo")
+
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s',
+                             datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)
+
+    return logger
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/datacite.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/datacite.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/datalogger_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/datalogger_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/definitions.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/definitions.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/experiment.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/experiment.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/filter.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/filter.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/instrumentation_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/instrumentation_base.schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990174002715121%*

 * *Differences: {"'definitions'": "{'instrumentation': {'properties': {delete: ['datalogger_configuration']}}, "*

 * *                  "'modifications': {'properties': {'datalogger': OrderedDict([('$ref', "*

 * *                  "'datalogger_base.schema.json#/definitions/modifications')]), 'preamplifier': "*

 * *                  "OrderedDict([('$ref', "*

 * *                  "'preamplifier_base.schema.json#/definitions/modifications')]), 'sensor': "*

 * *                  "OrderedDict([('$ref', "*

 * *                  "'sensor_base.schema.json#/de […]*

```diff
@@ -85,38 +85,14 @@
                 "^[N, E, Z, 1, 2, 3, H, \\*]-[0-9, \\*]+$": {
                     "$ref": "#/definitions/channel_modif"
                 }
             },
             "type": "object"
         },
         "channel_properties": {
-            "^comments": {
-                "$ref": "definitions.schema.json#/comments"
-            },
-            "^datalogger": {
-                "$ref": "datalogger_base.schema.json#/definitions/modifications"
-            },
-            "^external_references": {
-                "$ref": "definitions.schema.json#external_references"
-            },
-            "^extras": {
-                "$ref": "definitions.schema.json#/extras"
-            },
-            "^identifiers": {
-                "$ref": "definitions.schema.json#identifiers"
-            },
-            "^orientation": {
-                "$ref": "#/definitions/orientation"
-            },
-            "^preamplifier": {
-                "$ref": "preamplifier_base.schema.json#/definitions/modifications"
-            },
-            "^sensor": {
-                "$ref": "sensor_base.schema.json#/definitions/modifications"
-            },
             "comments": {
                 "$ref": "definitions.schema.json#/comments"
             },
             "datalogger": {
                 "$ref": "datalogger_base.schema.json#/definitions/modifications"
             },
             "external_references": {
@@ -231,17 +207,14 @@
                 },
                 "configuration": {
                     "type": [
                         "string",
                         "null"
                     ]
                 },
-                "datalogger_configuration": {
-                    "type": "string"
-                },
                 "modifications": {
                     "$ref": "#/definitions/modifications"
                 },
                 "notes": {
                     "$ref": "definitions.schema.json#/note_list"
                 },
                 "serial_number": {
@@ -275,17 +248,26 @@
                 },
                 "configuration": {
                     "type": [
                         "string",
                         "null"
                     ]
                 },
+                "datalogger": {
+                    "$ref": "datalogger_base.schema.json#/definitions/modifications"
+                },
                 "equipment": {
                     "$ref": "definitions.schema.json#/equipment"
                 },
+                "preamplifier": {
+                    "$ref": "preamplifier_base.schema.json#/definitions/modifications"
+                },
+                "sensor": {
+                    "$ref": "sensor_base.schema.json#/definitions/modifications"
+                },
                 "serial_number": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
         "orientation": {
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/iris_units.json` & `obsinfo-0.111b1/obsinfo/data/schemas/iris_units.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/location_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/location_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/network.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/network.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/operator.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/operator.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/person.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/person.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/preamplifier_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/preamplifier_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/sensor_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/sensor_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/stage_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/stage_base.schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996395661630036%*

 * *Differences: {"'definitions'": "{'base_properties': {'properties': {'calibration_date': OrderedDict([('$ref', "*

 * *                  "'definitions.schema.json#/date')]), delete: ['calibration_dates']}}, "*

 * *                  "'modifications': {'properties': {'calibration_date': OrderedDict([('$ref', "*

 * *                  "'definitions.schema.json#/date')]), delete: ['calibration_dates']}}, 'base': "*

 * *                  "{'properties': {'calibration_date': OrderedDict([('$ref', "*

 * *                  "'definitions.schema.json#/date' […]*

```diff
@@ -2,16 +2,16 @@
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": false,
     "definitions": {
         "base": {
             "additionalProperties": false,
             "description": "Response stage",
             "properties": {
-                "calibration_dates": {
-                    "$ref": "definitions.schema.json#calibration_dates_def"
+                "calibration_date": {
+                    "$ref": "definitions.schema.json#/date"
                 },
                 "configuration_default": {
                     "type": "string"
                 },
                 "configurations": {
                     "$ref": "#/definitions/configurations_map"
                 },
@@ -61,16 +61,16 @@
                 "filter"
             ],
             "type": "object"
         },
         "base_properties": {
             "description": "list of common properties in {element}, modifications, base, and configuration_definition.  This is unused because 'allOf' for makes ugly schema validation",
             "properties": {
-                "calibration_dates": {
-                    "$ref": "definitions.schema.json#calibration_dates_def"
+                "calibration_date": {
+                    "$ref": "definitions.schema.json#/date"
                 },
                 "decimation_factor": {
                     "description": "DecimationType:Factor",
                     "type": "integer"
                 },
                 "delay": {
                     "description": "DecimationType:Delay",
@@ -108,16 +108,16 @@
                 }
             }
         },
         "configuration_definition": {
             "additionalProperties": false,
             "description": "Configuration-specific properties",
             "properties": {
-                "calibration_dates": {
-                    "$ref": "definitions.schema.json#calibration_dates_def"
+                "calibration_date": {
+                    "$ref": "definitions.schema.json#/date"
                 },
                 "configuration_description": {
                     "type": "string"
                 },
                 "decimation_factor": {
                     "description": "DecimationType:Factor",
                     "type": "integer"
@@ -187,16 +187,16 @@
         "modifications": {
             "additionalProperties": false,
             "description": "Allowed stage modifications",
             "properties": {
                 "base": {
                     "$ref": "#/definitions/base"
                 },
-                "calibration_dates": {
-                    "$ref": "definitions.schema.json#calibration_dates_def"
+                "calibration_date": {
+                    "$ref": "definitions.schema.json#/date"
                 },
                 "configuration": {
                     "type": [
                         "string",
                         "null"
                     ]
                 },
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/stages.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/stages.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/subnetwork.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/subnetwork.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/data/schemas/timing_base.schema.json` & `obsinfo-0.111b1/obsinfo/data/schemas/timing_base.schema.json`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/__init__.py` & `obsinfo-0.111b1/obsinfo/helpers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 Helper classes, used by other classes
 """
-# noqa: F401 disables flake8 warning that imported modules are unused
 from .float_with_uncert import FloatWithUncert        # noqa: F401
 from .location import Location, Locations             # noqa: F401
-from .oi_date import OIDate, OIDates                  # noqa: F401
+from .oi_date import OIDate                           # noqa: F401
 from .comments import Comments                        # noqa: F401
 from .obsinfo_class_list import ObsinfoClassList      # noqa: F401
-from .functions import (str_indent, str_list_str, verify_dict_is_empty) # noqa: F401
+from .functions import (str_indent, str_list_str, verify_dict_is_empty)        # noqa: F401
 from .person import Person, Persons                   # noqa: F401
 from .phone import Phone, Phones                      # noqa: F401
 from .external_references import ExternalReferences   # noqa: F401
-from .identifiers import Identifiers                  # noqa: F401
-from .logger import init_logging                      # noqa: F401
+from .identifiers import Identifiers      # noqa: F401
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/comments.py` & `obsinfo-0.111b1/obsinfo/helpers/comments.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/external_references.py` & `obsinfo-0.111b1/obsinfo/helpers/external_references.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             Args:
                 attributes_list: (list of dict or str): list
                     of external references read from YAML/JSON file
         """
         if attributes_list is None:
             super().__init__([], ExternalReference)
         else:
-            super().__init__(attributes_list, ExternalReference)
+            super().__init__([ExternalReference(x) for x in attributes_list])
 
 
 class ExternalReference(object):
     def __init__(self, attributes_dict):
         self.uri = attributes_dict.pop('uri')
         self.description = attributes_dict.pop('description')
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/float_with_uncert.py` & `obsinfo-0.111b1/obsinfo/helpers/float_with_uncert.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/functions.py` & `obsinfo-0.111b1/obsinfo/helpers/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from textwrap import indent
 import inspect
-import logging
-
-logger = logging.getLogger("obsinfo")
 
 def str_indent(s, nchars: int):
     """
     Indents all lines of a string by a given # of spaces
 
     Normally indents all but the first line, if nchars is negative then indents
     all lines including the first, by -nchars
@@ -32,28 +29,25 @@
         indent (int):  # of characters to indent by
         n_subclasses (int): if < 0, return a one-line string
     """
     if slist is None:
         return 'None'
 
     if n_subclasses < 0:
-        if len(slist) == 0:
-            return '[]'
-        elif len(slist) == 1:
-            return f'["{slist[0]}"]'
-        return f'List of {len(slist)} strings'
+        return f'{len(slist)} strings'
+    
     s = 'List of strings:'
     for x in slist:
         s += f'\n- {x}'
     return str_indent(s, indent)
 
 
 def verify_dict_is_empty(attributes_dict):
     if len(attributes_dict) == 0:
         return
     stack = inspect.stack()
     the_class = stack[1][0].f_locals["self"].__class__.__name__
     the_method = stack[1][0].f_code.co_name
-    logger.error(f'attributes dict in {the_class}.{the_method} has '
+    raise ValueError(f'attributes dict in {the_class}.{the_method} has '
                      f'leftover keys: {list(attributes_dict.keys())}')
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/identifiers.py` & `obsinfo-0.111b1/obsinfo/helpers/identifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             Args:
                 attributes_list: (list of dict or str): list
                     of external references read from YAML/JSON file
         """
         if attributes_list is None:
             super().__init__([], Identifier)
         else:
-            super().__init__(attributes_list, Identifier)
+            super().__init__([Identifier(x) for x in attributes_list])
 
 
 class Identifier(object):
     """
     A type to document persistent identifiers. Must provide a scheme (prefix)
     """
     def __init__(self, uri):
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/location.py` & `obsinfo-0.111b1/obsinfo/helpers/location.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 # Standard library modules
 import warnings
 import numpy as np
 import logging
 
 from .float_with_uncert import FloatWithUncert
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .functions import str_indent
 from .obsinfo_class_list import ObsinfoClassList
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
@@ -66,22 +66,22 @@
         if code is not None:
             if 'code' in attributes_dict:
                 raise ValueError('provided location code as argument AND dict key')
             else:
                 attributes_dict['code'] = code
 
         position = attributes_dict.pop('position', None)
-        if position is None:
+        if not position:
             msg = 'No position in location'
             warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
-        self._lat = position.pop('lat')
-        self._lon = position.pop('lon')
-        self._elev = position.pop('elev')
+        self._lat = position.get('lat', None)
+        self._lon = position.get('lon', None)
+        self._elev = position.get('elev', None)
         self._position = position  # for __repr__()
         self.code = attributes_dict.pop('code', None)
 
         # Get base-config elements
         base_dict = attributes_dict.get_configured_modified_base()
         self.geology = base_dict.get('geology', None)
         self.vault = base_dict.get('vault', None)
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/obsinfo_class_list.py` & `obsinfo-0.111b1/obsinfo/helpers/obsinfo_class_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,57 +13,70 @@
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class ObsinfoClassList(list):
-    def __init__(self, seq, element_class):
+    def __init__(self, seq, element_class=None):
         """
         Args:
             seq (list or None): sequence of dicts or of :class:element_class.
                 If dicts, converts to element_class type using element_class()
                 If None, return empty instance
             element_class (:class:): the class that every element should be
                 (or become)
         """
         if seq is not None and not isinstance(seq, list):
             raise TypeError(f'seq ({type(seq)}) is neither a list nor None')
         # Validate element_class
-        if not inspect.isclass(element_class):
-            raise TypeError('element_class is not a class')
-        self.element_class = element_class
-        
+        if element_class is None:
+            if seq is None:
+                raise ValueError('You did not provide an element_class to '
+                                 'instantiate the empty input seq')            
+            elif len(seq) == 0:
+                raise ValueError('You did not provide an element_class to '
+                                 'instantiate the empty input seq')            
+            elif isinstance(seq[0], dict):        
+                raise ValueError('You did not provide an element_class to '
+                                 'translate the dicts in the input sequence')
+        else:
+            if not inspect.isclass(element_class):
+                raise TypeError('element_class is not a class')
+
         if seq is None:
             super().__init__([])
+            self.element_class = element_class
             return
         elif len(seq) == 0:
             super().__init__([])
+            self.element_class = element_class
             return
         
         # Verify all elements are of same type
         for x in seq:
             if not isinstance(x, type(seq[0])):
                 raise TypeError(f'seq elements are not all of same type '
                                 f'({type(x)} != {type(seq[0])})')
 
-        if not isinstance (seq[0], element_class):
+        if isinstance (seq[0], dict):
             seq = [element_class(x) for x in seq]
 
         super().__init__(x for x in seq)
-
+        self.element_class = self[0].__class__
+        
     def append(self, item):
         if not isinstance(item, self.element_class):
             item = element_class(item)
         super().append(item)
 
     def __str__(self, indent=0, n_subclasses=0):
         s = f'{self.__class__.__name__}:'
         if len(self) == 0:
-            return s + ' []'
+            return s + ' Empty'
         elif len(self) == 1:
             return s + f' [{self[0].__str__(4, n_subclasses-1)}]'
         if n_subclasses < 0:
             return s + f' {len(self)} {self.element_class}s'
         for x in self:
             s += f'\n    - {x.__str__(indent=8, n_subclasses=n_subclasses-1)}'
         return str_indent(s, indent)
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/person.py` & `obsinfo-0.111b1/obsinfo/helpers/person.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/helpers/phone.py` & `obsinfo-0.111b1/obsinfo/helpers/phone.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/__init__.py` & `obsinfo-0.111b1/obsinfo/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/channel.py` & `obsinfo-0.111b1/obsinfo/instrumentation/channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 
 # Non-standard modules
 from obspy.core.inventory.channel import Channel as obspy_Channel
 from obspy.core.inventory.util import Comment
 
 # obsinfo modules
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from ..helpers import (Location, OIDate, str_indent, verify_dict_is_empty,
                        Comments, ExternalReferences, Identifiers, ObsinfoClassList)
 from .orientation import Orientation
 from .instrument import Instrument
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
@@ -63,16 +63,16 @@
             ic_modifs (dict or :class:`ObsMetadata`): modifications to pass
                 through to InstrumentComponents
             location (:class:`Location`): channel location
             equipment (:class:`Equipment`): channel equipment
         """
         # For __repr__
         self.input = {
-                      'attributes_dict':   {} if not attributes_dict else '<ObsMetaData>',
-                      'ic_modifs':   {} if not ic_modifs else '<ObsMetaData>',
+                      'attributes_dict':   {} if not attributes_dict else '<obsinfo.ObsMetaData>',
+                      'ic_modifs':   {} if not ic_modifs else '<obsinfo.ObsMetaData>',
                       'location': location,
                       'equipment': '<obsinfo.Equipment>'
                      }
 
         orientation = attributes_dict.pop('orientation', None)
         o_code = self._get_orientation_code(orientation)
         self.equipment = equipment
@@ -110,23 +110,21 @@
     def __str__(self, indent=0, n_subclasses=0):
         """
         Args:
             indent (int): number of extra characters to indent lines by
             n_subclasses (int): number of levels of subclass to print out
         """
         if n_subclasses < 0:
-            if self.location is not None:
-                return f'{self.__class__.__name__} {self.location.code}.{self.seed_code}'
-            else:
-                return f'{self.__class__.__name__} {self.seed_code}'
+            return self.__class__.__name__
 
         kwargs = {'indent': 4, 'n_subclasses': n_subclasses-1}
-        s = f'{self.__class__.__name__} {self.seed_code}:\n'
-        if self.location is not None:
-            s += f'    location: {self.location.__str__(**kwargs)}\n'
+        s = f'Channel {self.seed_code}:\n'
+        s += f'    location code: {self.location.code}\n'
+        # Force print of at least location.__str__() and orientation.__str__()
+        s += f'    location: {self.location.__str__(**kwargs)}\n'
         s += f'    orientation: {self.orientation.__str__(**kwargs)}\n'
         s += f'    start_date: {self.start_date}\n'
         s += f'    end_date: {self.end_date}\n'
         s += f'    equipment: {self.equipment.__str__(**kwargs)}\n'
         s += f'    comments: {self.comments}\n'
         s += f'    equipment: {self.instrument.__str__(**kwargs)}\n'
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/equipment.py` & `obsinfo-0.111b1/obsinfo/instrumentation/equipment.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import logging
 
 # Non-standard modules
 from obspy.core.inventory.util import Equipment as obspy_Equipment
 from obspy.core.utcdatetime import UTCDateTime
 
 # obsinfo
-from ..obsmetadata import ObsMetadata
-from ..helpers import OIDate, OIDates, str_indent, str_list_str
+from ..obsMetadata import ObsMetadata
+from ..helpers import OIDate, str_indent
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Equipment(obspy_Equipment):
@@ -55,17 +55,19 @@
         self.model = attributes_dict.get('model', None)
         self.manufacturer = attributes_dict.get('manufacturer', None)
         self.vendor = attributes_dict.get('vendor', None)
         self.serial_number = attributes_dict.get('serial_number', None)
         self.resource_id = attributes_dict.get('resource_id', None)
         self.installation_date = OIDate(attributes_dict.get('installation_date', None))
         self.removal_date = OIDate(attributes_dict.get('removal_date', None))
-        self.calibration_dates = OIDates(attributes_dict.get('calibration_dates', None))
-        # equip = self.to_obspy()
-        # self.obspy_equipment = equip[0] if isinstance(equip, tuple) else equip
+        calibration_dates = attributes_dict.get('calibration_dates', [])
+        self.calibration_dates = [OIDate(x) for x in calibration_dates]
+
+        equip = self.to_obspy()
+        self.obspy_equipment = equip[0] if isinstance(equip, tuple) else equip
 
     def __repr__(self):
         args = []
         if self.type:
             args.append(f"'type': '{self.type}'")
         if self.description:
             args.append(f"'description': '{self.description}'")
@@ -101,29 +103,31 @@
         if self.resource_id is not None:
             s += f"\n    resource_id: {self.resource_id}"
         if self.installation_date.date is not None:
             s += f"\n    installation_date: {self.installation_date}"
         if self.removal_date.date is not None:
             s += f"\n    removal_date: {self.removal_date}"
         if self.calibration_dates:
-            s += f"\n    calibration_dates: {self.calibration_dates.__str__(indent=4, n_subclasses=n_subclasses-1)}"
+            s += f"\n    calibration_dates: {self.calibration_dates}"
         return str_indent(s, indent)
 
     def to_obspy(self):
         """
         Convert an equipment (including the equipment description in
         components) to its obspy object
 
         Returns:
             (:class:`obspy.core.invertory.util.Equipment`)
         """
-        return obspy_Equipment(
+        equip = obspy_Equipment(
             type=self.type,
             description=self.description,
             manufacturer=self.manufacturer,
             vendor=self.vendor,
             model=self.model,
             serial_number=self.serial_number,
             installation_date=self.installation_date.to_obspy(),
             removal_date=self.removal_date.to_obspy(),
-            calibration_dates=self.calibration_dates.to_obspy(),
+            calibration_dates=[x.to_obspy() for x in self.calibration_dates],
             resource_id=self.resource_id)
+
+        return equip
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/AD_conversion.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/AD_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Filter class and subclasses
 """
 # Standard library modules
+import warnings
 import logging
 
 from .coefficients import Coefficients
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class ADConversion(Coefficients):
     """
     ADConversion Filter (Flat Coefficients filter)
 
@@ -25,15 +28,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         attributes_dict["transfer_function_type"] = 'DIGITAL'
         attributes_dict["numerator_coefficients"] = [1.0]
         attributes_dict["denominator_coefficients"] = []
         # Have to pop these before super, or it will give an error.
         input_full_scale = attributes_dict.pop('input_full_scale', None)
         output_full_scale = attributes_dict.pop('output_full_scale', None)
         super().__init__(attributes_dict, stage_id)
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/FIR.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/FIR.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 """
 Finite Impulse Response Filter
 """
 # Standard library modules
+import warnings
 import logging
 
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class FIR(FilterTemplate):
     """
     FIR Filter
 
     Attributes:
         symmetry (str): filter symmetry, one of "EVEN", "ODD", "NONE"
         coefficients (list of floats)
         coefficient_divisor (float)
         delay_samples (float)
     """
-    def __init__(self, attributes_dict, stage_description):
+    def __init__(self, attributes_dict, stage_id=-1):
 
         """
         Constructor
 
         Args:
             attributes_dict (dict): information file
                 dictionaries for stages
-            stage_description (str): id + name of corresponding stage,
-                used for reporting only
+            stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attributes_dict)
         self.symmetry = attributes_dict.pop('symmetry', None)
         self.coefficients = attributes_dict.pop('coefficients', [])
         self.coefficient_divisor = attributes_dict.pop('coefficient_divisor', 1)
         self._validate_empty_attributes_dict(attributes_dict)
-        self._validate_values(stage_description)
 
-    def _validate_values(self, stage_description):
         # Validate values
         if not self.delay_samples:
             msg = 'No delay.samples in FIR filter'
             logger.error(msg)
             raise TypeError(msg)
 
         if self.symmetry not in ['ODD', 'EVEN', 'NONE']:
             msg = f'Illegal FIR symmetry: "{self.symmetry} in stage #{stage_id}"'
             logger.error(msg)
-            raise TypeError(msg)
+            raise TypeError()
 
         sum_coeff = 0
         coeff_cnt = 0
         if len(self.coefficients) > 0:
             for coeff in self.coefficients:
                 sum_coeff += coeff
                 coeff_cnt += 1
@@ -62,17 +61,19 @@
                 coeff_cnt *= 2
             if self.symmetry == 'ODD':
                 sum_coeff += sum_coeff - self.coefficients[-1]
                 coeff_cnt += coeff_cnt - 1
             norm_coeff = sum_coeff / self.coefficient_divisor
             norm_coeff = round(norm_coeff, 2)  # check up to two decimal places
             # last conditional verifies that there is at least one coeff
-            if norm_coeff != 1:
-                logger.warning(f'Sum of {coeff_cnt} coefficients in stage '
-                               f'{stage_description} is {norm_coeff}, not 1 ')
+            if norm_coeff != 1 and norm_coeff != 0:
+                msg = (f'Sum of {coeff_cnt} coefficients in stage "{stage_id}" is '
+                       f'{norm_coeff}, not 1 ')
+                warnings.warn(msg)
+                logger.warning(msg)
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
             return f'{type(self)}'
         s = super().__str__() + '\n'
         s += f"    symmetry: {self.symmetry}\n"
         s += f"    coefficient_divisor: {self.coefficient_divisor}\n"
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/analog.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/analog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Analog Filter (subclass of PolesZeros)
 """
 # Standard library modules
+import warnings
 import logging
 
 from .poles_zeros import PolesZeros
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Analog(PolesZeros):
     """
     Analog Filter (Flat PolesZeros filter)
     """
@@ -18,15 +21,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         attributes_dict["transfer_function_type"] = "LAPLACE (RADIANS/SECOND)"
         attributes_dict["poles"] = []
         attributes_dict["zeros"] = []
         if not "normalization_factor" in attributes_dict:
             attributes_dict["normalization_factor"] = 1.0
         # if not "normalization_frequency" in attributes_dict:
         #     attributes_dict["normalization_frequency"] = 1.
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/coefficients.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/coefficients.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Coefficients Filter
 """
+import warnings
 import logging
 
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Coefficients(FilterTemplate):
     """
     Coefficients Filter Class
 
@@ -23,15 +26,14 @@
         """
         Constructor
 
         Args:
             attr_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attr_dict, stage_id)
         self.transfer_function_type = attr_dict.pop('transfer_function_type',
                                                     'DIGITAL')
         self.numerator_coefficients = attr_dict.pop('numerator_coefficients',
                                                     [1.])
         self.denominator_coefficients = attr_dict.pop('denominator_coefficients', [])
         self._validate_empty_attributes_dict(attr_dict)
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/digital.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/digital.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Digital filter (subclass of Coefficents, which is subclass of Filter)
 """
 # Standard library modules
+import warnings
 import logging
 
 from .coefficients import Coefficients
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Digital(Coefficients):
     """
     Digital Filter (Flat Coefficients filter)
     """
@@ -18,15 +21,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         attributes_dict["transfer_function_type"] = 'DIGITAL'
         attributes_dict["numerator_coefficients"] = [1.0]
         attributes_dict["denominator_coefficients"] = []
         super().__init__(attributes_dict, stage_id)
         self._validate_empty_attributes_dict(attributes_dict)
 
     def __repr__(self):
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/filter.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 """
 Filter class and subclasses
 """
 # Standard library modules
+import warnings
 import logging
 
 from .poles_zeros import PolesZeros
 from .analog import Analog
 from .digital import Digital
 from .AD_conversion import ADConversion
 from .FIR import FIR
 from .response_list import ResponseList
 from .coefficients import Coefficients
 from .polynomial import Polynomial
-from ...obsmetadata import ObsMetadata
+from ...obsMetadata import ObsMetadata
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Filter(object):
     """
     Filter is a gateway to the other filter classes
     """
     @staticmethod
-    def construct(attributes_dict, stage_sequence_number, stage_name,
+    def construct(attributes_dict, stage_id="-1",
                   sensitivity_gain_frequency=1.):
         """
         Constructs an appropriate Filter subclass from an attributes_dict
 
         Args:
             attributes_dict (dict or list of dicts): information file
                 dict for stages
-            stage_sequence_number (int): sequence_number of corresponding stage.
-            stage_name (str): name of corresponding stage. Used for reporting only
+            stage_id (int): id of corresponding stage. Used for reporting only
             sensitivity_gain_frequency (float): frequency at which gain was
                 specified.
                 Used for PoleZeros Normalization factor/frequency
         Returns:
             (:class:`.Filter`): object of the adequate filter subclass
         Raises:
             (TypeError): if filter type is not valid
         """
-        logger.debug('in Filter.construct()')
         if attributes_dict is None:
             msg = "No attributes in filter"
             logger.error(msg)
             raise TypeError(msg)
         if not isinstance(attributes_dict, ObsMetadata):
             attributes_dict = ObsMetadata(attributes_dict)
 
-        stage_description = f'#{stage_sequence_number}'
-        if stage_name is not None:
-                stage_description += f' ("{stage_name}")'
-
         if "type" not in attributes_dict:
-            msg = f'No "type" specified for filter in stage {stage_description}'
+            msg = f'No "type" specified for filter in stage #{stage_id}'
             logger.error(msg)
             raise TypeError(msg)
         else:
-            args = (attributes_dict, stage_description)
             filter_type = attributes_dict.get('type', None)
             if filter_type == 'PolesZeros':
                 attributes_dict['sensitivity_gain_frequency'] = sensitivity_gain_frequency
-                obj = PolesZeros(*args)
+                obj = PolesZeros(attributes_dict, stage_id)
             elif filter_type == 'FIR':
-                obj = FIR(*args)
+                obj = FIR(attributes_dict, stage_id)
             elif filter_type == 'Coefficients':
-                obj = Coefficients(*args)
+                obj = Coefficients(attributes_dict, stage_id)
             elif filter_type == 'ResponseList':
-                obj = ResponseList(*args)
+                obj = ResponseList(attributes_dict, stage_id)
             elif filter_type == 'ADCONVERSION':
-                obj = ADConversion(*args)
+                obj = ADConversion(attributes_dict, stage_id)
             elif filter_type == 'ANALOG':
                 attributes_dict['sensitivity_gain_frequency'] = sensitivity_gain_frequency
-                obj = Analog(*args)
+                obj = Analog(attributes_dict, stage_id)
             elif filter_type == 'DIGITAL':
-                obj = Digital(*args)
+                obj = Digital(attributes_dict, stage_id)
             elif filter_type == 'Polynomial':
-                obj = Polynomial(*args)
+                obj = Polynomial(attributes_dict, stage_id)
             else:
                 msg = (f'Unknown Filter type: "{filter_type}" in '
                        'stage #{stage_id}')
                 logger.error(msg)
                 raise TypeError(msg)
         return obj
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/filter_template.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/filter_template.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 FilterTemplate class, used by all other filter classes
 """
 # Standard library modules
+import warnings
 import logging
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class FilterTemplate(object):
     """
     FilterTemplate is superclass of all filter classes
 
@@ -21,15 +24,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         self.delay_samples = attributes_dict.pop('delay.samples', None)
         self.delay_seconds = attributes_dict.pop('delay.seconds', None)
         self.resource_id = attributes_dict.pop('resource_id', None)
         self.stage_id = stage_id
         self.type = attributes_dict.pop('type', None)
 
     def _validate_empty_attributes_dict(self, attributes_dict):
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/poles_zeros.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/poles_zeros.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """
 Filter class and subclasses
 """
 # Standard library modules
 import math as m
+import warnings
 import logging
 
 # Non-standard modules
+# import obspy.core.inventory.response as obspy_response
+# from scipy._lib.doccer import extend_notes_in_docstring
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+# from ..misc.configuration import ObsinfoConfiguration
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class PolesZeros(FilterTemplate):
     """
     PolesZeros filter
 
@@ -29,15 +35,14 @@
         """
         Constructor
 
         Args:
             attr_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attr_dict, stage_id)
         self.transfer_function_type = attr_dict.pop(
             'transfer_function_type', 'LAPLACE (RADIANS/SECOND)')
         self.poles = [complex(x.replace(" ", ""))
                       for x in attr_dict.pop('poles', [])]
         self.zeros = [complex(x.replace(" ", ""))
                       for x in attr_dict.pop('zeros', [])]
@@ -71,16 +76,16 @@
             n_subclasses (int): number of levels of subclass to print out
         """
         if n_subclasses < 0:
             return f'{type(self)}'
         s = super().__str__() + '\n'
         s += f'    {len(self.poles)} poles, {len(self.zeros)} zeros\n'
         s += f'    transfer_function_type: {self.transfer_function_type}\n'
-        s += f'    normalization_frequency: {self.normalization_frequency:g}\n'
-        s += f'    normalization_factor: {self.normalization_factor:g}'
+        s += f'    normalization_frequency: {self.normalization_frequency:g}'
+        s += f'\n  normalization_factor: {self.normalization_factor:g}'
         return str_indent(s, indent)
 
     def calc_normalization_factor(self, stage_id=-1, debug=False):
         """
         Calculate the normalization factor for a given set of poles-zeros
 
         The norm factor A0 is calculated such that
@@ -105,20 +110,25 @@
 
         A0 = 1.0 + (1j * 0.0)
         if self.transfer_function_type == "LAPLACE (HERTZ)":
             s = 1j * self.normalization_frequency
         elif self.transfer_function_type == "LAPLACE (RADIANS/SECOND)":
             s = 1j * 2 * m.pi * self.normalization_frequency
         else:
-            logger.warning("Don't know how to calculate normalization factor"
-                           "for z-transform poles and zeros!")
+            msg = ("Don't know how to calculate normalization factor"
+                   "for z-transform poles and zeros!")
+            warnings.warn(msg)
+            logger.warning(msg)
             return None
 
         for p in self.poles:
             A0 *= (s - p)
         for z in self.zeros:
             A0 /= (s - z)
 
-        logger.debug(f"poles={self.poles}, zeros={self.zeros}, s={s}, A0={A0}")
+        if debug:
+            msg = f"poles={self.poles}, zeros={self.zeros}, s={s}, A0={A0}"
+            print(msg)
+            logger.debug(msg)
 
         A0 = abs(A0)
         return A0
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/polynomial.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/polynomial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Polynomial Filter
 """
+import warnings
 import logging
 
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Polynomial(FilterTemplate):
     """
     Polynomial Filter Class (never tested)
     """
@@ -18,15 +21,14 @@
         """
         Constructor
 
         Args:
             attr_dict (dict or :class`ObsMetadata`): filter attributes
            stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attr_dict, stage_id)
         self.frequency_lower_bound = attr_dict.pop('frequency_lower_bound', 0.)
         self.frequency_upper_bound = attr_dict.pop('frequency_upper_bound', 0.)
         self.approximation_lower_bound = attr_dict.pop('approximation_lower_bound', None)
         self.approximation_upper_bound = attr_dict.pop('approximation_upper_bound', None)
         self.maximum_error = attr_dict.pop('maximum_error', None)
         self.coefficients = attr_dict.pop('coefficients', [])
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/filter/response_list.py` & `obsinfo-0.111b1/obsinfo/instrumentation/filter/response_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """
 Filter class and subclasses
 """
+# Standard library modules
+import warnings
 import logging
 
+# Non-standard modules
+# import obspy.core.inventory.response as obspy_response
+# from scipy._lib.doccer import extend_notes_in_docstring
+
 from .filter_template import FilterTemplate
 from ...helpers import str_indent
 
+# from ..misc.configuration import ObsinfoConfiguration
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class ResponseList(FilterTemplate):
     """
     ResponseList Filter
 
@@ -22,15 +31,14 @@
         """
         Constructor
 
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): filter attributes
             stage_id (int): id of corresponding stage. Used for reporting only
         """
-        logger.debug(f'in {self.__class__.__name__}.__init__()')
         super().__init__(attributes_dict, stage_id)
         self.elements = attributes_dict.pop('elements', [])
         self._validate_empty_attributes_dict(attributes_dict)
 
         # Validate attributes
         for element in self.elements:
             if not len(element) == 3:
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/instrument.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         Args:
             attributes_dict (dict or :class:`.ObsMetadata`): instrument attributes_dict
             modifs (dict or :class:`ObsMetadata`): modifications passed
                 down from the Instrumentation level (including channel selection)
         """
         # For __repr__()
         if modifs:
-            self.inputs = {'modifs': "<ObsMetadata>"}
+            self.inputs = {'modifs': "<obsinfo.ObsMetadata>"}
         else:
             self.inputs = {'modifs': {}}
         
         self.correction = None
         self.delay = None
 
         if not attributes_dict:
@@ -78,15 +78,15 @@
         # # if self.stages is not None:
         # #     self.obspy_stages = [x.to_obspy() for x in self.stages]
         # # else:
         # #     self.obspy_stages = None
         # self.obspy_response = self.to_obspy()
 
     def __repr__(self):
-        s =   'Instrument(attributes_dict = <ObsMetadata>\n',
+        s =   'Instrument(attributes_dict = <obsinfo.ObsMetadata>\n',
         s += f'           modifs={self.inputs["modifs"]}'
         return s
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
             return self.__class__.__name__
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/instrument_component.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrument_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 InstrumentComponent class and subclasses Sensor, Preamplifier, Datalogger.
 Equipment class
 """
 # Standard library modules
+import warnings
 import logging
 
 # Non-standard modules
 
 # obsinfo
 from .stages import Stages
 from .equipment import Equipment
-from ..obsmetadata import (ObsMetadata)
-from ..helpers import str_indent, str_list_str, verify_dict_is_empty
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from ..helpers import str_indent, verify_dict_is_empty
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class InstrumentComponent(object):
     """
     InstrumentComponent class. Superclass of all component classes.
     No obspy/StationXML equivalent, because they only specify the whole
@@ -44,17 +47,17 @@
             msg = 'No attributes_dict'
             logger.error(msg)
             raise TypeError(msg)
         if not isinstance(attributes_dict, ObsMetadata):
             attributes_dict = ObsMetadata(attributes_dict)
 
         # Remove elements to be processed in Stages()
-        higher_stage_modifications = ObsMetadata(attributes_dict.pop('stage_modifications', {}))
+        response_modifs = ObsMetadata(attributes_dict.pop('stage_modifications', {}))
         if 'stage_modifications' in higher_modifs:
-            higher_stage_modifications.safe_update(higher_modifs.pop('stage_modifications'))
+            response_modifs.safe_update(higher_modifs.pop('stage_modifications'))
 
         # Put shortcuts in the right place:
         if 'serial_number' in attributes_dict:
             attributes_dict.safe_update(
                 {'modifications':
                     {'equipment':
                         {'serial_number': attributes_dict.pop('serial_number')}
@@ -73,20 +76,16 @@
         
         if 'notes' in base_dict:
             del base_dict['notes']
 
         self.equipment = Equipment(base_dict.pop('equipment', None))
         self.configuration = base_dict.pop('configuration', None)
         self.configuration_description = base_dict.pop('configuration_description', self.configuration)
-        stage_modifications = ObsMetadata(base_dict.pop('stage_modifications', {}))
-        stage_modifications.safe_update(higher_stage_modifications, warn_crush=True)
-        self.stages = Stages(base_dict.pop('stages', []), {'stage_modifications': stage_modifications},
+        self.stages = Stages(base_dict.pop('stages', []), response_modifs,
                              base_dict.get('correction', None))
-        self.equipment.calibration_dates += self.stages.calibration_dates
-        logger.info('Instrument_Component has {len(self.stages)} stages')
         self._error_check(self.stages)
         if self.configuration_description is not None:
             self.equipment.description += ' [config: {}]'.format(
                 self.configuration_description)
         # self.obspy_equipment = self.equipment.to_obspy()
         self.base_dict = base_dict  # leftovers for specific components
 
@@ -111,21 +110,24 @@
             s += f'\n    stages: {self.stages.__str__(**kwargs)}'
         return s
 
     def _error_check(self, stages):
         """Some of these checks seem redundant"""
         if stages is None:
             msg = f'stages is None {type(self)}'
+            warnings.warn(msg)
             logger.warning(msg)
         elif not stages:
             msg = f'No response stages in {type(self)}'
+            warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
         elif len(stages) == 0:
             msg = f'len(stages) == 0 in {type(self)}'
+            warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
 
 
 class Sensor(InstrumentComponent):
     """
     Sensor Instrument Component. No obspy equivalent
@@ -149,15 +151,14 @@
 
         Args:
             attributes_dict (dict or :class:`ObsMetadata`): InstrumentComponent
                 attributes
             higher_modifs (dict or :class:`ObsMetadata`): modifications
                 inherited from instrumentation
         """
-        logger.info('Creating Sensor()')
         super().__init__(attributes_dict, higher_modifs)
         seed_dict = self.base_dict.pop('seed_codes', {})
         self.seed_band_base_code = seed_dict.get('band_base', None)
         self.seed_instrument_code = seed_dict.get('instrument', None)
         verify_dict_is_empty(self.base_dict)
         del self.base_dict
 
@@ -195,15 +196,14 @@
             attributes_dict (dict or :class:`ObsMetadata`): InstrumentComponent
                 attributes
             higher_modifs (dict or :class:`ObsMetadata`): modifications
                 inherited from instrumentation
         Returns:
             (:class:`Datalogger`)
         """
-        logger.info('Creating Datalogger()')
         super().__init__(attributes_dict, higher_modifs)
         self.sample_rate = self.base_dict.pop('sample_rate', None)
         self.correction = self.base_dict.pop('correction', 0)
         verify_dict_is_empty(self.base_dict)
         del self.base_dict
 
     def __str__(self, indent=0, n_subclasses=0):
@@ -230,15 +230,14 @@
         """
         Args:
             attributes_dict (dict or :class:`ObsMetadata`): InstrumentComponent
                 attributes
             higher_modifs (dict or :class:`ObsMetadata`): modifications
                 inherited from instrumentation
         """
-        logger.info('Creating Preamplifier()')
         if not attributes_dict:
             return None   # It is acceptable to have no preamplifier
         super().__init__(attributes_dict, higher_modifs)
         verify_dict_is_empty(self.base_dict)
         del self.base_dict
 
     def __str__(self, indent=0, n_subclasses=0):
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/instrumentation.py` & `obsinfo-0.111b1/obsinfo/instrumentation/instrumentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 # Standard library modules
 import warnings
 import logging
 
 # Non-standard modules
 
 # obsinfo modules
-from ..obsmetadata import ObsMetadata
+from obsinfo.obsMetadata.obsmetadata import ObsMetadata
 from .instrument_component import Equipment
 from .channel import Channel, Channels
 from ..helpers import str_indent, verify_dict_is_empty, Location, ObsinfoClassList
+# from .operator_class import Operator
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Instrumentations(ObsinfoClassList):
@@ -74,15 +75,15 @@
             # No base instrument defined, should act like a None
             self.channels = Channels()
             self.equipment = Equipment({'description': attributes_dict['base']})
             return
         
         ic_names = ('datalogger', 'sensor', 'preamplifier')
 
-        self.input = {'attributes_dict': {} if not attributes_dict else '<ObsMetaData>',
+        self.input = {'attributes_dict': {} if not attributes_dict else '<obsinfo.ObsMetaData>',
                       'station_locations': station_locations,
                       'station_start_date': station_start_date,
                       'station_end_date': station_end_date,
                       'station_location_code': station_location_code}
         
         # Syntax checking - Check whether
         if not attributes_dict:
@@ -96,37 +97,41 @@
         else:
             # Easy mistake of including a dash in the yaml file
             msg = 'Instrumentation is not a dict'
             logger.error(msg)
             raise TypeError(msg)
 
         # Remove elements not to be processed here
-        channel_modifs = attributes_dict.pop('channel_modifications', ObsMetadata({}))
+        channel_modifs = attributes_dict.pop('channel_modifications', {})
 
         # Extract instrument_component modifications
         mods = attributes_dict.get('modifications', None)
         if mods is not None:
             # Extract InstrumentComponent modifications
             ic_modifs = ObsMetadata({ic: mods.pop(ic)
                                     for ic in ic_names if ic in mods})
             # Put remaining modifications back
             attributes_dict['modifications'] = mods
         else:
             ic_modifs = ObsMetadata({})
 
         # Put shortcuts in the right place:
         if 'serial_number' in attributes_dict:
-            x = attributes_dict.pop('serial_number')
             attributes_dict.safe_update(
-                {'modifications': {'equipment': {'serial_number': x}}},
+                {'modifications':
+                    {'equipment':
+                        {'serial_number':
+                         attributes_dict.pop('serial_number')}}},
                 warn_crush=True)
         if 'datalogger_configuration' in attributes_dict:
-            x = attributes_dict.pop('datalogger_configuration')
-            channel_modifs.safe_update(
-                {'*-*': {'datalogger': {'configuration': x}}},
+            attributes_dict.safe_update(
+                {'modifications':
+                    {'datalogger':
+                        {'configuration':
+                         attributes_dict.pop(datalogger_configuration)}}},
                 warn_crush=True)
 
         # Get main elements
         base_dict = attributes_dict.get_configured_modified_base()
         base_location_code = base_dict.pop('location_code', station_location_code)
         ### 'configuration' is solely informational
         base_configuration = base_dict.pop('configuration', None)
@@ -202,15 +207,15 @@
                 Must have 'orientation' and 'location_code' keys
             channel_modifs (dict): channel_modifications, keys are
                 id_codes, in order of priority:
                     "<ORT>-<LOC>": orientation_code <ORT> & location_code <LOC>
                     "<ORT>": orientation_code <ORT>
                     "*-<LOC>": location_code <LOC>, all orientation_codes
                     "<ORT>-*": orientation_code <ORT>, all location_codes
-                    "*-*": All ``id_codes``
+                   "*" or "*-*": All ``id_codes``
             location_code (str): The location
 
         Returns:
             (:class:`ObsMetadata``): the selected channel modifications
         """
         for k in ('orientation', 'location_code'):
             if k not in chan_dict:
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/orientation.py` & `obsinfo-0.111b1/obsinfo/instrumentation/orientation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 import logging
 
 # Non-standard modules
 import obspy.core.util.obspy_types as obspy_types
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
 from ..helpers import FloatWithUncert, str_indent
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
@@ -76,21 +76,19 @@
         self.code = key
         value = ObsMetadata(attributes_dict.pop(key, None))
         azimuth = value.get('azimuth.deg', None)
         dip = value.get('dip.deg', None)
         if azimuth is None and dip is None:
             raise ValueError(f'orientation {key}: neither azimuth nor dip specified')
         if azimuth is not None:
-            azimuth.safe_update({'unit': 'degrees'})
-            self.azimuth = FloatWithUncert(azimuth)
+            self.azimuth = FloatWithUncert(azimuth | {'unit': 'degrees'})
         else:
             self.azimuth = FloatWithUncert({'value': 0, 'unit': 'degrees'})
         if dip is not None:
-            dip.safe_update({'unit': 'degrees'})
-            self.dip = FloatWithUncert(dip)
+            self.dip = FloatWithUncert(dip | {'unit': 'degrees'})
         else:
             self.dip = FloatWithUncert({'value': 0, 'unit': 'degrees'})
             
         # Test required values
         if key in 'XYEN':
             if self.azimuth.uncertainty is None:
                 logger.warning("orientation XYEN should have azimuth uncertainty, doesn't")
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/stage.py` & `obsinfo-0.111b1/obsinfo/instrumentation/stage.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from obspy.core.inventory.response import (
     PolesZerosResponseStage, FIRResponseStage,
     CoefficientsTypeResponseStage, ResponseListResponseStage,
     PolynomialResponseStage)
 import obspy.core.util.obspy_types as obspy_types
 
 # Local modules
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .filter import (Filter, PolesZeros, FIR, Coefficients, ResponseList,
                      Analog, Digital, ADConversion, Polynomial)
-from ..helpers import str_indent, OIDates
+from ..helpers import str_indent
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Stage(object):
@@ -43,14 +43,15 @@
         input_sample_rate (float): input sample rate in sps
         delay (float): delay in seconds of stage. If not present, will be
             calculated from delay from digital stages
         decimation_factor (float): decimation factor of stage
         correction (float) : delay correction. Calculated from instrument
             delay correction
         polarity (str, either "+" or "-"): whether stage changes polarity
+        calibration_date (str in date format): calibration date of stage
         resource_id (str)
         instrument_sensitivity (float): Not used, set to None. Sensitivity
             is calculated for the whole response.
 
     """
     def __init__(self, attributes_dict, higher_modifs=ObsMetadata({}),
                  correction=None, sequence_number=-1,
@@ -70,49 +71,46 @@
            ext_config_name (str): higher-level configuration definition (overrides
                 whatever is in self)
         """
         if attributes_dict is None:
             return None
         
         # input parameters, for __repr__
-        self.inputs = {'attributes_dict': '<ObsMetadata>',
-                       'higher_modifs': '<ObsMetadata>',
+        self.inputs = {'higher_modifs': ':class:`ObsMetadata`',
                        'correction': correction,
                        'sequence_number': sequence_number,
                        'ext_config_name': ext_config_name}
         if not higher_modifs:
                     self.inputs['higher_modifs'] = '{}'
 
         if not isinstance(attributes_dict, ObsMetadata):
             attributes_dict = ObsMetadata(attributes_dict)
         if not isinstance(higher_modifs, ObsMetadata):
             higher_modifs = ObsMetadata(higher_modifs)
 
-        # put appropriate "stage_modifications" in "modifications"
+        # replace "stage_modifications" by "modifications" before sending off
+        # to ObsMetadata.get_configured_modified_base()
         m = self._get_stage_modifications(
             attributes_dict.pop('stage_modifications', {}), sequence_number)
+        hm = self._get_stage_modifications(
+            higher_modifs.pop('stage_modifications', {}), sequence_number)
         if "modifications" in attributes_dict:
             attributes_dict['modifications'].safe_update(m)
         elif not m == {}:
             attributes_dict['modifications'] = m
 
-        hm = self._get_stage_modifications(
-            higher_modifs.pop('stage_modifications', {}), sequence_number)
         if "modifications" in higher_modifs:
             higher_modifs['modifications'].safe_update(hm)
         elif not hm == {}:
             higher_modifs['modifications'] = hm
 
         base_dict = attributes_dict.get_configured_modified_base(higher_modifs)
 
         self.name = base_dict.pop('name', None)  
-        self.configuration = base_dict.pop('configuration', None)
-        # CalibrationDates belongs in equipment, but is more logical to state
-        # in stage, rely on equipment to look for it.    
-        self.calibration_dates = OIDates(base_dict.pop('calibration_dates', []) )     
+        self.configuration = base_dict.pop('configuration', None)      
         self.configuration_description = base_dict.pop('configuration_description',
                                                        self.configuration)      
         self.description = base_dict.pop('description', '')
         if self.configuration_description is not None:
             if self.name is None:
                 self.name = f'[config: {self.configuration_description}]'
             else:
@@ -121,26 +119,24 @@
         gd = base_dict.pop('gain', None)
         if gd is None:
             msg = f'No gain specified in stage {self.name}'
             logger.error(msg)
             raise TypeError(msg)
         self.gain = gd.get('value', 1.0)
         self.gain_frequency = gd.get('frequency', 0.0)
-        self.stage_sequence_number = sequence_number
 
-
-        self.filter = Filter.construct(base_dict.pop('filter'),
-                                       self.stage_sequence_number,
-                                       self.name,
+        self.filter = Filter.construct(base_dict.pop('filter'), self.name,
                                        self.gain_frequency)
         if not self.filter:
             msg = f'No filter in stage {self.name}'
             logger.error(msg)
             raise TypeError(msg)
 
+        self.stage_sequence_number = sequence_number
+
         x = base_dict.pop('input_units', None)
         if x:
             self.input_units = x.get('name', None)
             self.input_units_description = x.get('description', None)
 
         x = base_dict.pop('output_units', None)
         if x:
@@ -155,14 +151,15 @@
         self._delay = base_dict.pop('delay', None)
         self.decimation_factor = base_dict.pop('decimation_factor', 1)
         self.correction = correction
 
         # default polarity is positive
         self.polarity = base_dict.pop('polarity', 1)
         self.resource_id = base_dict.pop('resource_id', None)
+        self.calibration_date = base_dict.pop('calibration_date', None)
         self.instrument_sensitivity = None
         # Instrument sensitivity will be calculated using obspy and stored in
         # first stage
         if len(base_dict) > 0:
             raise ValueError('base_dict has remaing fields: {}'
                              .format([x for x in base_dict.keys()]))
 
@@ -194,15 +191,15 @@
         # Calculate delay based on filter
         if self.filter.delay_seconds is not None:
             filter_delay = self.filter.delay_seconds
         elif self.filter.delay_samples is not None:
             if not self.input_sample_rate:
                 # Delay is already none, leave it like that
                 msg = ('Cannot calculate delay from delay_samples '
-                       f'because stage {self.name} has no input_sample_rate')
+                       f'because stage {self.name}has no input_sample_rate')
                 logger.warning(msg)
                 warnings.warn(msg)
             else:
                 filter_delay = self.filter.delay_samples / self.input_sample_rate
 
         if self._delay is None:
             return filter_delay 
@@ -213,47 +210,44 @@
                    f" ({self._delay} != {filter_delay}): ignoring filter "
                    "delay")
             warning.warn(msg)
             logger.warning(msg)
         return self._delay
         
     def __repr__(self):
-        return (f"Stage({self.inputs['attributes_dict']}, "
-                f"{self.inputs['higher_modifs']}, "
-                f"{self.inputs['correction']}, "
-                f"{self.inputs['sequence_number']}, "
-                f"{self.inputs['ext_config_name']})")
+        return (f"Stage(:class:`ObsMetadata`, {self.inputs['higher_modifs']},"
+                f" {self.inputs['correction']}, {self.inputs['sequence_number']},"
+                f" {self.inputs['ext_config_name']})")
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
             return f'{type(self)}'
-        kwargs = {'indent': 4, 'n_subclasses': n_subclasses-1}
         s = f'Stage:\n'
         s += f'    name: {self.name}\n'
         s += f'    description: {self.description}\n'
         s += f'    input_units: {self.input_units}\n'
         s += f'    output_units: {self.output_units}\n'
         s += f'    gain: {self.gain}\n'
         s += f'    gain_frequency: {self.gain_frequency:g}\n'
-        s += f'    filter: {self.filter.__str__(**kwargs)}\n'
+        s += f'    filter: {self.filter.__str__(4, n_subclasses-1)}\n'
         if not self.stage_sequence_number == -1:
             s += f'    stage_sequence_number: {self.stage_sequence_number}\n'
-        if self.calibration_dates is not None:
-            s += f'    calibration_dates: {self.calibration_dates.__str__(**kwargs)}\n'
         if self.input_units_description:
             s += f'    input_units_description: {self.input_units_description}\n'
         if self.output_units_description:
             s += f'    output_units_description: {self.output_units_description}\n'
         if self.input_sample_rate:
             s += f'    input_sample_rate: {self.input_sample_rate}\n'
 
         s += f'    decimation_factor: {self.decimation_factor}\n'
         s += f'    delay: {self.delay}\n'
         s += f'    correction: {self.correction}'
 
+        if self.calibration_date:
+            s += f'\n    calibration_dates={self.calibration_date}'
         return str_indent(s, indent)
 
     def to_obspy(self):
         """
         Return equivalent *obspy.core.inventory.response* classes stages:
 
         Possible stage classes:
@@ -352,17 +346,16 @@
             msg = 'Unhandled response stage type in stage '\
                   f'#{self.stage_sequence_number}: "{filt.type}"'
             warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
 
         return obspy_stage
-    
-    @staticmethod
-    def _get_stage_modifications(resp_modifs, sequence_number):
+
+    def _get_stage_modifications(self, resp_modifs, sequence_number):
         """
         Select which channel modifications specified at station level apply
         to a given stage,  with the stage number (WITHIN an instrument
         component) as key code
 
         Args:
             resp_modifs (dict or :class:`.ObsMetadata`): response modifications:
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/instrumentation/stages.py` & `obsinfo-0.111b1/obsinfo/instrumentation/stages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Stages and Stage classes
 """
 # Standard library modules
 import warnings
 import logging
 
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .stage import Stage
-from ..helpers import ObsinfoClassList, OIDates
+from ..helpers import ObsinfoClassList
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Stages(ObsinfoClassList):
@@ -20,68 +20,61 @@
     
     Has a custom constructor using a list of attribute_dicts, and custom
     input_units(), output_units and to_obspy() methods
 
     Attributes:
         stages (list of objects of :class:`Stage`)
     """
-    def __init__(self, attribute_list=None, higher_modifications={},
-                 correction=None):
+    def __init__(self, attribute_list=None, modifs={},
+                 correction=None):  # , ext_config_name=None):
         """
         Constructor
 
         Args:
             attribute_list (list of dicts): information file
                 dictionaries for each stage
-            higher_modifications (dict or :class:`.ObsMetadata`): modifications to
-                pass down to Stage
+            modifs (dict or :class:`.ObsMetadata`):
+                modifications to pass down to Stage
             correction (float): used only for datalogger: the delay
                 correction for the entire instrument
+            # ext_config_name (str): external configuration name applied to
+            #     every stage.
         """
         if attribute_list is None:
             msg = 'No stages in information file'
             warnings.warn(msg)
             logger.warning(msg)
-            super().__init__([], Stage)
+            super().__init__([])
+            # self.stages = None
         else:
             stages = []
-            logger.debug(f'{higher_modifications=}')
             for s, i in zip(attribute_list, range(0, len(attribute_list))):
                 # Assign correction value
                 if correction is None:
                     correction = None
                 elif i == len(attribute_list)-1:
                     correction = correction
                 else:
                     correction = 0
-                stages.append(Stage(ObsMetadata(s),
-                                    higher_modifications,
-                                    correction, i+1))
+                stages.append(
+                    Stage(ObsMetadata(s), modifs, correction, i+1)) # , ext_config_name))
                 if i > 0:
                     # Check that input units match prior output units
                     s = stages
                     if not s[i].input_units == s[i-1].output_units:
                         raise ValueError(f'stage {i:d} input units do not '
                                          f'match stage {i-1:d} output units '
                                          '("{}"~="{}")'.format(
                                             s[i].input_units,
                                             s[i-1].output_units))
-            super().__init__(stages, Stage)
+            super().__init__(stages)
 
 
     @property
     def input_units(self):
         return self[0].input_units
         # return self.stages[0].input_units
 
     @property
     def output_units(self):
         return self[-1].output_units
         # return self.stages[-1].output_units
-
-    @property
-    def calibration_dates(self):
-        caldates = OIDates([])
-        for x in self:
-            if x is not None:
-                caldates.extend(x.calibration_dates)
-        return caldates
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/misc/configuration.py` & `obsinfo-0.111b1/obsinfo/misc/configuration.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/misc/const.py` & `obsinfo-0.111b1/obsinfo/misc/const.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/misc/discoveryfiles.py` & `obsinfo-0.111b1/obsinfo/misc/discoveryfiles.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/misc/printobs.py` & `obsinfo-0.111b1/obsinfo/misc/printobs.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/misc/remoteGitLab.py` & `obsinfo-0.111b1/obsinfo/misc/remoteGitLab.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/misc/yamlref.py` & `obsinfo-0.111b1/obsinfo/misc/yamlref.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,15 @@
         :returns: dictionary of parsed YAML or JSON formats
         :raises: FileNotFoundError, IOError, OSError
 
         """
         scheme = urlparse.urlsplit(uri).scheme
         path = urlparse.urlsplit(uri).path
 
-        logger.debug(f"Opening file: {path}")
+        logger.info(f"Opening file: {path}")
         # Open locally or remotely according to scheme
         if scheme == 'file':
             try:
                 with open(path, "rt") as fp:
                     strm = fp.read()
             except FileNotFoundError:
                 msg = f'File not found: {path}'
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/obsmetadata/obsmetadata.py` & `obsinfo-0.111b1/obsinfo/obsMetadata/obsmetadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 obsinfo information file routines, contained in superclass ObsMetadata for
 generality
 """
 # Standard library modules
 import json
 from pathlib import Path, PurePath
+import warnings
 from urllib.parse import urlparse
 from urllib.parse import unquote
 import logging
 import time
 
 # Non-standard modules
 import jsonschema
@@ -16,17 +17,18 @@
 
 # Local modules
 from ..misc import yamlref
 from ..misc.yamlref import JsonLoader
 from ..misc.remoteGitLab import gitLabFile
 from ..misc.discoveryfiles import Datapath
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
-overwrite_symbol = '^'      # Used by safe_update
 root_symbol = "#"
 VALID_FORMATS = ["JSON", "YAML"]
 DEFAULT_SCHEMA_PATH = Path(__file__).parent.parent.joinpath('data', 'schemas')
 VALID_TYPES = [Path(f.stem).stem
                for f in DEFAULT_SCHEMA_PATH.glob('*.schema.json')]
 
 
@@ -89,16 +91,14 @@
         if quiet:
             verbose = False
 
         # Get schema filename
         if not schema_filename:
             if not file_type:
                 file_type = ObsMetadata.get_information_file_type(info_filename)
-            if file_type is None:
-                logger.error(f'Could not determine file type for {info_filename}')
             schema_filename = file_type + '.schema.json'
 
         # Get infofile instance and schema
         if dp is None:
             dp = Datapath()
         instance = self.read_info_file(info_filename, dp, remote, False,
                                        file_format, verbose)
@@ -196,16 +196,16 @@
         """
         stem = PurePath(filename).stem
         suffix = PurePath(stem).suffix
         type = suffix[1:]
         if type in VALID_TYPES:
             return type
         msg = f"File '{filename}' is of unknown type: {type}"
-        logger.warning(msg)
-        return None
+        logger.error(msg)
+        raise ValueError(msg)
 
     def read_json_yaml(filename, file_format=None):
         """
         Reads a JSON or YAML file. Does NOT use jsonReference  DEPRECATED.
 
         DEPRECATED. Not being used by any obsinfo method or function. Kept
         for compatibility
@@ -349,16 +349,14 @@
         Returns:
             (:class:`ObsMetadata`): JSON or YAML parsed info files
         """
         if quiet is True:
             verbose = False
         if validate:
             file_type = ObsMetadata.get_information_file_type(filename)
-            if file_type is None:
-                logger.error(f'Could not determine type of file {filename}')
             msg = f'Validating {file_type} file: {filename}'
             logger.info(msg)
             if verbose:
                 print(msg)
             ObsMetadata().validate(str(filename), DEFAULT_SCHEMA_PATH,
                                    remote=remote, verbose=verbose, quiet=quiet)
         else:
@@ -432,16 +430,16 @@
             raise ValueError('higher_level base-configuration-modification '
                              f'dict had leftover elements: {b}')
 
         # Configure, then modify
         configs = base_dict.pop("configurations", None)
         if configuration is not None:
             if configs is None:
-                raise ValueError(f"'{configuration}' configuration was requested"
-                                 ', but no configurations were specified')
+                raise ValueError(f"Configuration requested ('{configuration}')"
+                                 ', but no configurations specified')
             if configuration not in configs:
                 raise ValueError(
                     f"Requested configuration ('{configuration}') doesn't "
                     f"match specified configurations: {list(configs.keys())}")
             base_dict.safe_update(configs[configuration])
             base_dict['configuration'] = configuration
         base_dict.safe_update(modifs)
@@ -449,16 +447,15 @@
         return base_dict
         
     def safe_update(self, update_dict, allow_overwrite=True, warn_crush=False):
         """
         Update that only changes explicitly specfied fields
 
         Drills recursively through dicts inside the dict, only changing fields
-        which are specified in update_dict.  Lists are completely replaced, 
-        however, to avoid ambiguity.
+        which are specified in update_dict
 
         Args:
             update_dict (dict or :class:`ObsMetadata`): dictionary containing
                 fields to update
             allow_overwrite (bool): allow a field that was originally a dict
                 to be overwritten by a field that is not a dict.  Same for lists.
             warn_crush (bool): write out a warning when a value is replaced
@@ -468,78 +465,73 @@
             raise TypeError('update_dict is not a dict')
         if not isinstance(update_dict, self.__class__):
             update_dict = self.__class__(update_dict)
         for key, value in update_dict.items():
             # Change any dict into ObsMetadata
             if isinstance(value, dict) and not isinstance(value, self.__class__):
                 value = self.__class__(value)
-            if key[0] == overwrite_symbol:
-                key=key[1:]
-                if key in self:
-                    logger.info('Overwrite ordered for key {key}')
-                self[key] = value
-                continue  # Go to next loop iteration
             if key not in self:  # Add new key and its value
                 self[key] = value
-                continue  # Go to next loop iteration
-            # Key exists in self and not forced overwrite
-            if isinstance(self[key], dict):  # If original item is a dict
-                # if value is also a dictionary, update it
-                if isinstance(value,  dict):
-                    # if replacement value is a dictionary, recurse
-                    self[key].safe_update(value,
-                                          allow_overwrite=allow_overwrite,
-                                          warn_crush=warn_crush)
-                else:
-                    # if replacement value is not a dictionary
-                    if allow_overwrite:  # replace & warn
-                        self[key] = value
-                        logger.warning(f'dict field "{key}" '
-                                       'was replaced by a non-dict')
-                    else:  # reject & warn
-                        logger.warning(
-                            f'replacement field "{key}" was not inserted '
-                            'into original because original was a dict '
-                            'but replacement was not')
-            elif isinstance(self[key], list):  # If original item is a list
-                if isinstance(value,  list):   # If replacement is also a list
-                    # Replace the list
-                    self[key] = value
-                    logger.debug(f'"{key}": {len(self[key])}-element list replaced by {len(value)}-element list')
-                    # Recurse on contents
-                    # replacer = []
-                    # for item, holder in zip(value, self[key]):
-                    #     if isinstance(item, (dict, ObsMetadata)):
-                    #         holder = ObsMetadata(holder)  # SHOULDN'T BE NECESSARY!
-                    #         holder.safe_update(self.__class__(item),
-                    #                            allow_overwrite=allow_overwrite,
-                    #                            warn_crush=warn_crush)
-                    #     elif isinstance(item, list):
-                    #         raise ValueError('does not handle lists in lists')
-                    #     else:
-                    #         holder = item
-                    #     replacer.append(holder)
-                    # self[key] = replacer
+            else:  # Key exists in self:
+                if isinstance(self[key], dict):  # If original item is a dict
+                    # if value is also a dictionary, update it
+                    if isinstance(value,  dict):
+                        # if replacement value is a dictionary, recurse
+                        self[key].safe_update(value,
+                                              allow_overwrite=allow_overwrite,
+                                              warn_crush=warn_crush)
+                    else:
+                        # if replacement value is not a dictionary
+                        if allow_overwrite:  # replace & warn
+                            self[key] = value
+                            msg = f'field "{key}" was a dict, replaced by a non-dict'
+                            warnings.warn(msg)
+                            logger.warning(msg)
+                        else:  # reject & warn
+                            msg = (f'replacement field "{key}" not inserted '
+                                   'into original because original was a dict '
+                                   'but replacement was not')
+                            warnings.warn(msg)
+                            logger.warning(msg)
+                elif isinstance(self[key], list):  # If original item is a list
+                    if isinstance(value,  list):   # If replacement is also a list
+                        # Recurse on contents
+                        replacer = []
+                        for item, holder in zip(value, self[key]):
+                            if isinstance(item, (dict, ObsMetadata)):
+                                holder = ObsMetadata(holder)  # SHOULDN'T BE NECESSARY!
+                                holder.safe_update(self.__class__(item),
+                                                   allow_overwrite=allow_overwrite,
+                                                   warn_crush=warn_crush)
+                            elif isinstance(item, list):
+                                raise ValueError('does not handle lists in lists')
+                            else:
+                                holder = item
+                            replacer.append(holder)
+                        self[key] = replacer
+                    else:
+                        # if replacement value is not a list
+                        if allow_overwrite:  # replace & warn
+                            self[key] = value
+                            msg = f'field "{key}" was a list, replaced by a non-list'
+                            warnings.warn(msg)
+                            logger.warning(msg)
+                        else:  # reject & warn
+                            msg = (f'replacement field "{key}" not inserted '
+                                   'into original because original was a list '
+                                   'but replacement was not')
+                            warnings.warn(msg)
+                            logger.warning(msg)
                 else:
-                    # if replacement value is not a list
-                    if allow_overwrite:  # replace & warn
-                        self[key] = value
-                        msg = f'field "{key}" was a list, replaced by a non-list'
+                    # Replace existing others
+                    if key in self and warn_crush is True:
+                        msg = f'replacing self["{key}"]: was {self[key]}, now {value}'
+                        warnings.warn(msg)
                         logger.warning(msg)
-                    else:  # reject & warn
-                        msg = (f'replacement field "{key}" not inserted '
-                               'into original because original was a list '
-                               'but replacement was not')
-                        logger.warning(msg)
-            else:
-                # Replace existing others
-                if key in self and warn_crush is True:
-                    msg = f'replacing self["{key}"]: was {self[key]}, now {value}'
-                    logger.warning(msg)
-                self[key] = value
+                    self[key] = value
 
     def copy(self):
         return ObsMetadata(super().copy())
 
     def _convert_to_obsmetadata(self):
         """
         Make all contained dictionaries objects of :class: `.ObsMetadata`
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/subnetwork/operator.py` & `obsinfo-0.111b1/obsinfo/subnetwork/operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         self.agency = attributes_dict['agency']     # required
         self.contacts = Persons(attributes_dict.get('contacts', None))
         self.website = attributes_dict.get('website', None)
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 1:
-            return f'agency: {self.agency}'
+            return f'{type(self)}'
         kwargs = dict(indent=4, n_subclasses=n_subclasses-1)
         s = f'{self.__class__.__name__}:\n'
         s += f'    agency: {self.agency}\n'
         s += f'    contacts: {self.contacts.__str__(**kwargs)}\n'
         s += f'    website: {self.website}'
         return str_indent(s, indent)
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/subnetwork/processing.py` & `obsinfo-0.111b1/obsinfo/subnetwork/processing.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/subnetwork/site.py` & `obsinfo-0.111b1/obsinfo/subnetwork/site.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/subnetwork/station.py` & `obsinfo-0.111b1/obsinfo/subnetwork/station.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Station Class
 """
 # Standard library modules
+import warnings
 import logging
 
 # Non-standard modules
 from obspy.core.inventory.station import Station as obspy_Station
 
 from obspy.core.inventory.util import (Comment)
 from obspy.core.utcdatetime import UTCDateTime
@@ -14,40 +15,41 @@
 # obsinfo modules
 from .processing import Processing
 from ..instrumentation import Instrumentation, Instrumentations
 from ..helpers import (Location, Locations, OIDate,
                        str_list_str, str_indent, verify_dict_is_empty,
                        ObsinfoClassList, Comments, ExternalReferences, Identifiers)
 from .operator import Operators
-from ..obsmetadata import ObsMetadata
+from ..obsMetadata import ObsMetadata
 from .site import Site
 
+warnings.simplefilter("once")
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 logger = logging.getLogger("obsinfo")
 
 
 class Stations(ObsinfoClassList):
     """
     A list of Station objects
     """
-    def __init__(self, stations_dict, station_only, operators, comments):
+    def __init__(self, stations_dict, station_only, stations_operators):
         """
-        Args:
-            stations_dict: (dict or :class:`.ObsMetadata`): dictionary
-                from station or network info file with YAML or JSON
-                attributes
-            station_only (boolean): Creates object with no instrumentation
-            operators (:class:`.Operators`): default station
-                operators
-            comments: (:class:`.Comments`): default station comments
+            Args:
+                stations_dict: (dict or :class:`.ObsMetadata`): dictionary
+                    from station or network info file with YAML or JSON
+                    attributes
+                station_only (boolean): Creates object with no instrumentation
+                stations_operators (:class:`.Operators`): default station
+                    operators
         """
         if stations_dict is None:
             super().__init__([])
         else:
-            super().__init__([Station(k, v, station_only, operators, comments)
-                             for k, v in (stations_dict.items())], Station)
+            super().__init__([Station(k, v, station_only, stations_operators)
+                             for k, v in (stations_dict.items())])
 
 
 class Station(object):
     """
     Station. Equivalent to obspy/StationXML Station
 
     Methods convert info files to an instance of this class and convert the
@@ -75,34 +77,33 @@
             a dict with keys ['uri', 'description']
         water_level (number): elevation (m) of water surface (useful for lakes)
         obspy_station (:class:`obspy.core.inventory.station.Station`):
             Equivalent obspy object
     """
 
     def __init__(self, code, attributes_dict, station_only=False,
-                 stations_operators=None, stations_comments=None):
+                 stations_operators=None):
         """
         Constructor
 
         Args:
             attributes_dict: (dict or :class:`.ObsMetadata`): dictionary
                 from station or network info file with YAML or JSON attributes
             station_only (boolean): Creates object with no instrumentation
             stations_operators (:class:`.Operators`): default station
                 operator(s)
-            stations_comments: (:class:`.Comments`): default station comments
         Raises:
             TypeError
         """
         if not attributes_dict:
             msg = 'No station attributes'
+            warnings.warn(msg)
             logger.error(msg)
             raise TypeError(msg)
 
-        logger.info(f'Creating Station "{code}"')
         self.code = code
         self.site = Site(attributes_dict.pop("site", None))
         self.start_date = OIDate(attributes_dict.pop("start_date"))
         self.end_date = OIDate(attributes_dict.pop("end_date"))
         self.location_code = attributes_dict.pop("location_code")
         self.restricted_status = attributes_dict.pop("restricted_status", None)
         self.operators = Operators(attributes_dict.pop("operators", None))
@@ -124,16 +125,14 @@
             else:
                 self.instrumentations = Instrumentations([Instrumentation(
                     instr_dict, self.locations, self.location_code,
                     self.start_date.date, self.end_date.date)])
 
         self.processing = Processing(attributes_dict.pop('processing', None))
         self.comments = Comments(attributes_dict.pop("comments", []))
-        if stations_comments is not None:
-            self.comments += stations_comments
         self.source_id = attributes_dict.pop('source_id', None)
         self.identifiers = Identifiers(attributes_dict.pop('identifiers', None))
         self.extras = attributes_dict.pop('extras', None)
         self.external_references = ExternalReferences(attributes_dict.pop('external_references', None))
         self.comments += Comments.from_extras(attributes_dict.pop('extras', None))
         self.comments += self.processing.to_comments()
         if 'notes' in attributes_dict:
@@ -148,15 +147,15 @@
         if self.processing:
             s += f'processing-steps: {self.processing.processing_list}'
         s += ')'
         return s
 
     def __str__(self, indent=0, n_subclasses=0):
         if n_subclasses < 0:
-            return f'{self.__class__.__name__} {self.code}'
+            return f'{self.__class__.__name__}: {self.code}'
         kwargs = dict(indent=4, n_subclasses=n_subclasses-1)
         s = f'{self.__class__.__name__}:\n'
         s += f'    code: {self.code}\n'
         s += f'    site: {self.site}\n'
         s += f'    start_date: {self.start_date}\n'
         s += f'    end_date: {self.end_date}\n'
         s += f'    location_code: {self.location_code}\n'
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/.DS_Store` & `obsinfo-0.111b1/obsinfo/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/components/datalogger.yaml` & `obsinfo-0.111b1/obsinfo/templates/components/datalogger.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/components/preamplifier.yaml` & `obsinfo-0.111b1/obsinfo/templates/components/preamplifier.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/components/sensor.yaml` & `obsinfo-0.111b1/obsinfo/templates/components/sensor.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/filters/PolesZeros.filter.yaml` & `obsinfo-0.111b1/obsinfo/templates/filters/PolesZeros.filter.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/instrumentation.yaml` & `obsinfo-0.111b1/obsinfo/templates/instrumentation.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/network.yaml` & `obsinfo-0.111b1/obsinfo/templates/network.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/templates/stage.yaml` & `obsinfo-0.111b1/obsinfo/templates/stage.yaml`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/tests/CompareXMLTree.py` & `obsinfo-0.111b1/obsinfo/tests/CompareXMLTree.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/tests/remoteGithub.py` & `obsinfo-0.111b1/obsinfo/tests/remoteGithub.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/tests/run_test_script.py` & `obsinfo-0.111b1/obsinfo/tests/run_test_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,35 +62,38 @@
 import inspect
 import difflib
 import re
 import glob
 from json.decoder import JSONDecodeError
 from argparse import ArgumentParser
 
+import logging
+from logging.handlers import RotatingFileHandler
+
+
 #Third party  imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import  (Latitude, Longitude, Site, Comment)
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
                                      Datalogger, Preamplifier, Sensor,
                                      Stages, Stage, Filter)
-from ..helpers import Location, init_logging
-from ..network import (Station, Subnetwork)
-from ..instrumentation.filter import (Filter, PolesZeros, FIR, Coefficients, ResponseList,
+from obsinfo.helpers import Location
+from obsinfo.network import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (Filter, PolesZeros, FIR, Coefficients, ResponseList,
                      Analog, Digital, AD_Conversion)
-from ..misc.printobs import  (PrintObs)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.misc.printobs import  (PrintObs)
+from obsinfo.misc.discoveryfiles import Datapath
 import obsinfo
-from ..misc.const import *
-from ..misc.configuration import Singleton
+from obsinfo.misc.const import *
+from obsinfo.misc.configuration import Singleton
 
 verbose = False
-logger = init_logging("run_test_script")
 
 class JsonRefTest(unittest.TestCase):
     """
     Class of test methods for information file format
     
     Attributes:
         testing_path (str): path to datafiles to be tested aside from the examples
@@ -1477,14 +1480,15 @@
     
     """
 
     args = retrieve_arguments()
     tst = TestObsinfo()
     tst.setUp(test=False, print_output=True, level=args.level) 
     dp = Datapath()
+    logger = init_logging()
         
     try:               
         
         type = ObsMetadata.get_information_file_type(args.input_filename)
          
         print(f'Printing {type} file: {args.input_filename}')
             
@@ -1500,16 +1504,14 @@
             tst._test_sensor(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "instrumentation":
             tst._test_instrumentation(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "station":
             tst._test_station(tst.infofiles_path.build_datapath(args.input_filename))
         elif type == "subnetwork":
             tst._test_subnetwork(tst.infofiles_path.build_datapath(args.input_filename))
-        else:
-            logger.error(f'Unknown file type "{type}" for file {args.input_filename}')
     
     except TypeError:
         print("Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         logger.error("TypeError: Illegal format: fields may be missing or with wrong format in input file, or there is a programming error")
         if args.debug:
             raise
         
@@ -1594,10 +1596,33 @@
      
     if not Path(args.input_filename[0]).is_absolute():
         args.input_filename = str(Path(os.getcwd()).joinpath(args.input_filename[0]).resolve())
              
     return args  
 
 
+def init_logging():
+    """
+    Create or open a rotating logging file and add it to ObsinfoConfiguration
+    
+    :returns: object of Logger class 
+    """
+    
+    logfile = Path.home().joinpath('.obsinfo', 'obsinfolog-validate')
+    
+    
+    logger = logging.getLogger("obsinfo")
+    
+    logger.setLevel(logging.DEBUG)
+    # add a rotating handler with 200K (approx) files and just two files
+    handler = RotatingFileHandler(logfile, maxBytes=200000,
+                                  backupCount=2)
+    frmt = logging.Formatter(fmt='%(asctime)s %(levelname)-8s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    handler.setFormatter(frmt)
+    logger.addHandler(handler)  
+    
+    return logger 
+
+
 if __name__ == '__main__':
     run_suite_yaml()
     run_suite_info_files(["--all"])
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/tests/test_datapath.py` & `obsinfo-0.111b1/obsinfo/tests/test_datapath.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,23 +66,23 @@
 import logging
 
 # Third party imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import Site
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
                                      Stage, Filter)
-from ..helpers import Location
-from ..subnetwork import (Station, Subnetwork)
-from ..instrumentation.filter import (PolesZeros, FIR, Coefficients,
+from obsinfo.helpers import Location
+from obsinfo.subnetwork import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (PolesZeros, FIR, Coefficients,
                                             ResponseList)
-from ..misc.printobs import (PrintObs)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.misc.printobs import (PrintObs)
+from obsinfo.misc.discoveryfiles import Datapath
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = True
 
 
 class TestDatapath(unittest.TestCase):
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/tests/test_infofile.py` & `obsinfo-0.111b1/obsinfo/tests/test_infofile.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,22 +79,22 @@
 # from logging.handlers import RotatingFileHandler
 
 # Third party imports
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.core.inventory.util import Site
 
 # obsinfo modules
-from ..obsmetadata import (ObsMetadata)
-from ..instrumentation import (Instrumentation, InstrumentComponent,
+from obsinfo.obsMetadata.obsmetadata import (ObsMetadata)
+from obsinfo.instrumentation import (Instrumentation, InstrumentComponent,
                                      Stages, Stage, Filter)
-from ..helpers import Location
-from ..subnetwork import (Station, Subnetwork)
-from ..instrumentation.filter import (PolesZeros, FIR, Coefficients, ResponseList)
-from ..misc.printobs import (PrintObs)
-from ..misc.discoveryfiles import Datapath
+from obsinfo.helpers import Location
+from obsinfo.subnetwork import (Station, Subnetwork)
+from obsinfo.instrumentation.filter import (PolesZeros, FIR, Coefficients, ResponseList)
+from obsinfo.misc.printobs import (PrintObs)
+from obsinfo.misc.discoveryfiles import Datapath
 
 warnings.simplefilter("once")
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 verbose = False
 
 
 class TestObsinfo(unittest.TestCase):
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo/tests/test_main.py` & `obsinfo-0.111b1/obsinfo/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `obsinfo-0.111.1.post5/src/obsinfo.egg-info/PKG-INFO` & `obsinfo-0.111b1/obsinfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsinfo
-Version: 0.111.1.post5
+Version: 0.111b1
 Summary: Tools for documenting ocean bottom seismometer experiments and creating metadata
 Home-page: https://gitlab.com/resif/obsinfo
 Author: Wayne Crawford
 Author-email: crawford@ipgp.fr
 Keywords: seismology OBS
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo.egg-info/SOURCES.txt` & `obsinfo-0.111b1/obsinfo.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,265 +1,253 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
-src/obsinfo/__init__.py
-src/obsinfo/version.py
-src/obsinfo.egg-info/PKG-INFO
-src/obsinfo.egg-info/SOURCES.txt
-src/obsinfo.egg-info/dependency_links.txt
-src/obsinfo.egg-info/entry_points.txt
-src/obsinfo.egg-info/requires.txt
-src/obsinfo.egg-info/top_level.txt
-src/obsinfo/_examples/.DS_Store
-src/obsinfo/_examples/Information_Files/.DS_Store
-src/obsinfo/_examples/Information_Files/README.rst
-src/obsinfo/_examples/Information_Files/README.txt
-src/obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store
-src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR1.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR2.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR3_LINEAR.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR4_LINEAR.stage_base.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR2.filter.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR1.filter.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR2.filter.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml
-src/obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml
-src/obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml
-src/obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml
-src/obsinfo/_examples/Information_Files/instrumentation/GURALP_CP.instrumentation.yaml
-src/obsinfo/_examples/Information_Files/instrumentation/GURALP_CP.instrumentation.yaml.orig
-src/obsinfo/_examples/Information_Files/instrumentation/HYDROCT1.instrumentation.yaml
-src/obsinfo/_examples/Information_Files/instrumentation/HYDROCT1.instrumentation.yaml.orig
-src/obsinfo/_examples/Information_Files/instrumentation_bases/.DS_Store
-src/obsinfo/_examples/Information_Files/instrumentation_bases/BBOBS1_2012+.instrumentation_base.yaml
-src/obsinfo/_examples/Information_Files/instrumentation_bases/BBOBS1_pre2012.instrumentation_base.yaml
-src/obsinfo/_examples/Information_Files/instrumentation_bases/GURALP_CP.instrumentation_base.yaml_error
-src/obsinfo/_examples/Information_Files/instrumentation_bases/HYDROCT1.instrumentation_base.yaml_error
-src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS1.instrumentation_base.yaml
-src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS2.instrumentation_base.yaml
-src/obsinfo/_examples/Information_Files/instrumentation_bases/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml
-src/obsinfo/_examples/Information_Files/instrumentation_bases/WBOBS1.instrumentation_base.yaml
-src/obsinfo/_examples/Information_Files/instrumentation_bases/empty.instrumentation_base.yaml
-src/obsinfo/_examples/Information_Files/location_bases/.DS_Store
-src/obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml
-src/obsinfo/_examples/Information_Files/networks/EMSO-AZORES.network.yaml
-src/obsinfo/_examples/Information_Files/networks/RHUM-RUM.network.yaml
-src/obsinfo/_examples/Information_Files/operators/.DS_Store
-src/obsinfo/_examples/Information_Files/operators/INSU-IPGP.operator.yaml
-src/obsinfo/_examples/Information_Files/persons/Kevin_Canjamale.person.yaml
-src/obsinfo/_examples/Information_Files/persons/Romuald_Daniel.person.yaml
-src/obsinfo/_examples/Information_Files/persons/Simon_Besancon.person.yaml
-src/obsinfo/_examples/Information_Files/persons/Wayne_Crawford.person.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier.yaml.orig
-src/obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x16_theoretical.stage.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x16_theoretical.stage.yaml.orig
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x32_theoretical.stage.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x32_theoretical.stage.yaml.orig
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x64_theoretical.stage.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_L28x64_theoretical.stage.yaml.orig
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/.DS_Store
-src/obsinfo/_examples/Information_Files/sensors/BUBBLEPHONE_HTI90U.sensor.yaml
-src/obsinfo/_examples/Information_Files/sensors/GURALP_CMG3T_ESPC.sensor.yaml
-src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/HITECH_HTI96-MIN.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/.DS_Store
-src/obsinfo/_examples/Information_Files/sensors/stages/BUBBLEPHONE_HTI90U_SIO-preamp_theoretical.stage.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/BUBBLEPHONE_HTI90U_SIO-preamp_theoretical.stage.yaml.orig
-src/obsinfo/_examples/Information_Files/sensors/stages/Guralp_CMG3T_ESPC_theoretical.stage.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/Guralp_CMG3T_ESPC_theoretical.stage.yaml.orig
-src/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-96-Min_voltage-mode_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_generic_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L22D_LCHEAPO_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/Guralp_CMG3T_ESPC_generic.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/Guralp_CMG3T_ESPC_generic.filter.yaml.orig
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-96-Min_voltage-mode_theoretical.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-96-Min_voltage-mode_theoretical.filter.yaml.orig
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5004_2007.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5017_2007.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__generic.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L22D_C510-S2000_generic.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L28LB-obs_C395-S2490_generic.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml
-src/obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/.DS_Store
-src/obsinfo/_examples/Information_Files/subnetworks/.obsinfo
-src/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml
-src/obsinfo/_examples/Information_Files/timing_bases/.DS_Store
-src/obsinfo/_examples/Information_Files/timing_bases/Seascan_GNSS.timing_base.yaml
-src/obsinfo/_examples/Training/templates/BBOBS-train.network.yaml
-src/obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml
-src/obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml
-src/obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml
-src/obsinfo/_examples/Training/templates/CS5322.stage.yaml
-src/obsinfo/_examples/Training/templates/T240.stage.yaml
-src/obsinfo/_examples/Training/templates/network.yaml
-src/obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml
-src/obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml
-src/obsinfo/_examples/Training/templates/components/preamplifier.yaml
-src/obsinfo/_examples/Training/templates/components/sensor.yaml
-src/obsinfo/_examples/Training/templates/filters/AD_Conversion.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/HiTechPZ.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/HiTech_PolesZeros.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/analog.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/coefficients.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/digital.filter.yaml
-src/obsinfo/_examples/Training/templates/filters/response_list.filter.yaml
-src/obsinfo/_examples/scripts/README.rst
-src/obsinfo/_examples/scripts/make_stationXML.sh
-src/obsinfo/_examples/scripts/print_info_files.sh
-src/obsinfo/_examples/scripts/validate_all.sh
-src/obsinfo/_examples/scripts/validate_files.sh
-src/obsinfo/_examples/scripts/add_ons/README.rst
-src/obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh
-src/obsinfo/addons/LC2SDS.py
-src/obsinfo/addons/LCHEAPO.py
-src/obsinfo/addons/OCA.py
-src/obsinfo/addons/SDPCHAIN.py
-src/obsinfo/addons/__init__.py
-src/obsinfo/addons/infodump.py
-src/obsinfo/console_scripts/__init__.py
-src/obsinfo/console_scripts/_test.py
-src/obsinfo/console_scripts/makeStationXML.py
-src/obsinfo/console_scripts/print.py
-src/obsinfo/console_scripts/print_version.py
-src/obsinfo/console_scripts/setup.py
-src/obsinfo/console_scripts/validate.py
-src/obsinfo/data/schemas/datacite.schema.json
-src/obsinfo/data/schemas/datalogger_base.schema.json
-src/obsinfo/data/schemas/definitions.schema.json
-src/obsinfo/data/schemas/experiment.schema.json
-src/obsinfo/data/schemas/filter.schema.json
-src/obsinfo/data/schemas/instrumentation_base.schema.json
-src/obsinfo/data/schemas/iris_units.json
-src/obsinfo/data/schemas/location_base.schema.json
-src/obsinfo/data/schemas/network.schema.json
-src/obsinfo/data/schemas/operator.schema.json
-src/obsinfo/data/schemas/person.schema.json
-src/obsinfo/data/schemas/preamplifier_base.schema.json
-src/obsinfo/data/schemas/sensor_base.schema.json
-src/obsinfo/data/schemas/stage_base.schema.json
-src/obsinfo/data/schemas/stages.schema.json
-src/obsinfo/data/schemas/subnetwork.schema.json
-src/obsinfo/data/schemas/timing_base.schema.json
-src/obsinfo/datacite/__init__.py
-src/obsinfo/helpers/__init__.py
-src/obsinfo/helpers/comments.py
-src/obsinfo/helpers/external_references.py
-src/obsinfo/helpers/float_with_uncert.py
-src/obsinfo/helpers/functions.py
-src/obsinfo/helpers/identifiers.py
-src/obsinfo/helpers/location.py
-src/obsinfo/helpers/logger.py
-src/obsinfo/helpers/obsinfo_class_list.py
-src/obsinfo/helpers/oi_date.py
-src/obsinfo/helpers/person.py
-src/obsinfo/helpers/phone.py
-src/obsinfo/instrumentation/__init__.py
-src/obsinfo/instrumentation/channel.py
-src/obsinfo/instrumentation/equipment.py
-src/obsinfo/instrumentation/instrument.py
-src/obsinfo/instrumentation/instrument_component.py
-src/obsinfo/instrumentation/instrumentation.py
-src/obsinfo/instrumentation/orientation.py
-src/obsinfo/instrumentation/stage.py
-src/obsinfo/instrumentation/stages.py
-src/obsinfo/instrumentation/filter/AD_conversion.py
-src/obsinfo/instrumentation/filter/FIR.py
-src/obsinfo/instrumentation/filter/__init__.py
-src/obsinfo/instrumentation/filter/analog.py
-src/obsinfo/instrumentation/filter/coefficients.py
-src/obsinfo/instrumentation/filter/digital.py
-src/obsinfo/instrumentation/filter/filter.py
-src/obsinfo/instrumentation/filter/filter_template.py
-src/obsinfo/instrumentation/filter/poles_zeros.py
-src/obsinfo/instrumentation/filter/polynomial.py
-src/obsinfo/instrumentation/filter/response_list.py
-src/obsinfo/misc/__init__.py
-src/obsinfo/misc/configuration.py
-src/obsinfo/misc/const.py
-src/obsinfo/misc/discoveryfiles.py
-src/obsinfo/misc/printobs.py
-src/obsinfo/misc/remoteGitLab.py
-src/obsinfo/misc/yamlref.py
-src/obsinfo/obsmetadata/__init__.py
-src/obsinfo/obsmetadata/obsmetadata.py
-src/obsinfo/subnetwork/__init__.py
-src/obsinfo/subnetwork/network.py
-src/obsinfo/subnetwork/operator.py
-src/obsinfo/subnetwork/processing.py
-src/obsinfo/subnetwork/site.py
-src/obsinfo/subnetwork/station.py
-src/obsinfo/subnetwork/subnetwork.py
-src/obsinfo/templates/.DS_Store
-src/obsinfo/templates/instrumentation.yaml
-src/obsinfo/templates/network.yaml
-src/obsinfo/templates/stage.yaml
-src/obsinfo/templates/components/datalogger.yaml
-src/obsinfo/templates/components/preamplifier.yaml
-src/obsinfo/templates/components/sensor.yaml
-src/obsinfo/templates/filters/AD_Conversion.filter.yaml
-src/obsinfo/templates/filters/FIR.filter.yaml
-src/obsinfo/templates/filters/PolesZeros.filter.yaml
-src/obsinfo/templates/filters/analog.filter.yaml
-src/obsinfo/templates/filters/coefficients.filter.yaml
-src/obsinfo/templates/filters/digital.filter.yaml
-src/obsinfo/templates/filters/response_list.filter.yaml
-src/obsinfo/tests/CompareXMLTree.py
-src/obsinfo/tests/__init__.py
-src/obsinfo/tests/remoteGithub.py
-src/obsinfo/tests/run_test_script.py
-src/obsinfo/tests/test_datapath.py
-src/obsinfo/tests/test_infofile.py
-src/obsinfo/tests/test_main.py
-src/obsinfo/tests/_old/testlog.py
-src/obsinfo/tests/_old/testmain.py
+obsinfo/__init__.py
+obsinfo/version.py
+obsinfo.egg-info/PKG-INFO
+obsinfo.egg-info/SOURCES.txt
+obsinfo.egg-info/dependency_links.txt
+obsinfo.egg-info/entry_points.txt
+obsinfo.egg-info/requires.txt
+obsinfo.egg-info/top_level.txt
+obsinfo/_examples/.DS_Store
+obsinfo/_examples/Information_Files/.DS_Store
+obsinfo/_examples/Information_Files/README.rst
+obsinfo/_examples/Information_Files/README.txt
+obsinfo/_examples/Information_Files/campaigns/SPOBS.campaign.yaml
+obsinfo/_examples/Information_Files/datacites/EMSO-MOMAR_OBS.datacite.yaml
+obsinfo/_examples/Information_Files/dataloggers/ADS1281.datalogger_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/LC2000.datalogger_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/.DS_Store
+obsinfo/_examples/Information_Files/dataloggers/stages/CS5321_FIR1.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR2.with-delay.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/CS5322_FIR3.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_100sps-SINC.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_200sps-SINC.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR1.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR2.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR3_LINEAR.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/TI_ADS1281_FIR4_LINEAR.stage_base.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR2.filter.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/filters/CirrusLogic_CS5322_FIR3.filter.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR1.filter.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR2.filter.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR3-linear.filter.yaml
+obsinfo/_examples/Information_Files/dataloggers/stages/filters/TexasInstruments_ADS1281_FIR4-linear.filter.yaml
+obsinfo/_examples/Information_Files/experiments/MAYOBS.experiment.yaml
+obsinfo/_examples/Information_Files/experiments/MOMAR.experiment.yaml
+obsinfo/_examples/Information_Files/instrumentations/.DS_Store
+obsinfo/_examples/Information_Files/instrumentations/BBOBS1_2012+.instrumentation_base.yaml
+obsinfo/_examples/Information_Files/instrumentations/BBOBS1_pre2012.instrumentation_base.yaml
+obsinfo/_examples/Information_Files/instrumentations/GURALP_CP.instrumentation_base.yaml_error.yaml
+obsinfo/_examples/Information_Files/instrumentations/HYDROCT1.instrumentation_base.yaml_error.yaml
+obsinfo/_examples/Information_Files/instrumentations/SPOBS1.instrumentation_base.yaml
+obsinfo/_examples/Information_Files/instrumentations/SPOBS2.instrumentation_base.yaml
+obsinfo/_examples/Information_Files/instrumentations/SPOBS3-for-channel-mod-testing.instrumentation_base.yaml
+obsinfo/_examples/Information_Files/instrumentations/WBOBS1.instrumentation_base.yaml
+obsinfo/_examples/Information_Files/instrumentations/empty.instrumentation_base.yaml
+obsinfo/_examples/Information_Files/location_bases/.DS_Store
+obsinfo/_examples/Information_Files/location_bases/INSU-IPGP.location_base.yaml
+obsinfo/_examples/Information_Files/networks/EMSO-AZORES.network.yaml
+obsinfo/_examples/Information_Files/networks/RHUM-RUM.network.yaml
+obsinfo/_examples/Information_Files/operators/.DS_Store
+obsinfo/_examples/Information_Files/operators/INSU-IPGP.operator.yaml
+obsinfo/_examples/Information_Files/persons/Kevin_Canjamale.person.yaml
+obsinfo/_examples/Information_Files/persons/Romuald_Daniel.person.yaml
+obsinfo/_examples/Information_Files/persons/Simon_Besancon.person.yaml
+obsinfo/_examples/Information_Files/persons/Wayne_Crawford.person.yaml
+obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_BBOBS.preamplifier_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_DPG.preamplifier_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_GEOPHONE.preamplifier_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO-no_redundancy.preamplifier_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/LCHEAPO_HYDRO.preamplifier_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_BBOBS_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/stages/INSU_SPOBS_geophone_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/stages/SIO-LDEO_DPG-Card_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/preamplifiers/stages/Scripps_SPOBS_HydroL22_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/.DS_Store
+obsinfo/_examples/Information_Files/sensors/HITECH_HTI04-PLC-ULF.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/HITECH_HTI90U.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240__theoretical.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/NANOMETRICS_T240_plusDates.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/NANOMETRICS_TCOMPACT_theoretical.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/SERCEL_L22.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/SERCEL_L28.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/SIO_DPG.sensor_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/.DS_Store
+obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/HiTech_HTI-90U_SIO-preamp_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5004_calibrated.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_5018_calibrated.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/SIO-LDEO_DPG_generic_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/Sercel_L22D_LCHEAPO_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/Sercel_L28LB_LCHEAPO_theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/Trillium_T240__theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/Trillium_TCompact__theoretical.stage_base.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/.DS_Store
+obsinfo/_examples/Information_Files/sensors/stages/filters/HiTech_HTI-04-PLC-ULF_voltage-mode_theoretical.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5004_2007.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__5017_2007.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/SIO-LDEO_DPG__generic.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L22D_C510-S2000_generic.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/Sercel_L28LB-obs_C395-S2490_generic.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN1-399_generic.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_T240_SN400-_generic.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/Trillium_TCompact__generic.filter.yaml
+obsinfo/_examples/Information_Files/sensors/stages/filters/test---attributes-poleszeros.filter.yaml
+obsinfo/_examples/Information_Files/subnetworks/.DS_Store
+obsinfo/_examples/Information_Files/subnetworks/.obsinfo
+obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP.subnetwork.yaml_error.yaml
+obsinfo/_examples/Information_Files/subnetworks/BBOBS.INSU-IPGP_with_gain_mods.subnetwork.yaml_error.yaml
+obsinfo/_examples/Information_Files/subnetworks/EMPTY-INSTRUMENTATION.INSU-IPGP.subnetwork.yaml
+obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential.subnetwork.yaml
+obsinfo/_examples/Information_Files/subnetworks/EXAMPLE_essential_noRefs.subnetwork.yaml
+obsinfo/_examples/Information_Files/subnetworks/LEAP_SECOND.INSU-IPGP.subnetwork.yaml_error.yaml
+obsinfo/_examples/Information_Files/subnetworks/ORIENTED.INSU-IPGP.subnetwork.yaml
+obsinfo/_examples/Information_Files/subnetworks/SPOBS.INSU-IPGP.subnetwork.yaml
+obsinfo/_examples/Information_Files/subnetworks/SPOBS_noAnchors.INSU-IPGP.subnetwork.yaml
+obsinfo/_examples/Information_Files/subnetworks/TEST.subnetwork.yaml_error.yaml
+obsinfo/_examples/Information_Files/timing_bases/.DS_Store
+obsinfo/_examples/Information_Files/timing_bases/Seascan_GNSS.timing_base.yaml
+obsinfo/_examples/Training/templates/BBOBS-train.network.yaml
+obsinfo/_examples/Training/templates/BBOBS.INSU-IPGP.network.yaml
+obsinfo/_examples/Training/templates/BBOBS1.instrumentation.yaml
+obsinfo/_examples/Training/templates/BBOBS1_2012+.instrumentation.yaml
+obsinfo/_examples/Training/templates/CS5322.stage.yaml
+obsinfo/_examples/Training/templates/T240.stage.yaml
+obsinfo/_examples/Training/templates/network.yaml
+obsinfo/_examples/Training/templates/components/LC2000-1.datalogger.yaml
+obsinfo/_examples/Training/templates/components/LC2000.datalogger.yaml
+obsinfo/_examples/Training/templates/components/preamplifier.yaml
+obsinfo/_examples/Training/templates/components/sensor.yaml
+obsinfo/_examples/Training/templates/filters/AD_Conversion.filter.yaml
+obsinfo/_examples/Training/templates/filters/CirrusLogic_FIR.filter.yaml
+obsinfo/_examples/Training/templates/filters/ExampleFIR.filter.yaml
+obsinfo/_examples/Training/templates/filters/HiTechPZ.filter.yaml
+obsinfo/_examples/Training/templates/filters/HiTech_PolesZeros.filter.yaml
+obsinfo/_examples/Training/templates/filters/analog.filter.yaml
+obsinfo/_examples/Training/templates/filters/coefficients.filter.yaml
+obsinfo/_examples/Training/templates/filters/digital.filter.yaml
+obsinfo/_examples/Training/templates/filters/response_list.filter.yaml
+obsinfo/_examples/scripts/README.rst
+obsinfo/_examples/scripts/make_stationXML.sh
+obsinfo/_examples/scripts/print_info_files.sh
+obsinfo/_examples/scripts/validate_all.sh
+obsinfo/_examples/scripts/validate_files.sh
+obsinfo/_examples/scripts/add_ons/README.rst
+obsinfo/_examples/scripts/add_ons/make_data_process_scripts.sh
+obsinfo/addons/LC2SDS.py
+obsinfo/addons/LCHEAPO.py
+obsinfo/addons/OCA.py
+obsinfo/addons/SDPCHAIN.py
+obsinfo/addons/__init__.py
+obsinfo/addons/infodump.py
+obsinfo/console_scripts/__init__.py
+obsinfo/console_scripts/_test.py
+obsinfo/console_scripts/makeStationXML.py
+obsinfo/console_scripts/print.py
+obsinfo/console_scripts/print_version.py
+obsinfo/console_scripts/setup.py
+obsinfo/console_scripts/validate.py
+obsinfo/data/schemas/datacite.schema.json
+obsinfo/data/schemas/datalogger_base.schema.json
+obsinfo/data/schemas/definitions.schema.json
+obsinfo/data/schemas/experiment.schema.json
+obsinfo/data/schemas/filter.schema.json
+obsinfo/data/schemas/instrumentation_base.schema.json
+obsinfo/data/schemas/iris_units.json
+obsinfo/data/schemas/location_base.schema.json
+obsinfo/data/schemas/network.schema.json
+obsinfo/data/schemas/operator.schema.json
+obsinfo/data/schemas/person.schema.json
+obsinfo/data/schemas/preamplifier_base.schema.json
+obsinfo/data/schemas/sensor_base.schema.json
+obsinfo/data/schemas/stage_base.schema.json
+obsinfo/data/schemas/stages.schema.json
+obsinfo/data/schemas/subnetwork.schema.json
+obsinfo/data/schemas/timing_base.schema.json
+obsinfo/datacite/__init__.py
+obsinfo/helpers/__init__.py
+obsinfo/helpers/comments.py
+obsinfo/helpers/external_references.py
+obsinfo/helpers/float_with_uncert.py
+obsinfo/helpers/functions.py
+obsinfo/helpers/identifiers.py
+obsinfo/helpers/location.py
+obsinfo/helpers/obsinfo_class_list.py
+obsinfo/helpers/oi_date.py
+obsinfo/helpers/person.py
+obsinfo/helpers/phone.py
+obsinfo/instrumentation/__init__.py
+obsinfo/instrumentation/channel.py
+obsinfo/instrumentation/equipment.py
+obsinfo/instrumentation/instrument.py
+obsinfo/instrumentation/instrument_component.py
+obsinfo/instrumentation/instrumentation.py
+obsinfo/instrumentation/orientation.py
+obsinfo/instrumentation/stage.py
+obsinfo/instrumentation/stages.py
+obsinfo/instrumentation/filter/AD_conversion.py
+obsinfo/instrumentation/filter/FIR.py
+obsinfo/instrumentation/filter/__init__.py
+obsinfo/instrumentation/filter/analog.py
+obsinfo/instrumentation/filter/coefficients.py
+obsinfo/instrumentation/filter/digital.py
+obsinfo/instrumentation/filter/filter.py
+obsinfo/instrumentation/filter/filter_template.py
+obsinfo/instrumentation/filter/poles_zeros.py
+obsinfo/instrumentation/filter/polynomial.py
+obsinfo/instrumentation/filter/response_list.py
+obsinfo/misc/__init__.py
+obsinfo/misc/configuration.py
+obsinfo/misc/const.py
+obsinfo/misc/discoveryfiles.py
+obsinfo/misc/printobs.py
+obsinfo/misc/remoteGitLab.py
+obsinfo/misc/yamlref.py
+obsinfo/obsMetadata/__init__.py
+obsinfo/obsMetadata/obsmetadata.py
+obsinfo/subnetwork/__init__.py
+obsinfo/subnetwork/operator.py
+obsinfo/subnetwork/processing.py
+obsinfo/subnetwork/site.py
+obsinfo/subnetwork/station.py
+obsinfo/subnetwork/subnetwork.py
+obsinfo/template_specifications/.DS_Store
+obsinfo/template_specifications/instrumentation.yaml
+obsinfo/template_specifications/network.yaml
+obsinfo/template_specifications/stage.yaml
+obsinfo/template_specifications/components/datalogger.yaml
+obsinfo/template_specifications/components/preamplifier.yaml
+obsinfo/template_specifications/components/sensor.yaml
+obsinfo/template_specifications/filters/AD_Conversion.filter.yaml
+obsinfo/template_specifications/filters/FIR.filter.yaml
+obsinfo/template_specifications/filters/PolesZeros.filter.yaml
+obsinfo/template_specifications/filters/analog.filter.yaml
+obsinfo/template_specifications/filters/coefficients.filter.yaml
+obsinfo/template_specifications/filters/digital.filter.yaml
+obsinfo/template_specifications/filters/response_list.filter.yaml
+obsinfo/templates/.DS_Store
+obsinfo/templates/instrumentation.yaml
+obsinfo/templates/network.yaml
+obsinfo/templates/stage.yaml
+obsinfo/templates/components/datalogger.yaml
+obsinfo/templates/components/preamplifier.yaml
+obsinfo/templates/components/sensor.yaml
+obsinfo/templates/filters/AD_Conversion.filter.yaml
+obsinfo/templates/filters/FIR.filter.yaml
+obsinfo/templates/filters/PolesZeros.filter.yaml
+obsinfo/templates/filters/analog.filter.yaml
+obsinfo/templates/filters/coefficients.filter.yaml
+obsinfo/templates/filters/digital.filter.yaml
+obsinfo/templates/filters/response_list.filter.yaml
+obsinfo/tests/CompareXMLTree.py
+obsinfo/tests/__init__.py
+obsinfo/tests/remoteGithub.py
+obsinfo/tests/run_test_script.py
+obsinfo/tests/test_datapath.py
+obsinfo/tests/test_infofile.py
+obsinfo/tests/test_main.py
```

### Comparing `obsinfo-0.111.1.post5/src/obsinfo.egg-info/entry_points.txt` & `obsinfo-0.111b1/obsinfo.egg-info/entry_points.txt`

 * *Files identical despite different names*

