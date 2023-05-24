# Comparing `tmp/RIFT-0.0.15.8rc9.tar.gz` & `tmp/RIFT-0.0.15.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RIFT-0.0.15.8rc9.tar", last modified: Thu Apr 20 10:33:07 2023, max compression
+gzip compressed data, was "RIFT-0.0.15.9rc1.tar", last modified: Wed May 24 11:47:24 2023, max compression
```

## Comparing `RIFT-0.0.15.8rc9.tar` & `RIFT-0.0.15.9rc1.tar`

### file list

```diff
@@ -1,188 +1,193 @@
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/AUTOMATED_OR_ONLINE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/README.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc9/TROUBLESHOOTING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/GETTING_STARTED.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc9/PACKAGING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/requirements.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/LICENSE.md
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10563 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   100226 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   119468 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37686 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    76651 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    96043 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2239 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   163149 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1885 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/switcheroo
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/config_yank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      163 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94119 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   109131 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53601 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28330 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    68867 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   244270 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/INSTALL_OPTIONAL_DEPENDENCIES.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/setup.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc9/howto.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/INSTALL.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/setup.cfg
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MANIFEST.in
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/Dockerfile
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.698197 RIFT-0.0.15.9rc1/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/AUTOMATED_OR_ONLINE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc1/Dockerfile
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/GETTING_STARTED.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/INSTALL.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/INSTALL_OPTIONAL_DEPENDENCIES.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/LICENSE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MANIFEST.in
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.266194 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.270195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.295195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      173 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.306195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/calmarg/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       22 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/calmarg/__init__.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6265 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.325195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53578 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28350 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    68875 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.343195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   249714 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.362195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94177 2023-04-24 19:45:36.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.403195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   109345 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.421195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.303195 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-05-24 11:47:22.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10749 2023-05-24 11:47:22.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-05-24 11:47:22.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-05-24 11:47:22.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-05-24 11:47:22.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-05-24 11:47:24.695196 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13848 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2371 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/config_yank.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2239 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   120192 2023-04-25 00:19:30.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    96043 2023-04-16 18:23:39.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   100973 2023-04-24 19:45:36.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37925 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/switcheroo
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   163553 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    78682 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      276 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_shuffle_file.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc1/PACKAGING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-05-24 11:47:24.697197 RIFT-0.0.15.9rc1/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc1/README.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc1/TROUBLESHOOTING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc1/howto.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       96 2023-04-24 19:45:36.000000 RIFT-0.0.15.9rc1/pyproject.toml
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc1/requirements.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-05-24 11:47:24.698197 RIFT-0.0.15.9rc1/setup.cfg
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `RIFT-0.0.15.8rc9/AUTOMATED_OR_ONLINE.md` & `RIFT-0.0.15.9rc1/AUTOMATED_OR_ONLINE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/README.md` & `RIFT-0.0.15.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/TROUBLESHOOTING.md` & `RIFT-0.0.15.9rc1/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/GETTING_STARTED.md` & `RIFT-0.0.15.9rc1/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/PACKAGING.md` & `RIFT-0.0.15.9rc1/PACKAGING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/LICENSE.md` & `RIFT-0.0.15.9rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,89 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc9
+Version: 0.0.15.9rc1
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
-License: UNKNOWN
-Description: research-projects (temp-RIT-Tides and descendants)
-        research-projects-RIT
-        
-        Repository for the rapid_PE / RIFT code, developed at RIT (forked long ago from work at UWM/CGCA).
-        
-        ## Installation
-        
-        Please see INSTALL.md
-        
-        ## Science
-        
-        If you are using this code for a production analysis, please contact us to make sure you follow the instructions included here!
-        Also, make sure you cite the relevant rapid_pe/RIFT papers
-        
-         1.  Pankow et al 2015
-         2.  Lange et al 2018 (RIFT)
-         3.  Wysocki et al 2019 (RIFT-GPU)
-         4.  Wofforde et al 2022 (RIFT-Update)
-        
-        When preparing your work, please cite 
-        
-         1. the relevant rapid_pe/RIFT papers
-             1.  Pankow et al 2015
-             2.  Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457)
-         
-         2. If you are using the surrogate-basis approach, please cite
-             3. O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O)
-        
-         3. If you are using a GPU-optimized version, please acknowledge
-             4.  Wysocki, O'Shaughnessy,  Fong, Lange [paper](https://arxiv.org/abs/1902.04934)
-        
-         4. If you are using a non-lalsuite waveform interface, please acknowledge
-             1.  gwsurrogate interface: (a) O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O); (b) F. Shaik et al (in prep)
-             2.  TEOBResumS interface (original):  Lange et al 2018 RIFT paper
-             3.  NR interface (parts inside ILE): Lange et al 2017 PRD 96, 404 [NR comparison methods paper](http://adsabs.harvard.edu/abs/2017PhRvD..96j4041L)
-             4.  NRSur7dq2 interface: Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457), and ...
-        
-          5. If you are using an updated Monte Carlo integration package, please acknowledge the authors; papers will be prepared soon
-             1.  GMM integrator: Elizabeth Champion; see [original repo](https://git.ligo.org/benjamin.champion/Monte-Carlo-Integrator), implemented via MonteCarloEnsemble and mcsamplerEnsemble; please cite Ristic et al https://arxiv.org/abs/2105.07013
-             2.  GPU MC integrator:  Wysocki, O'Shaughnessy; cite Wofford et al https://dcc.ligo.org/P2200059
-        
-          6. If you are using a distance-marginalized likeliihood, please acknowledge 
-             1. Distance marginalization : Soichiro Morisaki, Dan Wysocki, see  Wofford et al https://dcc.ligo.org/P2200059
-        
-          7. If you are using a special coordinate system
-             1. Rotated inspiral-phase : cite the original Lee, Morisaki, Tagoshi paper ([journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.124057) [dcc](https://dcc.ligo.org/LIGO-P2200037)); also cite Wofford et al  [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
-             1. Pseudo-cylindrical coordinates: see Wofford et al   [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
-          
-          8. If you are using calibration marginalization, please acknowledge Ethan Payne  (PRD 122004 (2020)), with RIFT integration provided by Jacob Lange and Daniel Williams
-        
-        ## Authorlists: Opt-in model
-        Several aspects of this code are very actively developed.  We encourage  close collaboration with the lead developers (O'Shaughnessy and Lange) to produce the best possible results, particularly given comparatively rapid changes to the interface and pipeline in the past and planned for the future as the user- and developer-base expands.
-        
-        We expect to make the final developed code widely available and free to use, in a release-based distribution model.  But we're not there yet.  To simplify discussions about authorlist and ettiquete, we have adopted the following simple model, to be revised 4 times per year (1/15, 4/15, 7/15, 10/15):  
-         * Free to use: Any code commit older than 3 years from the date an analysis <i>commences</i> is free to use for any scientific work.  
-         * Opt-in: Any more recent use should offer (opt-in) authorship to the lead developers, as well as to developers who contributed significantly to features used in the version of the code adopted in an analysis.  Loosely speaking, the newer the features you use, the more proactive you should be in contacting relevant developers, to insure all authors are suitably engaged with the final product.
-        This policy refers only to commits in this repository, and not to resources and code maintained elsewhere or by other developers (e.g., NR Surrogates), who presumably maintain their own policy.
-        
-        
-        The following authors should be contacted 
-          * O'Shaughnessy and Lange: Iterative pipeline, fitting and posterior generation code, external interfaces (EOB, surrogates)
-          * Field, O'Shaughnessy, Blackman: Surrogate basis method 
-          * Wysocki, O'Shaughnessy,  Fong, Lange: GPU optimizations
-          * ...
-        
-        ## Relationship to version of rapid_pe in lalsuite
-        Chris Pankow has also been maintaining a [port of the original rapid_pe as part of lalsuite](https://github.com/lscsoft/lalsuite/tree/master/lalinference/python/lalinference/rapid_pe). While this code is unreviewed and has many API and workflow differences, the underlying likelihood evaluation procedure has been the same (until the recent GPU rewrite).  We hope to eventually merge the codebases, likely by modernizing the version in lalsuite and/or by ports of rapid_pe techniques to next-generation PE codes.
-        
-        
-        ## Version numbers
-        
-        Short term: roughly major.minor.feature_upgrade.internal_rc_candidates.   So the 4th number are upgraded every few major bugfixes or moves; the 3rd number will upgrade if we add a feature.  We hope to eventually reach version 0.1 for production automated unsupervised analysis during O4
-        
-        Medium-term: Amajor API change or two we are thinking about for how the users specify workflows should be 0.2
-        
-        Long-term: Version 1 will reduce dependency on hardcoded parameter names. More flexibility in how inference is done. 
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+research-projects (temp-RIT-Tides and descendants)
+research-projects-RIT
+
+Repository for the rapid_PE / RIFT code, developed at RIT (forked long ago from work at UWM/CGCA).
+
+## Installation
+
+Please see INSTALL.md
+
+## Science
+
+If you are using this code for a production analysis, please contact us to make sure you follow the instructions included here!
+Also, make sure you cite the relevant rapid_pe/RIFT papers
+
+ 1.  Pankow et al 2015
+ 2.  Lange et al 2018 (RIFT)
+ 3.  Wysocki et al 2019 (RIFT-GPU)
+ 4.  Wofforde et al 2022 (RIFT-Update)
+
+When preparing your work, please cite 
+
+ 1. the relevant rapid_pe/RIFT papers
+     1.  Pankow et al 2015
+     2.  Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457)
+ 
+ 2. If you are using the surrogate-basis approach, please cite
+     3. O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O)
+
+ 3. If you are using a GPU-optimized version, please acknowledge
+     4.  Wysocki, O'Shaughnessy,  Fong, Lange [paper](https://arxiv.org/abs/1902.04934)
+
+ 4. If you are using a non-lalsuite waveform interface, please acknowledge
+     1.  gwsurrogate interface: (a) O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O); (b) F. Shaik et al (in prep)
+     2.  TEOBResumS interface (original):  Lange et al 2018 RIFT paper
+     3.  NR interface (parts inside ILE): Lange et al 2017 PRD 96, 404 [NR comparison methods paper](http://adsabs.harvard.edu/abs/2017PhRvD..96j4041L)
+     4.  NRSur7dq2 interface: Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457), and ...
+
+  5. If you are using an updated Monte Carlo integration package, please acknowledge the authors; papers will be prepared soon
+     1.  GMM integrator: Elizabeth Champion; see [original repo](https://git.ligo.org/benjamin.champion/Monte-Carlo-Integrator), implemented via MonteCarloEnsemble and mcsamplerEnsemble; please cite Ristic et al https://arxiv.org/abs/2105.07013
+     2.  GPU MC integrator:  Wysocki, O'Shaughnessy; cite Wofford et al https://dcc.ligo.org/P2200059
+
+  6. If you are using a distance-marginalized likeliihood, please acknowledge 
+     1. Distance marginalization : Soichiro Morisaki, Dan Wysocki, see  Wofford et al https://dcc.ligo.org/P2200059
+
+  7. If you are using a special coordinate system
+     1. Rotated inspiral-phase : cite the original Lee, Morisaki, Tagoshi paper ([journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.124057) [dcc](https://dcc.ligo.org/LIGO-P2200037)); also cite Wofford et al  [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
+     1. Pseudo-cylindrical coordinates: see Wofford et al   [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
+  
+  8. If you are using calibration marginalization, please acknowledge Ethan Payne  (PRD 122004 (2020)), with RIFT integration provided by Jacob Lange and Daniel Williams
+
+## Authorlists: Opt-in model
+Several aspects of this code are very actively developed.  We encourage  close collaboration with the lead developers (O'Shaughnessy and Lange) to produce the best possible results, particularly given comparatively rapid changes to the interface and pipeline in the past and planned for the future as the user- and developer-base expands.
+
+We expect to make the final developed code widely available and free to use, in a release-based distribution model.  But we're not there yet.  To simplify discussions about authorlist and ettiquete, we have adopted the following simple model, to be revised 4 times per year (1/15, 4/15, 7/15, 10/15):  
+ * Free to use: Any code commit older than 3 years from the date an analysis <i>commences</i> is free to use for any scientific work.  
+ * Opt-in: Any more recent use should offer (opt-in) authorship to the lead developers, as well as to developers who contributed significantly to features used in the version of the code adopted in an analysis.  Loosely speaking, the newer the features you use, the more proactive you should be in contacting relevant developers, to insure all authors are suitably engaged with the final product.
+This policy refers only to commits in this repository, and not to resources and code maintained elsewhere or by other developers (e.g., NR Surrogates), who presumably maintain their own policy.
+
+
+The following authors should be contacted 
+  * O'Shaughnessy and Lange: Iterative pipeline, fitting and posterior generation code, external interfaces (EOB, surrogates)
+  * Field, O'Shaughnessy, Blackman: Surrogate basis method 
+  * Wysocki, O'Shaughnessy,  Fong, Lange: GPU optimizations
+  * ...
+
+## Relationship to version of rapid_pe in lalsuite
+Chris Pankow has also been maintaining a [port of the original rapid_pe as part of lalsuite](https://github.com/lscsoft/lalsuite/tree/master/lalinference/python/lalinference/rapid_pe). While this code is unreviewed and has many API and workflow differences, the underlying likelihood evaluation procedure has been the same (until the recent GPU rewrite).  We hope to eventually merge the codebases, likely by modernizing the version in lalsuite and/or by ports of rapid_pe techniques to next-generation PE codes.
+
+
+## Version numbers
+
+Short term: roughly major.minor.feature_upgrade.internal_rc_candidates.   So the 4th number are upgraded every few major bugfixes or moves; the 3rd number will upgrade if we add a feature.  We hope to eventually reach version 0.1 for production automated unsupervised analysis during O4
+
+Medium-term: Amajor API change or two we are thinking about for how the users specify workflows should be 0.2
+
+Long-term: Version 1 will reduce dependency on hardcoded parameter names. More flexibility in how inference is done.
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 INSTALL_OPTIONAL_DEPENDENCIES.md
 LICENSE.md
 MANIFEST.in
 PACKAGING.md
 README.md
 TROUBLESHOOTING.md
 howto.md
+pyproject.toml
 requirements.txt
 setup.py
 MonteCarloMarginalizeCode/Code/RIFT/__init__.py
 MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
 MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
 MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
 MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
 MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
 MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
+MonteCarloMarginalizeCode/Code/RIFT/calmarg/__init__.py
+MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py
 MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
 MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
 MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
 MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
 MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
 MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
 MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
@@ -168,8 +171,9 @@
 MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
 MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
 MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
 MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
 MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
 MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
 MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
-MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+MonteCarloMarginalizeCode/Code/bin/util_shuffle_file.py
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,16 @@
 optp.add_option("-O", "--output-format", default='xml', help="[xml|hdf5]")
 optp.add_option("-S", "--save-samples", action="store_true", help="Save sample points to output-file. Requires --output-file to be defined.")
 optp.add_option("-L", "--save-deltalnL", type=float, default=float("Inf"), help="Threshold on deltalnL for points preserved in output file.  Requires --output-file to be defined")
 optp.add_option("-P", "--save-P", type=float,default=0.1, help="Threshold on cumulative probability for points preserved in output file.  Requires --output-file to be defined")
 optp.add_option("--internal-hard-fail-on-error",action='store_true',help='If true, fails with exit code 1 if any point is unsuccessful')
 optp.add_option("--internal-soft-fail-on-cuda-error",action='store_true',help='If true, returns with exit code 0 on any CUDA error. Use with care (e.g., if many jobs failing)')
 optp.add_option("--internal-make-empty-file-on-error",action='store_true',help='If true, failed points generate empty output file. Protects against OSG workflow problems')
+optp.add_option("--internal-waveform-fd-L-frame",action='store_true',help='If true, passes extra_waveform_kwargs = {fd_L_frame=True} to lalsimutils hlmoft. Impacts outputs of ChooseFDWaveform calls only.')
+optp.add_option("--internal-waveform-fd-no-condition",action='store_true',help='If true, adds extra_waveform_kwargs = {no_condition=True} to lalsimutils hlmoft. Impacts outputs of ChooseFDWaveform calls only. Provided to enable controlled tests of conditioning impact on PE')
 optp.add_option("--verbose",action='store_true')
 optp.add_option("--save-eccentricity", action="store_true")
 #
 # Add the integration options
 #
 integration_params = OptionGroup(optp, "Integration Parameters", "Control the integration with these options.")
 # Default is actually None, but that tells the integrator to go forever or until n_eff is hit.
@@ -1097,23 +1099,28 @@
     if opts.pin_distance_to_sim:
       pinned_params['distance']=P.dist/(1.e6 * lal.PC_SI)
 
     # Call external likleihood preparation if any
     if supplemental_ln_likelhood_prep:
       supplemental_ln_likelhood_prep(P=P,config=supplemental_ln_likelhood_parsed_ini)
 
+    extra_waveform_kwargs = {}
+    if opts.internal_waveform_fd_L_frame:
+      extra_waveform_kwargs = {'fd_L_frame':True}
+    if opts.internal_waveform_fd_no_condition:
+      extra_waveform_kwargs['no_condition'] = True
     # Precompute
     t_window = 0.15
     rholms_intp, cross_terms, cross_terms_V,  rholms,  guess_snr, rest=factored_likelihood.PrecomputeLikelihoodTerms(
             fiducial_epoch, t_window, P, data_dict, psd_dict, opts.l_max, fmax,
             False, inv_spec_trunc_Q, T_spec,
             NR_group=NR_template_group,NR_param=NR_template_param,
             use_gwsignal=opts.use_gwsignal,
             use_gwsignal_approx=opts.approximant,
-            use_external_EOB=opts.use_external_EOB,nr_lookup=opts.nr_lookup,nr_lookup_valid_groups=opts.nr_lookup_group,perturbative_extraction=opts.nr_perturbative_extraction,perturbative_extraction_full=opts.nr_perturbative_extraction_full,use_provided_strain=opts.nr_use_provided_strain,hybrid_use=opts.nr_hybrid_use,hybrid_method=opts.nr_hybrid_method,ROM_group=opts.rom_group,ROM_param=opts.rom_param,ROM_use_basis=opts.rom_use_basis,verbose=opts.verbose,quiet=not opts.verbose,ROM_limit_basis_size=opts.rom_limit_basis_size_to,no_memory=opts.no_memory,skip_interpolation=opts.vectorized)
+            use_external_EOB=opts.use_external_EOB,nr_lookup=opts.nr_lookup,nr_lookup_valid_groups=opts.nr_lookup_group,perturbative_extraction=opts.nr_perturbative_extraction,perturbative_extraction_full=opts.nr_perturbative_extraction_full,use_provided_strain=opts.nr_use_provided_strain,hybrid_use=opts.nr_hybrid_use,hybrid_method=opts.nr_hybrid_method,ROM_group=opts.rom_group,ROM_param=opts.rom_param,ROM_use_basis=opts.rom_use_basis,verbose=opts.verbose,quiet=not opts.verbose,ROM_limit_basis_size=opts.rom_limit_basis_size_to,no_memory=opts.no_memory,skip_interpolation=opts.vectorized, extra_waveform_kwargs=extra_waveform_kwargs)
 
     if opts.auto_logarithm_offset and guess_snr:
       # important: this only impacts *this* analysis
       # important: if we have a very loud signal, it is important to change this dynamically to avoid *underflow*, which sometimes happens otherwise if we fix the scale early on.
       print("    : naive overflow protection: updating lnL overflow based on SNR guess of {} ".format(guess_snr))
       print("    : reminder, diagnostics for lnLmax below are offset by this amount! ")
       # Note by changing the offset, we change how adapt-weight-exponent is being applied (because we've offset the range before squashing it!).  Use with care: pipeline auto-sets the weight exponent
@@ -1750,15 +1757,15 @@
 no_adapt_sky = False
 for indx in numpy.arange(len(P_list)):
  try:
   res = analyze_event(P_list, indx, data_dict, psd_dict, fmax, opts)
   lnL_sofar = np.max([lnL_sofar,res])
   if opts.force_reset_all:
     for name in sampler.params:
-      sampler.reset_sampling(param)
+      sampler.reset_sampling(name)
   if opts.no_adapt_after_first and (not no_adapt_sky):
     if lnL_sofar > 20:  # Use absolute threshold.  Expect this will give modest sky localization.
       # remove right_ascension, declination from adaptive parameters
       params_adapt = sampler.adaptive
       params_adapt  = list(set(params_adapt) - set(['right_ascension','declination']))
       sampler.adaptive = params_adapt
       # Disable saving of the integrand -- saves on memory and will reduce speed.
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,17 @@
 parser.add_argument("--test-exe",default=None,help="filename of test code or equivalent executable.  Must have a --test-output <fname> argument.  Used for convergence testing or other termination. NOT ACTIVE; see 'convergence_test_samples.py' for example")
 parser.add_argument("--plot-exe",default=None,help="filename of plot code or equivalent executable.  Will default to `which plot_posterior_corner.py`.  Default is to plot last set of samples")
 parser.add_argument("--gridinit-exe",default=None,help="filename of initial grid creation or equivalent executable.  Will default to `which util_ManualOverlapGrid.py`.  Must create overlap-grid-0.xml.gz")
 parser.add_argument("--frame-rotation",action='store_true',help=" Calculation was done in J frame, not L frame.  Rotate at end. Only if extrinsic samples.")
 parser.add_argument("--calibration-reweighting-exe",default=None,help="Calibration reweighting script")
 parser.add_argument("--calibration-reweighting",action='store_true',help="Run calibration reweighting on final posterior samples")
 parser.add_argument("--calibration-reweighting-batchsize",type=int,default=None,help="If not 'None', tries to group the final set of points based on jobs of a fixed size")
+parser.add_argument("--calibration-reweighting-initial-extra-args",type=str,default='',help="Passed to reweighting script as extra args")
+parser.add_argument("--calibration-reweighting-extra-args",type=str,default='',help="Passed to the combination script as extra arguments. ")
+parser.add_argument("--calibration-reweighting-count",type=int,default=100,help="Number of calibration marginalization realizations. Default is 100")
 parser.add_argument("--convert-ascii2h5-exe",default=None,help="Converting ascii to h5 file script")
 parser.add_argument("--comov-distance-reweighting-exe",default=None,help="Comoving distance reweighting script")
 parser.add_argument("--comov-distance-reweighting",action='store_true',help="Run comoving distance reweighting on final posterior samples")
 parser.add_argument("--bilby-pickle-exe",default=None,help="Bilby pickle generation script")
 parser.add_argument("--bilby-ini-file",default=None,help="Filename of bilby ini file used to generate pickle file (used for calibration reweighting)")
 parser.add_argument("--bilby-pickle-file",default=None,help="Filename of bilby pickle file used for calibration reweighting")
 parser.add_argument("--bw-exe",default=None,help="BayesWave location (or wrapper)")
@@ -1070,22 +1073,24 @@
     if opts.use_osg:
         rotate_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
         rotate_job.add_condor_cmd("+flock_local",'true')
     rotate_job.write_sub_file()
 
 if opts.calibration_reweighting:
     if opts.last_iteration_extrinsic_time_resampling and opts.bilby_pickle_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args,n_cal=opts.calibration_reweighting_count)
     elif opts.last_iteration_extrinsic_time_resampling and opts.bilby_ini_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args,n_cal=opts.calibration_reweighting_count)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_ini_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,cache_file=opts.cache_file,frames_dir=opts.frames_dir,ile_args=ile_args)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,lle_args=ile_args,n_cal=opts.calibration_reweighting_count)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_pickle_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args,n_cal=opts.calibration_reweighting_count)
         
+    if opts.calibration_reweighting_initial_extra_args:
+        calibration_job.add_arg(opts.calibration_reweighting_initial_extra_args)
     if not(opts.calibration_reweighting_batchsize): # single run
         calibration_job.set_log_file(opts.working_directory+"/calmarg/logs/calibration-$(cluster)-$(process).log")
         calibration_job.set_stderr_file(opts.working_directory+"/calmarg/logs/calibration-$(cluster)-$(process).err")
         calibration_job.set_stdout_file(opts.working_directory+"/calmarg/logs/calibration-$(cluster)-$(process).out")
     else:
         calibration_job.add_condor_cmd("initialdir",opts.working_directory+"/calmarg/")
         calibration_job.add_arg(" --start_index $(macrostartidx) ")
@@ -1098,15 +1103,15 @@
     if opts.use_full_submit_paths:
         fname = opts.working_directory+"/"+calibration_job.get_sub_file()
         calibration_job.set_sub_file(fname)
     calibration_job.write_sub_file()
 
     # job to combine things. Write here to make logic human-readable
     if (opts.calibration_reweighting_batchsize): # single run
-        reweight_merge_job, reweight_merge_job_name = dag_utils.write_convert_sub(exe=which('combine_weights_and_rejection_sample.py'),tag='CAL_REWEIGHT_COMBINE',log_dir=None,arg_str='',file_input=opts.working_directory+'/extrinsic_posterior_samples.dat weight_files/',file_output=None, out_dir=opts.working_directory,universe=local_worker_universe,no_grid=no_worker_grid)
+        reweight_merge_job, reweight_merge_job_name = dag_utils.write_convert_sub(exe=which('combine_weights_and_rejection_sample.py'),tag='CAL_REWEIGHT_COMBINE',log_dir=None,arg_str=opts.calibration_reweighting_extra_args,file_input=opts.working_directory+'/extrinsic_posterior_samples.dat weight_files/',file_output=None, out_dir=opts.working_directory,universe=local_worker_universe,no_grid=no_worker_grid)
         reweight_merge_job.add_condor_cmd("initialdir",opts.working_directory+"/calmarg/")
         reweight_merge_job.set_log_file(opts.working_directory+"/calmarg/logs/reweight-merge-$(cluster)-$(process).log")
         reweight_merge_job.set_stderr_file(opts.working_directory+"/calmarg/logs/reweight-merge-$(cluster)-$(process).err")
         reweight_merge_job.set_stdout_file(opts.working_directory+"/calmarg/logs/reweight-merge-$(cluster)-$(process).out")
         reweight_merge_job.add_condor_cmd('request_disk',opts.cal_request_disk)
         if opts.use_full_submit_paths:
             fname = opts.working_directory+"/"+reweight_merge_job.get_sub_file()
@@ -1619,15 +1624,15 @@
         dag.add_node(cat_node)
         last_node=cat_node
     else:
         dag.add_node(convert_node)   # this is the time resampling task
         last_node=convert_node
 
 # Create rotation job (if extrinsic available)
-if opts.frame_rotation and opts.add_extrinsic:
+if opts.frame_rotation and opts.last_iteration_extrinsic:
     rotate_node = pipeline.CondorDAGNode(rotate_job)
     rotate_node.set_category("ROTATE")
     rotate_node.add_parent(last_node)
     last_node=rotate_node
     dag.add_node(rotate_node)
 
 # Creating calibration uncertainty job
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,15 @@
 parser.add_argument("--quantiles",default=None,help='List for 1d quantiles intervals. Default is 0.95,0.05')
 parser.add_argument("--chi-max",default=1,type=float)
 parser.add_argument("--lambda-plot-max",default=2000,type=float)
 parser.add_argument("--lnL-cut",default=None,type=float)
 parser.add_argument("--sigma-cut",default=0.4,type=float)
 parser.add_argument("--eccentricity", action="store_true", help="Read sample files in format including eccentricity")
 parser.add_argument("--matplotlib-block-defaults",action="store_true",help="Relies entirely on user to set plot options for plot styles from matplotlibrc")
+parser.add_argument("--no-mod-psi",action="store_true",help="Default is to take psi mod pi. If present, does not do this")
 parser.add_argument("--verbose",action='store_true',help='print matplotlibrc data')
 opts=  parser.parse_args()
 
 plt.rc('axes',unicode_minus=False)
 dpi_base=200
 if not(opts.matplotlib_block_defaults):
     legend_font_base=16
@@ -338,14 +339,16 @@
 posteriorP_list = []
 label_list = []
 # Load posterior files
 if opts.posterior_file:
  for fname in opts.posterior_file:
     samples = np.genfromtxt(fname,names=True,replace_space=None)  # don't replace underscores in names
     samples = standard_expand_samples(samples)
+    if not(opts.no_mod_psi) and 'psi' in samples.dtype.names:
+        samples['psi'] = np.mod(samples['psi'],np.pi)
     # if not 'mtotal' in samples.dtype.names and 'mc' in samples.dtype.names:  # raw LI samples use 
     #     q_here = samples['q']
     #     eta_here = q_here/(1+q_here)
     #     mc_here = samples['mc']
     #     mtot_here = mc_here / np.power(eta_here, 3./5.)
     #     m1_here = mtot_here/(1+q_here)
     #     samples = add_field(samples, [('mtotal', float)]); samples['mtotal'] = mtot_here
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,16 @@
 parser.add_argument("--use-rundir",default=None,type=str,help="Intended to reproduce lalinference_pipe functionality. Must be absolute path.")
 parser.add_argument("--use-online-psd-file",default=None,type=str,help="Provides specific online PSD file, so no downloads are needed")
 parser.add_argument("--use-coinc",default=None,type=str,help="Intended to reproduce lalinference_pipe functionality")
 parser.add_argument("--manual-ifo-list",default=None,type=str,help="Overrides IFO list normally retrieve by event ID.  Use with care (e.g., glitch studies) or for events specified with --event-time.")
 parser.add_argument("--online",action='store_true')
 parser.add_argument("--calibration-reweighting",action='store_true',help="Option to add job to DAG to reweight posterior samples due to calibration uncertainty.")
 parser.add_argument("--calibration-reweighting-batchsize",type=int,default=None,help="If not 'None', tries to group the final set of points based on jobs of a fixed size")
+parser.add_argument("--calibration-reweighting-count",type=int,default=None,help="If not 'None', the number of calibration curves to request when marginalizing. Default is 100")
+parser.add_argument("--calibration-reweighting-extra-args",type=str,default=None,help="If not 'None', pass through. One argument targets effective sample size, other duplicates inoutput")
 parser.add_argument("--distance-reweighting",action='store_true',help="Option to add job to DAG to reweight posterior samples due to different distance prior (LVK prod prior)")
 parser.add_argument("--extra-args-helper",action=None, help="Filename with arguments for the helper. Use to provide alternative channel names and other advanced configuration (--channel-name, data type)!")
 parser.add_argument("--manual-postfix",default='',type=str)
 parser.add_argument("--gracedb-id",default=None,type=str)
 parser.add_argument("--gracedb-exe",default="gracedb")
 parser.add_argument("--use-legacy-gracedb",action='store_true')
 parser.add_argument("--internal-use-gracedb-bayestar",action='store_true',help="Retrieve BS skymap from gracedb (bayestar.fits), and use it internally in integration with --use-skymap bayestar.fits.")
@@ -252,14 +254,15 @@
 parser.add_argument("--use-osg-file-transfer",action='store_true',help="Restructuring for ILE on OSG. The code will NOT use CVMFS, and instead will try to transfer the frame files.")
 parser.add_argument("--internal-truncate-files-for-osg-file-transfer",action='store_true',help="If use-osg-file-transfer, will use FrCopy plus the start/end time to build the frame directory.")
 parser.add_argument("--condor-local-nonworker",action='store_true',help="Provide this option if job will run in non-NFS space. ")
 parser.add_argument("--condor-nogrid-nonworker",action='store_true',help="NOW STANDARD, auto-set if you pass use-osg   Causes flock_local for 'internal' jobs")
 parser.add_argument("--use-osg-simple-requirements",action='store_true',help="Provide this option if job should use a more aggressive setting for OSG matching ")
 parser.add_argument("--archive-pesummary-label",default=None,help="If provided, creates a 'pesummary' directory and fills it with this run's final output at the end of the run")
 parser.add_argument("--archive-pesummary-event-label",default="this_event",help="Label to use on the pesummary page itself")
+parser.add_argument("--internal-mitigate-fd-J-frame",default="L_frame",help="L_frame|rotate, choose method to deal with ChooseFDWaveform being in wrong frame. Default is to request L frame for inputs")
 opts=  parser.parse_args()
 
 
 if (opts.use_ini):
     # Attempt to lazy-parse all command line arguments from ini file
     config = ConfigParser.ConfigParser()
     config.optionxform=str # force preserve case! Important for --choose-data-LI-seglen
@@ -292,14 +295,19 @@
                 else:
                     config_dict[item_renamed] = True
         print(config_dict)
 
 if opts.ile_copies <=0:
     raise Exception(" Must have 1 or more ILE instances per intrinsic point")
 
+if not(opts.internal_mitigate_fd_J_frame in ['L_frame', 'rotate']):
+    raise Exception(" Unknown option for internal_mitigate_fd_J_frame")
+if (opts.approx in ['IMRPhenomXPHM' or 'IMRPhenomXO4']) and opts.assume_precessing:
+    print(" NOTE NOTE NOTE : Mitigation of ChooseFDWaveform frame being applied : {} ".format(opts.internal_mitigate_fd_J_frame))
+
 if opts.internal_loud_signal_mitigation_suite:
     opts.internal_ile_freezeadapt=False  # make sure to adapt every iteration, and adapt in distance if present
     opts.internal_ile_sky_network_coordinates=True # skymap is better
     opts.internal_ile_rotate_phase = True  # phase coordinates can be sharper
 
 # Default prior for aligned analysis should be z prior !
 if opts.assume_nonprecessing or opts.approx == "IMRPhenomD":
@@ -745,29 +753,29 @@
     dmax_guess = 10000
 # Last stage of commands done by other tools: too annoying to copy stuff over and run the next generation of the pipeline
 instructions_ile = np.loadtxt("helper_ile_args.txt", dtype=str)  # should be one line
 line = ' '.join(instructions_ile)
 if opts.internal_ile_n_max:
     line = line.replace('--n-max 4000000 ', str(opts.internal_ile_n_max)+" ")
 line += " --l-max " + str(opts.l_max) 
-if 'data-start-time' in line:
+if 'data-start-time' in line and 's1z' in event_dict:  # only call this if we have (a) fixed time interval and (b) CBC parameters for event
     # Print warnings based on duration and fmin
     line_dict = unsafe_parse_arg_string_dict(line)
-    data_start_time = line_dict['data-start-time']
-    data_end_time = line_dict['data-end-time']
+    data_start_time = float(line_dict['data-start-time'])
+    data_end_time = float(line_dict['data-end-time'])
     P.m1 = event_dict["m1"]*lal.MSUN_SI; P.m2=event_dict["m2"]*lal.MSUN_SI; P.s1z = event_dict["s1z"]; P.s2z = event_dict["s2z"]
     P.fmin = opts.fmin  #  fmin we will use internally
     if opts.fmin_template:
         P.fmin = opts.fmin_template
     if opts.l_max > 2 and (("IMRPhenomXP" in opts.approx) or ('XO4a' in opts.approx)):
         # fmin is start for all modes.   If Lmax>2, use fmin*(2/Lmax) to estimate starting frequecy
         P_temp = P.copy()
         P_temp.fmin *= 2./opts.l_max
         t_HM = lalsimutils.estimateWaveformDuration(P_temp)
-        if  opts.data_LI_seglen < t_HM/2:
+        if  data_end_time - data_start_time < t_HM/2:
             print("""  WARNING WARNING WARNING WARNING WARNING WARNING WARNING WARNING 
 Your choice of fmin, lmax, and approximant suggests waveform wraparound will occur.  We recommend a longer segment length
 """
 )
     elif opts.l_max > 2 and opts.fmin_template:
         # all modes start at the same time, possibly with different frequencies. Starting frequency needs to be reduced 
         # User has specified fmin_template, and therefore overridden our default plan to lower the starting frequency
@@ -812,14 +820,16 @@
     line += " --sampler-method {} ".format(opts.ile_sampler_method)
 if opts.internal_ile_sky_network_coordinates:
     line += " --internal-sky-network-coordinates "
 if opts.ile_no_gpu:  # make sure we are using the standard code path if not using GPUs
     line += " --force-xpy " 
 if opts.internal_ile_force_noreset_adapt:
     line = line.replace(' --force-reset-all ', ' ')
+if opts.internal_mitigate_fd_J_frame == 'L_frame':
+    line += " --internal-waveform-fd-L-frame "
 with open('args_ile.txt','w') as f:
         f.write(line)
 
 
 #os.system("cp helper_test_args.txt args_test.txt")
 with open ("helper_test_args.txt",'r') as f:
     line = f.readline()
@@ -1140,18 +1150,26 @@
     cmd += " --ile-runtime-max-minutes {} ".format(opts.ile_runtime_max_minutes)
 if not(opts.internal_use_amr) or opts.internal_use_amr_puff:
     cmd+= " --puff-exe `which util_ParameterPuffball.py` --puff-cadence 1 --puff-max-it " + str(puff_max_it)+ " --puff-args `pwd`/args_puff.txt "
 if opts.assume_eccentric:
     cmd += " --use-eccentricity "
 if opts.calibration_reweighting and (not opts.bilby_pickle_file):
     cmd += " --calibration-reweighting --calibration-reweighting-exe `which calibration_reweighting.py` --bilby-ini-file {} --bilby-pickle-exe `which bilby_pipe_generation` ".format(str(opts.bilby_ini_file))
+    if opts.calibration_reweighting_count:
+        cmd+= " --calibration-reweighting-count {} ".format(opts.calibration_reweighting_count)
     if opts.calibration_reweighting_batchsize:
         cmd += " --calibration-reweighting-batchsize {} ".format(opts.calibration_reweighting_batchsize)
+    if opts.calibration_reweighting_extra_args:
+        cmd += " --calibration-reweighting-extra-args '{}' ".format(opts.calibration_reweighting_extra_args)
 elif opts.calibration_reweighting and opts.bilby_pickle_file:
     cmd += " --calibration-reweighting --calibration-reweighting-exe `which calibration_reweighting.py` --bilby-pickle-file {} ".format(str(opts.bilby_pickle_file))
+    if opts.calibration_reweighting_count:
+        cmd+= " --calibration-reweighting-count {} ".format(opts.calibration_reweighting_count)
+    if opts.calibration_reweighting_extra_args:
+        cmd += " --calibration-reweighting-extra-args '{}' ".format(opts.calibration_reweighting_extra_args)
 
 if opts.distance_reweighting:
     cmd += " --comov-distance-reweighting --comov-distance-reweighting-exe `which make_uni_comov_skymap.py` --convert-ascii2h5-exe `which convert_output_format_ascii2h5.py` "
 if opts.use_gauss_early:
     cmd += " --cip-exe-G `which util_ConstructIntrinsicPosterior_GaussianResampling.py ` "
 if opts.internal_use_amr:
     print(" AMR prototype: Using hardcoded aligned-spin settings, assembling grid, requires coinc!")
@@ -1255,20 +1273,24 @@
     cmd += " --condor-nogrid-nonworker "
 if opts.use_osg_simple_requirements:
     cmd += " --use-osg-simple-reqirements "
 if opts.archive_pesummary_label:
 #    cmd += " --plot-exe `which summarypages` --plot-args  args_plot.txt "
     cmd += " --plot-exe summarypages --plot-args  args_plot.txt "
 # Horribly annoying XPHM/XO4a fix because ChooseFDWaveform called.  Seems to be UNIVERSAL for the approximant name, but only if precessing
-if (opts.approx == 'IMRPhenomXPHM' or 'XO4a' in opts.approx) and opts.assume_precessing:
+if opts.internal_mitigate_fd_J_frame == 'rotate' and (opts.approx == 'IMRPhenomXPHM' or 'XO4a' in opts.approx) and opts.assume_precessing:
     cmd += " --frame-rotation "
+if opts.internal_mitigate_fd_J_frame =="L_frame":
+    cmd +=" --calibration-reweighting-initial-extra-args='--internal-waveform-fd-L-frame' "
 print(cmd)
 os.system(cmd)
 
 if opts.use_osg_file_transfer and opts.internal_truncate_files_for_osg_file_transfer:
+    if opts.fake_data_cache:
+        shutil.copyfile(opts.fake_data_cache, 'local.cache')
     # build truncated frames.  Note this parses ILE arguments, so must be done last
     os.system("util_ForOSG_MakeTruncatedLocalFramesDir.sh .")
 
 ## RUNMON
 try:
     from runmonitor import store_tools as sto
     if opts.use_ini != None: # making an assumption that opts.use_ini corresponds to prod_O3b file structures, and that opts.use_ini == None corresponds to standard setup with opts.gracedb_id passed. Maybe not a robust assumptio
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -910,15 +910,20 @@
             # just a  trick to make reweighting more efficient.
             prior_map['chiz_plus'] = s_component_zprior
             prior_map['chiz_minus'] = s_component_zprior
         else:
             prior_map['chiz_plus'] = s_component_gaussian_prior
             prior_map['chiz_minus'] = s_component_gaussian_prior
 
-if opts.transverse_prior == 'uniform-mag':
+if opts.transverse_prior == 'uniform':
+    # Don't do anything: let the default uniform priros for s1x, s1y ... OR chi1_perp-bar, etc used be used
+    # Note these have different physical meaning!
+    print(" Transverse prior: Uniform in PROPOSED COORDINATES (defaults). Note physical meaning depends on coordinate choice!")
+    True
+elif opts.transverse_prior == 'uniform-mag':   # intent: only for these chi1_perp_bar, chi2_perp_bar coordinates
     # allow for better transverse spin prior, 
     prior_map['chi1_perp_bar'] = unnormalized_uniform_prior
     prior_map['chi2_perp_bar'] = unnormalized_uniform_prior
 elif opts.transverse_prior == "Rbar-singular":
     prior_map["chi1_perp_bar"] = normalized_Rbar_singular_prior
     prior_map["chi2_perp_bar"] = normalized_Rbar_singular_prior
 elif opts.transverse_prior == 'alignedspin-zprior':
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 parser.add(
     "--posterior_sample_file", default=None,
     help="Bilby result file or text file with posterior samples to reweight")
 parser.add(
     "--data_dump_file", default=None,
     help="Bilby pipe data_dump file. This stores all the relevant data for PE")
 parser.add(
+    "--waveform_approximant", default=None,
+    help="Approximant. Override what is in the pickle file (as expected if running across settings)")
+parser.add(
     "--number_of_calibration_curves", type=int, default=1000,
     help="Number of calibration curve realizations to use to reweight samples.")
 parser.add(
     "--time_marginalization", type=bool, default=False,
     help="Uses time maginalization when evaluating the likelihoods. Defaults to False")
 parser.add(
     "--phase_marginalization", type=bool, default=False,
@@ -80,14 +83,19 @@
     help="Use nested samples with their weights to generate the samples. This significantly improves efficiency.")
 parser.add(
     "--time_marginalization_interval", default=0.1, type=float,
     help="Interval over which the time marginalization is undertaken")
 parser.add(
     "--use_rift_samples", type=bool, default=False,
     help="Uses a different waveform function if using RIFT samples. This matches the phase definitions in RIFT")
+parser.add(
+    "--h_method", type=str, default='hlmoft',
+    help="For RIFT, uses two different options for h(t) reconstruction ")
+parser.add("--internal-waveform-fd-L-frame",action='store_true',help='If true, passes extra_waveform_kwargs = {fd_L_frame=True} to lalsimutils hlmoft. Impacts outputs of ChooseFDWaveform calls only.')
+parser.add("--internal-waveform-fd-no-condition",action='store_true',help='If true, adds extra_waveform_kwargs = {no_condition=True} to lalsimutils hlmoft. Impacts outputs of ChooseFDWaveform calls only. Provided to enable controlled tests of conditioning impact on PE')
 parser.add("--fmin", default=None, type=float)
 parser.add("--l-max", default=4, type=int)
 parser.add("--start_index", default=None, type=int)
 parser.add("--end_index", default=None, type=int)
 
 args = parser.parse_args()
 
@@ -110,19 +118,22 @@
     if end_index is not None:
         if end_index > len(result.posterior):
             end_index = len(result.posterior)
     result.posterior = result.posterior.iloc[start_index:end_index].reset_index(drop=True)
     result.meta_data = {}
 
     if args.use_rift_samples:
+        result.posterior  = result.posterior.drop(columns=['lnL','ps'])
+        result.posterior['p'] = np.log(result.posterior['p'])  # not sure if used, but if so define correctly
         key_swap_dict = {'m1':'mass_1', 'm2':'mass_2', 'a1x':'spin_1x', 'a1y':'spin_1y', 'a1z':'spin_1z',
             'a2x':'spin_2x', 'a2y':'spin_2y', 'a2z':'spin_2z', 'incl':'iota', 'time':'geocent_time',
         'phiorb':'phase', 'p':'log_prior', 'distance':'luminosity_distance', 'lambda1':'lambda_1', 'lambda2':'lambda_2'}
 
-        for old_key in result.posterior.keys():
+        names = list(result.posterior.keys())  # dangerous to have iterator tied to changing structure
+        for old_key in names:
             if old_key in key_swap_dict:
                 result.posterior[key_swap_dict[old_key]] = result.posterior[old_key]
                 del result.posterior[old_key]
         # add tides if not present
         if not('lambda_1' in result.posterior):
             print(" Populating empty tidal params to avoid hang")
             if end_index:
@@ -153,15 +164,25 @@
         result.posterior['phase'] = np.zeros(len(result.posterior))
 
 # Setting up the waveform generator using the data dump features
 waveform_arguments = dict(
     reference_frequency=data.meta_data['command_line_args']['reference_frequency'],
     minimum_frequency=args.fmin,
     waveform_approximant=data.meta_data['command_line_args']['waveform_approximant'],
-    sampling_frequency=ifos.sampling_frequency)
+    sampling_frequency=ifos.sampling_frequency,
+    h_method=args.h_method)
+
+extra_waveform_kwargs={}
+if args.internal_waveform_fd_L_frame:
+    extra_waveform_kwargs = {'fd_L_frame':True}
+if args.internal_waveform_fd_no_condition:
+    extra_waveform_kwargs['no_condition'] = True
+waveform_arguments['extra_waveform_kwargs'] = extra_waveform_kwargs
+if args.waveform_approximant:
+    waveform_arguments['waveform_approximant'] = args.waveform_approximant
 
 if args.use_rift_samples:
     waveform_arguments['Lmax'] = args.l_max
 #    waveform_arguments['waveform_approximant'] = 'SEOBNRv4PHM'
     wf_func = rift_source.RIFT_lal_binary_black_hole
 else:
     wf_func = eval('bilby.gw.source.'+data.meta_data['command_line_args']['frequency_domain_source_model'])
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     file_num = file.lstrip('weights_s')
     number = file_num.split('e')[0]
     return int(number)
 
 # load in the arguments
 sample_file = sys.argv[1]
 weights_file_directory = sys.argv[2]
+allow_alternate=False
+allow_duplicates = False
+if len(sys.argv) > 3:   # if 3 arguments passed, target the effective sample size as output size
+    allow_alternate=True
+if len(sys.argv) > 4:
+    allow_duplicates=True
 
 outdir = os.path.dirname(os.path.abspath(sample_file))
 
 # Load the sample file
 if sample_file.split(".")[-1] == 'json':
     result = bilby.core.result.read_in_result(sample_file)
 elif (sample_file.split(".")[-1] == 'txt') or (sample_file.split(".")[-1] == 'dat'):
@@ -51,9 +57,13 @@
 npts_samples = len(result.posterior['m1'])
 print(" Sizes ", npts_samples, npts_wts)
 if npts_samples > len(weights):
     print(" Truncating input samples to weight size (=requested output size) ")
     result.posterior = result.posterior.truncate(after=npts_wts-1)
 
 print(f'Importance sampling efficiency: {np.sum(weights)**2/np.sum(weights**2)/len(weights)}')
-result.posterior = bilby.core.result.rejection_sample(result.posterior, weights)
+if not(allow_alternate):
+    result.posterior = bilby.core.result.rejection_sample(result.posterior, weights)
+else:
+    n_est = int(len(weights)*np.sum(weights)**2/np.sum(weights**2)/len(weights))+1  # effective sample size used to draw
+    result.posterior = result.posterior.sample(n=n_est,weights=weights/np.sum(weights),replace=allow_duplicates)
 result.save_posterior_samples(filename=outdir+'/reweighted_posterior_samples.dat', outdir=outdir)
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/config_yank.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/config_yank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 # Main driver functions
 #
 def PrecomputeLikelihoodTerms(event_time_geo, t_window, P, data_dict,
         psd_dict, Lmax, fMax, analyticPSD_Q=False,
         inv_spec_trunc_Q=False, T_spec=0., verbose=True,quiet=False,
          NR_group=None,NR_param=None,
         ignore_threshold=1e-4,   # dangerous for peak lnL of 25^2/2~300 : biases
+        extra_waveform_kwargs={},
         use_gwsignal=False,
         use_gwsignal_approx=None,
        use_external_EOB=False,nr_lookup=False,nr_lookup_valid_groups=None,no_memory=True,perturbative_extraction=False,perturbative_extraction_full=False,hybrid_use=False,hybrid_method='taper_add',use_provided_strain=False,ROM_group=None,ROM_param=None,ROM_use_basis=False,ROM_limit_basis_size=None,skip_interpolation=False):
     """
     Compute < h_lm(t) | d > and < h_lm | h_l'm' >
 
     Returns:
@@ -241,15 +242,15 @@
         # else:
         #         hlms = hlms_list
         # hlms_conj_list = lsu.conj_hlmoff(P, Lmax)
         # if not isinstance(hlms_list,dict):
         #         hlms_conj = lsu.SphHarmFrequencySeries_to_dict(hlms_conj_list, Lmax) # a dictionary
         # else:
         #         hlms_conj = hlms_conj_list
-        hlms, hlms_conj = lsu.std_and_conj_hlmoff(P,Lmax)
+        hlms, hlms_conj = lsu.std_and_conj_hlmoff(P,Lmax,**extra_waveform_kwargs)
     elif (nr_lookup or NR_group) and useNR:
 	    # look up simulation
 	    # use nrwf to get hlmf
         print(" Using NR waveforms ")
         group = None
         param = None
         if nr_lookup:
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1940,15 +1940,15 @@
         ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
     except:
         print(" LIGO accounting information not available.  You must add this manually to integrate.sub !")
 
     return ile_job, ile_sub_name
 
 
-def write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight', exe=None, log_dir=None, ncopies=1,request_memory=8192,time_marg=True,pickle_file=None,posterior_file=None,universe='vanilla',no_grid=False,ile_args=None,**kwargs):
+def write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight', exe=None, log_dir=None, ncopies=1,request_memory=8192,time_marg=True,pickle_file=None,posterior_file=None,universe='vanilla',no_grid=False,ile_args=None,n_cal=100,**kwargs):
     """
     Write a submit file for launching jobs to reweight final posterior samples due to calibration uncertainty 
 
     Inputs:
      - posterior samples, event pickle file (generated by Bilby)
     Outputs:
      - reweighted samples due to calibration uncertainty and corresponding weights
@@ -1977,41 +1977,45 @@
     ile_job.set_stderr_file("%s%s-%s.err" % (log_dir, tag, uniq_str))
     ile_job.set_stdout_file("%s%s-%s.out" % (log_dir, tag, uniq_str))
 
     #
     # Add mandatory options
     ile_job.add_opt('data_dump_file', str(pickle_file))
     ile_job.add_opt('posterior_sample_file', str(posterior_file))
-    ile_job.add_opt('number_of_calibration_curves', '100')
+    ile_job.add_opt('number_of_calibration_curves', str(n_cal))
     ile_job.add_opt('reevaluate_likelihood', 'True')
     ile_job.add_opt('use_rift_samples', 'True')
     if time_marg:
         # problem with this argument: 'False' is often parsed as 'True' by argparsing (weird). Default is 'false'
         ile_job.add_opt('time_marginalization', str(time_marg))
 
     lmax=None
+    approx=None
     if ile_args:
         ile_args_split = ile_args.split('--')
         fmin_list = []
         fmin_template = None
         for line in ile_args_split:
             line_split = line.split()
             if len(line_split)>1:
                 if line_split[0] == 'fmin-ifo':
                     fmin_list += [line_split[1]]
                 if line_split[0] == 'fmin-template':
                     fmin_template = line_split[1]
                 elif line_split[0] == 'l-max':
                     lmax = int(line_split[1])
+                elif line_split[0] == 'approx':
+                    approx = line_split[1]
 #        fmin = np.min(fmin_list)
         if fmin_template:
             ile_job.add_arg(" --fmin {} ".format(fmin_template))  # code will fail without this, and it is always written anyways, but 
         if lmax:
             ile_job.add_arg(" --l-max {} ".format(lmax))
-
+        if approx:
+            ile_job.add_arg(" --waveform_approximant {} ".format(approx))
     #
     # Add normal arguments
     #
     for opt, param in list(kwargs.items()):
         if isinstance(param, list) or isinstance(param, tuple):
             # NOTE: Hack to get around multiple instances of the same option
             for p in param:
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         if isinstance(rvs, int) or isinstance(rvs, float):
             #
             # Convert all arguments to tuples
             #
             # FIXME: UGH! Really? This was the most elegant thing you could come
             # up with?
             rvs_tmp = [numpy.random.uniform(0,1,(len(p), int(rvs))) for p in [(i,) if not isinstance(i, tuple) else i for i in args]]
-            rvs_tmp = numpy.array([self.cdf_inv[param](*rv) for (rv, param) in zip(rvs_tmp, args)], dtype=numpy.object)
+            rvs_tmp = numpy.array([self.cdf_inv[param](*rv) for (rv, param) in zip(rvs_tmp, args)], dtype=object)
         else:
             rvs_tmp = numpy.array(rvs)
 
         # FIXME: ELegance; get some of that...
         # This is mainly to ensure that the array can be "splatted", e.g.
         # separated out into its components for matching with args. The case of
         # one argument has to be handled specially.
@@ -678,16 +678,15 @@
                     if rosDebugMessages:
                         print("     -  New adaptive exponent  ", tempering_exp_running, " based on max 1d weight ", numpy.max(weights), " based on parameter ", p)
 
 #                print "      Weights",  type(weights),weights.dtype
                 self._hist[p], edges = numpy.histogram( points,
                     bins = 100,
                     range = (self.llim[p], self.rlim[p]),
-                    weights = weights,
-                    normed = True
+                    weights = weights
                 )
                 # FIXME: numpy.hist can't normalize worth a damn
                 self._hist[p] /= self._hist[p].sum()
 
                 # Mix with uniform distribution
                 self._hist[p] = (1-floor_integrated_probability)*self._hist[p] + numpy.ones(len(self._hist[p]))*floor_integrated_probability/len(self._hist[p])
                 if rosDebugMessages and bShowEvaluationLog:
@@ -774,15 +773,15 @@
                 return 0
 def uniform_samp_cdf_inv_vector(a,b,p):
     # relies on input being a numpy array, with range from 0 to 1
     out= p.copy()
     out = p*(b-a) + a
     return out
 #uniform_samp_vector = numpy.vectorize(uniform_samp,excluded=['a','b'],otypes=[numpy.float])
-uniform_samp_vector = numpy.vectorize(uniform_samp,otypes=[numpy.float])
+uniform_samp_vector = numpy.vectorize(uniform_samp,otypes=[numpy.float64])
 
 def ret_uniform_samp_vector_alt(a,b):
     return lambda x: numpy.where( (x>a) & (x<b), numpy.reciprocal(b-a),0.0)
 
 # def uniform_samp_withfloor_vector(rmaxQuad,rmaxFlat,pFlat,x):
 #     ret =0.
 #     if x<rmaxQuad:
@@ -822,27 +821,27 @@
 
 def quadratic_samp(rmax,x):
         if x<rmax:
                 return x**2/(3*rmax**3)
         else:
                 return 0
 
-quadratic_samp_vector = numpy.vectorize(quadratic_samp, otypes=[numpy.float])
+quadratic_samp_vector = numpy.vectorize(quadratic_samp, otypes=[numpy.float64])
 
 def inv_uniform_cdf(a, b, x):
     return (b-a)*x+a
 
 def gauss_samp(mu, std, x):
     return 1.0/numpy.sqrt(2*numpy.pi*std**2)*numpy.exp(-(x-mu)**2/2/std**2)
 
 def gauss_samp_withfloor(mu, std, myfloor, x):
     return 1.0/numpy.sqrt(2*numpy.pi*std**2)*numpy.exp(-(x-mu)**2/2/std**2) + myfloor
 
 #gauss_samp_withfloor_vector = numpy.vectorize(gauss_samp_withfloor,excluded=['mu','std','myfloor'],otypes=[numpy.float])
-gauss_samp_withfloor_vector = numpy.vectorize(gauss_samp_withfloor,otypes=[numpy.float])
+gauss_samp_withfloor_vector = numpy.vectorize(gauss_samp_withfloor,otypes=[numpy.float64])
 
 
 # Mass ratio. PDF propto 1/(1+q)^2.  Defined so mass ratio is < 1
 # expr = Integrate[1/(1 + q)^2, q]
 # scale = (expr /. q -> qmax )  - (expr /. q -> qmin)
 # (expr - (expr /. q -> qmin))/scale == x // Simplify
 # q /. Solve[%, q][[1]] // Simplify
@@ -862,40 +861,40 @@
 def cos_samp(x):
         return numpy.sin(x)/2   # x from 0, pi
 
 def dec_samp(x):
         return numpy.sin(x+numpy.pi/2)/2   # x from 0, pi
 
 
-cos_samp_vector = lambda x: cos_samp(numpy.array(x,dtype=numpy.float))
-dec_samp_vector = lambda x: dec_samp(numpy.array(x,dtype=numpy.float))
+cos_samp_vector = lambda x: cos_samp(numpy.array(x,dtype=numpy.float64))
+dec_samp_vector = lambda x: dec_samp(numpy.array(x,dtype=numpy.float64))
 
 #cos_samp_vector = numpy.vectorize(cos_samp,otypes=[numpy.float])
 #dec_samp_vector = numpy.vectorize(dec_samp,otypes=[numpy.float])
 def cos_samp_cdf_inv_vector(p):
     return numpy.arccos( 2*p-1)   # returns from 0 to pi
 def dec_samp_cdf_inv_vector(p):
     return numpy.arccos(2*p-1) - numpy.pi/2  # target from -pi/2 to pi/2
 
 
 def pseudo_dist_samp(r0,r):
         return r*r*numpy.exp( - (r0/r)*(r0/r)/2. + r0/r)+0.01  # put a floor on probability, so we converge. Note this floor only cuts out NEARBY distances
 
 #pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[numpy.float])
-pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,otypes=[numpy.float])
+pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,otypes=[numpy.float64])
 
 def delta_func_pdf(x_0, x):
     return 1.0 if x == x_0 else 0.0
 
-delta_func_pdf_vector = numpy.vectorize(delta_func_pdf, otypes=[numpy.float])
+delta_func_pdf_vector = numpy.vectorize(delta_func_pdf, otypes=[numpy.float64])
 
 def delta_func_samp(x_0, x):
     return x_0
 
-delta_func_samp_vector = numpy.vectorize(delta_func_samp, otypes=[numpy.float])
+delta_func_samp_vector = numpy.vectorize(delta_func_samp, otypes=[numpy.float64])
 
 
 def linear_down_samp(x,xmin=0,xmax=1):
     """
     distribution p(x) \propto (xmax-x) 
     """
     return 2./(xmax-xmin)**2 * numpy.power(xmax-x,1)
@@ -1056,15 +1055,15 @@
             rnd_n = numpy.random.randint(0, np, len(ra_in))
             dec_in, ra_in = self.valid_points_hist[:,rnd_n]
             return numpy.array([dec_in, ra_in])
         else:
             raise ValueError("%s is not a recgonized sampling type" % stype)
 
 #pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[numpy.float])
-pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,otypes=[numpy.float])
+pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,otypes=[numpy.float64])
 
 
 def sanityCheckSamplerIntegrateUnity(sampler,*args,**kwargs):
         return sampler.integrate(lambda *args: 1,*args,**kwargs)
 
 ###
 ### CONVERGENCE TESTS
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,16 +398,16 @@
 
 def gauss_samp(mu, std, x):
     return 1.0/np.sqrt(2*np.pi*std**2)*np.exp(-(x-mu)**2/2/std**2)
 
 def gauss_samp_withfloor(mu, std, myfloor, x):
     return 1.0/np.sqrt(2*np.pi*std**2)*np.exp(-(x-mu)**2/2/std**2) + myfloor
 
-#gauss_samp_withfloor_vector = np.vectorize(gauss_samp_withfloor,excluded=['mu','std','myfloor'],otypes=[np.float])
-gauss_samp_withfloor_vector = np.vectorize(gauss_samp_withfloor,otypes=[np.float])
+#gauss_samp_withfloor_vector = np.vectorize(gauss_samp_withfloor,excluded=['mu','std','myfloor'],otypes=[np.float64])
+gauss_samp_withfloor_vector = np.vectorize(gauss_samp_withfloor,otypes=[np.float64])
 
 
 # Mass ratio. PDF propto 1/(1+q)^2.  Defined so mass ratio is < 1
 # expr = Integrate[1/(1 + q)^2, q]
 # scale = (expr /. q -> qmax )  - (expr /. q -> qmin)
 # (expr - (expr /. q -> qmin))/scale == x // Simplify
 # q /. Solve[%, q][[1]] // Simplify
@@ -426,37 +426,37 @@
 
 def cos_samp(x):
         return np.sin(x)/2   # x from 0, pi
 
 def dec_samp(x):
         return np.sin(x+np.pi/2)/2   # x from 0, pi
 
-cos_samp_vector = np.vectorize(cos_samp,otypes=[np.float])
-dec_samp_vector = np.vectorize(dec_samp,otypes=[np.float])
+cos_samp_vector = np.vectorize(cos_samp,otypes=[np.float64])
+dec_samp_vector = np.vectorize(dec_samp,otypes=[np.float64])
 def cos_samp_cdf_inv_vector(p):
     return np.arccos( 2*p-1)   # returns from 0 to pi
 def dec_samp_cdf_inv_vector(p):
     return np.arccos(2*p-1) - np.pi/2  # target from -pi/2 to pi/2
 
 
 def pseudo_dist_samp(r0,r):
         return r*r*np.exp( - (r0/r)*(r0/r)/2. + r0/r)+0.01  # put a floor on probability, so we converge. Note this floor only cuts out NEARBY distances
 
-#pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[np.float])
-pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,otypes=[np.float])
+#pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[np.float64])
+pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,otypes=[np.float64])
 
 def delta_func_pdf(x_0, x):
     return 1.0 if x == x_0 else 0.0
 
-delta_func_pdf_vector = np.vectorize(delta_func_pdf, otypes=[np.float])
+delta_func_pdf_vector = np.vectorize(delta_func_pdf, otypes=[np.float64])
 
 def delta_func_samp(x_0, x):
     return x_0
 
-delta_func_samp_vector = np.vectorize(delta_func_samp, otypes=[np.float])
+delta_func_samp_vector = np.vectorize(delta_func_samp, otypes=[np.float64])
 
 class HealPixSampler(object):
     """
     Class to sample the sky using a FITS healpix map. Equivalent to a joint 2-D pdf in RA and dec.
     """
 
     @staticmethod
@@ -589,16 +589,16 @@
             np = self.valid_points_hist.shape[1]
             rnd_n = np.random.randint(0, np, len(ra_in))
             dec_in, ra_in = self.valid_points_hist[:,rnd_n]
             return np.array([dec_in, ra_in])
         else:
             raise ValueError("%s is not a recgonized sampling type" % stype)
 
-#pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[np.float])
-pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,otypes=[np.float])
+#pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[np.float64])
+pseudo_dist_samp_vector = np.vectorize(pseudo_dist_samp,otypes=[np.float64])
 
 
 def sanityCheckSamplerIntegrateUnity(sampler,*args,**kwargs):
         return sampler.integrate(lambda *args: 1,*args,**kwargs)
 
 ###
 ### CONVERGENCE TESTS
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py`

 * *Files 0% similar despite different names*

```diff
@@ -1356,26 +1356,26 @@
     return x*scale
 
 
 
 def pseudo_dist_samp(r0,r):
         return r*r*numpy.exp( - (r0/r)*(r0/r)/2. + r0/r)+0.01  # put a floor on probability, so we converge. Note this floor only cuts out NEARBY distances
 
-#pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[numpy.float])
-pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,otypes=[numpy.float])
+#pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[numpy.float64])
+pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,otypes=[numpy.float64])
 
 def delta_func_pdf(x_0, x):
     return 1.0 if x == x_0 else 0.0
 
-delta_func_pdf_vector = numpy.vectorize(delta_func_pdf, otypes=[numpy.float])
+delta_func_pdf_vector = numpy.vectorize(delta_func_pdf, otypes=[numpy.float64])
 
 def delta_func_samp(x_0, x):
     return x_0
 
-delta_func_samp_vector = numpy.vectorize(delta_func_samp, otypes=[numpy.float])
+delta_func_samp_vector = numpy.vectorize(delta_func_samp, otypes=[numpy.float64])
 
 
 
 def sanityCheckSamplerIntegrateUnity(sampler,*args,**kwargs):
         return sampler.integrate(lambda *args: 1,*args,**kwargs)
 
 ###
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3114,15 +3114,15 @@
 
 
 ## Version protection
 #   Pull out arguments of the ModesFromPolarizations function
 #argist_FromPolarizations=lalsim.SimInspiralTDModesFromPolarizations.__doc__.split('->')[0].replace('SimInspiralTDModesFromPolarizations','').replace('REAL8','').replace('Dict','').replace('Approximant','').replace('(','').replace(')','').split(',')
 
 
-def hlmoft(P, Lmax=2,nr_polarization_convention=False, fixed_tapering=False, silent=True, fd_standoff_factor=0.964,no_condition=False,**kwargs ):
+def hlmoft(P, Lmax=2,nr_polarization_convention=False, fixed_tapering=False, silent=True, fd_standoff_factor=0.964,no_condition=False,fd_L_frame=False,**kwargs ):
     """
     Generate the TD h_lm -2-spin-weighted spherical harmonic modes of a GW
     with parameters P. Returns a SphHarmTimeSeries, a linked-list of modes with
     a COMPLEX16TimeSeries and indices l and m for each node.
 
     The linked list will contain all modes with l <= Lmax
     and all values of m for these l.
@@ -3131,14 +3131,15 @@
 
     fd_standoff_factor: for ChooseFDWaveform, reduce starting frequency P.fmin by this factor internally when generating.
           FD waveform calculation implicitly assumes fmin is in the inspiral regime (if not you are making bad life choices).
           Default value of 0.964 is based on changing inspiral duration by 10% (1.1^(3/8) ~ 1.036). Any constant factor will change
           the inspiral duration by a factor (1./fd_standoff_factor)^(8/3) or so.
 
     no_condition: disable conditioning (for ChooseFDModes specifically). For diagnostic plots on impact of/need for conditioning.
+    fd_L_frame: rotate hlmoft to L frame from J frame for return values from ChooseFDModes (XO4/XPHM). 
     """
     assert Lmax >= 2
 
     # Check that masses are not nan!
     assert (not np.isnan(P.m1)) and (not np.isnan(P.m2)), " masses are NaN "
 
     sign_factor = 1
@@ -3191,14 +3192,20 @@
                   # just multiply the very end by a small amount of tapering
                   hlmsT[mode].data.data[TDlen-ntaper:]*=vectaper[::-1]
               else:
                   # zero out a a lot of time at the end, and taper time as we approach this critical extra time
                   hlmsT[mode].data.data[indx_crit:indx_crit+ntaper] *= vectaper[::-1]
                   hlmsT[mode].data.data[indx_crit+ntaper:] = 0
 
+       # Rotate if requested, and if P.fref is specified
+       if fd_L_frame and P.fref:
+           alpha,beta,gamma =extract_JL_angles(P)
+           hlmsT_alt = rotate_hlm_static(hlmsT, alpha,beta,gamma)
+           hlmsT = hlmsT_alt
+
        if P.deltaF is not None:
           if not silent:
               print(hlmsT[mode].data.length,TDlen, " and in seconds ", hlmsT[mode].data.length*hlmsT[mode].deltaT,TDlen*P.deltaT, " with deltaT={} {}".format(hlmsT[mode].deltaT,P.deltaT))
           for mode in hlmsT:
              hlms[mode] = lal.ResizeCOMPLEX16TimeSeries(hlmsT[mode],0,TDlen)
        return hlms
 
@@ -3753,16 +3760,16 @@
             if hxx:
                 hxx.data.data = np.conj(hxx.data.data)
     # FFT the hlms
     Hlms = lalsim.SphHarmFrequencySeriesFromSphHarmTimeSeries(hlms)
 
     return Hlms
 
-def std_and_conj_hlmoff(P, Lmax=2):
-    hlms = hlmoft(P, Lmax)
+def std_and_conj_hlmoff(P, Lmax=2,**kwargs):
+    hlms = hlmoft(P, Lmax,**kwargs)
     if isinstance(hlms,dict):
         hlmsF = {}
         hlms_conj_F = {}
         for mode in hlms:
             hlmsF[mode] = DataFourier(hlms[mode])
             hlms[mode].data.data = np.conj(hlms[mode].data.data)
             hlms_conj_F[mode] = DataFourier(hlms[mode])
@@ -3974,28 +3981,28 @@
             P.psi, P.eccentricity, P.meanPerAno, \
             P.deltaF, P.fmin, TDlen*P.deltaF/2, P.fref, \
             extra_params, P.approx)
 
         if TDlen > 0:
             if P.approx != lalsim.IMRPhenomP:
                 assert TDlen/2+1 >= hptilde.data.length  # validates nyqist for real-valued series
-            hptilde = lal.ResizeCOMPLEX16FrequencySeries(hptilde, 0, TDlen/2+1)
-            hctilde = lal.ResizeCOMPLEX16FrequencySeries(hctilde, 0, TDlen/2+1)
+            hptilde = lal.ResizeCOMPLEX16FrequencySeries(hptilde, 0, int(TDlen/2)+1)
+            hctilde = lal.ResizeCOMPLEX16FrequencySeries(hctilde, 0, int(TDlen/2)+1)
 
 
         # Pack so f=0 occurs at one side
         hoff = lal.CreateCOMPLEX16FrequencySeries("Template h(f)", 
             hptilde.epoch, hptilde.f0, 1./P.deltaT/TDlen, lsu_HertzUnit, 
             TDlen)
 
         # create the 2-sided hoff
         tmp  = hptilde.data.data + sgn*1j*hctilde.data.data
-        hoff.data.data[-TDlen/2-2:-1] = tmp
+        hoff.data.data[-int(TDlen/2)-2:-1] = tmp
         tmp= np.conj(hptilde.data.data) + sgn*1j*np.conj(hctilde.data.data)
-        hoff.data.data[0:TDlen/2+1] = tmp[::-1]
+        hoff.data.data[0:int(TDlen/2)+1] = tmp[::-1]
 
         # Translate the wavefront to the detector, if we are not at the origin of spacetime
         # Implement by just changing 'epoch', not by any fancy frequency-domain modulation? 
         #   - NO, we want all timesamples to have regular timestamps in the geocenter. So we WILL modulate
         if P.radec==False:
             return hoff
         else:
@@ -4910,15 +4917,14 @@
         m2_vals =np.zeros(len(x_in))  
         if ('delta_mc' in low_level_coord_names):
             indx_delta = low_level_coord_names.index('delta_mc')
             eta_vals = 0.25*(1- x_in[:,indx_delta]**2)
         elif ('eta' in low_level_coord_names):
             indx_eta = low_level_coord_names.index('eta')
             eta_vals = x_in[:,indx_eta]
-            m1_vals,m2_vals = m1m2(x_in[:,indx_mc],eta_vals)
         m1_vals,m2_vals = m1m2(x_in[:,indx_mc],eta_vals)
         x_out[:,indx_p_out] = (m1_vals*x_in[:,indx_s1z] + m2_vals*x_in[:,indx_s2z])/(m1_vals+m2_vals)
         coord_names_reduced.remove('xi')
     if ('chiMinus' in coord_names_reduced) and ('s1z' in low_level_coord_names) and ('s2z' in low_level_coord_names) and ('mc' in low_level_coord_names):
         indx_p_out = coord_names.index('chiMinus')
         p = 'chiMinus'
         indx_mc = low_level_coord_names.index('mc')
@@ -5233,14 +5239,41 @@
         A1S1p =  np.c_[A1*m1_vals**2 *s1x,  A1*m1_vals**2 *s1y]
         A2S2p =  np.c_[A2*m2_vals**2 *s2x,  A2*m2_vals**2 *s2y]
         Sp =np.maximum(np.linalg.norm( A1S1p,axis=-1), np.linalg.norm(A2S2p,axis=-1))
         x_out[:,indx_pout_chip] = Sp/(A1*m1_vals**2)
         coord_names_reduced.remove('chi_p')
         
 
+    if ('LambdaTilde' in coord_names_reduced) and ('lambda1' in low_level_coord_names and 'lambda2' in low_level_coord_names):
+        # deal with scenario where only one of lambda1, lambda2 specified IN FUTURE
+        indx_p_out = coord_names.index('LambdaTilde')
+        indx_la1 = low_level_coord_names.index('lambda1')
+        indx_la2 = low_level_coord_names.index('lambda2')
+        la1_vals = x_in[:,indx_la1]
+        la2_vals = x_in[:,indx_la2]
+        if 'mc' in low_level_coord_names and 'delta_mc' in low_level_coord_names:
+            eta_vals = np.zeros(len(x_in))  
+            m1_vals =np.zeros(len(x_in))  
+            m2_vals =np.zeros(len(x_in))  
+            if ('delta_mc' in low_level_coord_names):
+                indx_delta = low_level_coord_names.index('delta_mc')
+                eta_vals = 0.25*(1- x_in[:,indx_delta]**2)
+            elif ('eta' in low_level_coord_names):
+                indx_eta = low_level_coord_names.index('eta')
+                eta_vals = x_in[:,indx_eta]
+            m1_vals,m2_vals = m1m2(x_in[:,indx_mc],eta_vals)
+            Lt, dLt   = tidal_lambda_tilde(m1_vals, m2_vals, la1_vals, la2_vals)
+            x_out[:,indx_p_out] = Lt
+            coord_names_reduced.remove('LambdaTilde')
+            if 'DeltaLambdaTilde' in coord_names_reduced:
+                indx_q_out = coord_names.index('DeltLambdaTilde')
+                x_out[:,indx_q_out] = dLt
+                coord_names_reduced.remove('DeltaLambdaTilde')
+
+
     # return if we don't need to do any more conversions (e.g., if we only have --parameter specification)
     if len(coord_names_reduced)<1:
         return x_out
 
     print(" Fallthrough to non-vector-coords for ", coord_names_reduced,low_level_coord_names)
     
     P = ChooseWaveformParams()
@@ -5415,7 +5448,79 @@
     mc_min = np.exp( -ln_mc_error_pseudo_fisher) * Mchirp_event
 
     if force_mc_range:
         mc_min,mc_max = list(map(float, force_mc_range.replace('[','').replace(']','').split(',')))
 
     return mc_min,mc_max
 
+
+def rotate_hlm_static(hlm,alphaA,betaA,gammaA):
+    """
+    Rotate output hlm by these Euler angles
+    Note this is a full system rotation, and therefore should be associated with rotation of the physical quantities (e.g., spin vectors, J,L)
+    """
+    hCatOut = {}
+    modes = list(hlm)
+    Lmax = np.max(np.array(modes)[:,0]) # Lmax
+    h0 = hlm[modes[0]] # some reference mode, for types
+    lal_type=False
+
+    for L in range(2, Lmax+1):
+        for M in range(-L,L+1):
+            hCatOut[(L,M)] = None
+            # Define output data
+            if isinstance(hlm[(L,M)], lal.COMPLEX16TimeSeries):
+                hCatOut[(L,M)] = lal.CreateCOMPLEX16TimeSeries("Template h(t)", 
+                                                 h0.epoch, h0.f0, h0.deltaT, lsu_DimensionlessUnit, 
+                                                 h0.data.length)
+                hCatOut[(L,M)].data.data *=0 # initialize
+                lal_type=True
+            elif isinstance(hlm[(L,M)] , lal.Complex16FrequencySeries):
+                hCatOut[(L,M)] =  lal.CreateCOMPLEX16FrequencySeries("Template h(t)", 
+                                                                     h0.epoch, h0.f0, h0.deltaF, lsu_HertzUnit ,
+                                                                     h0.data.length)
+                hCatOut[(L,M)].data.data *=0 # initialize
+                lal_type=True
+            elif isinstance(hlm[(L,M)], np.ndarray):
+                hCatOut[(L,M)] = np.zeros(h0.shape)
+            else:
+                raise ValueError(" hlm unknown data type for rotation")
+            # Loop and populate, based on input modes. Does not need to be full in input, but will be full output
+            for mode in modes:
+                if mode[0]==L:
+                    if lal_type:
+                        hCatOut[(L,M)].data.data += lal.WignerDMatrix(L,M,mode[1], alphaA, betaA,gammaA)*hlm[mode].data.data
+                    else:
+                        hCatOut[(L,M)] += lal.WignerDMatrix(L,M,mode[1], alphaA, betaA,gammaA)*hlm[mode]
+
+    return hCatOut
+
+
+def extract_JL_angles(P):
+    Lref = P.OrbitalAngularMomentumAtReferenceOverM2()
+    Lhat = Lref/np.sqrt(np.dot(Lref,Lref))
+    Jref = P.TotalAngularMomentumAtReferenceOverM2()
+    Jhat = Jref/np.sqrt(np.dot(Jref, Jref))
+
+    nhat_obs = np.array([ np.sin(P.incl)*np.cos(np.pi/2-P.phiref), np.sin(P.incl)*np.sin(np.pi/2-P.phiref), np.cos(P.incl)])  # base vector
+    vecZ = np.array([0,0,1])
+    vecY = np.array([0,1,0])
+
+    # thetaJL == beta
+    # To make review-stable, be VERY explicit : try to use lalsuite function calls, not above
+    my_cos = np.dot(Lhat, Jhat)
+    theta_JL = P.incl   # this is pretty close. Good enough if we are nearly aligned
+    if my_cos < 1-1e-5:  # but if we are even slightly misaligned, use the acos of above
+        theta_JL = np.arccos( my_cos ) #P.extract_param('beta')  # this is just Jhat.Jhat
+    theta_jn, phi_JL, theta_1, theta_2, phi_12, a_1, a_2 =lalsim.SimInspiralTransformPrecessingWvf2PE(
+            P.incl, P.s1x, P.s1y, P.s1z, P.s2x, P.s2y, P.s2z, P.m1, P.m2, P.fref, P.phiref)
+#    phi_JL = P.extract_param('phiJL')   # note should be related to euler angles of 
+
+    # rotation from J to point along L for example
+    rot = np.matmul(rotation_matrix( vecY, -theta_JL), rotation_matrix( vecZ, -phi_JL))
+
+    # Rotation around L needed to rotate viewing direction
+    nhat_rot = np.matmul(rot, nhat_obs)
+    last_angle = np.angle( nhat_rot[0]+1j*nhat_rot[1])
+
+    # Phase conventions as in XPHM paper https://journals.aps.org/prd/abstract/10.1103/PhysRevD.103.104056
+    return np.pi - last_angle, theta_JL, np.pi-phi_JL
```

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py` & `RIFT-0.0.15.9rc1/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/PKG-INFO` & `RIFT-0.0.15.9rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,89 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc9
+Version: 0.0.15.9rc1
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
-License: UNKNOWN
-Description: research-projects (temp-RIT-Tides and descendants)
-        research-projects-RIT
-        
-        Repository for the rapid_PE / RIFT code, developed at RIT (forked long ago from work at UWM/CGCA).
-        
-        ## Installation
-        
-        Please see INSTALL.md
-        
-        ## Science
-        
-        If you are using this code for a production analysis, please contact us to make sure you follow the instructions included here!
-        Also, make sure you cite the relevant rapid_pe/RIFT papers
-        
-         1.  Pankow et al 2015
-         2.  Lange et al 2018 (RIFT)
-         3.  Wysocki et al 2019 (RIFT-GPU)
-         4.  Wofforde et al 2022 (RIFT-Update)
-        
-        When preparing your work, please cite 
-        
-         1. the relevant rapid_pe/RIFT papers
-             1.  Pankow et al 2015
-             2.  Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457)
-         
-         2. If you are using the surrogate-basis approach, please cite
-             3. O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O)
-        
-         3. If you are using a GPU-optimized version, please acknowledge
-             4.  Wysocki, O'Shaughnessy,  Fong, Lange [paper](https://arxiv.org/abs/1902.04934)
-        
-         4. If you are using a non-lalsuite waveform interface, please acknowledge
-             1.  gwsurrogate interface: (a) O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O); (b) F. Shaik et al (in prep)
-             2.  TEOBResumS interface (original):  Lange et al 2018 RIFT paper
-             3.  NR interface (parts inside ILE): Lange et al 2017 PRD 96, 404 [NR comparison methods paper](http://adsabs.harvard.edu/abs/2017PhRvD..96j4041L)
-             4.  NRSur7dq2 interface: Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457), and ...
-        
-          5. If you are using an updated Monte Carlo integration package, please acknowledge the authors; papers will be prepared soon
-             1.  GMM integrator: Elizabeth Champion; see [original repo](https://git.ligo.org/benjamin.champion/Monte-Carlo-Integrator), implemented via MonteCarloEnsemble and mcsamplerEnsemble; please cite Ristic et al https://arxiv.org/abs/2105.07013
-             2.  GPU MC integrator:  Wysocki, O'Shaughnessy; cite Wofford et al https://dcc.ligo.org/P2200059
-        
-          6. If you are using a distance-marginalized likeliihood, please acknowledge 
-             1. Distance marginalization : Soichiro Morisaki, Dan Wysocki, see  Wofford et al https://dcc.ligo.org/P2200059
-        
-          7. If you are using a special coordinate system
-             1. Rotated inspiral-phase : cite the original Lee, Morisaki, Tagoshi paper ([journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.124057) [dcc](https://dcc.ligo.org/LIGO-P2200037)); also cite Wofford et al  [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
-             1. Pseudo-cylindrical coordinates: see Wofford et al   [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
-          
-          8. If you are using calibration marginalization, please acknowledge Ethan Payne  (PRD 122004 (2020)), with RIFT integration provided by Jacob Lange and Daniel Williams
-        
-        ## Authorlists: Opt-in model
-        Several aspects of this code are very actively developed.  We encourage  close collaboration with the lead developers (O'Shaughnessy and Lange) to produce the best possible results, particularly given comparatively rapid changes to the interface and pipeline in the past and planned for the future as the user- and developer-base expands.
-        
-        We expect to make the final developed code widely available and free to use, in a release-based distribution model.  But we're not there yet.  To simplify discussions about authorlist and ettiquete, we have adopted the following simple model, to be revised 4 times per year (1/15, 4/15, 7/15, 10/15):  
-         * Free to use: Any code commit older than 3 years from the date an analysis <i>commences</i> is free to use for any scientific work.  
-         * Opt-in: Any more recent use should offer (opt-in) authorship to the lead developers, as well as to developers who contributed significantly to features used in the version of the code adopted in an analysis.  Loosely speaking, the newer the features you use, the more proactive you should be in contacting relevant developers, to insure all authors are suitably engaged with the final product.
-        This policy refers only to commits in this repository, and not to resources and code maintained elsewhere or by other developers (e.g., NR Surrogates), who presumably maintain their own policy.
-        
-        
-        The following authors should be contacted 
-          * O'Shaughnessy and Lange: Iterative pipeline, fitting and posterior generation code, external interfaces (EOB, surrogates)
-          * Field, O'Shaughnessy, Blackman: Surrogate basis method 
-          * Wysocki, O'Shaughnessy,  Fong, Lange: GPU optimizations
-          * ...
-        
-        ## Relationship to version of rapid_pe in lalsuite
-        Chris Pankow has also been maintaining a [port of the original rapid_pe as part of lalsuite](https://github.com/lscsoft/lalsuite/tree/master/lalinference/python/lalinference/rapid_pe). While this code is unreviewed and has many API and workflow differences, the underlying likelihood evaluation procedure has been the same (until the recent GPU rewrite).  We hope to eventually merge the codebases, likely by modernizing the version in lalsuite and/or by ports of rapid_pe techniques to next-generation PE codes.
-        
-        
-        ## Version numbers
-        
-        Short term: roughly major.minor.feature_upgrade.internal_rc_candidates.   So the 4th number are upgraded every few major bugfixes or moves; the 3rd number will upgrade if we add a feature.  We hope to eventually reach version 0.1 for production automated unsupervised analysis during O4
-        
-        Medium-term: Amajor API change or two we are thinking about for how the users specify workflows should be 0.2
-        
-        Long-term: Version 1 will reduce dependency on hardcoded parameter names. More flexibility in how inference is done. 
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+research-projects (temp-RIT-Tides and descendants)
+research-projects-RIT
+
+Repository for the rapid_PE / RIFT code, developed at RIT (forked long ago from work at UWM/CGCA).
+
+## Installation
+
+Please see INSTALL.md
+
+## Science
+
+If you are using this code for a production analysis, please contact us to make sure you follow the instructions included here!
+Also, make sure you cite the relevant rapid_pe/RIFT papers
+
+ 1.  Pankow et al 2015
+ 2.  Lange et al 2018 (RIFT)
+ 3.  Wysocki et al 2019 (RIFT-GPU)
+ 4.  Wofforde et al 2022 (RIFT-Update)
+
+When preparing your work, please cite 
+
+ 1. the relevant rapid_pe/RIFT papers
+     1.  Pankow et al 2015
+     2.  Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457)
+ 
+ 2. If you are using the surrogate-basis approach, please cite
+     3. O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O)
+
+ 3. If you are using a GPU-optimized version, please acknowledge
+     4.  Wysocki, O'Shaughnessy,  Fong, Lange [paper](https://arxiv.org/abs/1902.04934)
+
+ 4. If you are using a non-lalsuite waveform interface, please acknowledge
+     1.  gwsurrogate interface: (a) O'Shaughnessy, Blackman, Field 2017 [paper](http://adsabs.harvard.edu/abs/2017CQGra..34n4002O); (b) F. Shaik et al (in prep)
+     2.  TEOBResumS interface (original):  Lange et al 2018 RIFT paper
+     3.  NR interface (parts inside ILE): Lange et al 2017 PRD 96, 404 [NR comparison methods paper](http://adsabs.harvard.edu/abs/2017PhRvD..96j4041L)
+     4.  NRSur7dq2 interface: Lange et al 2018 (RIFT) [paper](https://arxiv.org/abs/1805.10457), and ...
+
+  5. If you are using an updated Monte Carlo integration package, please acknowledge the authors; papers will be prepared soon
+     1.  GMM integrator: Elizabeth Champion; see [original repo](https://git.ligo.org/benjamin.champion/Monte-Carlo-Integrator), implemented via MonteCarloEnsemble and mcsamplerEnsemble; please cite Ristic et al https://arxiv.org/abs/2105.07013
+     2.  GPU MC integrator:  Wysocki, O'Shaughnessy; cite Wofford et al https://dcc.ligo.org/P2200059
+
+  6. If you are using a distance-marginalized likeliihood, please acknowledge 
+     1. Distance marginalization : Soichiro Morisaki, Dan Wysocki, see  Wofford et al https://dcc.ligo.org/P2200059
+
+  7. If you are using a special coordinate system
+     1. Rotated inspiral-phase : cite the original Lee, Morisaki, Tagoshi paper ([journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.124057) [dcc](https://dcc.ligo.org/LIGO-P2200037)); also cite Wofford et al  [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
+     1. Pseudo-cylindrical coordinates: see Wofford et al   [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
+  
+  8. If you are using calibration marginalization, please acknowledge Ethan Payne  (PRD 122004 (2020)), with RIFT integration provided by Jacob Lange and Daniel Williams
+
+## Authorlists: Opt-in model
+Several aspects of this code are very actively developed.  We encourage  close collaboration with the lead developers (O'Shaughnessy and Lange) to produce the best possible results, particularly given comparatively rapid changes to the interface and pipeline in the past and planned for the future as the user- and developer-base expands.
+
+We expect to make the final developed code widely available and free to use, in a release-based distribution model.  But we're not there yet.  To simplify discussions about authorlist and ettiquete, we have adopted the following simple model, to be revised 4 times per year (1/15, 4/15, 7/15, 10/15):  
+ * Free to use: Any code commit older than 3 years from the date an analysis <i>commences</i> is free to use for any scientific work.  
+ * Opt-in: Any more recent use should offer (opt-in) authorship to the lead developers, as well as to developers who contributed significantly to features used in the version of the code adopted in an analysis.  Loosely speaking, the newer the features you use, the more proactive you should be in contacting relevant developers, to insure all authors are suitably engaged with the final product.
+This policy refers only to commits in this repository, and not to resources and code maintained elsewhere or by other developers (e.g., NR Surrogates), who presumably maintain their own policy.
+
+
+The following authors should be contacted 
+  * O'Shaughnessy and Lange: Iterative pipeline, fitting and posterior generation code, external interfaces (EOB, surrogates)
+  * Field, O'Shaughnessy, Blackman: Surrogate basis method 
+  * Wysocki, O'Shaughnessy,  Fong, Lange: GPU optimizations
+  * ...
+
+## Relationship to version of rapid_pe in lalsuite
+Chris Pankow has also been maintaining a [port of the original rapid_pe as part of lalsuite](https://github.com/lscsoft/lalsuite/tree/master/lalinference/python/lalinference/rapid_pe). While this code is unreviewed and has many API and workflow differences, the underlying likelihood evaluation procedure has been the same (until the recent GPU rewrite).  We hope to eventually merge the codebases, likely by modernizing the version in lalsuite and/or by ports of rapid_pe techniques to next-generation PE codes.
+
+
+## Version numbers
+
+Short term: roughly major.minor.feature_upgrade.internal_rc_candidates.   So the 4th number are upgraded every few major bugfixes or moves; the 3rd number will upgrade if we add a feature.  We hope to eventually reach version 0.1 for production automated unsupervised analysis during O4
+
+Medium-term: Amajor API change or two we are thinking about for how the users specify workflows should be 0.2
+
+Long-term: Version 1 will reduce dependency on hardcoded parameter names. More flexibility in how inference is done.
```

### Comparing `RIFT-0.0.15.8rc9/INSTALL_OPTIONAL_DEPENDENCIES.md` & `RIFT-0.0.15.9rc1/INSTALL_OPTIONAL_DEPENDENCIES.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/setup.py` & `RIFT-0.0.15.9rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #  - ourio.py, ourparams.py
 #  - anything with 'test'
 #print " Identified scripts ", my_scripts\
 #print setuptools.find_packages('MonteCarloMarginalizeCode/Code')
 
 setuptools.setup(
     name="RIFT",
-    version="0.0.15.8rc9", # do not build on OSX machine, side effects
+    version="0.0.15.9rc1", # do not build on OSX machine, side effects
     author="Richard O'Shaughnessy",
     author_email="richard.oshaughnessy@ligo.org",
     description="RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.ligo.org/rapidpe-rift/rift",
     package_dir = {'':'MonteCarloMarginalizeCode/Code'},
```

### Comparing `RIFT-0.0.15.8rc9/howto.md` & `RIFT-0.0.15.9rc1/howto.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/INSTALL.md` & `RIFT-0.0.15.9rc1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc9/Dockerfile` & `RIFT-0.0.15.9rc1/Dockerfile`

 * *Files identical despite different names*

