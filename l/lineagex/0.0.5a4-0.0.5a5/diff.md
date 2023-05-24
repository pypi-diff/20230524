# Comparing `tmp/lineagex-0.0.5a4.tar.gz` & `tmp/lineagex-0.0.5a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineagex-0.0.5a4.tar", max compression
+gzip compressed data, was "lineagex-0.0.5a5.tar", max compression
```

## Comparing `lineagex-0.0.5a4.tar` & `lineagex-0.0.5a5.tar`

### file list

```diff
@@ -1,15 +1,165 @@
--rw-r--r--   0        0        0       55 2023-05-24 01:42:09.254432 lineagex-0.0.5a4/lineagex/__init__.py
--rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.5a4/lineagex/app.js
--rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.5a4/lineagex/ColumnLineage.py
--rw-r--r--   0        0        0    24066 2023-05-24 01:05:18.342710 lineagex-0.0.5a4/lineagex/ColumnLineageNoConn.py
--rw-r--r--   0        0        0     1703 2023-05-24 01:59:23.537019 lineagex-0.0.5a4/lineagex/example.py
--rw-r--r--   0        0        0     1802 2023-05-24 01:42:19.469427 lineagex-0.0.5a4/lineagex/lineagex.py
--rw-r--r--   0        0        0     4691 2023-05-23 23:48:42.350240 lineagex-0.0.5a4/lineagex/LineageXNoConn.py
--rw-r--r--   0        0        0    13522 2023-05-23 21:34:23.590817 lineagex-0.0.5a4/lineagex/LineageXWithConn.py
--rw-r--r--   0        0        0     7176 2023-05-23 22:40:25.559899 lineagex-0.0.5a4/lineagex/SqlToDict.py
--rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.5a4/lineagex/stack.py
--rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.5a4/lineagex/utils.py
--rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.5a4/lineagex/vendor.js
--rw-r--r--   0        0        0      456 2023-05-24 01:59:38.059270 lineagex-0.0.5a4/pyproject.toml
--rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.5a4/README.md
--rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 lineagex-0.0.5a4/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-05-24 01:42:09.254432 lineagex-0.0.5a5/lineagex/__init__.py
+-rw-r--r--   0        0        0    54175 2023-04-22 19:33:20.371862 lineagex-0.0.5a5/lineagex/app.js
+-rw-r--r--   0        0        0    32350 2023-05-20 01:29:26.901284 lineagex-0.0.5a5/lineagex/ColumnLineage.py
+-rw-r--r--   0        0        0    24066 2023-05-24 01:05:18.342710 lineagex-0.0.5a5/lineagex/ColumnLineageNoConn.py
+-rw-r--r--   0        0        0     1566 2023-05-24 02:03:11.160110 lineagex-0.0.5a5/lineagex/example.py
+-rw-r--r--   0        0        0       75 2022-10-26 09:03:26.188175 lineagex-0.0.5a5/lineagex/examples/dependency_example/a_table.sql
+-rw-r--r--   0        0        0      251 2022-12-02 00:51:03.820262 lineagex-0.0.5a5/lineagex/examples/dependency_example/aa_table.sql
+-rw-r--r--   0        0        0      523 2022-07-21 07:17:33.218837 lineagex-0.0.5a5/lineagex/examples/dependency_example/basic_patient_info.sql
+-rw-r--r--   0        0        0       25 2023-05-08 21:37:17.347109 lineagex-0.0.5a5/lineagex/examples/dependency_example/from_aa_table.sql
+-rw-r--r--   0        0        0       92 2022-10-26 09:03:35.427267 lineagex-0.0.5a5/lineagex/examples/dependency_example/no_dob.sql
+-rw-r--r--   0        0        0       46 2023-05-23 21:49:30.792377 lineagex-0.0.5a5/lineagex/examples/github_example/desktop.ini
+-rw-r--r--   0        0        0       77 2023-05-14 05:13:01.960169 lineagex-0.0.5a5/lineagex/examples/github_example/table1.sql
+-rw-r--r--   0        0        0       76 2023-05-14 05:13:16.805234 lineagex-0.0.5a5/lineagex/examples/github_example/table2.sql
+-rw-r--r--   0        0        0     2984 2023-05-17 19:49:22.688529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/code_status.sql
+-rw-r--r--   0        0        0    31332 2023-05-17 19:49:22.688529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37.sql
+-rw-r--r--   0        0        0    18975 2023-05-17 19:49:22.688529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/comorbidity/elixhauser_ahrq_v37_no_drg.sql
+-rw-r--r--   0        0        0    10347 2023-05-17 19:49:22.689529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/comorbidity/elixhauser_quan.sql
+-rw-r--r--   0        0        0     2938 2023-05-17 19:49:22.689529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_ahrq.sql
+-rw-r--r--   0        0        0     2925 2023-05-17 19:49:22.689529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/comorbidity/elixhauser_score_quan.sql
+-rw-r--r--   0        0        0     3506 2023-05-23 23:50:36.510324 lineagex-0.0.5a5/lineagex/examples/mimic-iii/demographics/heightweight.sql
+-rw-r--r--   0        0        0     3891 2023-05-17 19:49:22.689529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/demographics/icustay_detail.sql
+-rw-r--r--   0        0        0     1396 2023-05-17 19:49:22.690529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/demographics/icustay_hours.sql
+-rw-r--r--   0        0        0     1808 2023-05-17 19:49:22.690529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/demographics/icustay_times.sql
+-rw-r--r--   0        0        0     6521 2023-05-17 19:49:22.690529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/demographics/note_counts.sql
+-rw-r--r--   0        0        0      143 2023-05-17 19:49:22.690529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/demographics/weight_durations.sql
+-rw-r--r--   0        0        0    63797 2023-05-17 19:49:22.691529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/diagnosis/ccs_multi_dx.csv.gz
+-rw-r--r--   0        0        0     2172 2023-05-17 19:49:22.690529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/diagnosis/README.md
+-rw-r--r--   0        0        0     7140 2023-05-17 19:49:22.691529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/adenosine_durations.sql
+-rw-r--r--   0        0        0     6273 2023-05-17 19:49:22.692529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/arterial_line_durations.sql
+-rw-r--r--   0        0        0     7217 2023-05-17 19:49:22.692529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/central_line_durations.sql
+-rw-r--r--   0        0        0     6331 2023-05-17 19:49:22.692529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/crrt_durations.sql
+-rw-r--r--   0        0        0     7521 2023-05-17 19:49:22.692529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/dobutamine_dose.sql
+-rw-r--r--   0        0        0     7051 2023-05-17 19:49:22.692529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/dobutamine_durations.sql
+-rw-r--r--   0        0        0     7526 2023-05-17 19:49:22.693529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/dopamine_dose.sql
+-rw-r--r--   0        0        0     7056 2023-05-17 19:49:22.693529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/dopamine_durations.sql
+-rw-r--r--   0        0        0     8067 2023-05-17 19:49:22.693529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/epinephrine_dose.sql
+-rw-r--r--   0        0        0     7110 2023-05-17 19:49:22.693529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/epinephrine_durations.sql
+-rw-r--r--   0        0        0     6979 2023-05-17 19:49:22.693529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/isuprel_durations.sql
+-rw-r--r--   0        0        0     6991 2023-05-17 19:49:22.693529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/milrinone_durations.sql
+-rw-r--r--   0        0        0     9660 2023-05-17 19:49:22.693529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/neuroblock_dose.sql
+-rw-r--r--   0        0        0     8192 2023-05-17 19:49:22.694529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/norepinephrine_dose.sql
+-rw-r--r--   0        0        0     7080 2023-05-17 19:49:22.694529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/norepinephrine_durations.sql
+-rw-r--r--   0        0        0     7541 2023-05-17 19:49:22.694529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/phenylephrine_dose.sql
+-rw-r--r--   0        0        0     7086 2023-05-17 19:49:22.694529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/phenylephrine_durations.sql
+-rw-r--r--   0        0        0     7531 2023-05-17 19:49:22.694529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/vasopressin_dose.sql
+-rw-r--r--   0        0        0     7003 2023-05-17 19:49:22.694529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/vasopressin_durations.sql
+-rw-r--r--   0        0        0     9595 2023-05-17 19:49:22.694529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/vasopressor_durations.sql
+-rw-r--r--   0        0        0     5576 2023-05-17 19:49:22.695529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/ventilation_classification.sql
+-rw-r--r--   0        0        0     4521 2023-05-17 19:49:22.695529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/ventilation_durations.sql
+-rw-r--r--   0        0        0     6839 2023-05-17 19:49:22.695529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/durations/weight_durations.sql
+-rw-r--r--   0        0        0     2346 2023-05-17 19:49:22.695529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/echo_data.sql
+-rw-r--r--   0        0        0     5885 2023-05-23 23:51:44.365020 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/blood_gas_first_day.sql
+-rw-r--r--   0        0        0     5385 2023-05-23 23:24:51.648101 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/blood_gas_first_day_arterial.sql
+-rw-r--r--   0        0        0      139 2023-05-17 19:49:22.696529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/first_day_sofa.sql
+-rw-r--r--   0        0        0     5015 2023-05-17 19:49:22.696529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/gcs_first_day.sql
+-rw-r--r--   0        0        0     2415 2023-05-17 19:49:22.696529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/height_first_day.sql
+-rw-r--r--   0        0        0     9180 2023-05-17 19:49:22.696529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/labs_first_day.sql
+-rw-r--r--   0        0        0     9357 2023-05-17 19:49:22.697528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/rrt_first_day.sql
+-rw-r--r--   0        0        0     2205 2023-05-17 19:49:22.697528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/urine_output_first_day.sql
+-rw-r--r--   0        0        0     1148 2023-05-17 19:49:22.697528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/ventilation_first_day.sql
+-rw-r--r--   0        0        0     5200 2023-05-17 19:49:22.697528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/vitals_first_day.sql
+-rw-r--r--   0        0        0     3766 2023-05-17 19:49:22.697528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/firstday/weight_first_day.sql
+-rw-r--r--   0        0        0     3117 2023-05-17 19:49:22.698529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/fluid_balance/colloid_bolus.sql
+-rw-r--r--   0        0        0     4388 2023-05-17 19:49:22.698529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/fluid_balance/crystalloid_bolus.sql
+-rw-r--r--   0        0        0     2669 2023-05-17 19:49:22.698529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/fluid_balance/ffp_transfusion.sql
+-rw-r--r--   0        0        0     2500 2023-05-17 19:49:22.698529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/fluid_balance/rbc_transfusion.sql
+-rw-r--r--   0        0        0     1555 2023-05-17 19:49:22.698529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/fluid_balance/urine_output.sql
+-rw-r--r--   0        0        0      135 2023-05-17 19:49:22.698529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/measurement/urine_output.sql
+-rw-r--r--   0        0        0      171 2023-05-17 19:49:22.699531 lineagex-0.0.5a5/lineagex/examples/mimic-iii/medication/norepinephrine_equivalent_dose.sql
+-rw-r--r--   0        0        0      143 2023-05-17 19:49:22.699531 lineagex-0.0.5a5/lineagex/examples/mimic-iii/medication/vasoactive_agent.sql
+-rw-r--r--   0        0        0     1411 2023-05-17 19:49:22.699531 lineagex-0.0.5a5/lineagex/examples/mimic-iii/organfailure/kdigo_creatinine.sql
+-rw-r--r--   0        0        0     3085 2023-05-17 19:49:22.699531 lineagex-0.0.5a5/lineagex/examples/mimic-iii/organfailure/kdigo_stages.sql
+-rw-r--r--   0        0        0     2229 2023-05-17 19:49:22.699531 lineagex-0.0.5a5/lineagex/examples/mimic-iii/organfailure/kdigo_stages_48hr.sql
+-rw-r--r--   0        0        0     2223 2023-05-17 19:49:22.700528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/organfailure/kdigo_stages_7day.sql
+-rw-r--r--   0        0        0     3287 2023-05-17 19:49:22.700528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/organfailure/kdigo_uo.sql
+-rw-r--r--   0        0        0     4829 2023-05-17 19:49:22.700528 lineagex-0.0.5a5/lineagex/examples/mimic-iii/organfailure/meld.sql
+-rw-r--r--   0        0        0     3516 2023-05-17 19:49:22.701529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/sepsis/angus.sql
+-rw-r--r--   0        0        0     1035 2023-05-17 19:49:22.701529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/sepsis/explicit.sql
+-rw-r--r--   0        0        0     3954 2023-05-17 19:49:22.701529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/sepsis/martin.sql
+-rw-r--r--   0        0        0      125 2023-05-17 19:49:22.701529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/sepsis/sepsis3.sql
+-rw-r--r--   0        0        0    28187 2023-05-17 19:49:22.702529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/apsiii.sql
+-rw-r--r--   0        0        0     7370 2023-05-17 19:49:22.702529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/lods.sql
+-rw-r--r--   0        0        0     6878 2023-05-17 19:49:22.702529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/mlods.sql
+-rw-r--r--   0        0        0     9670 2023-05-17 19:49:22.702529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/oasis.sql
+-rw-r--r--   0        0        0     2594 2023-05-17 19:49:22.703529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/qsofa.sql
+-rw-r--r--   0        0        0    10867 2023-05-17 19:49:22.703529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/saps.sql
+-rw-r--r--   0        0        0    12484 2023-05-17 19:49:22.703529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/sapsii.sql
+-rw-r--r--   0        0        0     3790 2023-05-17 19:49:22.703529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/sirs.sql
+-rw-r--r--   0        0        0    10302 2023-05-17 19:49:22.704529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/severityscores/sofa.sql
+-rw-r--r--   0        0        0     8176 2023-05-17 19:49:22.704529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/treatment/abx_prescriptions_list.sql
+-rw-r--r--   0        0        0     4490 2023-05-17 19:49:22.704529 lineagex-0.0.5a5/lineagex/examples/mimic-iii/treatment/suspicion_of_infection.sql
+-rw-r--r--   0        0        0    14187 2023-05-17 19:49:22.831516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/comorbidity/charlson.sql
+-rw-r--r--   0        0        0     6645 2023-05-17 19:49:22.831516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/comorbidity/first_day_lab.sql
+-rw-r--r--   0        0        0     1645 2023-05-17 19:49:22.831516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/demographics/age.sql
+-rw-r--r--   0        0        0     1816 2023-05-17 19:49:22.831516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/demographics/icustay_detail.sql
+-rw-r--r--   0        0        0     1732 2023-05-17 19:49:22.831516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/demographics/icustay_hourly.sql
+-rw-r--r--   0        0        0      803 2023-05-17 19:49:22.832517 lineagex-0.0.5a5/lineagex/examples/mimic-iv/demographics/icustay_times.sql
+-rw-r--r--   0        0        0     3921 2023-05-17 19:49:22.832517 lineagex-0.0.5a5/lineagex/examples/mimic-iv/demographics/weight_durations.sql
+-rw-r--r--   0        0        0     2030 2023-05-17 19:49:22.832517 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_bg.sql
+-rw-r--r--   0        0        0     2039 2023-05-17 19:49:22.832517 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_bg_art.sql
+-rw-r--r--   0        0        0     1758 2023-05-17 19:49:22.832517 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_gcs.sql
+-rw-r--r--   0        0        0      757 2023-05-17 19:49:22.832517 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_height.sql
+-rw-r--r--   0        0        0     7164 2023-05-17 19:49:22.833516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_lab.sql
+-rw-r--r--   0        0        0      715 2023-05-17 19:49:22.833516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_rrt.sql
+-rw-r--r--   0        0        0     9485 2023-05-17 19:49:22.833516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_sofa.sql
+-rw-r--r--   0        0        0      686 2023-05-17 19:49:22.833516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_urine_output.sql
+-rw-r--r--   0        0        0     1389 2023-05-17 19:49:22.833516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_vitalsign.sql
+-rw-r--r--   0        0        0      987 2023-05-17 19:49:22.834516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/firstday/first_day_weight.sql
+-rw-r--r--   0        0        0     8614 2023-05-17 19:49:22.834516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/bg.sql
+-rw-r--r--   0        0        0     7196 2023-05-17 19:49:22.834516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/blood_differential.sql
+-rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.835515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/cardiac_marker.sql
+-rw-r--r--   0        0        0     3165 2023-05-17 19:49:22.835515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/chemistry.sql
+-rw-r--r--   0        0        0     1310 2023-05-17 19:49:22.835515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/coagulation.sql
+-rw-r--r--   0        0        0     1578 2023-05-17 19:49:22.835515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/complete_blood_count.sql
+-rw-r--r--   0        0        0     2136 2023-05-17 19:49:22.835515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/creatinine_baseline.sql
+-rw-r--r--   0        0        0     1835 2023-05-17 19:49:22.836515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/enzyme.sql
+-rw-r--r--   0        0        0     4839 2023-05-18 04:41:01.815148 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/gcs.sql
+-rw-r--r--   0        0        0     1443 2023-05-17 19:49:22.836515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/height.sql
+-rw-r--r--   0        0        0      770 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/icp.sql
+-rw-r--r--   0        0        0      654 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/inflammation.sql
+-rw-r--r--   0        0        0      116 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/kdigo_uo.sql
+-rw-r--r--   0        0        0     3793 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/oxygen_delivery.sql
+-rw-r--r--   0        0        0     1000 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/rhythm.sql
+-rw-r--r--   0        0        0     1323 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/urine_output.sql
+-rw-r--r--   0        0        0     4550 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/urine_output_rate.sql
+-rw-r--r--   0        0        0     3415 2023-05-17 19:49:22.837515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/ventilator_setting.sql
+-rw-r--r--   0        0        0     3709 2023-05-17 19:49:22.838515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/measurement/vitalsign.sql
+-rw-r--r--   0        0        0    10373 2023-05-17 19:49:22.838515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/antibiotic.sql
+-rw-r--r--   0        0        0      493 2023-05-17 19:49:22.838515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/dobutamine.sql
+-rw-r--r--   0        0        0      486 2023-05-17 19:49:22.838515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/dopamine.sql
+-rw-r--r--   0        0        0      499 2023-05-17 19:49:22.838515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/epinephrine.sql
+-rw-r--r--   0        0        0      471 2023-05-17 19:49:22.838515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/milrinone.sql
+-rw-r--r--   0        0        0      561 2023-05-17 19:49:22.838515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/neuroblock.sql
+-rw-r--r--   0        0        0      865 2023-05-17 19:49:22.839516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/norepinephrine.sql
+-rw-r--r--   0        0        0     1644 2023-05-17 19:49:22.839516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/norepinephrine_equivalent_dose.sql
+-rw-r--r--   0        0        0      601 2023-05-17 19:49:22.839516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/phenylephrine.sql
+-rw-r--r--   0        0        0     4576 2023-05-17 19:49:22.839516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/vasoactive_agent.sql
+-rw-r--r--   0        0        0      722 2023-05-17 19:49:22.839516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/medication/vasopressin.sql
+-rw-r--r--   0        0        0     2036 2023-05-17 19:49:22.840515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/organfailure/kdigo_creatinine.sql
+-rw-r--r--   0        0        0     5580 2023-05-17 19:49:22.840515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/organfailure/kdigo_stages.sql
+-rw-r--r--   0        0        0     3802 2023-05-17 19:49:22.840515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/organfailure/kdigo_uo.sql
+-rw-r--r--   0        0        0     5701 2023-05-17 19:49:22.840515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/organfailure/meld.sql
+-rw-r--r--   0        0        0      675 2023-05-17 19:49:22.831516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/README.md
+-rw-r--r--   0        0        0    33864 2023-05-17 19:49:22.841515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/score/apsiii.sql
+-rw-r--r--   0        0        0     7695 2023-05-17 19:49:22.842515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/score/lods.sql
+-rw-r--r--   0        0        0    11246 2023-05-17 19:49:22.842515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/score/oasis.sql
+-rw-r--r--   0        0        0    17903 2023-05-17 19:49:22.842515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/score/sapsii.sql
+-rw-r--r--   0        0        0     3517 2023-05-17 19:49:22.842515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/score/sirs.sql
+-rw-r--r--   0        0        0    12603 2023-05-17 19:49:22.842515 lineagex-0.0.5a5/lineagex/examples/mimic-iv/score/sofa.sql
+-rw-r--r--   0        0        0     2994 2023-05-17 19:49:22.843516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/sepsis/sepsis3.sql
+-rw-r--r--   0        0        0     6418 2023-05-17 19:49:22.843516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/sepsis/suspicion_of_infection.sql
+-rw-r--r--   0        0        0     6011 2023-05-17 19:49:22.843516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/treatment/crrt.sql
+-rw-r--r--   0        0        0     4777 2023-05-17 19:49:22.843516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/treatment/invasive_line.sql
+-rw-r--r--   0        0        0    13683 2023-05-18 23:24:29.938626 lineagex-0.0.5a5/lineagex/examples/mimic-iv/treatment/rrt.sql
+-rw-r--r--   0        0        0     9285 2023-05-17 19:49:22.843516 lineagex-0.0.5a5/lineagex/examples/mimic-iv/treatment/ventilation.sql
+-rw-r--r--   0        0        0     1802 2023-05-24 01:42:19.469427 lineagex-0.0.5a5/lineagex/lineagex.py
+-rw-r--r--   0        0        0     4691 2023-05-23 23:48:42.350240 lineagex-0.0.5a5/lineagex/LineageXNoConn.py
+-rw-r--r--   0        0        0    13522 2023-05-23 21:34:23.590817 lineagex-0.0.5a5/lineagex/LineageXWithConn.py
+-rw-r--r--   0        0        0     7176 2023-05-23 22:40:25.559899 lineagex-0.0.5a5/lineagex/SqlToDict.py
+-rw-r--r--   0        0        0     1460 2023-05-08 20:36:59.378380 lineagex-0.0.5a5/lineagex/stack.py
+-rw-r--r--   0        0        0     7305 2023-05-19 22:10:39.261810 lineagex-0.0.5a5/lineagex/utils.py
+-rw-r--r--   0        0        0  3761177 2023-04-22 19:33:20.645016 lineagex-0.0.5a5/lineagex/vendor.js
+-rw-r--r--   0        0        0      456 2023-05-24 02:04:10.341420 lineagex-0.0.5a5/pyproject.toml
+-rw-r--r--   0        0        0     4158 2023-05-17 20:42:55.789941 lineagex-0.0.5a5/README.md
+-rw-r--r--   0        0        0     4865 1970-01-01 00:00:00.000000 lineagex-0.0.5a5/PKG-INFO
```

### Comparing `lineagex-0.0.5a4/lineagex/app.js` & `lineagex-0.0.5a5/lineagex/app.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/ColumnLineage.py` & `lineagex-0.0.5a5/lineagex/ColumnLineage.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/ColumnLineageNoConn.py` & `lineagex-0.0.5a5/lineagex/ColumnLineageNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/example.py` & `lineagex-0.0.5a5/lineagex/example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,17 @@
+from .lineagex import lineagex
 import os
 
 
 class example:
     def __init__(self, case: str = ""):
         def get_current_path():
             # Returns the path of the current script
             return os.path.dirname(os.path.realpath(__file__))
-
-        print("Current path is: ", get_current_path())
-        import lineagex
-        print(os.path.abspath(lineagex.__file__))
-
-        cwd = os.getcwd()
-        from .lineagex import lineagex
+        cwd = get_current_path()
         if case == "github_example":
             t_noconn = lineagex(sql=os.path.join(cwd, 'examples', 'github_example'), target_schema="schema1", search_path_schema="schema1, public")
             print("{} finished, please check in the folder for output.json and index.html".format(case))
         elif case == "dependency_example":
             t_noconn = lineagex(sql=os.path.join(cwd, 'examples', 'dependency_example'), target_schema="mimiciii_derived", search_path_schema="mimiciii_clinical, public")
             print("{} finished, please check in the folder for output.json and index.html".format(case))
         elif case == "mimic-iv":
```

### Comparing `lineagex-0.0.5a4/lineagex/lineagex.py` & `lineagex-0.0.5a5/lineagex/lineagex.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/LineageXNoConn.py` & `lineagex-0.0.5a5/lineagex/LineageXNoConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/LineageXWithConn.py` & `lineagex-0.0.5a5/lineagex/LineageXWithConn.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/SqlToDict.py` & `lineagex-0.0.5a5/lineagex/SqlToDict.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/stack.py` & `lineagex-0.0.5a5/lineagex/stack.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/utils.py` & `lineagex-0.0.5a5/lineagex/utils.py`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/lineagex/vendor.js` & `lineagex-0.0.5a5/lineagex/vendor.js`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/README.md` & `lineagex-0.0.5a5/README.md`

 * *Files identical despite different names*

### Comparing `lineagex-0.0.5a4/PKG-INFO` & `lineagex-0.0.5a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineagex
-Version: 0.0.5a4
+Version: 0.0.5a5
 Summary: A column lineage tool
 License: MIT
 Author: zshandy
 Author-email: zshandy@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

