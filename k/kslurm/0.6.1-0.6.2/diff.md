# Comparing `tmp/kslurm-0.6.1.tar.gz` & `tmp/kslurm-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kslurm-0.6.1.tar", max compression
+gzip compressed data, was "kslurm-0.6.2.tar", max compression
```

## Comparing `kslurm-0.6.1.tar` & `kslurm-0.6.2.tar`

### file list

```diff
@@ -1,157 +1,155 @@
--rw-r--r--   0        0        0     1066 2022-10-04 17:47:11.397692 kslurm-0.6.1/LICENSE
--rw-r--r--   0        0        0    17900 2022-10-04 17:47:11.397692 kslurm-0.6.1/README.md
--rw-r--r--   0        0        0       93 2022-10-17 15:33:43.578128 kslurm-0.6.1/kslurm/__init__.py
--rw-r--r--   0        0        0     1079 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/appcache.py
--rw-r--r--   0        0        0     1793 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/appconfig.py
--rw-r--r--   0        0        0      740 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/__init__.py
--rw-r--r--   0        0        0     3345 2022-10-17 15:25:44.658128 kslurm-0.6.1/kslurm/args/actions.py
--rw-r--r--   0        0        0    12022 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/arg.py
--rw-r--r--   0        0        0     5786 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/arg_types.py
--rw-r--r--   0        0        0     4020 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/arg_types.pyi
--rw-r--r--   0        0        0    10142 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/command.py
--rw-r--r--   0        0        0     3625 2022-11-07 16:04:50.836961 kslurm-0.6.1/kslurm/args/help.py
--rw-r--r--   0        0        0     4509 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/help_templates.py
--rw-r--r--   0        0        0     8950 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/helpers.py
--rw-r--r--   0        0        0     2702 2022-10-17 15:31:21.688128 kslurm-0.6.1/kslurm/args/matchers.py
--rw-r--r--   0        0        0     2156 2022-10-04 18:28:50.607692 kslurm-0.6.1/kslurm/args/parser.py
--rw-r--r--   0        0        0      539 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/args/protocols.py
--rw-r--r--   0        0        0       13 2022-10-17 15:33:43.558128 kslurm-0.6.1/kslurm/bin/__init__.py
--rw-r--r--   0        0        0     1403 2022-10-04 17:47:11.397692 kslurm-0.6.1/kslurm/bin/bash.sh
--rw-r--r--   0        0        0      559 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/bin/kpy-init.sh
--rw-r--r--   0        0        0      737 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/bin/kpy-wrapper.sh
--rw-r--r--   0        0        0     1372 2022-10-04 17:47:11.397692 kslurm-0.6.1/kslurm/bin/neuroglia-helpers.sh
--rw-r--r--   0        0        0       70 2022-10-17 15:33:43.568128 kslurm-0.6.1/kslurm/cli/__init__.py
--rw-r--r--   0        0        0     3692 2022-10-04 17:47:11.397692 kslurm-0.6.1/kslurm/cli/config.py
--rw-r--r--   0        0        0       70 2022-10-17 15:33:43.528128 kslurm-0.6.1/kslurm/cli/kapp/__init__.py
--rw-r--r--   0        0        0     1218 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/kapp/alias.py
--rw-r--r--   0        0        0     2462 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/kapp/image.py
--rw-r--r--   0        0        0     9107 2022-12-08 23:28:14.293538 kslurm-0.6.1/kslurm/cli/kapp/main.py
--rw-r--r--   0        0        0     4072 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/kbatch.py
--rw-r--r--   0        0        0    12012 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/kjupyter.py
--rw-r--r--   0        0        0    12367 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/kpy.py
--rw-r--r--   0        0        0     2030 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/krun.py
--rw-r--r--   0        0        0     1457 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/main.py
--rw-r--r--   0        0        0     3373 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/cli/ssnake.py
--rw-r--r--   0        0        0    13570 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/container.py
--rw-r--r--   0        0        0       13 2022-10-17 15:33:43.578128 kslurm-0.6.1/kslurm/data/__init__.py
--rw-r--r--   0        0        0      129 2022-10-04 17:47:11.397692 kslurm-0.6.1/kslurm/data/download_frozen_container.hash
--rw-r--r--   0        0        0     2243 2022-10-04 17:47:11.397692 kslurm-0.6.1/kslurm/data/slurm_job_templates.json
--rw-r--r--   0        0        0      776 2022-10-04 18:28:50.607692 kslurm-0.6.1/kslurm/exceptions.py
--rw-r--r--   0        0        0       70 2022-10-17 15:33:43.568128 kslurm-0.6.1/kslurm/installer/__init__.py
--rw-r--r--   0        0        0     4306 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/installer/installer.py
--rw-r--r--   0        0        0     4204 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/installer/utils.py
--rw-r--r--   0        0        0      937 2022-10-04 17:47:11.397692 kslurm-0.6.1/kslurm/installer/version.py
--rw-r--r--   0        0        0       70 2022-10-17 15:33:43.558128 kslurm-0.6.1/kslurm/models/__init__.py
--rw-r--r--   0        0        0     1083 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/models/formatters.py
--rw-r--r--   0        0        0     1530 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/models/job_templates.py
--rw-r--r--   0        0        0     2585 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/models/slurm.py
--rw-r--r--   0        0        0      685 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/models/update.py
--rw-r--r--   0        0        0      534 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/models/validators.py
--rw-r--r--   0        0        0     3052 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/shell.py
--rw-r--r--   0        0        0       90 2022-10-17 15:33:43.568128 kslurm-0.6.1/kslurm/slurm/__init__.py
--rw-r--r--   0        0        0      483 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/slurm/helpers.py
--rw-r--r--   0        0        0     5937 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/slurm/slurm_command.py
--rw-r--r--   0        0        0      161 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/style/__init__.py
--rw-r--r--   0        0        0      206 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/style/console.py
--rw-r--r--   0        0        0      340 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/style/themes.py
--rw-r--r--   0        0        0       70 2022-10-17 15:33:43.558128 kslurm-0.6.1/kslurm/test/__init__.py
--rw-r--r--   0        0        0       70 2022-10-17 15:33:43.528128 kslurm-0.6.1/kslurm/test/args/__init__.py
--rw-r--r--   0        0        0     1620 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/test/args/test_model_parsing.py
--rw-r--r--   0        0        0     7389 2022-10-17 15:33:34.328128 kslurm-0.6.1/kslurm/test/args/test_parser.py
--rw-r--r--   0        0        0   269230 2022-10-04 17:47:11.397692 kslurm-0.6.1/kslurm/test/installer/fake_releases.json
--rw-r--r--   0        0        0     1780 2022-10-17 15:33:38.778128 kslurm-0.6.1/kslurm/test/installer/test_install.py
--rw-r--r--   0        0        0     4412 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/test/installer/test_utils.py
--rw-r--r--   0        0        0     1839 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/test/test_batch.py
--rw-r--r--   0        0        0      132 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/test/test_help.py
--rw-r--r--   0        0        0      758 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/test/test_slurm_helpers.py
--rw-r--r--   0        0        0      583 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/test/test_validators.py
--rw-r--r--   0        0        0     1800 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/text.py
--rw-r--r--   0        0        0      470 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/utils.py
--rw-r--r--   0        0        0     5174 2022-11-07 16:00:48.696961 kslurm-0.6.1/kslurm/venv.py
--rw-r--r--   0        0        0       42 2022-10-04 17:49:07.857692 kslurm-0.6.1/neuroglia_helpers/.git
--rw-r--r--   0        0        0      676 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/.github/workflows/valdate_bids-apps.tsv.yml
--rw-r--r--   0        0        0      883 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/.github_scripts/install_singularity.sh
--rw-r--r--   0        0        0       11 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/.gitignore
--rwxr-xr-x   0        0        0     1310 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/00_init.sh
--rwxr-xr-x   0        0        0      363 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/00_initrc.sh
--rw-r--r--   0        0        0    35147 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/LICENSE
--rw-r--r--   0        0        0     4716 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/README.md
--rw-r--r--   0        0        0        0 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/__init__.py
--rw-r--r--   0        0        0    11448 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bids-apps.tsv
--rwxr-xr-x   0        0        0     3308 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/archivefolders
--rwxr-xr-x   0        0        0     4160 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/archivescratch
--rwxr-xr-x   0        0        0    10980 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/bidsBatch
--rwxr-xr-x   0        0        0      374 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/cfmm2tar
--rwxr-xr-x   0        0        0      320 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/dicom2tar
--rwxr-xr-x   0        0        0      412 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/fetch_templateflow_templates
--rwxr-xr-x   0        0        0     3860 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/joblistSubmit
--rwxr-xr-x   0        0        0      229 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/joblistSubmitSequential
--rwxr-xr-x   0        0        0      521 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/jupyter_snakemake
--rwxr-xr-x   0        0        0      174 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/listNumberFiles
--rwxr-xr-x   0        0        0     2622 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/listusage
--rwxr-xr-x   0        0        0     3095 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/moveandlink
--rwxr-xr-x   0        0        0      424 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/neuroglia
--rwxr-xr-x   0        0        0     6899 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/neurogliaBatch
--rwxr-xr-x   0        0        0      425 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/neurogliaShell
--rwxr-xr-x   0        0        0     4449 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/neurogliaSubmit
--rwxr-xr-x   0        0        0     6060 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/regularBatch
--rwxr-xr-x   0        0        0     1547 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/regularInteractive
--rwxr-xr-x   0        0        0     3847 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/regularSubmit
--rwxr-xr-x   0        0        0     1135 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/run_freesurfer_bids
--rwxr-xr-x   0        0        0     1393 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/run_sclimbic_bids
--rwxr-xr-x   0        0        0     1070 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/setAccess
--rwxr-xr-x   0        0        0     2938 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/shub-cache
--rwxr-xr-x   0        0        0     1383 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/shub-cache-remote
--rwxr-xr-x   0        0        0     2309 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/shub-upgrade
--rwxr-xr-x   0        0        0     1581 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/snakemake_remotebatch
--rwxr-xr-x   0        0        0      192 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/snakemake_slurm
--rwxr-xr-x   0        0        0      369 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/tar2bids
--rwxr-xr-x   0        0        0      271 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/bin/validator
--rw-r--r--   0        0        0     1579 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg/graham.cfg
--rw-r--r--   0        0        0     1293 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg/graham_bmi.cfg
--rw-r--r--   0        0        0     2169 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg/graham_ctb-akhanf-ab.cfg
--rw-r--r--   0        0        0     2477 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg/graham_khanlab.cfg
--rw-r--r--   0        0        0     1212 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg/graham_local.cfg
--rw-r--r--   0        0        0     1210 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg/graham_lpalaniy.cfg
--rw-r--r--   0        0        0      114 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg_apps/fmriprep_multiproc_16c_64gb.yaml
--rw-r--r--   0        0        0      113 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/cfg_apps/fmriprep_multiproc_8c_32gb.yaml
--rwxr-xr-x   0        0        0     1828 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/bash_lib.sh
--rwxr-xr-x   0        0        0       79 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/jupyter.sh
--rwxr-xr-x   0        0        0     3472 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/make_snakemake_singularity_links.py
--rwxr-xr-x   0        0        0     1057 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/printGroupUsage
--rwxr-xr-x   0        0        0      729 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/remote_pull
--rwxr-xr-x   0        0        0      214 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/sacct_full
--rwxr-xr-x   0        0        0      383 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/setup_passwdless
--rwxr-xr-x   0        0        0      824 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/setup_sshfs_graham
--rw-r--r--   0        0        0      258 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/snakemake_containers.tsv
--rwxr-xr-x   0        0        0     2753 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/etc/snakemake_slurm_submit.py
--rw-r--r--   0        0        0      120 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/16core64gb24h.job
--rw-r--r--   0        0        0      119 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/16core64gb3h.job
--rw-r--r--   0        0        0       99 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/2core8gb.job
--rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/2core8gb16h.job
--rw-r--r--   0        0        0      121 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/32core128gb12h.job
--rw-r--r--   0        0        0      120 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/32core128gb3h.job
--rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/4core16gb.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/4core16gb12h.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/4core16gb24h.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/4core64gb12h.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/5core32gb24h.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/5core32gb72h.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/8core32gb12h.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/8core32gb28h.job
--rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/8core32gb3h.job
--rw-r--r--   0        0        0      121 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/Fat.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/Long.job
--rw-r--r--   0        0        0      121 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/LongFat.job
--rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/LongSkinny.job
--rw-r--r--   0        0        0       99 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/Quick.job
--rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/Regular.job
--rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/Short.job
--rw-r--r--   0        0        0      120 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/ShortFat.job
--rw-r--r--   0        0        0       99 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/ShortSkinny.job
--rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/job-templates/Skinny.job
--rwxr-xr-x   0        0        0      305 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/setup.sh
--rw-r--r--   0        0        0     3842 2022-10-04 17:49:07.887692 kslurm-0.6.1/neuroglia_helpers/validate_bids-apps.tsv.py
--rw-r--r--   0        0        0     2916 2022-12-08 23:33:00.413538 kslurm-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    20293 2022-12-08 23:33:34.338787 kslurm-0.6.1/setup.py
--rw-r--r--   0        0        0    19556 2022-12-08 23:33:34.339837 kslurm-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-10-04 17:47:11.397692 kslurm-0.6.2/LICENSE
+-rw-r--r--   0        0        0    17900 2022-10-04 17:47:11.397692 kslurm-0.6.2/README.md
+-rw-r--r--   0        0        0       93 2022-10-17 15:33:43.578128 kslurm-0.6.2/kslurm/__init__.py
+-rw-r--r--   0        0        0     1079 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/appcache.py
+-rw-r--r--   0        0        0     1793 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/appconfig.py
+-rw-r--r--   0        0        0      740 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/__init__.py
+-rw-r--r--   0        0        0     3345 2022-10-17 15:25:44.658128 kslurm-0.6.2/kslurm/args/actions.py
+-rw-r--r--   0        0        0    12022 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/arg.py
+-rw-r--r--   0        0        0     5786 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/arg_types.py
+-rw-r--r--   0        0        0     4020 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/arg_types.pyi
+-rw-r--r--   0        0        0    10142 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/command.py
+-rw-r--r--   0        0        0     3625 2022-11-07 16:04:50.836961 kslurm-0.6.2/kslurm/args/help.py
+-rw-r--r--   0        0        0     4509 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/help_templates.py
+-rw-r--r--   0        0        0     8950 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/helpers.py
+-rw-r--r--   0        0        0     2702 2022-10-17 15:31:21.688128 kslurm-0.6.2/kslurm/args/matchers.py
+-rw-r--r--   0        0        0     2156 2022-10-04 18:28:50.607692 kslurm-0.6.2/kslurm/args/parser.py
+-rw-r--r--   0        0        0      539 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/args/protocols.py
+-rw-r--r--   0        0        0       13 2022-10-17 15:33:43.558128 kslurm-0.6.2/kslurm/bin/__init__.py
+-rw-r--r--   0        0        0     1403 2022-10-04 17:47:11.397692 kslurm-0.6.2/kslurm/bin/bash.sh
+-rw-r--r--   0        0        0      559 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/bin/kpy-init.sh
+-rw-r--r--   0        0        0      737 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/bin/kpy-wrapper.sh
+-rw-r--r--   0        0        0     1370 2023-05-24 21:01:50.965509 kslurm-0.6.2/kslurm/bin/neuroglia-helpers.sh
+-rw-r--r--   0        0        0       70 2022-10-17 15:33:43.568128 kslurm-0.6.2/kslurm/cli/__init__.py
+-rw-r--r--   0        0        0     3692 2022-10-04 17:47:11.397692 kslurm-0.6.2/kslurm/cli/config.py
+-rw-r--r--   0        0        0       70 2022-10-17 15:33:43.528128 kslurm-0.6.2/kslurm/cli/kapp/__init__.py
+-rw-r--r--   0        0        0     1218 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/cli/kapp/alias.py
+-rw-r--r--   0        0        0     2462 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/cli/kapp/image.py
+-rw-r--r--   0        0        0     9089 2023-02-03 16:38:59.674259 kslurm-0.6.2/kslurm/cli/kapp/main.py
+-rw-r--r--   0        0        0     4072 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/cli/kbatch.py
+-rw-r--r--   0        0        0    12012 2023-04-03 15:06:46.036920 kslurm-0.6.2/kslurm/cli/kjupyter.py
+-rw-r--r--   0        0        0    12367 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/cli/kpy.py
+-rw-r--r--   0        0        0     2030 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/cli/krun.py
+-rw-r--r--   0        0        0     1457 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/cli/main.py
+-rw-r--r--   0        0        0     3373 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/cli/ssnake.py
+-rw-r--r--   0        0        0    13570 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/container.py
+-rw-r--r--   0        0        0       13 2022-10-17 15:33:43.578128 kslurm-0.6.2/kslurm/data/__init__.py
+-rw-r--r--   0        0        0      129 2022-10-04 17:47:11.397692 kslurm-0.6.2/kslurm/data/download_frozen_container.hash
+-rw-r--r--   0        0        0     2243 2022-10-04 17:47:11.397692 kslurm-0.6.2/kslurm/data/slurm_job_templates.json
+-rw-r--r--   0        0        0      776 2022-10-04 18:28:50.607692 kslurm-0.6.2/kslurm/exceptions.py
+-rw-r--r--   0        0        0       70 2022-10-17 15:33:43.568128 kslurm-0.6.2/kslurm/installer/__init__.py
+-rw-r--r--   0        0        0     4306 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/installer/installer.py
+-rw-r--r--   0        0        0     4204 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/installer/utils.py
+-rw-r--r--   0        0        0      937 2022-10-04 17:47:11.397692 kslurm-0.6.2/kslurm/installer/version.py
+-rw-r--r--   0        0        0       70 2022-10-17 15:33:43.558128 kslurm-0.6.2/kslurm/models/__init__.py
+-rw-r--r--   0        0        0     1083 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/models/formatters.py
+-rw-r--r--   0        0        0     1530 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/models/job_templates.py
+-rw-r--r--   0        0        0     2585 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/models/slurm.py
+-rw-r--r--   0        0        0      685 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/models/update.py
+-rw-r--r--   0        0        0      534 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/models/validators.py
+-rw-r--r--   0        0        0     3052 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/shell.py
+-rw-r--r--   0        0        0       90 2022-10-17 15:33:43.568128 kslurm-0.6.2/kslurm/slurm/__init__.py
+-rw-r--r--   0        0        0      483 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/slurm/helpers.py
+-rw-r--r--   0        0        0     6173 2023-02-03 16:36:55.447088 kslurm-0.6.2/kslurm/slurm/slurm_command.py
+-rw-r--r--   0        0        0      161 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/style/__init__.py
+-rw-r--r--   0        0        0      206 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/style/console.py
+-rw-r--r--   0        0        0      340 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/style/themes.py
+-rw-r--r--   0        0        0       70 2022-10-17 15:33:43.558128 kslurm-0.6.2/kslurm/test/__init__.py
+-rw-r--r--   0        0        0       70 2022-10-17 15:33:43.528128 kslurm-0.6.2/kslurm/test/args/__init__.py
+-rw-r--r--   0        0        0     1620 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/test/args/test_model_parsing.py
+-rw-r--r--   0        0        0     7389 2022-10-17 15:33:34.328128 kslurm-0.6.2/kslurm/test/args/test_parser.py
+-rw-r--r--   0        0        0   269230 2022-10-04 17:47:11.397692 kslurm-0.6.2/kslurm/test/installer/fake_releases.json
+-rw-r--r--   0        0        0     1780 2022-10-17 15:33:38.778128 kslurm-0.6.2/kslurm/test/installer/test_install.py
+-rw-r--r--   0        0        0     4412 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/test/installer/test_utils.py
+-rw-r--r--   0        0        0     1839 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/test/test_batch.py
+-rw-r--r--   0        0        0      132 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/test/test_help.py
+-rw-r--r--   0        0        0      758 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/test/test_slurm_helpers.py
+-rw-r--r--   0        0        0      583 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/test/test_validators.py
+-rw-r--r--   0        0        0     1800 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/text.py
+-rw-r--r--   0        0        0      470 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/utils.py
+-rw-r--r--   0        0        0     5174 2022-11-07 16:00:48.696961 kslurm-0.6.2/kslurm/venv.py
+-rw-r--r--   0        0        0       42 2022-10-04 17:49:07.857692 kslurm-0.6.2/neuroglia_helpers/.git
+-rw-r--r--   0        0        0      676 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/.github/workflows/valdate_bids-apps.tsv.yml
+-rw-r--r--   0        0        0      883 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/.github_scripts/install_singularity.sh
+-rwxr-xr-x   0        0        0     1310 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/00_init.sh
+-rwxr-xr-x   0        0        0      363 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/00_initrc.sh
+-rw-r--r--   0        0        0    35147 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/LICENSE
+-rw-r--r--   0        0        0     4716 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/README.md
+-rw-r--r--   0        0        0    11771 2023-05-24 21:02:00.555637 kslurm-0.6.2/neuroglia_helpers/bids-apps.tsv
+-rwxr-xr-x   0        0        0     3308 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/archivefolders
+-rwxr-xr-x   0        0        0     4160 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/archivescratch
+-rwxr-xr-x   0        0        0    10980 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/bidsBatch
+-rwxr-xr-x   0        0        0      374 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/cfmm2tar
+-rwxr-xr-x   0        0        0      320 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/dicom2tar
+-rwxr-xr-x   0        0        0      412 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/fetch_templateflow_templates
+-rwxr-xr-x   0        0        0  9293824 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/bin/gdu
+-rwxr-xr-x   0        0        0     3860 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/joblistSubmit
+-rwxr-xr-x   0        0        0      229 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/joblistSubmitSequential
+-rwxr-xr-x   0        0        0      521 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/jupyter_snakemake
+-rwxr-xr-x   0        0        0      174 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/listNumberFiles
+-rwxr-xr-x   0        0        0     2622 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/listusage
+-rwxr-xr-x   0        0        0     3095 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/moveandlink
+-rwxr-xr-x   0        0        0      424 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/neuroglia
+-rwxr-xr-x   0        0        0     6899 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/neurogliaBatch
+-rwxr-xr-x   0        0        0      425 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/neurogliaShell
+-rwxr-xr-x   0        0        0     4449 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/neurogliaSubmit
+-rwxr-xr-x   0        0        0     6060 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/regularBatch
+-rwxr-xr-x   0        0        0     1547 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/regularInteractive
+-rwxr-xr-x   0        0        0     3847 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/regularSubmit
+-rwxr-xr-x   0        0        0     1309 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/bin/run_freesurfer_bids
+-rwxr-xr-x   0        0        0     1393 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/run_sclimbic_bids
+-rwxr-xr-x   0        0        0     1070 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/setAccess
+-rwxr-xr-x   0        0        0     2938 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/shub-cache
+-rwxr-xr-x   0        0        0     1383 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/shub-cache-remote
+-rwxr-xr-x   0        0        0     2309 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/shub-upgrade
+-rwxr-xr-x   0        0        0     1581 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/snakemake_remotebatch
+-rwxr-xr-x   0        0        0      192 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/snakemake_slurm
+-rwxr-xr-x   0        0        0      369 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/tar2bids
+-rwxr-xr-x   0        0        0      271 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/bin/validator
+-rw-r--r--   0        0        0     1592 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/cfg/graham.cfg
+-rw-r--r--   0        0        0     1310 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/cfg/graham_bmi.cfg
+-rw-r--r--   0        0        0     2179 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/cfg/graham_ctb-akhanf-ab.cfg
+-rw-r--r--   0        0        0     2483 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/cfg/graham_khanlab.cfg
+-rw-r--r--   0        0        0     1208 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/cfg/graham_local.cfg
+-rw-r--r--   0        0        0     1223 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/cfg/graham_lpalaniy.cfg
+-rw-r--r--   0        0        0      114 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/cfg_apps/fmriprep_multiproc_16c_64gb.yaml
+-rw-r--r--   0        0        0      113 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/cfg_apps/fmriprep_multiproc_8c_32gb.yaml
+-rwxr-xr-x   0        0        0     1828 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/bash_lib.sh
+-rwxr-xr-x   0        0        0       79 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/jupyter.sh
+-rwxr-xr-x   0        0        0     3472 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/make_snakemake_singularity_links.py
+-rwxr-xr-x   0        0        0     1057 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/printGroupUsage
+-rwxr-xr-x   0        0        0      729 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/remote_pull
+-rwxr-xr-x   0        0        0      214 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/sacct_full
+-rwxr-xr-x   0        0        0      383 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/setup_passwdless
+-rwxr-xr-x   0        0        0      824 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/setup_sshfs_graham
+-rw-r--r--   0        0        0      258 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/snakemake_containers.tsv
+-rwxr-xr-x   0        0        0     2753 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/etc/snakemake_slurm_submit.py
+-rw-r--r--   0        0        0      120 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/16core64gb24h.job
+-rw-r--r--   0        0        0      119 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/16core64gb3h.job
+-rw-r--r--   0        0        0       99 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/2core8gb.job
+-rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/2core8gb16h.job
+-rw-r--r--   0        0        0      121 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/32core128gb12h.job
+-rw-r--r--   0        0        0      120 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/32core128gb3h.job
+-rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/4core16gb.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/4core16gb12h.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/4core16gb24h.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/4core64gb12h.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/5core32gb24h.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/5core32gb72h.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/8core32gb12h.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/8core32gb28h.job
+-rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/8core32gb3h.job
+-rw-r--r--   0        0        0      121 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/Fat.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/Long.job
+-rw-r--r--   0        0        0      121 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/LongFat.job
+-rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/LongSkinny.job
+-rw-r--r--   0        0        0       99 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/Quick.job
+-rw-r--r--   0        0        0      101 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/Regular.job
+-rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/Short.job
+-rw-r--r--   0        0        0      120 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/ShortFat.job
+-rw-r--r--   0        0        0       99 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/ShortSkinny.job
+-rw-r--r--   0        0        0      100 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/job-templates/Skinny.job
+-rwxr-xr-x   0        0        0      303 2023-05-24 21:02:00.615638 kslurm-0.6.2/neuroglia_helpers/setup.sh
+-rw-r--r--   0        0        0     3842 2022-10-04 17:49:07.887692 kslurm-0.6.2/neuroglia_helpers/validate_bids-apps.tsv.py
+-rw-r--r--   0        0        0     3059 2023-05-24 21:09:14.534529 kslurm-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    19607 1970-01-01 00:00:00.000000 kslurm-0.6.2/PKG-INFO
```

### Comparing `kslurm-0.6.1/LICENSE` & `kslurm-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/README.md` & `kslurm-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/appcache.py` & `kslurm-0.6.2/kslurm/appcache.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/appconfig.py` & `kslurm-0.6.2/kslurm/appconfig.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/__init__.py` & `kslurm-0.6.2/kslurm/args/__init__.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/actions.py` & `kslurm-0.6.2/kslurm/args/actions.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/arg.py` & `kslurm-0.6.2/kslurm/args/arg.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/arg_types.py` & `kslurm-0.6.2/kslurm/args/arg_types.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/arg_types.pyi` & `kslurm-0.6.2/kslurm/args/arg_types.pyi`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/command.py` & `kslurm-0.6.2/kslurm/args/command.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/help.py` & `kslurm-0.6.2/kslurm/args/help.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/help_templates.py` & `kslurm-0.6.2/kslurm/args/help_templates.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/helpers.py` & `kslurm-0.6.2/kslurm/args/helpers.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/matchers.py` & `kslurm-0.6.2/kslurm/args/matchers.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/parser.py` & `kslurm-0.6.2/kslurm/args/parser.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/args/protocols.py` & `kslurm-0.6.2/kslurm/args/protocols.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/bin/bash.sh` & `kslurm-0.6.2/kslurm/bin/bash.sh`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/bin/kpy-init.sh` & `kslurm-0.6.2/kslurm/bin/kpy-init.sh`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/bin/kpy-wrapper.sh` & `kslurm-0.6.2/kslurm/bin/kpy-wrapper.sh`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/bin/neuroglia-helpers.sh` & `kslurm-0.6.2/kslurm/bin/neuroglia-helpers.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-module load singularity python/3
+module load apptainer python/3
 
 #light version doesn't display welcome message
 if [ "$#" = 1 ]
 then
 	use_light=1
 else
 	use_light=0
```

### Comparing `kslurm-0.6.1/kslurm/cli/config.py` & `kslurm-0.6.2/kslurm/cli/config.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/kapp/alias.py` & `kslurm-0.6.2/kslurm/cli/kapp/alias.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/kapp/image.py` & `kslurm-0.6.2/kslurm/cli/kapp/image.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/kapp/main.py` & `kslurm-0.6.2/kslurm/cli/kapp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import absolute_import
 
-import importlib.resources as impr
 import os
 import os.path
-import shutil
 import subprocess as sp
 import tarfile
 from pathlib import Path
+import shutil
 from typing import DefaultDict, Optional
 
 import attrs
 import requests
 from InquirerPy import inquirer as inq  # type: ignore
 
 from kslurm.appcache import Cache
@@ -108,15 +107,14 @@
     if _SINGULARITY_DIR.has_raw_uri_file(app):
         if not inq.confirm(
             f"An image matching {app.uri.uri} already exists, but we can't verify if "
             "it's up to date. Would you like to pull it again?"
         ).execute():
             return
 
-
     image_path = _SINGULARITY_DIR.get_data_path(app)
 
     # Small images we can directly use the singularity command
     if app.docker_data and app.docker_data.size_mb < 200 and not mem:
         sp.run(["singularity", "pull", str(image_path), app.uri.uri])
         _update_aliases(_SINGULARITY_DIR, app, uri, alias)
         return
@@ -142,15 +140,16 @@
         # if get_hash(script, method="sha512") != hashed.strip():
         #     raise CommandError(
         #         "Frozen image download script does not match hash. Cannot continue."
         #     )
         cache[url] = script
         os.chmod(cache.get_path(url), 0o776)
 
-    frozen_image = _SINGULARITY_DIR.work / get_hash(app.uri.address)
+    workdir = _SINGULARITY_DIR.work / get_hash(app.uri.address)
+    frozen_image = workdir / "image"
     proc = sp.run(
         [
             str(cache.get_path(url)),
             str(frozen_image),
             (app.friendly_uri or app.uri).address,
         ]
     )
@@ -177,15 +176,15 @@
             "build",
             "--disable-cache",
             str(image_path),
             f"docker-archive://{frozen_image.with_suffix('.tar')}",
         ]
     )
     if ret == 0:
-        shutil.rmtree(_SINGULARITY_DIR.work)
+        shutil.rmtree(workdir)
 
         _update_aliases(_SINGULARITY_DIR, app, uri, alias)
     return ret
 
 
 @command(inline=True)
 def _path(
```

### Comparing `kslurm-0.6.1/kslurm/cli/kbatch.py` & `kslurm-0.6.2/kslurm/cli/kbatch.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/kjupyter.py` & `kslurm-0.6.2/kslurm/cli/kjupyter.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/kpy.py` & `kslurm-0.6.2/kslurm/cli/kpy.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/krun.py` & `kslurm-0.6.2/kslurm/cli/krun.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/main.py` & `kslurm-0.6.2/kslurm/cli/main.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/cli/ssnake.py` & `kslurm-0.6.2/kslurm/cli/ssnake.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/container.py` & `kslurm-0.6.2/kslurm/container.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/data/slurm_job_templates.json` & `kslurm-0.6.2/kslurm/data/slurm_job_templates.json`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/exceptions.py` & `kslurm-0.6.2/kslurm/exceptions.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/installer/installer.py` & `kslurm-0.6.2/kslurm/installer/installer.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/installer/utils.py` & `kslurm-0.6.2/kslurm/installer/utils.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/installer/version.py` & `kslurm-0.6.2/kslurm/installer/version.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/models/formatters.py` & `kslurm-0.6.2/kslurm/models/formatters.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/models/job_templates.py` & `kslurm-0.6.2/kslurm/models/job_templates.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/models/slurm.py` & `kslurm-0.6.2/kslurm/models/slurm.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/models/update.py` & `kslurm-0.6.2/kslurm/models/update.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/models/validators.py` & `kslurm-0.6.2/kslurm/models/validators.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/shell.py` & `kslurm-0.6.2/kslurm/shell.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/slurm/slurm_command.py` & `kslurm-0.6.2/kslurm/slurm/slurm_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -186,15 +186,20 @@
     def batch(self):
         if self.test:
             s = "cat"
         else:
             s = f"sbatch {self.slurm_args} --parsable {self.output}"
         if self.command:
             if "/" in self._command[0] and Path(self._command[0]).is_file():
-                return f"{s} {self.command}"
+                try:
+                    with open(self._command[0], "r", encoding="utf-8") as f:
+                        if f.readline().startswith("#/"):
+                            return f"{s} {self.command}"
+                except UnicodeDecodeError:
+                    pass
             return f"echo {shlex.quote(self.script)} | {s}"
         else:
             raise ValidationError("No command given")
 
     @property
     def batch_test(self):
         s = f"sbatch {self.slurm_args} --test-only"
```

### Comparing `kslurm-0.6.1/kslurm/test/args/test_model_parsing.py` & `kslurm-0.6.2/kslurm/test/args/test_model_parsing.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/test/args/test_parser.py` & `kslurm-0.6.2/kslurm/test/args/test_parser.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/test/installer/fake_releases.json` & `kslurm-0.6.2/kslurm/test/installer/fake_releases.json`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/test/installer/test_install.py` & `kslurm-0.6.2/kslurm/test/installer/test_install.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/test/installer/test_utils.py` & `kslurm-0.6.2/kslurm/test/installer/test_utils.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/test/test_batch.py` & `kslurm-0.6.2/kslurm/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/test/test_slurm_helpers.py` & `kslurm-0.6.2/kslurm/test/test_slurm_helpers.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/test/test_validators.py` & `kslurm-0.6.2/kslurm/test/test_validators.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/text.py` & `kslurm-0.6.2/kslurm/text.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/kslurm/venv.py` & `kslurm-0.6.2/kslurm/venv.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/.github/workflows/valdate_bids-apps.tsv.yml` & `kslurm-0.6.2/neuroglia_helpers/.github/workflows/valdate_bids-apps.tsv.yml`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/.github_scripts/install_singularity.sh` & `kslurm-0.6.2/neuroglia_helpers/.github_scripts/install_singularity.sh`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/00_init.sh` & `kslurm-0.6.2/neuroglia_helpers/00_init.sh`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/LICENSE` & `kslurm-0.6.2/neuroglia_helpers/LICENSE`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/README.md` & `kslurm-0.6.2/neuroglia_helpers/README.md`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bids-apps.tsv` & `kslurm-0.6.2/neuroglia_helpers/bids-apps.tsv`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 name	url	base_options	job_template
+fmriprep_23.0.1	docker://nipreps/fmriprep:23.0.1	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --notrack	Regular
 fmriprep_21.0.0	docker://nipreps/fmriprep:21.0.0	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --notrack	Regular
 fmriprep_20.2.6	docker://nipreps/fmriprep:20.2.6	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --notrack --output-layout bids	Regular
 fmriprep_20.2.5	docker://nipreps/fmriprep:20.2.5	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --notrack --output-layout bids	Regular
 fmriprep_20.2.3	docker://nipreps/fmriprep:20.2.3	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --notrack --output-layout bids	Regular
 fmriprep_20.2.1	docker://nipreps/fmriprep:20.2.1	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --notrack --output-layout bids	Regular
 fmriprep_20.2.0	docker://poldracklab/fmriprep:20.2.0	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor --notrack	Regular
 fmriprep_20.1.1	docker://poldracklab/fmriprep:20.1.1	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor --notrack	Regular
@@ -20,14 +21,15 @@
 fmriprep_1.1.8_withFS	docker://poldracklab/fmriprep:1.1.8	--nthreads 8 --n_cpus 8 --mem_mb 32000 --omp-nthreads 8 --use-plugin ${FMRIPREP_MULTIPROC_YAML} -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor --notrack	Long
 fmriprep_1.1.4	docker://poldracklab/fmriprep:1.1.4	--nthreads 8 --n_cpus 8 --omp-nthreads 8 --mem_mb 32000 -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor --notrack	Regular
 fmriprep_1.1.1	docker://poldracklab/fmriprep:1.1.1	--nthreads 8 --n_cpus 8 --omp-nthreads 8 --mem_mb 32000 -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor --notrack	Regular
 fmriprep_1.0.13	docker://poldracklab/fmriprep:1.0.13	--nthreads 8 --n_cpus 8 --omp-nthreads 8 --mem_mb 32000 -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor --notrack	Regular
 fmriprep_1.0.7	docker://poldracklab/fmriprep:1.0.7	--nthreads 8 --n_cpus 8 --omp-nthreads 8 --mem_mb 32000 -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor	Regular
 fmriprep_1.0.6	docker://poldracklab/fmriprep:1.0.6	--nthreads 8 --n_cpus 8 --omp-nthreads 8 --mem_mb 32000 -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor	Regular
 fmriprep_1.0.4	docker://poldracklab/fmriprep:1.0.4	--nthreads 8 --n_cpus 8 --omp-nthreads 8 --mem_mb 32000 -w ${SLURM_TMPDIR} --fs-license-file ${FS_LICENSE_FILE} --resource-monitor	Regular
+mriqc_23.0.1	docker://nipreps/mriqc:23.0.1	--no-sub --n_procs 8 --mem_gb 32000 -w ${SLURM_TMPDIR}	Short
 mriqc_0.15.1	docker://poldracklab/mriqc:0.15.1	--no-sub --n_procs 8 --mem_gb 32000 -w ${SLURM_TMPDIR}	Short
 mriqc_0.14.2	docker://poldracklab/mriqc:0.14.2	--no-sub --n_procs 8 --mem_gb 32000 -w ${SLURM_TMPDIR}	Short
 mriqc_0.10.2	docker://poldracklab/mriqc:0.10.2	--no-sub --n_procs 8 --mem_gb 32000 -w ${SLURM_TMPDIR}	Short
 mriqc_0.10.1	docker://poldracklab/mriqc:0.10.1	--no-sub --n_procs 8 --mem_gb 32000 -w ${SLURM_TMPDIR}	Short
 mriqc_0.10.0	docker://poldracklab/mriqc:0.10.0	--no-sub --n_procs 8 --mem_gb 32000 -w ${SLURM_TMPDIR}	Short
 prepdwi_v0.0.13	docker://khanlab/prepdwi:v0.0.13	--no-bedpost --n_cpus 4 -w $SLURM_TMPDIR	4core16gb12h
 prepdwi_v0.0.12d	docker://khanlab/prepdwi:v0.0.12d	--no-bedpost --n_cpus 4 -w $SLURM_TMPDIR	4core16gb12h
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/archivefolders` & `kslurm-0.6.2/neuroglia_helpers/bin/archivefolders`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/archivescratch` & `kslurm-0.6.2/neuroglia_helpers/bin/archivescratch`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/bidsBatch` & `kslurm-0.6.2/neuroglia_helpers/bin/bidsBatch`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/joblistSubmit` & `kslurm-0.6.2/neuroglia_helpers/bin/joblistSubmit`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/jupyter_snakemake` & `kslurm-0.6.2/neuroglia_helpers/bin/jupyter_snakemake`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/listusage` & `kslurm-0.6.2/neuroglia_helpers/bin/listusage`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/moveandlink` & `kslurm-0.6.2/neuroglia_helpers/bin/moveandlink`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/neurogliaBatch` & `kslurm-0.6.2/neuroglia_helpers/bin/neurogliaBatch`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/neurogliaSubmit` & `kslurm-0.6.2/neuroglia_helpers/bin/neurogliaSubmit`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/regularBatch` & `kslurm-0.6.2/neuroglia_helpers/bin/regularBatch`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/regularInteractive` & `kslurm-0.6.2/neuroglia_helpers/bin/regularInteractive`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/regularSubmit` & `kslurm-0.6.2/neuroglia_helpers/bin/regularSubmit`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/run_freesurfer_bids` & `kslurm-0.6.2/neuroglia_helpers/bin/run_freesurfer_bids`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #!/bin/bash
 
-
+version=7.2.0
 
 if [ "$#" -lt 3 ]
 then 
- echo "Freesurfer 7.1.0 *mini* bids-app  - runs recon-all -parallel -hires -threads 8 -all ... "
+ echo "Freesurfer ${version} *mini* bids-app  - runs recon-all -parallel -hires -threads 8 -all ... "
  echo ""
  echo "Must use this command with regularBatch, regularSubmit, or in a regularInteractive job"
  echo " as it uses the SLURM_TMPDIR local scratch to run. "
  echo ""
  echo "Usage: $0 <subject> <bids_dir> <output_dir> <optional recon-all args>"
  echo ""
  echo " e.g.: regularBatch $0 subjects.txt -a \"/path/to/bids_dir /path/to/output_dir\" -j 8core32gb12h "
  echo " where each line of subjects.txt contains e.g. sub-001"
  exit 1
 fi
 
 subject=$1
-bids_dir=$2
-out_dir=$3
+bids_dir=`realpath $2`
+out_dir=`realpath $3`
+
+if [ -z "$SLURM_TMPDIR" ]; then echo "must run this script on compute node"; exit 1; else echo "SLURM_TMPDIR=$SLURM_TMPDIR"; fi
 
 shift 3
 optargs=$@
 
 in_imgs=`ls $bids_dir/${subject}/*/anat/*T1w.nii.gz $bids_dir/${subject}/anat/*T1w.nii.gz`
 
 in_cmd=""
 for img in $in_imgs
 do
  in_cmd="$in_cmd -i $img"
 done
     
 
-module load freesurfer/7.1.0
+module load freesurfer/${version}
 mkdir -p $out_dir
 #run it in tempdir, then copy it over when finished
 recon-all -threads 8 -sd $SLURM_TMPDIR  -subjid $subject -parallel -hires -all $in_cmd $optargs
 if [ "$?" = "0" ]
 then
     pushd $SLURM_TMPDIR
     tar -cvf $out_dir/$subject.tar ${subject}
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/run_sclimbic_bids` & `kslurm-0.6.2/neuroglia_helpers/bin/run_sclimbic_bids`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/setAccess` & `kslurm-0.6.2/neuroglia_helpers/bin/setAccess`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/shub-cache` & `kslurm-0.6.2/neuroglia_helpers/bin/shub-cache`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/shub-cache-remote` & `kslurm-0.6.2/neuroglia_helpers/bin/shub-cache-remote`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/shub-upgrade` & `kslurm-0.6.2/neuroglia_helpers/bin/shub-upgrade`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/bin/snakemake_remotebatch` & `kslurm-0.6.2/neuroglia_helpers/bin/snakemake_remotebatch`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/cfg/graham.cfg` & `kslurm-0.6.2/neuroglia_helpers/cfg/graham.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 default_allocation=$(groups | tr ' ' '\n' |  grep --color=never def- | cut -d" " -f1 | head -n 1)
 
 CC_COMPUTE_ALLOC=${default_allocation} #for compute resources
 CC_STORAGE_ALLOC=${default_allocation} #for storage resources
 CC_GPU_ALLOC=${default_allocation} #for compute resources
 
 #Singularity options
-SINGULARITY_OPTS="-e -B /cvmfs:/cvmfs -B /project:/project -B /scratch:/scratch -B /localscratch:/localscratch"
+SINGULARITY_OPTS="-e -B /cvmfs:/cvmfs -B /project:/project -B /scratch:/scratch -B /local:/local -B /localscratch:/localscratch"
 NEUROGLIA_URI="docker://khanlab/neuroglia-core:latest"
 
 # paths for storing singularity images - default: shared singularity folder in akhanf
 SINGULARITY_DIR=/scratch/${USER}
-SINGULARITY_TMPDIR=/tmp #tmp folder for building images
+APPTAINER_TMPDIR=/tmp #tmp folder for building images
 
 JOB_SCRATCH_DIR=/scratch/${USER}/${SLURM_JOB_ID}_${SLURM_ARRAY_TASK_ID}
 ALT_JOB_SCRATCH_DIR=$SLURM_TMPDIR
 
 # app-specific settings we can distribute
 FMRIPREP_MULTIPROC_YAML=$NEUROGLIA_DIR/cfg_apps/fmriprep_multiproc_8c_32gb.yaml
-SINGULARITYENV_TEMPLATEFLOW_HOME=/home/fmriprep/.cache/templateflow #for newer fmriprep versions that require templateflow
+APPTAINERENV_TEMPLATEFLOW_HOME=/home/fmriprep/.cache/templateflow #for newer fmriprep versions that require templateflow
 
 #files we can't distribute:
 FS_LICENSE_FILE=$HOME/projects/$CC_STORAGE_ALLOC/shared/.license
 GRAD_COEFF_7T=$HOME/projects/$CC_STORAGE_ALLOC/shared/.coeff_AC84.grad
 #BEAST_PATH=/project/6007967/xiaobird/beast
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/cfg/graham_bmi.cfg` & `kslurm-0.6.2/neuroglia_helpers/cfg/graham_bmi.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # update these with your specific allocation
 #----
 CC_COMPUTE_ALLOC= #for compute resources
 CC_STORAGE_ALLOC= #for storage resources
 CC_GPU_ALLOC= #for compute resources
 
 #Singularity options
-SINGULARITY_OPTS="-e -B /cvmfs:/cvmfs -B /project:/project -B /scratch:/scratch -B /localscratch:/localscratch"
+SINGULARITY_OPTS="-e -B /cvmfs:/cvmfs -B /project:/project -B /scratch:/scratch -B /local:/local -B /localscratch:/localscratch"
 NEUROGLIA_URI="shub://akhanf/vasst-dev:v0.0.4g"
 
 # paths for storing singularity images - default: shared singularity folder in akhanf
 SINGULARITY_DIR=$HOME/projects/$CC_STORAGE_ALLOC/shared/singularity
 
 
 #see if SLURM_TMPDIR would work instead?
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/cfg/graham_ctb-akhanf-ab.cfg` & `kslurm-0.6.2/neuroglia_helpers/cfg/graham_ctb-akhanf-ab.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NEUROGLIA_URI="docker://khanlab/neuroglia-core:latest"
 
 # paths for storing singularity images - default: shared singularity folder in akhanf
 SINGULARITY_DIR=/project/6059441/shared/singularity
 #SINGULARITY_DIR=$HOME/projects/$CC_COMPUTE_ALLOC/$USER/singularity
 #SINGULARITY_TMPDIR=/tmp #tmp folder for building images
 
-SINGULARITY_BINDPATH="/cvmfs:/cvmfs,/project:/project,/scratch:/scratch,/localscratch:/localscratch"
+APPTAINER_BINDPATH="/cvmfs:/cvmfs,/project:/project,/scratch:/scratch,/local:/local,/localscratch:/localscratch"
 
 
 #lines commented out below have khanlab configuration not yet migrated to ctb-akhanf-ab
 
 #transparent singularity 
 export MODULEPATH=/project/6050199/software/transparentsingularity/modules:$MODULEPATH
 
@@ -26,15 +26,15 @@
 
 # app-specific settings we can distribute
 FMRIPREP_MULTIPROC_YAML=$NEUROGLIA_DIR/cfg_apps/fmriprep_multiproc_8c_32gb.yaml
 #SINGULARITYENV_TEMPLATEFLOW_HOME=/project/6007967/akhanf/opt/templateflow
 
 #files we can't distribute:
 FS_LICENSE_FILE=/project/6059441/shared/opt/.license
-SINGULARITYENV_FS_LICENSE=/project/6059441/shared/opt/.license
+APPTAINERENV_FS_LICENSE=/project/6059441/shared/opt/.license
 GRAD_COEFF_7T=/project/6059441/shared/opt/.coeff_AC84.grad
 #BEAST_PATH=/project/6007967/xiaobird/beast
 
 #pre-installed snakemake
 #SNAKEMAKE_VENV_DIR=/project/6007967/akhanf/opt/virtualenvs/snakemake/bin
 
 #snakemake path for --singularity-prefix, store symlinks to shub-cache containers here
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/cfg/graham_khanlab.cfg` & `kslurm-0.6.2/neuroglia_helpers/cfg/graham_khanlab.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 #Singularity options
 SINGULARITY_OPTS="-e"
 NEUROGLIA_URI="docker://khanlab/neuroglia-core:latest"
 
 # paths for storing singularity images - default: shared singularity folder in akhanf
 SINGULARITY_DIR=/project/6050199/akhanf/singularity # comment this line and uncomment line below to use personal singularity folder
 #SINGULARITY_DIR=$HOME/projects/$CC_COMPUTE_ALLOC/$USER/singularity
-SINGULARITY_TMPDIR=/tmp #tmp folder for building images
+APPTAINER_TMPDIR=/tmp #tmp folder for building images
 
-SINGULARITY_BINDPATH="/cvmfs:/cvmfs,/project:/project,/scratch:/scratch,/localscratch:/localscratch"
+APPTAINER_BINDPATH="/cvmfs:/cvmfs,/project:/project,/scratch:/scratch,/local:/local,/localscratch:/localscratch"
 
 #transparent singularity 
 export MODULEPATH=/project/6050199/software/transparentsingularity/modules:$MODULEPATH
 
 #see if SLURM_TMPDIR would work instead?
 JOB_SCRATCH_DIR=/scratch/${USER}/${SLURM_JOB_ID}_${SLURM_ARRAY_TASK_ID}
 ALT_JOB_SCRATCH_DIR=$SLURM_TMPDIR
 
 # app-specific settings we can distribute
 FMRIPREP_MULTIPROC_YAML=$NEUROGLIA_DIR/cfg_apps/fmriprep_multiproc_8c_32gb.yaml
 #centralized templateflow home can get out of date quickly, so disabled now -- 
 # you should pre-download templates to your home directory instead (see readme)
-#SINGULARITYENV_TEMPLATEFLOW_HOME=/project/ctb-akhanf/akhanf/opt/templateflow
+#APPTAINERENV_TEMPLATEFLOW_HOME=/project/ctb-akhanf/akhanf/opt/templateflow
 
 #files we can't distribute:
 FS_LICENSE_FILE=/project/ctb-akhanf/akhanf/opt/freesurfer/.license
-SINGULARITYENV_FS_LICENSE=/project/ctb-akhanf/akhanf/opt/freesurfer/.license
+APPTAINERENV_FS_LICENSE=/project/ctb-akhanf/akhanf/opt/freesurfer/.license
 GRAD_COEFF_7T=/project/ctb-akhanf/akhanf/opt/grad/.coeff_AC84.grad
 #BEAST_PATH=/project/6007967/xiaobird/beast
 
 #pre-installed snakemake
 SNAKEMAKE_VENV_DIR=/project/ctb-akhanf/akhanf/opt/virtualenvs/snakemake/bin
 
 #snakemake path for --singularity-prefix, store symlinks to shub-cache containers here
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/cfg/graham_local.cfg` & `kslurm-0.6.2/neuroglia_helpers/cfg/graham_local.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 #Singularity options
 SINGULARITY_OPTS="-e -B /mnt:/mnt"
 NEUROGLIA_URI="docker://khanlab/neuroglia-core:latest"
 
 # paths for storing singularity images - default: shared singularity folder in akhanf
 SINGULARITY_DIR=$HOME/singularity  # comment this line and uncomment line below to use personal singularity folder
 #SINGULARITY_DIR=$HOME/projects/$CC_COMPUTE_ALLOC/$USER/singularity
-SINGULARITY_TMPDIR=/tmp #tmp folder for building images
+APPTAINER_TMPDIR=/tmp #tmp folder for building images
 
 
 #see if SLURM_TMPDIR would work instead?
 JOB_SCRATCH_DIR=/scratch/${USER}/${SLURM_JOB_ID}_${SLURM_ARRAY_TASK_ID}
 ALT_JOB_SCRATCH_DIR=$SLURM_TMPDIR
 
 # app-specific settings we can distribute
 FMRIPREP_MULTIPROC_YAML=$NEUROGLIA_DIR/cfg_apps/fmriprep_multiproc_8c_32gb.yaml
-SINGULARITYENV_TEMPLATEFLOW_HOME=/home/fmriprep/.cache/templateflow #for newer fmriprep versions that require templateflow
+APPTAINERENV_TEMPLATEFLOW_HOME=/home/fmriprep/.cache/templateflow #for newer fmriprep versions that require templateflow
 
 #files we can't distribute:
 FS_LICENSE_FILE=/project/6007967/akhanf/opt/freesurfer/.license
 GRAD_COEFF_7T=/project/6007967/akhanf/opt/grad/.coeff_AC84.grad
 BEAST_PATH=/project/6007967/xiaobird/beast
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/cfg/graham_lpalaniy.cfg` & `kslurm-0.6.2/neuroglia_helpers/cfg/graham_lpalaniy.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # compute canada rrg:
 CC_COMPUTE_ALLOC=rrg-lpalaniy #for compute resources
 CC_STORAGE_ALLOC=rrg-lpalaniy #for compute resources
 CC_GPU_ALLOC=rrg-lpalaniy_gpu #for compute resources
 
 #Singularity options
-SINGULARITY_OPTS="-e -B /cvmfs:/cvmfs -B /project:/project -B /scratch:/scratch -B /localscratch:/localscratch"
+SINGULARITY_OPTS="-e -B /cvmfs:/cvmfs -B /project:/project -B /scratch:/scratch -B /local:/local -B /localscratch:/localscratch"
 NEUROGLIA_URI="docker://khanlab/neuroglia-core:latest"
 
 # paths for storing singularity images - default: shared singularity folder in akhanf
 SINGULARITY_DIR=/project/6033503/singularity  # comment this line and uncomment line below to use personal singularity folder
-SINGULARITY_TMPDIR=/tmp #tmp folder for building images
+APPTAINER_TMPDIR=/tmp #tmp folder for building images
 
 #see if SLURM_TMPDIR would work instead?
 JOB_SCRATCH_DIR=/scratch/${USER}/${SLURM_JOB_ID}_${SLURM_ARRAY_TASK_ID}
 ALT_JOB_SCRATCH_DIR=$SLURM_TMPDIR
 
 # app-specific settings we can distribute
 FMRIPREP_MULTIPROC_YAML=$NEUROGLIA_DIR/cfg_apps/fmriprep_multiproc_8c_32gb.yaml
-SINGULARITYENV_TEMPLATEFLOW_HOME=/home/fmriprep/.cache/templateflow #for newer fmriprep versions that require templateflow
+APPTAINERENV_TEMPLATEFLOW_HOME=/home/fmriprep/.cache/templateflow #for newer fmriprep versions that require templateflow
 
 #files we can't distribute:
 FS_LICENSE_FILE=/project/6033503/shared/.license
 GRAD_COEFF_7T=/project/6033503/shared/.coeff_AC84.grad
 #BEAST_PATH=/project/6007967/xiaobird/beast
```

### Comparing `kslurm-0.6.1/neuroglia_helpers/etc/bash_lib.sh` & `kslurm-0.6.2/neuroglia_helpers/etc/bash_lib.sh`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/etc/make_snakemake_singularity_links.py` & `kslurm-0.6.2/neuroglia_helpers/etc/make_snakemake_singularity_links.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/etc/printGroupUsage` & `kslurm-0.6.2/neuroglia_helpers/etc/printGroupUsage`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/etc/remote_pull` & `kslurm-0.6.2/neuroglia_helpers/etc/remote_pull`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/etc/setup_sshfs_graham` & `kslurm-0.6.2/neuroglia_helpers/etc/setup_sshfs_graham`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/etc/snakemake_slurm_submit.py` & `kslurm-0.6.2/neuroglia_helpers/etc/snakemake_slurm_submit.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/neuroglia_helpers/validate_bids-apps.tsv.py` & `kslurm-0.6.2/neuroglia_helpers/validate_bids-apps.tsv.py`

 * *Files identical despite different names*

### Comparing `kslurm-0.6.1/pyproject.toml` & `kslurm-0.6.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kslurm"
-version = "0.6.1"
+version = "0.6.2"
 description = "Helper scripts and wrappers for running commands on SLURM compute clusters."
 license = "MIT"
 readme = "README.md"
 authors = ["Peter Van Dyken <pvandyk2@uwo.ca>"]
 repository = "https://github.com/pvandyken/kslurm"
 keywords = ["slurm", "compute cluster"]
 classifiers = [
@@ -21,14 +21,22 @@
     "Typing :: Typed"
 ]
 packages = [
     { include = "kslurm" },
     { include = "neuroglia_helpers" }
 ]
 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+dirty = true
+style = "pep440"
+bump = true
+
+
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 attrs = "^21.2.0"
 colorama = "^0.4.4"
 typing-extensions = ">=3.10"
 rich = "^12.2.0"
 tabulate = "^0.8.9"
@@ -63,16 +71,16 @@
 krun = 'kslurm.cli.krun:krun.cli'
 kjupyter = 'kslurm.cli.kjupyter:kjupyter.cli'
 kslurm = 'kslurm.cli.main:main.cli'
 kpy = 'kslurm.cli.kpy:kpy.cli'
 kapp = 'kslurm.cli.kapp.main:kapp.cli'
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 add_imports = ["from __future__ import absolute_import"]
 # We ignore __init__ file so that mkinit and isort don't undo each other
 extend_skip = ["__init__.py", "neuroglia_helpers"]
```

### Comparing `kslurm-0.6.1/setup.py` & `kslurm-0.6.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,411 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kslurm
+Version: 0.6.2
+Summary: Helper scripts and wrappers for running commands on SLURM compute clusters.
+Home-page: https://github.com/pvandyken/kslurm
+License: MIT
+Keywords: slurm,compute cluster
+Author: Peter Van Dyken
+Author-email: pvandyk2@uwo.ca
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: InquirerPy (>=0.3.3,<0.4.0)
+Requires-Dist: Pint (>=0.19.2,<0.20.0)
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: attrs (>=21.2.0,<22.0.0)
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
+Requires-Dist: docstring-parser (>=0.14.1,<0.15.0)
+Requires-Dist: flake8 (>=4.0.1,<5.0.0)
+Requires-Dist: more-itertools (>=8.13.0,<9.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: rich (>=12.2.0,<13.0.0)
+Requires-Dist: semver (>=2.13.0,<3.0.0)
+Requires-Dist: shellingham (>=1.4.0,<2.0.0)
+Requires-Dist: tabulate (>=0.8.9,<0.9.0)
+Requires-Dist: typing-extensions (>=3.10)
+Requires-Dist: virtualenv (>=20.0.24,<21)
+Requires-Dist: yaspin (>=2.2.0,<3.0.0)
+Project-URL: Repository, https://github.com/pvandyken/kslurm
+Description-Content-Type: text/markdown
 
-packages = \
-['kslurm',
- 'kslurm.args',
- 'kslurm.bin',
- 'kslurm.cli',
- 'kslurm.cli.kapp',
- 'kslurm.data',
- 'kslurm.installer',
- 'kslurm.models',
- 'kslurm.slurm',
- 'kslurm.style',
- 'kslurm.test',
- 'kslurm.test.args',
- 'kslurm.test.installer',
- 'neuroglia_helpers',
- 'neuroglia_helpers.etc']
-
-package_data = \
-{'': ['*'],
- 'neuroglia_helpers': ['.github/workflows/*',
-                       '.github_scripts/*',
-                       'bin/*',
-                       'cfg/*',
-                       'cfg_apps/*',
-                       'job-templates/*']}
-
-install_requires = \
-['InquirerPy>=0.3.3,<0.4.0',
- 'Pint>=0.19.2,<0.20.0',
- 'appdirs>=1.4.4,<2.0.0',
- 'attrs>=21.2.0,<22.0.0',
- 'colorama>=0.4.4,<0.5.0',
- 'docstring-parser>=0.14.1,<0.15.0',
- 'flake8>=4.0.1,<5.0.0',
- 'more-itertools>=8.13.0,<9.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'rich>=12.2.0,<13.0.0',
- 'semver>=2.13.0,<3.0.0',
- 'shellingham>=1.4.0,<2.0.0',
- 'tabulate>=0.8.9,<0.9.0',
- 'typing-extensions>=3.10',
- 'virtualenv>=20.0.24,<21',
- 'yaspin>=2.2.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['kapp = kslurm.cli.kapp.main:kapp.cli',
-                     'kbatch = kslurm.cli.kbatch:kbatch.cli',
-                     'kjupyter = kslurm.cli.kjupyter:kjupyter.cli',
-                     'kpy = kslurm.cli.kpy:kpy.cli',
-                     'krun = kslurm.cli.krun:krun.cli',
-                     'kslurm = kslurm.cli.main:main.cli']}
-
-setup_kwargs = {
-    'name': 'kslurm',
-    'version': '0.6.1',
-    'description': 'Helper scripts and wrappers for running commands on SLURM compute clusters.',
-    'long_description': 'Utility functions to make working with SLURM easier.\n\n# Installation\nThe recommend way to install kslurm is via [`pipx`](https://pypa.github.io/pipx), a tool for installing python applications.\nThis will make kslurm globally available without infecting your global python environment.\nInstallation instructions for pipx can be found on their [website](https://pypa.github.io/pipx).\nOnce installed, simply run\n```bash\npipx install kslurm\n```\n\nNote that kslurm requires Python 3.9 or higher.\nIf pipx was installed using a lower version (e.g. 3.8), you will need to manually specify the python executable to use.\nActivate the appropriate python version (e.g. `module load python/3.10`) so that when you run `python --version`, the correct version appears.\nThen run\n\n```bash\npipx install kslurm --python $(which python)\n```\n\nFor full kslurm features, including integration with `pip`, you need to source the init script, preferably in your `~.bash_profile` (the init script contains commands that may not be available on non-login nodes). You can do this by running:\n\n```bash\nkpy bash >> $HOME/.bash_profile\n```\n\nFinally, you need to complete some basic configuration. First, set your SLURM account. Run\n\n```bash\nkslurm config account -i\n```\n\nThis will begin an interactive session letting you choose from the accounts available to you. Each account will be listed with it\'s LevelFS. The higher the LevelFS, the more underused the account is, so prefer accounts with higher values.\n\nNext, set your pipdir. This will be used to store python wheels and virtual envs. It should be in a permanent storage or project directory. For instance, on ComputeCanada servers, it should go in `$HOME/projects/<account_name>/<user_name>/.kslurm`. Use the following command:\n\n```bash\nkslurm config pipdir <dir>\n```\n\n## Upgrading and uninstalling\n\nThe app can be updated by running\n```bash\npipx upgrade kslurm\n```\n\nand removed using\n```bash\npipx uninstall kslurm\n```\n\n## Neuroglia-helpers Integration\n\nSee the [dedicated page](docs/neuroglia-helpers.md).\n\n## Legacy Installer\nkslurm includes an installation script that, previously, was the recommended install method.\nWhile it should technically still work, it is no longer supported and may be removed in the future.\nIts instructions are included, for reference, below.\n\nUsers who previously installed kslurm via this script should switch to a pipx install for long term support. Simply uninstall `kslurm` using the instructions below, then install via pipx as described above\n\nInstallation is via the following command:\n```\ncurl -sSL https://raw.githubusercontent.com/pvandyken/kslurm/master/install_kslurm.py | python -\n```\n\nIf you wish to uninstall, run the same command with `--uninstall` added to the end.\n\nThe package can be updated by running `kslurm update`.\n\n# Features\nCurrently offers four commands:\n* kbatch: for batch submission jobs (no immediate output)\n* krun: for interactive submission\n* kjupyter: for Jupyter sessions\n* kpy: for python environment management\n\nAll three use a regex-based argument parsing, meaning that instead of writing a SLURM file or supplying confusing `--arguments`, you can request resources with an intuitive syntax:\n\n```\nkrun 4 3:00 15G gpu\n```\nThis command will request an interactive session with __4__ cores, for __3hr__, using __15GB__ of memory, and a __gpu__.\n\nAnything not specfically requested will fall back to a default. For instance, by default the commands will request 3hr jobs using 1 core with 4GB of memory. You can also run a predefined job template using -j _template_. Run either command with -J to get a list of all templates. Any template values can be overriden simply by providing the appropriate argument.\n\nThe full list of possible requests, their syntaxes, and their defaults can be found at the bottom of the README.\n\n## krun\n\nkrun is used for interactive sessions on the cluster. If you run krun all by itself, it will fire up an interactive session on the cluster:\n\n```\nkrun\n```\nYou\'ll notice the server name in your terminal prompt will be changed to the cluster assigned to you. To end the session, simply use the `exit` command.\n\nYou can also submit a specific program to run:\n\n```\nkrun 1:00 1G python my_program.py\n```\nThis will request a 1hr session with one core and 1 GB of memory. The output of the job will be displayed on the console. Note that your terminal will be tied to the job, so if you quit, or get disconnected, your job will end. (tmux can be used to help mitigate this, see this [tutorial from Yale](https://docs.ycrc.yale.edu/clusters-at-yale/guides/tmux/) for an excellent overview).\n\nNote that you should never request more than the recommended amount of time for interactive jobs as specified by your cluster administrator. For ComputeCanada servers, you should never request more than 3 hr. If you do, you\'ll be placed in the general pool for resource assignment, and the job could take hours to start. Jobs of 3hr or less typically start in less than a minute.\n\n## kbatch\n\nJobs that don\'t require monitoring of the output or immediate submission, or will run for more than three hours, should be submitted using `kbatch`. This command schedules the job, then returns control of the terminal. Output from the job will be placed in a file in your current working directory entitled `slurm-[jobid].out`.\n\nImproving on `sbatch`, `kbatch` does not require a script file. You can directly submit a command:\n\n```\nkbatch 2-00:00 snakemake --profile slurm\n```\nThis will schedule a 2 day job running snakemake.\n\nOf course, complicated jobs can still be submitted using a script. Note that kbatch explictely specifies the resources it knows about in the command line. Command line args override `#SBATCH --directives` in the submit script, so at this time, you cannot use such directives to request resources unless they are not currently supported by kslurm. This may change in a future release.\n\n## kjupyter\n\nThis command requests an interactive job running a jupyter server. As with krun, you should not request a job more than the recommended maximum time for your cluster (3hr for ComputeCanada). If you need more time than that, just request a new job when the old one expires.\n\nIn addition to the desired resources, you should use the `--venv` flag to request a saved virtual environment (see `kpy save`). Jupyter will be started in whatever environment you request. `jupyter-lab` should already be installed in the venv.\n```\nkjupyter 32G 2 --venv <your_venv_name>\n```\nThis will start a jupyter session with 32 GB of memory and 2 cores.\n\nIf no venv is specified, `kjupyter` will assume that the `jupyter-lab` command is already available on the `$PATH`. This is useful to run a global instance of jupyter, or jupyter installed in an active venv. Note that this prevents installing jupyter on local scratch, so performance will take a hit.\n\n# Unsupported SLURM args\n\nCurrently, the only way to supply arguments to SLURM beyond the items listed below is to list it as an `#SBATCH --directive` in a submission script. This only works with `kbatch`, not `krun` or `kjupyter`. A future release may support a method to supply these arguments directly on the command line. If you frequently use an option not listed below, make an issue and we can discuss adding support!\n\n# Slurm Syntax\n\nThe full syntax is outlined below. You can always run a command with `-h` to get help.\n\n| Resource  |           Syntax           |                                                                   Default |                                                    Description |\n| :-------- | :------------------------: | ------------------------------------------------------------------------: | -------------------------------------------------------------: |\n| Time      | [d-]dd:dd -> [days-]hh:mm  |                                                                       3hr |                                   The amount of time requested |\n| CPUS      |     d -> just a number     |                                                                         1 |                                   The number of CPUs requested |\n| Memory    |            d(G/M)[B] -> e.g. 4G, 500MB |                                                            4GB | The amount of memory requested |\n| Account   | --account <_account name_> |                                                                           |                      The account under which to submit the job. A default account can be configured using `kslurm config account <account_name>` |\n| GPU       |            gpu             |                                                                     False |                         Provide flag to request 1 GPU instance |\n| Directory |  <_any valid directory_>   |                                                                        ./ | Change the current working directory before submitting the job |\n| x11       |           --x11            |                                                                     False |                   Requests x11 forwarding for GUI applications |\n\n# kpy\n\nkpy bundles a set of commands to help manage pip virtual environments on Slurm compute clusters, specifically addressing a few issues unique to such servers:\n\n## Ephemeral venvs\nIn most use cases, python venvs are installed on compute clusters, ideally on local scratch storage.\nThis makes venvs inherently ephemeral.\nBecause installing a venv can take an appreciable amount of time, kpy packs tools to archive entire venvs for storage in a permanent local repository (ideally located in project-specific or permanent storage). Once saved, venvs can be quickly reloaded into a new compute environment.\n\nNote that copying venvs from one location to another is not a trivial task. The current setup has been tested on ComputeCanada servers without any issues so far, but problems may arise on another environment.\n\n## No internet\nCompute clusters often don\'t have an internet connection, limiting our install repertoire to locally available wheels.\nWith kpy, venvs can be created on a login node (using the available internet connection), then saved and loaded onto a compute node.\nKpy also includes some optional bash tools (see `kpy bash`), including a wrapper around pip that prevents it from accessing the internet on compute nodes, and connecting it with a local private wheelhouse.\n\n## Commands\n### `create`\n\n```bash\n# usage\nkpy create [<version|3.x>] [<name>]\n```\n\nCreate a new environment.\nName is optional; if not provided, a placeholder name will be created.\nVersion must be of the form `3.x` where x is any number (e.g `3.8`, `3.10`).\nIf provided, the corresponding python version will be used in the virtual env.\nNote that an appropriate python executable must be somewhere on your path (e.g. for `3.8` -> `python3.8`).\nIf not provided, the python version used to install kslurm will be used.\n\nIf run on a login node, the env will be created in a `$TMPDIR`.\nIf run on a compute node, it will be created in `$SLURM_TMPDIR`.\n\n### `save`\n\n```bash\n# usage\nkpy save [-f] <name>\n```\n\nSave the venv to your permanent cache.\nThis requires setting `pipdir` in the kslurm config (see below).\nBy default, `save` will not oversave an existing cache, but `-f` can be included to override this behaviour.\nIf a new name is provided, it will be used to update the current venv name and prompt.\n\n### `load`\n\n\n```bash\n# usage\nkpy load [<name>] [--as <newname>]\n```\n\nLoad a saved venv from the cache.\nIf a venv called `<name>` already exists, the command will fail, as each name can only be used once.\n`--as <newname>` works around this by changing the name of the loaded venv (the name of the saved venv will remain the same)\nCalling `load` without any `<name>` will print a list of current cached venvs.\n\n### `activate`\n\n```bash\n# usage\nkpy activate [<name>]\n```\n\nActivate venv initialized using `create` or `load`.\nName will be the same as the name appearing in the venv prompt (i.e. the name provided on initial loading or creation, through `--as`, or the last saved name).\nThis command only works on a compute node.\nVenvs created on a login node cannot be directly activated using kpy.\nCall without a name to list the venvs you can activate.\n\n### `list`\n\n```bash\n# usage\nkpy list\n```\n\nList all saved venvs (i.e. venvs you can `load`)\n\n### `rm`\n\n```bash\n# usage\nkpy rm <name>\n```\n\nDelete a saved venv.\n\n\n### `bash`\n\n```bash\n# usage\nkpy bash\n```\n\nEchos a line of bash script that can be added to your `.bashrc` file:\n\n```bash\nkpy bash >> $HOME/.bashrc\n```\n\nThis adds a few features to your command line environment:\n\n- **pip wrapper**: Adds a wrapper around pip that detects if you are on a login node when running `install`, `wheel`, or `download`. If not on a login node, the `--no-index` flag will be appended to the command, preventing the use of an internet connection.\n- **wheelhouse management**: If `pipdir` is configured in the kslurm config, a wheelhouse will be created in your pip repository. Any wheels downloaded using `pip wheel` will be placed in that wheelhouse, and all wheels in the wheelhouse will be discoverable by `pip install`, both on login and compute nodes.\n\n## Kapp\n\nKapp provides a set of tools to manage singularity containers. Pull images from docker hub without worring about image size, pulling the same image twice, or tracking whether your ":latest" image is up to date. Kapp manages your `.sif` image files so you can run them from anywhere on the cluster, without managing environment variables or remembering paths. Kapp managed images can be seamlessly consumed by snakemake workflows using the provided `--singularity-prefix` directory.\n\n### `pull`\n\n```bash\n# usage\nkapp pull <image_uri> [-a <alias>] [--mem <memory>]\n```\n\nPull an image from a repository. Currently, only docker-hub is supported. The image uri should look like this:\n\n```bash\n[<scheme>://[<organization>/]<repo>:<tag>]\n\n# examples\ndocker://ubuntu:latest\nnipreps/fmriprep:21.0.2\nbusybox:latest\n```\n\nNote that the scheme is optional, and defaults to `docker`. The organization should be omitted for official docker images.\n\nWhen you call `kapp pull`, the tag gets resolved to the specific container it points to. Thus, if you pull multiple tags pointing to the same container (e.g. `:latest` and its associated version tag), the container will only be pulled once. Plus, if tags get updated (e.g. `:latest` when a new release comes out), `kapp pull` will download the latest version of the tag, even if you\'ve pulled that tag before.\n\nWhen pulling a container, you can use `-a <alias>` to set an alias for the uri. This alias can be used in place of the uri in future kapp commands (except for `kapp pull`). For instance, you could download fmriprep and run it using the following:\n\n```bash\nkapp pull nipreps/fmriprep:latest -a fmriprep\nkapp run fmriprep\n```\n\nBuilding `.sif` files from docker containers can consume a significant amount of memory and resources, making an unsuitable operation for login nodes. kapp works around this by first downloading the container on the login node, then scheduling a build step on an interactive compute node. It will automatically try to estimate how much memory will be needed, but if a build fails due to lack of memory, you can specify how much memory to request using the `--mem <memory>` parameter. Note that very small containers will be built directly on the login node without a compute step.\n\n### `path`\n```bash\n# usage\nkapp path <uri_or_alias>\n```\n\nPrints the path of the specified container. This creates an easy way to use kapp managed containers with any arbitrary singularity command:\n\n```bash\nsingularity -b /path/to/bind/dir $(kapp path my_container)\n```\n\n### `image`\n\n```bash\n# usage\nkapp image (list|rm <uri_or_alias>)\n```\n\nHas two subcommands `list` and `rm <container>` to list all pulled containers and remove a container.\n\n`kapp image rm` does not actually remove any data, it just removes the supplied uri (along with any aliases that point to it). This is because the underlying data may be used by other image tags. Dangling containers, which aren\'t pointed to by any local uris, can be deleted using `kapp purge dangling`\n\n### `purge`\n\n```bash\n# usage\nkapp purge dangling\n```\n\nDelete all dangling image files: i.e. files that aren\'t pointed to by any local uris. This command also removes any snakemake aliases pointing to the data.\n\n### `alias`\n\n```bash\n# usage\nkapp alias list\n```\n\nList all aliases currently in use, along with the containers they point to.\n\n### `exec`, `shell`, `run`\n\n```bash\n# usage\nkapp (exec|shell|run) <uri_or_alias> [args...]\n```\n\nSimple wrapper around `singularity (exec|shell|run)`. No singularity args can be specified, only args for the container. If you need to specify singularity args, call singularity directly and use `kapp path <container>` to get the container path. Note that most singularity args (e.g. directory bids) can be specified using environment variable, and such variables will be consumed by `kapp` as normal.\n\n### `snakemake`\n\nPrints the path to the snakemake directory. This path can be supplied to the snakemake parameter `--singularity-prefix`, allowing snakemake to seamlessly consume containers downloaded using kapp. This is especially usefull for cluster execution without internet connection: containers can be pulled in advance on a login node, then used by snakemake later.\n\n## Configuration\n\nkslurm currently supports a few basic configuration values, and more will come with time. All configuration can be set using the command\n\n```bash\nkslurm config <key> <value>\n```\n\nYou can print the value of a configuration using\n\n```bash\nkslurm config <key>\n```\n\n### Current values\n\n* `account`: Default account to use for kslurm commands (e.g. `kbatch`, `krun`, etc)\n* `pipdir`: Directory to store cached venvs and wheels. Should be a project or permanent storage dir.\n',
-    'author': 'Peter Van Dyken',
-    'author_email': 'pvandyk2@uwo.ca',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pvandyken/kslurm',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+Utility functions to make working with SLURM easier.
 
+# Installation
+The recommend way to install kslurm is via [`pipx`](https://pypa.github.io/pipx), a tool for installing python applications.
+This will make kslurm globally available without infecting your global python environment.
+Installation instructions for pipx can be found on their [website](https://pypa.github.io/pipx).
+Once installed, simply run
+```bash
+pipx install kslurm
+```
+
+Note that kslurm requires Python 3.9 or higher.
+If pipx was installed using a lower version (e.g. 3.8), you will need to manually specify the python executable to use.
+Activate the appropriate python version (e.g. `module load python/3.10`) so that when you run `python --version`, the correct version appears.
+Then run
+
+```bash
+pipx install kslurm --python $(which python)
+```
+
+For full kslurm features, including integration with `pip`, you need to source the init script, preferably in your `~.bash_profile` (the init script contains commands that may not be available on non-login nodes). You can do this by running:
+
+```bash
+kpy bash >> $HOME/.bash_profile
+```
+
+Finally, you need to complete some basic configuration. First, set your SLURM account. Run
+
+```bash
+kslurm config account -i
+```
+
+This will begin an interactive session letting you choose from the accounts available to you. Each account will be listed with it's LevelFS. The higher the LevelFS, the more underused the account is, so prefer accounts with higher values.
+
+Next, set your pipdir. This will be used to store python wheels and virtual envs. It should be in a permanent storage or project directory. For instance, on ComputeCanada servers, it should go in `$HOME/projects/<account_name>/<user_name>/.kslurm`. Use the following command:
+
+```bash
+kslurm config pipdir <dir>
+```
+
+## Upgrading and uninstalling
+
+The app can be updated by running
+```bash
+pipx upgrade kslurm
+```
+
+and removed using
+```bash
+pipx uninstall kslurm
+```
+
+## Neuroglia-helpers Integration
+
+See the [dedicated page](docs/neuroglia-helpers.md).
+
+## Legacy Installer
+kslurm includes an installation script that, previously, was the recommended install method.
+While it should technically still work, it is no longer supported and may be removed in the future.
+Its instructions are included, for reference, below.
+
+Users who previously installed kslurm via this script should switch to a pipx install for long term support. Simply uninstall `kslurm` using the instructions below, then install via pipx as described above
+
+Installation is via the following command:
+```
+curl -sSL https://raw.githubusercontent.com/pvandyken/kslurm/master/install_kslurm.py | python -
+```
+
+If you wish to uninstall, run the same command with `--uninstall` added to the end.
+
+The package can be updated by running `kslurm update`.
+
+# Features
+Currently offers four commands:
+* kbatch: for batch submission jobs (no immediate output)
+* krun: for interactive submission
+* kjupyter: for Jupyter sessions
+* kpy: for python environment management
+
+All three use a regex-based argument parsing, meaning that instead of writing a SLURM file or supplying confusing `--arguments`, you can request resources with an intuitive syntax:
+
+```
+krun 4 3:00 15G gpu
+```
+This command will request an interactive session with __4__ cores, for __3hr__, using __15GB__ of memory, and a __gpu__.
+
+Anything not specfically requested will fall back to a default. For instance, by default the commands will request 3hr jobs using 1 core with 4GB of memory. You can also run a predefined job template using -j _template_. Run either command with -J to get a list of all templates. Any template values can be overriden simply by providing the appropriate argument.
+
+The full list of possible requests, their syntaxes, and their defaults can be found at the bottom of the README.
+
+## krun
+
+krun is used for interactive sessions on the cluster. If you run krun all by itself, it will fire up an interactive session on the cluster:
+
+```
+krun
+```
+You'll notice the server name in your terminal prompt will be changed to the cluster assigned to you. To end the session, simply use the `exit` command.
+
+You can also submit a specific program to run:
+
+```
+krun 1:00 1G python my_program.py
+```
+This will request a 1hr session with one core and 1 GB of memory. The output of the job will be displayed on the console. Note that your terminal will be tied to the job, so if you quit, or get disconnected, your job will end. (tmux can be used to help mitigate this, see this [tutorial from Yale](https://docs.ycrc.yale.edu/clusters-at-yale/guides/tmux/) for an excellent overview).
+
+Note that you should never request more than the recommended amount of time for interactive jobs as specified by your cluster administrator. For ComputeCanada servers, you should never request more than 3 hr. If you do, you'll be placed in the general pool for resource assignment, and the job could take hours to start. Jobs of 3hr or less typically start in less than a minute.
+
+## kbatch
+
+Jobs that don't require monitoring of the output or immediate submission, or will run for more than three hours, should be submitted using `kbatch`. This command schedules the job, then returns control of the terminal. Output from the job will be placed in a file in your current working directory entitled `slurm-[jobid].out`.
+
+Improving on `sbatch`, `kbatch` does not require a script file. You can directly submit a command:
+
+```
+kbatch 2-00:00 snakemake --profile slurm
+```
+This will schedule a 2 day job running snakemake.
+
+Of course, complicated jobs can still be submitted using a script. Note that kbatch explictely specifies the resources it knows about in the command line. Command line args override `#SBATCH --directives` in the submit script, so at this time, you cannot use such directives to request resources unless they are not currently supported by kslurm. This may change in a future release.
+
+## kjupyter
+
+This command requests an interactive job running a jupyter server. As with krun, you should not request a job more than the recommended maximum time for your cluster (3hr for ComputeCanada). If you need more time than that, just request a new job when the old one expires.
+
+In addition to the desired resources, you should use the `--venv` flag to request a saved virtual environment (see `kpy save`). Jupyter will be started in whatever environment you request. `jupyter-lab` should already be installed in the venv.
+```
+kjupyter 32G 2 --venv <your_venv_name>
+```
+This will start a jupyter session with 32 GB of memory and 2 cores.
+
+If no venv is specified, `kjupyter` will assume that the `jupyter-lab` command is already available on the `$PATH`. This is useful to run a global instance of jupyter, or jupyter installed in an active venv. Note that this prevents installing jupyter on local scratch, so performance will take a hit.
+
+# Unsupported SLURM args
+
+Currently, the only way to supply arguments to SLURM beyond the items listed below is to list it as an `#SBATCH --directive` in a submission script. This only works with `kbatch`, not `krun` or `kjupyter`. A future release may support a method to supply these arguments directly on the command line. If you frequently use an option not listed below, make an issue and we can discuss adding support!
+
+# Slurm Syntax
+
+The full syntax is outlined below. You can always run a command with `-h` to get help.
+
+| Resource  |           Syntax           |                                                                   Default |                                                    Description |
+| :-------- | :------------------------: | ------------------------------------------------------------------------: | -------------------------------------------------------------: |
+| Time      | [d-]dd:dd -> [days-]hh:mm  |                                                                       3hr |                                   The amount of time requested |
+| CPUS      |     d -> just a number     |                                                                         1 |                                   The number of CPUs requested |
+| Memory    |            d(G/M)[B] -> e.g. 4G, 500MB |                                                            4GB | The amount of memory requested |
+| Account   | --account <_account name_> |                                                                           |                      The account under which to submit the job. A default account can be configured using `kslurm config account <account_name>` |
+| GPU       |            gpu             |                                                                     False |                         Provide flag to request 1 GPU instance |
+| Directory |  <_any valid directory_>   |                                                                        ./ | Change the current working directory before submitting the job |
+| x11       |           --x11            |                                                                     False |                   Requests x11 forwarding for GUI applications |
+
+# kpy
+
+kpy bundles a set of commands to help manage pip virtual environments on Slurm compute clusters, specifically addressing a few issues unique to such servers:
+
+## Ephemeral venvs
+In most use cases, python venvs are installed on compute clusters, ideally on local scratch storage.
+This makes venvs inherently ephemeral.
+Because installing a venv can take an appreciable amount of time, kpy packs tools to archive entire venvs for storage in a permanent local repository (ideally located in project-specific or permanent storage). Once saved, venvs can be quickly reloaded into a new compute environment.
+
+Note that copying venvs from one location to another is not a trivial task. The current setup has been tested on ComputeCanada servers without any issues so far, but problems may arise on another environment.
+
+## No internet
+Compute clusters often don't have an internet connection, limiting our install repertoire to locally available wheels.
+With kpy, venvs can be created on a login node (using the available internet connection), then saved and loaded onto a compute node.
+Kpy also includes some optional bash tools (see `kpy bash`), including a wrapper around pip that prevents it from accessing the internet on compute nodes, and connecting it with a local private wheelhouse.
+
+## Commands
+### `create`
+
+```bash
+# usage
+kpy create [<version|3.x>] [<name>]
+```
+
+Create a new environment.
+Name is optional; if not provided, a placeholder name will be created.
+Version must be of the form `3.x` where x is any number (e.g `3.8`, `3.10`).
+If provided, the corresponding python version will be used in the virtual env.
+Note that an appropriate python executable must be somewhere on your path (e.g. for `3.8` -> `python3.8`).
+If not provided, the python version used to install kslurm will be used.
+
+If run on a login node, the env will be created in a `$TMPDIR`.
+If run on a compute node, it will be created in `$SLURM_TMPDIR`.
+
+### `save`
+
+```bash
+# usage
+kpy save [-f] <name>
+```
+
+Save the venv to your permanent cache.
+This requires setting `pipdir` in the kslurm config (see below).
+By default, `save` will not oversave an existing cache, but `-f` can be included to override this behaviour.
+If a new name is provided, it will be used to update the current venv name and prompt.
+
+### `load`
+
+
+```bash
+# usage
+kpy load [<name>] [--as <newname>]
+```
+
+Load a saved venv from the cache.
+If a venv called `<name>` already exists, the command will fail, as each name can only be used once.
+`--as <newname>` works around this by changing the name of the loaded venv (the name of the saved venv will remain the same)
+Calling `load` without any `<name>` will print a list of current cached venvs.
+
+### `activate`
+
+```bash
+# usage
+kpy activate [<name>]
+```
+
+Activate venv initialized using `create` or `load`.
+Name will be the same as the name appearing in the venv prompt (i.e. the name provided on initial loading or creation, through `--as`, or the last saved name).
+This command only works on a compute node.
+Venvs created on a login node cannot be directly activated using kpy.
+Call without a name to list the venvs you can activate.
+
+### `list`
+
+```bash
+# usage
+kpy list
+```
+
+List all saved venvs (i.e. venvs you can `load`)
+
+### `rm`
+
+```bash
+# usage
+kpy rm <name>
+```
+
+Delete a saved venv.
+
+
+### `bash`
+
+```bash
+# usage
+kpy bash
+```
+
+Echos a line of bash script that can be added to your `.bashrc` file:
+
+```bash
+kpy bash >> $HOME/.bashrc
+```
+
+This adds a few features to your command line environment:
+
+- **pip wrapper**: Adds a wrapper around pip that detects if you are on a login node when running `install`, `wheel`, or `download`. If not on a login node, the `--no-index` flag will be appended to the command, preventing the use of an internet connection.
+- **wheelhouse management**: If `pipdir` is configured in the kslurm config, a wheelhouse will be created in your pip repository. Any wheels downloaded using `pip wheel` will be placed in that wheelhouse, and all wheels in the wheelhouse will be discoverable by `pip install`, both on login and compute nodes.
+
+## Kapp
+
+Kapp provides a set of tools to manage singularity containers. Pull images from docker hub without worring about image size, pulling the same image twice, or tracking whether your ":latest" image is up to date. Kapp manages your `.sif` image files so you can run them from anywhere on the cluster, without managing environment variables or remembering paths. Kapp managed images can be seamlessly consumed by snakemake workflows using the provided `--singularity-prefix` directory.
+
+### `pull`
+
+```bash
+# usage
+kapp pull <image_uri> [-a <alias>] [--mem <memory>]
+```
+
+Pull an image from a repository. Currently, only docker-hub is supported. The image uri should look like this:
+
+```bash
+[<scheme>://[<organization>/]<repo>:<tag>]
+
+# examples
+docker://ubuntu:latest
+nipreps/fmriprep:21.0.2
+busybox:latest
+```
+
+Note that the scheme is optional, and defaults to `docker`. The organization should be omitted for official docker images.
+
+When you call `kapp pull`, the tag gets resolved to the specific container it points to. Thus, if you pull multiple tags pointing to the same container (e.g. `:latest` and its associated version tag), the container will only be pulled once. Plus, if tags get updated (e.g. `:latest` when a new release comes out), `kapp pull` will download the latest version of the tag, even if you've pulled that tag before.
+
+When pulling a container, you can use `-a <alias>` to set an alias for the uri. This alias can be used in place of the uri in future kapp commands (except for `kapp pull`). For instance, you could download fmriprep and run it using the following:
+
+```bash
+kapp pull nipreps/fmriprep:latest -a fmriprep
+kapp run fmriprep
+```
+
+Building `.sif` files from docker containers can consume a significant amount of memory and resources, making an unsuitable operation for login nodes. kapp works around this by first downloading the container on the login node, then scheduling a build step on an interactive compute node. It will automatically try to estimate how much memory will be needed, but if a build fails due to lack of memory, you can specify how much memory to request using the `--mem <memory>` parameter. Note that very small containers will be built directly on the login node without a compute step.
+
+### `path`
+```bash
+# usage
+kapp path <uri_or_alias>
+```
+
+Prints the path of the specified container. This creates an easy way to use kapp managed containers with any arbitrary singularity command:
+
+```bash
+singularity -b /path/to/bind/dir $(kapp path my_container)
+```
+
+### `image`
+
+```bash
+# usage
+kapp image (list|rm <uri_or_alias>)
+```
+
+Has two subcommands `list` and `rm <container>` to list all pulled containers and remove a container.
+
+`kapp image rm` does not actually remove any data, it just removes the supplied uri (along with any aliases that point to it). This is because the underlying data may be used by other image tags. Dangling containers, which aren't pointed to by any local uris, can be deleted using `kapp purge dangling`
+
+### `purge`
+
+```bash
+# usage
+kapp purge dangling
+```
+
+Delete all dangling image files: i.e. files that aren't pointed to by any local uris. This command also removes any snakemake aliases pointing to the data.
+
+### `alias`
+
+```bash
+# usage
+kapp alias list
+```
+
+List all aliases currently in use, along with the containers they point to.
+
+### `exec`, `shell`, `run`
+
+```bash
+# usage
+kapp (exec|shell|run) <uri_or_alias> [args...]
+```
+
+Simple wrapper around `singularity (exec|shell|run)`. No singularity args can be specified, only args for the container. If you need to specify singularity args, call singularity directly and use `kapp path <container>` to get the container path. Note that most singularity args (e.g. directory bids) can be specified using environment variable, and such variables will be consumed by `kapp` as normal.
+
+### `snakemake`
+
+Prints the path to the snakemake directory. This path can be supplied to the snakemake parameter `--singularity-prefix`, allowing snakemake to seamlessly consume containers downloaded using kapp. This is especially usefull for cluster execution without internet connection: containers can be pulled in advance on a login node, then used by snakemake later.
+
+## Configuration
+
+kslurm currently supports a few basic configuration values, and more will come with time. All configuration can be set using the command
+
+```bash
+kslurm config <key> <value>
+```
+
+You can print the value of a configuration using
+
+```bash
+kslurm config <key>
+```
+
+### Current values
+
+* `account`: Default account to use for kslurm commands (e.g. `kbatch`, `krun`, etc)
+* `pipdir`: Directory to store cached venvs and wheels. Should be a project or permanent storage dir.
 
-setup(**setup_kwargs)
```

